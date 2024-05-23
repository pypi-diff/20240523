# Comparing `tmp/ntv_numpy-0.2.1.tar.gz` & `tmp/ntv_numpy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntv_numpy-0.2.1.tar", last modified: Wed May 15 22:15:58 2024, max compression
+gzip compressed data, was "ntv_numpy-0.2.2.tar", last modified: Thu May 23 14:10:13 2024, max compression
```

## Comparing `ntv_numpy-0.2.1.tar` & `ntv_numpy-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 22:15:58.710364 ntv_numpy-0.2.1/
--rw-rw-rw-   0        0        0    12126 2024-05-15 22:15:58.709867 ntv_numpy-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    11352 2024-05-05 21:16:27.000000 ntv_numpy-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 22:15:58.703394 ntv_numpy-0.2.1/ntv_numpy/
--rw-rw-rw-   0        0        0     1983 2024-05-05 21:28:10.000000 ntv_numpy-0.2.1/ntv_numpy/__init__.py
--rw-rw-rw-   0        0        0     9057 2024-05-05 20:21:42.000000 ntv_numpy-0.2.1/ntv_numpy/data_array.py
--rw-rw-rw-   0        0        0    22905 2024-05-15 07:00:55.000000 ntv_numpy-0.2.1/ntv_numpy/ndarray.py
--rw-rw-rw-   0        0        0     2603 2024-05-05 20:56:51.000000 ntv_numpy-0.2.1/ntv_numpy/ndtype.py
--rw-rw-rw-   0        0        0     5166 2024-04-23 08:57:01.000000 ntv_numpy-0.2.1/ntv_numpy/ntv_numpy.ini
--rw-rw-rw-   0        0        0     8050 2024-05-05 20:29:43.000000 ntv_numpy-0.2.1/ntv_numpy/numpy_ntv_connector.py
--rw-rw-rw-   0        0        0    26743 2024-05-15 21:28:45.000000 ntv_numpy-0.2.1/ntv_numpy/xconnector.py
--rw-rw-rw-   0        0        0    19592 2024-05-15 21:39:27.000000 ntv_numpy-0.2.1/ntv_numpy/xdataset.py
--rw-rw-rw-   0        0        0     9535 2024-05-15 07:54:18.000000 ntv_numpy-0.2.1/ntv_numpy/xndarray.py
-drwxrwxrwx   0        0        0        0 2024-05-15 22:15:58.708373 ntv_numpy-0.2.1/ntv_numpy.egg-info/
--rw-rw-rw-   0        0        0    12126 2024-05-15 22:15:58.000000 ntv_numpy-0.2.1/ntv_numpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2024-05-15 22:15:58.000000 ntv_numpy-0.2.1/ntv_numpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 22:15:58.000000 ntv_numpy-0.2.1/ntv_numpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-05-15 22:15:58.000000 ntv_numpy-0.2.1/ntv_numpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-15 22:15:58.000000 ntv_numpy-0.2.1/ntv_numpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-05-15 22:15:58.712357 ntv_numpy-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1223 2024-05-15 22:02:36.000000 ntv_numpy-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 22:15:58.707378 ntv_numpy-0.2.1/tests/
--rw-rw-rw-   0        0        0    31123 2024-05-15 21:31:13.000000 ntv_numpy-0.2.1/tests/tests_ntv_numpy.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:10:13.471621 ntv_numpy-0.2.2/
+-rw-rw-rw-   0        0        0    11779 2024-05-23 14:10:13.471124 ntv_numpy-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    11005 2024-05-21 09:22:23.000000 ntv_numpy-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 14:10:13.460166 ntv_numpy-0.2.2/ntv_numpy/
+-rw-rw-rw-   0        0        0     2173 2024-05-21 12:12:02.000000 ntv_numpy-0.2.2/ntv_numpy/__init__.py
+-rw-rw-rw-   0        0        0     9060 2024-05-21 09:22:23.000000 ntv_numpy-0.2.2/ntv_numpy/data_array.py
+-rw-rw-rw-   0        0        0    23156 2024-05-21 09:22:23.000000 ntv_numpy-0.2.2/ntv_numpy/ndarray.py
+-rw-rw-rw-   0        0        0     2626 2024-05-21 09:22:23.000000 ntv_numpy-0.2.2/ntv_numpy/ndtype.py
+-rw-rw-rw-   0        0        0     5119 2024-05-21 09:22:23.000000 ntv_numpy-0.2.2/ntv_numpy/ntv_numpy.ini
+-rw-rw-rw-   0        0        0     8334 2024-05-21 09:22:23.000000 ntv_numpy-0.2.2/ntv_numpy/numpy_ntv_connector.py
+-rw-rw-rw-   0        0        0     2783 2024-05-23 13:18:29.000000 ntv_numpy-0.2.2/ntv_numpy/xarray_accessors.py
+-rw-rw-rw-   0        0        0    27463 2024-05-21 09:22:23.000000 ntv_numpy-0.2.2/ntv_numpy/xconnector.py
+-rw-rw-rw-   0        0        0    20474 2024-05-21 09:22:23.000000 ntv_numpy-0.2.2/ntv_numpy/xdataset.py
+-rw-rw-rw-   0        0        0     9731 2024-05-21 09:22:23.000000 ntv_numpy-0.2.2/ntv_numpy/xndarray.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:10:13.470626 ntv_numpy-0.2.2/ntv_numpy.egg-info/
+-rw-rw-rw-   0        0        0    11779 2024-05-23 14:10:13.000000 ntv_numpy-0.2.2/ntv_numpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      474 2024-05-23 14:10:13.000000 ntv_numpy-0.2.2/ntv_numpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 14:10:13.000000 ntv_numpy-0.2.2/ntv_numpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-05-23 14:10:13.000000 ntv_numpy-0.2.2/ntv_numpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-23 14:10:13.000000 ntv_numpy-0.2.2/ntv_numpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      368 2024-05-21 08:07:05.000000 ntv_numpy-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       85 2024-05-23 14:10:13.478089 ntv_numpy-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1231 2024-05-23 12:42:17.000000 ntv_numpy-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:10:13.469131 ntv_numpy-0.2.2/tests/
+-rw-rw-rw-   0        0        0    33632 2024-05-23 14:04:36.000000 ntv_numpy-0.2.2/tests/tests_ntv_numpy.py
```

### Comparing `ntv_numpy-0.2.1/PKG-INFO` & `ntv_numpy-0.2.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntv_numpy
-Version: 0.2.1
+Version: 0.2.2
 Summary: NTV-NumPy : A multidimensional semantic, compact and reversible format for interoperability
 Home-page: https://github.com/loco-philippe/ntv-numpy/blob/main/README.md
 Author: Philippe Thomy
 Author-email: philippe@loco-labs.io
 Keywords: numpy,JSON-NTV,semantic JSON,development,environmental data,multidimensional
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -67,26 +67,26 @@
 ```python
 In [1]: example = {
                 'example:xdataset': {
                         'var1': [['float[kg]', [2, 2], [10.1, 0.4, 3.4, 8.2]], ['x', 'y']],
                         'var1.variance': [[[2, 2], [0.1, 0.2, 0.3, 0.4]]],
                         'var1.mask1': [[[True, False]], ['x']],
                         'var1.mask2': [[[2, 2], [True, False, False, True]]],
-                
-                        'var2': [['var2.ntv'], ['x', 'y']],    
-                        
+
+                        'var2': [['var2.ntv'], ['x', 'y']],
+
                         'x': [['string', ['23F0AE', '578B98']], {'test': 21}],
                         'y': [['date', ['2021-01-01', '2022-02-02']]],
-                        
+
                         'ranking': [['month', [2, 2], [1, 2, 3, 4]], ['var1']],
                         'z': [['float', [10, 20]], ['x']],
                         'z.uncertainty': [[[0.1, 0.2]]],
-                        
+
                         'z_bis': [[['z1_bis', 'z2_bis']]],
-                
+
                         'info': {'path': 'https://github.com/loco-philippe/ntv-numpy/tree/main/example/',
                         'location': [['string', ['paris']]]}
                 }
         }
 
 In [2]: from ntv_numpy import Xdataset
 
@@ -151,28 +151,28 @@
 
 ### Pandas interoperability
 
 ```python
 In [6]: x_dataframe = x_example.to_dataframe()
         print(x_example.to_dataframe(json_name=False))
         print(x_xarray)
-Out[6]: 
+Out[6]:
                    ranking     z  z.uncertainty  var1  var1.mask1  var1.mask2  \
-x      y                                                                        
-23F0AE 2021-01-01        1  10.0            0.1  10.1        True        True   
-       2022-02-02        2  10.0            0.1   0.4        True       False   
-578B98 2021-01-01        3  20.0            0.2   3.4       False       False   
-       2022-02-02        4  20.0            0.2   8.2       False        True   
-
-                   var1.variance location  
-x      y                                   
-23F0AE 2021-01-01            0.1    paris  
-       2022-02-02            0.2    paris  
-578B98 2021-01-01            0.3    paris  
-       2022-02-02            0.4    paris 
+x      y
+23F0AE 2021-01-01        1  10.0            0.1  10.1        True        True
+       2022-02-02        2  10.0            0.1   0.4        True       False
+578B98 2021-01-01        3  20.0            0.2   3.4       False       False
+       2022-02-02        4  20.0            0.2   8.2       False        True
+
+                   var1.variance location
+x      y
+23F0AE 2021-01-01            0.1    paris
+       2022-02-02            0.2    paris
+578B98 2021-01-01            0.3    paris
+       2022-02-02            0.4    paris
 ```
 
 Reversibility:
 
 ```python
 In [7]: x_example_pd = Xdataset.from_dataframe(x_dataframe)
         x_example_pd == x_example_xr == x_example_json == x_example
@@ -218,17 +218,17 @@
                         'wcs':  {'WCSAXES': 2, 'CRPIX1': 2048.0, 'CRPIX2': 1024.0, 'PC1_1': 1.2905625619716e-05,
                                 'PC1_2': 5.9530912331034e-06, 'PC2_1': 5.0220581265601e-06, 'PC2_2': -1.2644774105568e-05,
                                 'CDELT1': 1.0, 'CDELT2': 1.0, 'CUNIT1': 'deg', 'CUNIT2': 'deg', 'CTYPE1': 'RA---TAN',
                                 'CTYPE2': 'DEC--TAN', 'CRVAL1': 5.63056810618, 'CRVAL2': -72.05457184279, 'LONPOLE': 180.0,
                                 'LATPOLE': -72.05457184279, 'WCSNAME': 'IDC_qbu1641sj', 'MJDREF': 0.0, 'RADESYS': 'ICRS'},
                         'psf': [['float[erg/s]', [1,2,3,4]]]
                 }
-        } 
+        }
         n_example = Xdataset.read_json(example)
-        n_example.info 
+        n_example.info
 Out[1]: {'name': 'example',
         'xtype': 'group',
         'data_arrays': ['data', 'psf'],
         'additionals': ['data.mask', 'data.uncertainty'],
         'metadata': ['meta', 'wcs'],
         'validity': 'valid',
         'width': 6}
@@ -255,26 +255,26 @@
 ```python
 In [1]: example = {
                 'example:xdataset': {
                         'var1': [['float[kg]', [2, 2], 'var1.ntv'], ['x', 'y']],
                         'var1.variance': [[[2, 2], 'var1_variance.ntv']],
                         'var1.mask1': [['var1_mask1.ntv'], ['x']],
                         'var1.mask2': [[[2, 2], 'var1_mask2.ntv']],
-                
-                        'var2': [['var2.ntv'], ['x', 'y']],    
-                        
+
+                        'var2': [['var2.ntv'], ['x', 'y']],
+
                         'x': [['x.ntv'], {'test': 21}],
                         'y': [['date', 'y.ntv']],
-                        
+
                         'ranking': [['month', [2, 2], 'ranking.ntv'], ['var1']],
                         'z': [['float', 'z.ntv'], ['x']],
                         'z.uncertainty': [['z_uncertainty.ntv']],
-                        
+
                         'z_bis': [['z_bis.ntv']],
-                
+
                         'info': {'path': 'https://github.com/loco-philippe/ntv-numpy/tree/main/example/'}
                 }
         }
 ```
 
 The complete example can be rebuild with loading data (path + file name).
```

### Comparing `ntv_numpy-0.2.1/README.md` & `ntv_numpy-0.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -48,26 +48,26 @@
 ```python
 In [1]: example = {
                 'example:xdataset': {
                         'var1': [['float[kg]', [2, 2], [10.1, 0.4, 3.4, 8.2]], ['x', 'y']],
                         'var1.variance': [[[2, 2], [0.1, 0.2, 0.3, 0.4]]],
                         'var1.mask1': [[[True, False]], ['x']],
                         'var1.mask2': [[[2, 2], [True, False, False, True]]],
-                
-                        'var2': [['var2.ntv'], ['x', 'y']],    
-                        
+
+                        'var2': [['var2.ntv'], ['x', 'y']],
+
                         'x': [['string', ['23F0AE', '578B98']], {'test': 21}],
                         'y': [['date', ['2021-01-01', '2022-02-02']]],
-                        
+
                         'ranking': [['month', [2, 2], [1, 2, 3, 4]], ['var1']],
                         'z': [['float', [10, 20]], ['x']],
                         'z.uncertainty': [[[0.1, 0.2]]],
-                        
+
                         'z_bis': [[['z1_bis', 'z2_bis']]],
-                
+
                         'info': {'path': 'https://github.com/loco-philippe/ntv-numpy/tree/main/example/',
                         'location': [['string', ['paris']]]}
                 }
         }
 
 In [2]: from ntv_numpy import Xdataset
 
@@ -132,28 +132,28 @@
 
 ### Pandas interoperability
 
 ```python
 In [6]: x_dataframe = x_example.to_dataframe()
         print(x_example.to_dataframe(json_name=False))
         print(x_xarray)
-Out[6]: 
+Out[6]:
                    ranking     z  z.uncertainty  var1  var1.mask1  var1.mask2  \
-x      y                                                                        
-23F0AE 2021-01-01        1  10.0            0.1  10.1        True        True   
-       2022-02-02        2  10.0            0.1   0.4        True       False   
-578B98 2021-01-01        3  20.0            0.2   3.4       False       False   
-       2022-02-02        4  20.0            0.2   8.2       False        True   
-
-                   var1.variance location  
-x      y                                   
-23F0AE 2021-01-01            0.1    paris  
-       2022-02-02            0.2    paris  
-578B98 2021-01-01            0.3    paris  
-       2022-02-02            0.4    paris 
+x      y
+23F0AE 2021-01-01        1  10.0            0.1  10.1        True        True
+       2022-02-02        2  10.0            0.1   0.4        True       False
+578B98 2021-01-01        3  20.0            0.2   3.4       False       False
+       2022-02-02        4  20.0            0.2   8.2       False        True
+
+                   var1.variance location
+x      y
+23F0AE 2021-01-01            0.1    paris
+       2022-02-02            0.2    paris
+578B98 2021-01-01            0.3    paris
+       2022-02-02            0.4    paris
 ```
 
 Reversibility:
 
 ```python
 In [7]: x_example_pd = Xdataset.from_dataframe(x_dataframe)
         x_example_pd == x_example_xr == x_example_json == x_example
@@ -199,17 +199,17 @@
                         'wcs':  {'WCSAXES': 2, 'CRPIX1': 2048.0, 'CRPIX2': 1024.0, 'PC1_1': 1.2905625619716e-05,
                                 'PC1_2': 5.9530912331034e-06, 'PC2_1': 5.0220581265601e-06, 'PC2_2': -1.2644774105568e-05,
                                 'CDELT1': 1.0, 'CDELT2': 1.0, 'CUNIT1': 'deg', 'CUNIT2': 'deg', 'CTYPE1': 'RA---TAN',
                                 'CTYPE2': 'DEC--TAN', 'CRVAL1': 5.63056810618, 'CRVAL2': -72.05457184279, 'LONPOLE': 180.0,
                                 'LATPOLE': -72.05457184279, 'WCSNAME': 'IDC_qbu1641sj', 'MJDREF': 0.0, 'RADESYS': 'ICRS'},
                         'psf': [['float[erg/s]', [1,2,3,4]]]
                 }
-        } 
+        }
         n_example = Xdataset.read_json(example)
-        n_example.info 
+        n_example.info
 Out[1]: {'name': 'example',
         'xtype': 'group',
         'data_arrays': ['data', 'psf'],
         'additionals': ['data.mask', 'data.uncertainty'],
         'metadata': ['meta', 'wcs'],
         'validity': 'valid',
         'width': 6}
@@ -236,26 +236,26 @@
 ```python
 In [1]: example = {
                 'example:xdataset': {
                         'var1': [['float[kg]', [2, 2], 'var1.ntv'], ['x', 'y']],
                         'var1.variance': [[[2, 2], 'var1_variance.ntv']],
                         'var1.mask1': [['var1_mask1.ntv'], ['x']],
                         'var1.mask2': [[[2, 2], 'var1_mask2.ntv']],
-                
-                        'var2': [['var2.ntv'], ['x', 'y']],    
-                        
+
+                        'var2': [['var2.ntv'], ['x', 'y']],
+
                         'x': [['x.ntv'], {'test': 21}],
                         'y': [['date', 'y.ntv']],
-                        
+
                         'ranking': [['month', [2, 2], 'ranking.ntv'], ['var1']],
                         'z': [['float', 'z.ntv'], ['x']],
                         'z.uncertainty': [['z_uncertainty.ntv']],
-                        
+
                         'z_bis': [['z_bis.ntv']],
-                
+
                         'info': {'path': 'https://github.com/loco-philippe/ntv-numpy/tree/main/example/'}
                 }
         }
 ```
 
 The complete example can be rebuild with loading data (path + file name).
```

### Comparing `ntv_numpy-0.2.1/ntv_numpy/__init__.py` & `ntv_numpy-0.2.2/ntv_numpy/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -45,20 +45,34 @@
     - `ntv-numpy.ntv_numpy.xdataset.XdatasetInterface`
     - `ntv-numpy.ntv_numpy.xdataset.XdatasetCategory`
 
 - `ntv-numpy.ntv_numpy.ndtype` :
 
     - `ntv-numpy.ntv_numpy.ndtype.Ndtype`
 
+
+- `ntv-numpy.ntv_numpy.xarray_accessors` :
+
+    - `ntv-numpy.ntv_numpy.xarray_accessors.NxrDatasetAccessor`
 """
-# from pathlib import Path
-# , read_json, to_json
+
 from ntv_numpy.numpy_ntv_connector import XndarrayConnec, NdarrayConnec
 from ntv_numpy.data_array import Dfull, Dcomplete, Darray, Dutil
 from ntv_numpy.ndarray import Ndarray, Nutil
 from ntv_numpy.xndarray import Xndarray
 from ntv_numpy.xdataset import Xdataset
-# import ntv_pandas.pandas_ntv_connector
 
-# path = Path(ntv_numpy.numpy_ntv_connector.__file__).parent
+import ntv_numpy.xarray_accessors as xarray_accessors
 
-# print('package :', __package__)
+__all__ = [
+    "XndarrayConnec",
+    "NdarrayConnec",
+    "Dfull",
+    "Dcomplete",
+    "Darray",
+    "Dutil",
+    "Ndarray",
+    "Nutil",
+    "Xndarray",
+    "Xdataset",
+    "xarray_accessors",
+]
```

### Comparing `ntv_numpy-0.2.1/ntv_numpy/data_array.py` & `ntv_numpy-0.2.2/ntv_numpy/data_array.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,262 +8,272 @@
 It contains the classes `Darray` (abstract), `Dfull`, `Dcomplete` for the
 representation of unidimensional arrays.
 
 For more information, see the
 [user guide](https://loco-philippe.github.io/ntv-numpy/docs/user_guide.html)
  or the [github repository](https://github.com/loco-philippe/ntv-numpy).
 """
+
 from abc import ABC, abstractmethod
 import json
 import numpy as np
 import pandas as pd
 from json_ntv import Ntv, NtvConnector
 
 
 class Darray(ABC):
-    ''' The Darray class is an abstract class used by `Dfull`and `Dcomplete` classes.
+    """The Darray class is an abstract class used by `Dfull`and `Dcomplete` classes.
 
     *Attributes :*
     - **data** :  np.ndarray - data after coding
     - **ref**:  int or string - reference to another Darray data
     - **coding**: np.ndarray of int - mapping between data and the values
 
     *dynamic values (@property)*
     - `values`
 
     *methods*
     - `read_json` (staticmethod)
     - `to_json`
-    '''
+    """
 
     def __init__(self, data, ref=None, coding=None, dtype=None, unidim=False):
-        '''Darray constructor.
+        """Darray constructor.
 
         *Parameters*
 
         - **data**: list, Darray or np.ndarray - data to represent (after coding)
         - **ref** : String or integer (default None) - name or index of another Darray
         - **coding**: List of integer (default None) - mapping between data and the list of values
         - **dtype**: string (default None) - numpy.dtype to apply
-        '''
+        """
         if isinstance(data, Darray):
             self.data = data.data
             self.ref = data.ref
             self.coding = data.coding
             return
         data = data if isinstance(data, (list, np.ndarray)) else [data]
         if (len(data) > 0 and isinstance(data[0], (list, np.ndarray))) or unidim:
-            dtype = data.dtype if isinstance(data, np.ndarray) else 'object'
+            dtype = data.dtype if isinstance(data, np.ndarray) else "object"
             self.data = np.fromiter(data, dtype=dtype)
         else:
             self.data = np.array(data, dtype=dtype).reshape(-1)
         self.ref = ref
         self.coding = np.array(coding)
 
     def __repr__(self):
-        '''return classname and number of value'''
-        return self.__class__.__name__ + '[' + str(len(self)) + ']'
+        """return classname and number of value"""
+        return self.__class__.__name__ + "[" + str(len(self)) + "]"
 
     def __str__(self):
-        '''return json string format'''
+        """return json string format"""
         return json.dumps(self.to_json())
 
     def __eq__(self, other):
-        ''' equal if values are equal'''
+        """equal if values are equal"""
         return np.array_equal(self.values, other.values, equal_nan=False)
 
     def __len__(self):
-        ''' len of values'''
+        """len of values"""
         return self._len_val
 
     def __contains__(self, item):
-        ''' item of values'''
+        """item of values"""
         return item in self.values
 
     def __getitem__(self, ind):
-        ''' return value item'''
+        """return value item"""
         if isinstance(ind, tuple):
             return [self.values[i] for i in ind]
             # return [copy(self.values[i]) for i in ind]
         return self.values[ind]
         # return copy(self.values[ind])
 
     def __copy__(self):
-        ''' Copy all the data '''
+        """Copy all the data"""
         return self.__class__(self)
 
     @staticmethod
     def read_json(val, dtype=None, unidim=False):
-        ''' return a Darray entity from a list of data.
+        """return a Darray entity from a list of data.
 
         *Parameters*
 
         - **val**: list of data
         - **dtype** : string (default None) - numpy.dtype to apply
-        '''
+        """
         val = val if isinstance(val, list) else [val]
         if not val or not isinstance(val[0], list):
             return Dfull(val, dtype=dtype, unidim=unidim)
         match val:
-            case [data, ref, list(coding)] if (isinstance(ref, (int, str)) and
-                                               isinstance(coding[0], int) and
-                                               max(coding) < len(data)):
+            case [data, ref, list(coding)] if (
+                isinstance(ref, (int, str))
+                and isinstance(coding[0], int)
+                and max(coding) < len(data)
+            ):
                 return None
-            case [data, ref] if (isinstance(data, list) and
-                                 isinstance(ref, (int, str))):
+            case [data, ref] if (
+                isinstance(data, list) and isinstance(ref, (int, str))
+            ):
                 return None
             case [data, list(coef)] if len(coef) == 1:
                 return None
-            case [data, list(coding)] if (isinstance(coding[0], int) and
-                                          max(coding) < len(data)):
+            case [data, list(coding)] if (
+                isinstance(coding[0], int) and max(coding) < len(data)
+            ):
                 return Dcomplete(data, None, coding, dtype=dtype, unidim=unidim)
             case _:
                 return Dfull(val, dtype=dtype, unidim=unidim)
 
     @abstractmethod
     def to_json(self):
-        ''' return a JsonValue'''
+        """return a JsonValue"""
 
     @property
     @abstractmethod
     def values(self):
-        ''' return the list of values'''
+        """return the list of values"""
 
     @property
     @abstractmethod
     def _len_val(self):
-        '''return the length of the entity'''
+        """return the length of the entity"""
 
 
 class Dfull(Darray):
-    ''' Representation of a one dimensional Array with full representation
+    """Representation of a one dimensional Array with full representation
 
     *dynamic values (@property)*
     - `values`
 
     *methods*
     - `read_json` (staticmethod)
     - `to_json`
-    '''
+    """
 
     def __init__(self, data, ref=None, coding=None, dtype=None, unidim=False):
-        '''Dfull constructor.
+        """Dfull constructor.
 
         *Parameters*
 
         - **data**: list, Darray or np.ndarray - data to represent (after coding)
         - **ref** : unused
         - **coding**: unused
         - **dtype**: string (default None) - numpy.dtype to apply
-        '''
+        """
         super().__init__(data, dtype=dtype, unidim=unidim)
 
     def to_json(self):
-        ''' return a JsonValue of the Dfull entity.'''
+        """return a JsonValue of the Dfull entity."""
         return Dutil.list_json(self.data)
 
     @property
     def values(self):
-        ''' return the list of values'''
+        """return the list of values"""
         return self.data
 
     @property
     def _len_val(self):
-        '''return the length of the Dfull entity'''
+        """return the length of the Dfull entity"""
         return len(self.data) if self.data.ndim > 0 else 0
 
 
 class Dcomplete(Darray):
-    ''' Representation of a one dimensional Array with full representation
+    """Representation of a one dimensional Array with full representation
 
     *dynamic values (@property)*
     - `values`
 
     *methods*
     - `read_json` (staticmethod)
     - `to_json`
-    '''
+    """
 
     def __init__(self, data, ref=None, coding=None, dtype=None, unidim=False):
-        '''Dcomplete constructor.
+        """Dcomplete constructor.
 
         *Parameters*
 
         - **data**: list, Darray or np.ndarray - data to represent (after coding)
         - **ref** : unused
         - **coding**: List of integer (default None) - mapping between data and the list of values
         - **dtype**: string (default None) - numpy.dtype to apply
-        '''
+        """
         if coding is None:
             try:
                 data, coding = np.unique(data, return_inverse=True)
             except (TypeError, ValueError):
-                dat, idx, coding = np.unique(np.frompyfunc(Ntv.from_obj, 1, 1)(data),
-                                             return_index=True, return_inverse=True)
+                dat, idx, coding = np.unique(
+                    np.frompyfunc(Ntv.from_obj, 1, 1)(data),
+                    return_index=True,
+                    return_inverse=True,
+                )
                 data = data[idx]
         super().__init__(data, coding=coding, dtype=dtype, unidim=unidim)
 
     def to_json(self):
-        ''' return a JsonValue of the Dcomplete entity.'''
+        """return a JsonValue of the Dcomplete entity."""
         return [Dutil.list_json(self.data), self.coding.tolist()]
 
     @property
     def values(self):
-        ''' return the list of values'''
+        """return the list of values"""
         return self.data[self.coding]
 
     @property
     def _len_val(self):
-        '''return the length of the Dcomplete entity'''
+        """return the length of the Dcomplete entity"""
         return len(self.coding) if self.coding.ndim > 0 else 0
 
 
 class Dutil:
-    '''np.ndarray utilities.
+    """np.ndarray utilities.
 
     *static methods*
     - `convert`
     - `is_json`
     - `ntv_val`
     - `add_ext`
     - `split_type`
     - `ntv_type`
     - `nda_ntv_type`
     - `dtype`
     - `json_ntv`
     - `split_name`
     - `split_json_name`
-    '''
+    """
 
     @staticmethod
     def equals(nself, nother):
-        '''return True if all elements are equals and dtype are equal'''
+        """return True if all elements are equals and dtype are equal"""
         if not (isinstance(nself, np.ndarray) and isinstance(nother, np.ndarray)):
             return False
         if nself.dtype != nother.dtype or nself.shape != nother.shape:
             return False
         if len(nself.shape) == 0:
             return True
         if len(nself) != len(nother):
             return False
         if len(nself) == 0:
             return True
         if isinstance(nself[0], (np.ndarray, pd.Series, pd.DataFrame)):
-            SeriesConnec = NtvConnector.connector().get('SeriesConnec')
-            DataFrameConnec = NtvConnector.connector().get('DataFrameConnec')
-            equal = {np.ndarray: Dutil.equals,
-                     pd.Series: SeriesConnec.equals,
-                     pd.DataFrame: DataFrameConnec.equals}
+            SeriesConnec = NtvConnector.connector().get("SeriesConnec")
+            DataFrameConnec = NtvConnector.connector().get("DataFrameConnec")
+            equal = {
+                np.ndarray: Dutil.equals,
+                pd.Series: SeriesConnec.equals,
+                pd.DataFrame: DataFrameConnec.equals,
+            }
             for nps, npo in zip(nself, nother):
                 if not equal[type(nself[0])](nps, npo):
                     return False
             return True
         return np.array_equal(nself, nother)
 
     @staticmethod
     def list_json(nda):
-        '''return a JSON representation of a unidimensional np.ndarray'''
+        """return a JSON representation of a unidimensional np.ndarray"""
         if len(nda) == 0:
             return []
         if isinstance(nda[0], np.ndarray):
             return [Dutil.list_json(arr) for arr in nda]
         return nda.tolist()
```

### Comparing `ntv_numpy-0.2.1/ntv_numpy/ndarray.py` & `ntv_numpy-0.2.2/ntv_numpy/ndarray.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,33 +22,33 @@
 import numpy as np
 from json_ntv import Ntv, ShapelyConnec, NtvConnector  # , Datatype
 from ntv_numpy.data_array import Dfull, Dcomplete, Darray, Dutil
 from ntv_numpy.ndtype import Ndtype, NP_NTYPE
 
 
 class Ndarray:
-    ''' The Ndarray class is the JSON interface of numpy.ndarrays.
+    """The Ndarray class is the JSON interface of numpy.ndarrays.
 
     *static methods*
     - `read_json`
     - `to_json`
     - `set_shape`
-    '''
+    """
 
     def __init__(self, dar, ntv_type=None, shape=None, str_uri=True):
-        '''Ndarray constructor.
+        """Ndarray constructor.
 
         *Parameters*
 
         - **dar**: Darray or np.ndarray - data to represent
         - **shape** : list of integer (default None) - length of dimensions
         - **ntv_type**: string (default None) - NTVtype to apply
         - **str_uri**: boolean(default True) - if True and dar is a string,
         dar is an uri else a np.array
-        '''
+        """
         dar = [None] if isinstance(dar, list) and len(dar) == 0 else dar
         if isinstance(dar, Ndarray):
             self.uri = dar.uri
             self.is_json = dar.is_json
             self.ntvtype = dar.ntvtype
             self.shape = dar.shape
             self.darray = dar.darray
@@ -70,289 +70,333 @@
         self.uri = None
         self.is_json = Nutil.is_json(dar[0])
         self.ntvtype = Ndtype(ntv_type)
         self.shape = shape
         self.darray = dar.astype(Nutil.dtype(str(self.ntvtype)))
 
     def __repr__(self):
-        '''return classname, the shape and the ntv_type'''
-        uri = self.uri if self.uri else ''
-        typ = self.ntv_type if self.ntv_type else ''
-        sha = str(self.shape) if self.shape else ''
-        u_t = ', ' if uri and typ + sha else ''
-        t_s = ', ' if typ and sha else ''
-        return self.__class__.__name__ + '(' + uri + u_t + typ + t_s + sha + ')'
+        """return classname, the shape and the ntv_type"""
+        uri = self.uri if self.uri else ""
+        typ = self.ntv_type if self.ntv_type else ""
+        sha = str(self.shape) if self.shape else ""
+        u_t = ", " if uri and typ + sha else ""
+        t_s = ", " if typ and sha else ""
+        return self.__class__.__name__ + "(" + uri + u_t + typ + t_s + sha + ")"
 
     def __str__(self):
-        '''return json string format'''
+        """return json string format"""
         return json.dumps(self.to_json())
 
     def __eq__(self, other):
-        ''' equal if attributes are equal'''
+        """equal if attributes are equal"""
         if self.ntv_type != other.ntv_type:
             return False
         if self.uri != other.uri:
             return False
         if self.shape != other.shape:
             return False
         if self.darray is None and other.darray is None:
             return True
         if self.darray is None or other.darray is None:
             return False
         return Dutil.equals(self.darray, other.darray)
 
     def __len__(self):
-        ''' len of ndarray'''
+        """len of ndarray"""
         return len(self.darray) if self.darray is not None else 0
 
     def __contains__(self, item):
-        ''' item of darray values'''
+        """item of darray values"""
         return item in self.darray if self.darray is not None else None
 
     def __getitem__(self, ind):
-        ''' return darray value item'''
+        """return darray value item"""
         if self.darray is None:
             return None
         if isinstance(ind, tuple):
             return [self.darray[i] for i in ind]
         return self.darray[ind]
 
     def __copy__(self):
-        ''' Copy all the data '''
+        """Copy all the data"""
         return self.__class__(self)
 
     def __array__(self):
-        '''numpy array interface'''
+        """numpy array interface"""
         return self.ndarray
 
     @property
     def ntv_type(self):
-        ''' string representation of ntvtype'''
+        """string representation of ntvtype"""
         return str(self.ntvtype) if self.ntvtype else None
 
     @property
     def ndarray(self):
-        '''representation with a np.ndarray not flattened'''
+        """representation with a np.ndarray not flattened"""
         return self.darray.reshape(self.shape) if self.darray is not None else None
 
     def set_shape(self, shape):
-        '''update the shape'''
+        """update the shape"""
         if Ndarray.len_shape(shape) != len(self.darray):
-            raise NdarrayError(
-                "shape is not consistent with the ndarray length")
+            raise NdarrayError("shape is not consistent with the ndarray length")
         self.shape = list(shape)
 
     def update(self, nda, nda_uri=True):
-        '''update uri and darray and return the result (True, False)
+        """update uri and darray and return the result (True, False)
 
         *Parameters*
 
         - **nda** : string, list, np.ndarray, Ndarray - data to include
         - **nda_uri** : boolean (default True) - if True, existing shape and
-        ntv_type are not updated (but are created if not existing)'''
-        if not nda_uri and not (self.shape is None or nda.shape is None
-                                ) and self.shape != nda.shape:
+        ntv_type are not updated (but are created if not existing)"""
+        if (
+            not nda_uri
+            and not (self.shape is None or nda.shape is None)
+            and self.shape != nda.shape
+        ):
             return False
-        if not nda_uri and not (self.ntv_type is None or nda.ntv_type is None
-                                ) and self.ntv_type != nda.ntv_type:
+        if (
+            not nda_uri
+            and not (self.ntv_type is None or nda.ntv_type is None)
+            and self.ntv_type != nda.ntv_type
+        ):
             return False
         if nda_uri:
             len_s = self.len_shape(self.shape)
             if len_s and len(nda) and len_s != len(nda):
                 return False
             self.ntvtype = nda.ntvtype if self.ntv_type is None else self.ntvtype
             self.shape = nda.shape if self.shape is None else self.shape
         else:
             self.ntvtype = nda.ntvtype if nda.ntv_type is not None else self.ntvtype
             self.shape = nda.shape if nda.shape is not None else self.shape
-        self.uri, self.darray = (
-            nda.uri, None) if nda.uri else (None, nda.darray)
+        self.uri, self.darray = (nda.uri, None) if nda.uri else (None, nda.darray)
         return True
 
     def set_array(self, darray):
-        '''set a new darray and remove uri, return the result (True, False)
+        """set a new darray and remove uri, return the result (True, False)
 
         *Parameters*
 
-        - **darray** : list, np.ndarray, Ndarray - data to include'''
+        - **darray** : list, np.ndarray, Ndarray - data to include"""
         ndarray = Ndarray(darray)
         darray = ndarray.darray
         ntv_type = ndarray.ntv_type
         shape = ndarray.shape
         new_shape = shape if self.shape is None else self.shape
         new_ntv_type = ntv_type if self.ntv_type is None else self.ntv_type
-        if (len(darray) != Ndarray.len_shape(new_shape) or
-                new_ntv_type != ntv_type or new_shape != shape):
+        if (
+            len(darray) != Ndarray.len_shape(new_shape)
+            or new_ntv_type != ntv_type
+            or new_shape != shape
+        ):
             return False
         self.uri = None
         self.darray = darray
         self.ntvtype = Ndtype(new_ntv_type)
         self.shape = new_shape
         return True
 
     def set_uri(self, uri, no_ntv_type=False, no_shape=False):
-        '''set a new uri and remove ndarray and optionaly ntv_type and shape.
+        """set a new uri and remove ndarray and optionaly ntv_type and shape.
         Return the result (True, False)
 
         *Parameters*
 
         - **uri** : string - URI of the Ndarray
         - **no_ntv_type** : boolean (default False) - If True, ntv_type is None
         - **no_shape** : boolean (default False) - If True, shape is None
-        '''
+        """
         if not isinstance(uri, str) or not uri:
             return False
         self.uri = uri
         self.darray = None
         self.ntvtype = None if no_ntv_type else self.ntvtype
         self.shape = None if no_shape else self.shape
         return True
 
     def to_ndarray(self):
-        '''representation with a np.ndarray not flattened'''
+        """representation with a np.ndarray not flattened"""
         return self.ndarray
 
     @property
     def mode(self):
-        '''representation mode of the darray/uri data (relative, absolute,
-        undefined, inconsistent)'''
+        """representation mode of the darray/uri data (relative, absolute,
+        undefined, inconsistent)"""
         match [self.darray, self.uri]:
             case [None, str()]:
-                return 'relative'
+                return "relative"
             case [None, None]:
-                return 'undefined'
+                return "undefined"
             case [_, None]:
-                return 'absolute'
+                return "absolute"
             case _:
-                return 'inconsistent'
+                return "inconsistent"
 
     @staticmethod
     def read_json(jsn, **kwargs):
-        ''' convert json ntv_value into a ndarray.
+        """convert json ntv_value into a ndarray.
 
         *Parameters*
 
         - **convert** : boolean (default True) - If True, convert json data with
         non Numpy ntv_type into data with python type
-        '''
-        option = {'convert': True} | kwargs
+        """
+        option = {"convert": True} | kwargs
         jso = json.loads(jsn) if isinstance(jsn, str) else jsn
-        ntv_value, = Ntv.decode_json(jso)[:1]
+        (ntv_value,) = Ntv.decode_json(jso)[:1]
 
         ntv_type = None
         shape = None
         match ntv_value[:-1]:
-            case []: ...
-            case [ntv_type, shape]: ...
-            case [str(ntv_type)]: ...
-            case [list(shape)]: ...
+            case []:
+                ...
+            case [ntv_type, shape]:
+                ...
+            case [str(ntv_type)]:
+                ...
+            case [list(shape)]:
+                ...
         unidim = shape is not None
         if isinstance(ntv_value[-1], str):
             return Ndarray(ntv_value[-1], shape=shape, ntv_type=ntv_type)
-        darray = Darray.read_json(ntv_value[-1], dtype=Nutil.dtype(ntv_type),
-                                  unidim=unidim)
-        darray.data = Nutil.convert(ntv_type, darray.data, tojson=False,
-                                    convert=option['convert'])
+        darray = Darray.read_json(
+            ntv_value[-1], dtype=Nutil.dtype(ntv_type), unidim=unidim
+        )
+        darray.data = Nutil.convert(
+            ntv_type, darray.data, tojson=False, convert=option["convert"]
+        )
         return Ndarray(darray.values, shape=shape, ntv_type=ntv_type)
 
     def to_json(self, **kwargs):
-        ''' convert a Ndarray into json-value
+        """convert a Ndarray into json-value
 
         *Parameters*
 
         - **noshape** : Boolean (default True) - if True, without shape if dim < 1
         - **notype** : Boolean (default False) - including data type if False
         - **novalue** : Boolean (default False) - including value if False
         - **format** : string (default 'full') - representation format of the ndarray,
         - **encoded** : Boolean (default False) - json-value if False else json-text
         - **header** : Boolean (default True) - including ndarray type
-        '''
-        option = {'format': 'full', 'header': True, 'encoded': False,
-                  'notype': False, 'noshape': True, 'novalue': False} | kwargs
-        if self.mode in ['undefined', 'inconsistent']:
+        """
+        option = {
+            "format": "full",
+            "header": True,
+            "encoded": False,
+            "notype": False,
+            "noshape": True,
+            "novalue": False,
+        } | kwargs
+        if self.mode in ["undefined", "inconsistent"]:
             return None
-        if self.mode == 'absolute' and len(self.darray) == 0:
+        if self.mode == "absolute" and len(self.darray) == 0:
             return [[]]
 
-        shape = None if not self.shape or (len(self.shape) < 2 and
-                                           option['noshape']) else self.shape
+        shape = (
+            None
+            if not self.shape or (len(self.shape) < 2 and option["noshape"])
+            else self.shape
+        )
 
-        if self.mode == 'relative':
+        if self.mode == "relative":
             js_val = self.uri
         else:
-            js_val = Nutil.ntv_val(self.ntv_type, self.darray, option['format'],
-                                   self.is_json) if not option['novalue'] else ['-']
-
-        lis = [self.ntv_type if not option['notype'] else None, shape, js_val]
-        return Nutil.json_ntv(None, 'ndarray',
-                              [val for val in lis if val is not None],
-                              header=option['header'], encoded=option['encoded'])
+            js_val = (
+                Nutil.ntv_val(
+                    self.ntv_type, self.darray, option["format"], self.is_json
+                )
+                if not option["novalue"]
+                else ["-"]
+            )
+
+        lis = [self.ntv_type if not option["notype"] else None, shape, js_val]
+        return Nutil.json_ntv(
+            None,
+            "ndarray",
+            [val for val in lis if val is not None],
+            header=option["header"],
+            encoded=option["encoded"],
+        )
 
     @property
     def info(self):
-        ''' infos of the Ndarray'''
-        inf = {'shape': self.shape}
-        inf['length'] = len(self)
-        inf['ntvtype'] = self.ntv_type
-        inf['shape'] = self.shape
-        inf['uri'] = self.uri
+        """infos of the Ndarray"""
+        inf = {"shape": self.shape}
+        inf["length"] = len(self)
+        inf["ntvtype"] = self.ntv_type
+        inf["shape"] = self.shape
+        inf["uri"] = self.uri
         return {key: val for key, val in inf.items() if val}
 
     @staticmethod
     def len_shape(shape):
-        '''return a length from a shape (product of dimensions)'''
+        """return a length from a shape (product of dimensions)"""
         if not shape:
             return 0
         prod = 1
         for dim in shape:
             prod *= dim
         return prod
 
 
 class Nutil:
-    '''ntv-ndarray utilities.
+    """ntv-ndarray utilities.
 
     *static methods*
     - `convert`
     - `is_json`
     - `ntv_val`
     - `add_ext`
     - `split_type`
     - `ntv_type`
     - `nda_ntv_type`
     - `dtype`
     - `json_ntv`
     - `split_name`
     - `split_json_name`
 
-    '''
-    CONNECTOR_DT = {'field': 'Series', 'tab': 'DataFrame'}
-    PYTHON_DT = {'array': 'list', 'time': 'datetime.time',
-                 'object': 'dict', 'null': 'NoneType', 'decimal64': 'Decimal',
-                 'ndarray': 'ndarray', 'narray': 'narray'}
-    LOCATION_DT = {'point': 'Point',
-                   'line': 'LineString', 'polygon': 'Polygon'}
+    """
+
+    CONNECTOR_DT = {"field": "Series", "tab": "DataFrame"}
+    PYTHON_DT = {
+        "array": "list",
+        "time": "datetime.time",
+        "object": "dict",
+        "null": "NoneType",
+        "decimal64": "Decimal",
+        "ndarray": "ndarray",
+        "narray": "narray",
+    }
+    LOCATION_DT = {"point": "Point", "line": "LineString", "polygon": "Polygon"}
     DT_CONNECTOR = {val: key for key, val in CONNECTOR_DT.items()}
     DT_PYTHON = {val: key for key, val in PYTHON_DT.items()}
     DT_LOCATION = {val: key for key, val in LOCATION_DT.items()}
     DT_NTVTYPE = DT_LOCATION | DT_CONNECTOR | DT_PYTHON
 
-    FORMAT_CLS = {'full': Dfull, 'complete': Dcomplete}
-    STRUCT_DT = {'Ntv': 'object', 'NtvSingle': 'object', 'NtvList': 'object'}
-    CONVERT_DT = {'object': 'object', 'array': 'object', 'json': 'object',
-                  'number': 'float', 'boolean': 'bool', 'null': 'object',
-                  'string': 'str', 'integer': 'int'}
+    FORMAT_CLS = {"full": Dfull, "complete": Dcomplete}
+    STRUCT_DT = {"Ntv": "object", "NtvSingle": "object", "NtvList": "object"}
+    CONVERT_DT = {
+        "object": "object",
+        "array": "object",
+        "json": "object",
+        "number": "float",
+        "boolean": "bool",
+        "null": "object",
+        "string": "str",
+        "integer": "int",
+    }
 
     @staticmethod
     def is_json(obj):
-        ''' check if obj is a json structure and return True if obj is a json-value
+        """check if obj is a json structure and return True if obj is a json-value
 
         *Parameters*
 
-        - **obj** : object to check'''
+        - **obj** : object to check"""
         if obj is None:
             return True
         is_js = NtvConnector.is_json
         match obj:
             case str() | int() | float() | bool():
                 return True
             case list() | tuple() as obj:
@@ -366,233 +410,233 @@
                     return False
                 return min(is_js(obj_in) for obj_in in obj.values())
             case _:
                 return False
 
     @staticmethod
     def extend_array(arr, til, shap, order):
-        '''return a flattened np.ndarray extended in additional dimensions
+        """return a flattened np.ndarray extended in additional dimensions
 
         parameters:
 
         - arr: np.array to extend
         - til: integer - parameter to apply to np.tile function
         - shap: list of integer - shape of the array
         - order: list of integer - order of dimensions to apply
-        '''
+        """
         old_order = list(range(len(order)))
         arr_tab = np.tile(arr, til).reshape(shap)
         return np.moveaxis(arr_tab, old_order, order).flatten()
 
     @staticmethod
     def convert(ntv_type, nda, tojson=True, convert=True):
-        ''' convert np.ndarray with external NTVtype.
+        """convert np.ndarray with external NTVtype.
 
         *Parameters*
 
         - **ntv_type** : string - NTVtype deduced from the np.ndarray name_type and dtype,
         - **nda** : np.ndarray to be converted.
         - **tojson** : boolean (default True) - apply to json function
         - **convert** : boolean (default True) - If True, convert json data with
         non Numpy ntv_type into data with python type
-        '''
+        """
 
         dtype = Nutil.dtype(ntv_type)
         jtype = Nutil.dtype(ntv_type, convert=False)
         if tojson:
             match ntv_type:
-                case dat if Ndtype(dat).category == 'datation':
+                case dat if Ndtype(dat).category == "datation":
                     return nda.astype(dtype).astype(jtype)
-                case 'base16':
+                case "base16":
                     return nda.astype(dtype)
-                case 'time' | 'decimal64':
+                case "time" | "decimal64":
                     return nda.astype(jtype)
-                case 'geojson':
+                case "geojson":
                     return np.frompyfunc(ShapelyConnec.to_geojson, 1, 1)(nda)
                 case _:
                     return nda
         else:
             match [ntv_type, convert]:
                 case [None, _]:
                     return nda
                 case [_, False]:
                     return nda.astype(jtype)
-                case ['time', _]:
+                case ["time", _]:
                     return np.frompyfunc(datetime.time.fromisoformat, 1, 1)(nda)
-                case ['decimal64', _]:
+                case ["decimal64", _]:
                     return np.frompyfunc(Decimal, 1, 1)(nda)
-                case ['narray', _]:
+                case ["narray", _]:
                     nar = np.frompyfunc(Ndarray.read_json, 1, 1)(nda)
                     return np.frompyfunc(Ndarray.to_ndarray, 1, 1)(nar)
-                case ['ndarray', _]:
+                case ["ndarray", _]:
                     return np.frompyfunc(Ndarray.read_json, 1, 1)(nda)
-                case [('point' | 'line' | 'polygon' | 'geometry'), _]:
+                case [("point" | "line" | "polygon" | "geometry"), _]:
                     return np.frompyfunc(ShapelyConnec.to_geometry, 1, 1)(nda)
                 case [connec, _] if connec in Nutil.CONNECTOR_DT:
-                    return np.fromiter([NtvConnector.uncast(nd, None, connec)[0]
-                                        for nd in nda], dtype='object')
+                    return np.fromiter(
+                        [NtvConnector.uncast(nd, None, connec)[0] for nd in nda],
+                        dtype="object",
+                    )
                 case _:
                     return nda.astype(dtype)
 
         # float.fromhex(x.hex()) == x, bytes(bytearray.fromhex(x.hex())) == x
+
     @staticmethod
     def ntv_val(ntv_type, nda, form, is_json=False):
-        ''' convert a np.ndarray into NTV json-value.
+        """convert a np.ndarray into NTV json-value.
 
         *Parameters*
 
         - **ntv_type** : string - NTVtype deduced from the ndarray, name_type and dtype,
         - **nda** : ndarray to be converted.
         - **form** : format of data ('full', 'complete', 'sparse', 'primary').
         - **is_json** : boolean (defaut False) - True if nda data is Json data
-        '''
-        if form == 'complete' and len(nda) < 2:
+        """
+        if form == "complete" and len(nda) < 2:
             raise NdarrayError(
-                "complete format is not available with ndarray length < 2")
+                "complete format is not available with ndarray length < 2"
+            )
         Format = Nutil.FORMAT_CLS[form]
         darray = Format(nda)
         ref = darray.ref
         coding = darray.coding
         if is_json:
             return Format(darray.data, ref=ref, coding=coding).to_json()
         match ntv_type:
-            case 'narray':
-                data = [Ndarray(nd).to_json(header=False)
-                        for nd in darray.data]
-            case 'ndarray':
-                data = [Ndarray(nd).to_json(header=False)
-                        for nd in darray.data]
+            case "narray":
+                data = [Ndarray(nd).to_json(header=False) for nd in darray.data]
+            case "ndarray":
+                data = [Ndarray(nd).to_json(header=False) for nd in darray.data]
             case connec if connec in Nutil.CONNECTOR_DT:
-                data = [NtvConnector.cast(nd, None, connec)[0]
-                        for nd in darray.data]
-            case 'point' | 'line' | 'polygon' | 'geometry':
+                data = [NtvConnector.cast(nd, None, connec)[0] for nd in darray.data]
+            case "point" | "line" | "polygon" | "geometry":
                 data = np.frompyfunc(ShapelyConnec.to_coord, 1, 1)(darray.data)
             case None:
                 data = nda
             case _:
                 data = Nutil.convert(ntv_type, darray.data)
         return Format(data, ref=ref, coding=coding).to_json()
 
     @staticmethod
     def add_ext(typ, ext):
         '''return extended type string: "typ[ext]"'''
-        ext = '[' + ext + ']' if ext else ''
-        return '' if not typ else typ + ext
+        ext = "[" + ext + "]" if ext else ""
+        return "" if not typ else typ + ext
 
     @staticmethod
     def split_type(typ):
-        '''return a tuple with typ and extension'''
+        """return a tuple with typ and extension"""
         if not isinstance(typ, str):
             return (None, None)
-        spl = typ.split('[', maxsplit=1)
+        spl = typ.split("[", maxsplit=1)
         return (spl[0], None) if len(spl) == 1 else (spl[0], spl[1][:-1])
 
     @staticmethod
     def split_json_name(string, notnone=False):
-        '''return a tuple with name, ntv_type from string'''
-        null = '' if notnone else None
-        if not string or string == ':':
+        """return a tuple with name, ntv_type from string"""
+        null = "" if notnone else None
+        if not string or string == ":":
             return (null, null)
-        spl = string.rsplit(':', maxsplit=1)
+        spl = string.rsplit(":", maxsplit=1)
         if len(spl) == 1:
             return (string, null)
-        if spl[0] == '':
+        if spl[0] == "":
             return (null, spl[1])
-        sp0 = spl[0][:-1] if spl[0][-1] == ':' else spl[0]
-        return (null if sp0 == '' else sp0, null if spl[1] == '' else spl[1])
+        sp0 = spl[0][:-1] if spl[0][-1] == ":" else spl[0]
+        return (null if sp0 == "" else sp0, null if spl[1] == "" else spl[1])
 
     @staticmethod
     def split_name(string):
-        '''return a list with name, add_name from string'''
-        if not string or string == '.':
-            return ['', '']
-        spl = string.split('.', maxsplit=1)
-        spl = [spl[0], ''] if len(spl) < 2 else spl
+        """return a list with name, add_name from string"""
+        if not string or string == ".":
+            return ["", ""]
+        spl = string.split(".", maxsplit=1)
+        spl = [spl[0], ""] if len(spl) < 2 else spl
         return spl
 
     @staticmethod
     def ntv_type(dtype, ntv_type=None, ext=None):
-        ''' return ntv_type string from dtype, additional type and extension.
+        """return ntv_type string from dtype, additional type and extension.
 
         *Parameters*
 
         - **dtype** : string - dtype of the ndarray
         - **ntv_type** : string - additional type
         - **ext** : string - type extension
-        '''
-        np_ntype = NP_NTYPE | Nutil.DT_NTVTYPE | {
-            'int': 'int', 'object': 'object'}
+        """
+        np_ntype = NP_NTYPE | Nutil.DT_NTVTYPE | {"int": "int", "object": "object"}
         if ntv_type:
             return Nutil.add_ext(ntv_type, ext)
         match dtype:
-            case string if string[:3] == 'str':
-                return Nutil.add_ext('string', ext)
-            case bytesxx if bytesxx[:5] == 'bytes':
-                return Nutil.add_ext('base16', ext)
+            case string if string[:3] == "str":
+                return Nutil.add_ext("string", ext)
+            case bytesxx if bytesxx[:5] == "bytes":
+                return Nutil.add_ext("base16", ext)
             case dtyp if dtyp in np_ntype:
                 return Nutil.add_ext(np_ntype[dtyp], ext)
-            case date if date[:10] == 'datetime64':
-                return 'datetime' + date[10:]
-            case delta if delta[:11] == 'timedelta64':
-                return 'timedelta' + delta[11:]
+            case date if date[:10] == "datetime64":
+                return "datetime" + date[10:]
+            case delta if delta[:11] == "timedelta64":
+                return "timedelta" + delta[11:]
             case _:
                 return Nutil.add_ext(dtype, ext)
 
     @staticmethod
     def nda_ntv_type(nda, ntv_type=None, ext=None):
-        '''return ntv_type string from an ndarray, additional type and extension.
+        """return ntv_type string from an ndarray, additional type and extension.
 
         *Parameters*
 
         - **nda** : ndarray - data used to calculate the ntv_type
         - **ntv_type** : string - additional type
         - **ext** : string - type extension
-        '''
+        """
         if ntv_type or nda is None:
             return ntv_type
         dtype = nda.dtype.name
         pytype = nda.flat[0].__class__.__name__
-        dtype = pytype if dtype == 'object' and pytype not in Nutil.STRUCT_DT else dtype
+        dtype = pytype if dtype == "object" and pytype not in Nutil.STRUCT_DT else dtype
         return Nutil.ntv_type(dtype, ntv_type, ext)
 
     @staticmethod
     def dtype(ntv_type, convert=True):
-        ''' return dtype from ntv_type
+        """return dtype from ntv_type
 
         *parameters*
 
         - **convert** : boolean (default True) - if True, dtype if from converted data
-        '''
+        """
         if not ntv_type:
             return None
         if convert:
-            if ntv_type[:8] == 'datetime' and ntv_type[8:]:
-                return 'datetime64' + ntv_type[8:]
+            if ntv_type[:8] == "datetime" and ntv_type[8:]:
+                return "datetime64" + ntv_type[8:]
             return Ndtype(ntv_type).dtype
         return Nutil.CONVERT_DT[Ndtype(ntv_type).json_type]
 
     @staticmethod
     def json_ntv(ntv_name, ntv_type, ntv_value, **kwargs):
-        ''' return the JSON representation of a NTV entity
+        """return the JSON representation of a NTV entity
 
         *parameters*
 
         - **ntv_name** : string - name of the NTV
         - **ntv_type** : string - type of the NTV
         - **ntv_value** : string - Json value of the NTV
         - **encoded** : boolean (default False) - if True return JsonText else JsonValue
         - **header** : boolean (default True) - if True include ntv_name + ntv_type
-        '''
-        name = ntv_name if ntv_name else ''
-        option = {'encoded': False, 'header': True} | kwargs
-        if option['header'] or name:
-            typ = ':' + ntv_type if option['header'] and ntv_type else ''
+        """
+        name = ntv_name if ntv_name else ""
+        option = {"encoded": False, "header": True} | kwargs
+        if option["header"] or name:
+            typ = ":" + ntv_type if option["header"] and ntv_type else ""
             jsn = {name + typ: ntv_value} if name + typ else ntv_value
         else:
             jsn = ntv_value
-        if option['encoded']:
+        if option["encoded"]:
             return json.dumps(jsn)
         return jsn
 
 
 class NdarrayError(Exception):
-    '''Multidimensional exception'''
+    """Multidimensional exception"""
```

### Comparing `ntv_numpy-0.2.1/ntv_numpy/ndtype.py` & `ntv_numpy-0.2.2/ntv_numpy/ndtype.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,23 +7,24 @@
 
 It contains the class `Ndtype` for NTVtype with extension.
 
 For more information, see the
 [user guide](https://loco-philippe.github.io/ntv-numpy/docs/user_guide.html)
  or the [github repository](https://github.com/loco-philippe/ntv-numpy).
 """
+
 import configparser
 from pathlib import Path
 import json
 from json_ntv import Datatype
 import ntv_numpy
 
 
 class Ndtype(Datatype):
-    ''' The Ndtype is a child class of Datatype with additional attributes.
+    """The Ndtype is a child class of Datatype with additional attributes.
 
     *Additional attributes :*
     - add_type: additional data added to the JSON ndarray
     - dtype: data type of the np.ndarray
 
     *Inherited attributes :*
     - **name** : String - name of the Datatype
@@ -31,36 +32,39 @@
     - **custom** : boolean - True if not referenced
     - **validate** : function (default None) - validate function
     - **typebase** : TypeBase - TypeBas of the Datatype
     - **extension** : String (default None) - extension of the TypeBase
 
     The methods defined in this class are :
     - `read_ini` (static method)
-    '''
+    """
+
     @staticmethod
     def read_ini():
-        '''return a dict with config data read in ntv_numpy.ini'''
+        """return a dict with config data read in ntv_numpy.ini"""
         config = configparser.ConfigParser()
-        p_file = Path('ntv_numpy.ini')
+        p_file = Path("ntv_numpy.ini")
         config.read(Path(ntv_numpy.__file__).parent / p_file)
-        types = json.loads(config['data']['types'])
-        return {ntv_type: {'add_type': add_type, 'dtype': dtype}
-                for [ntv_type, add_type, dtype] in types}
+        types = json.loads(config["data"]["types"])
+        return {
+            ntv_type: {"add_type": add_type, "dtype": dtype}
+            for [ntv_type, add_type, dtype] in types
+        }
 
     def __init__(self, full_name, module=False, force=False, validate=None):
-        '''NdType constructor.
+        """NdType constructor.
 
         *Parameters*
 
         - **full_name** : String - absolut name of the Datatype
         - **module** : boolean (default False) - if True search data in the
         local .ini file, else in the distant repository
         - **force** : boolean (default False) - if True, no Namespace control
-        - **validate** : function (default None) - validate function to include'''
+        - **validate** : function (default None) - validate function to include"""
         super().__init__(full_name, module=module, force=force, validate=validate)
         np_type = NP_TYPES.get(self.base_name)
-        self.dtype = np_type['dtype'] if np_type else None
-        self.add_type = np_type['add_type'] if np_type else None
+        self.dtype = np_type["dtype"] if np_type else None
+        self.add_type = np_type["add_type"] if np_type else None
 
 
 NP_TYPES = Ndtype.read_ini()
-NP_NTYPE = {val['dtype']: key for key, val in NP_TYPES.items()}
+NP_NTYPE = {val["dtype"]: key for key, val in NP_TYPES.items()}
```

### Comparing `ntv_numpy-0.2.1/ntv_numpy/ntv_numpy.ini` & `ntv_numpy-0.2.2/ntv_numpy/ntv_numpy.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,323 +1,320 @@
 00000000: 5b64 6174 615d 0d0a 0d0a 2320 6465 6669  [data]....# defi
 00000010: 6e65 2074 6865 2063 6174 6567 6f72 6965  ne the categorie
 00000020: 7320 6f66 2064 6174 6120 6465 6669 6e65  s of data define
 00000030: 6420 696e 2027 7479 7065 270d 0a63 6f6c  d in 'type'..col
-00000040: 756d 6e20 3d20 5b0d 0a20 2020 200d 0a20  umn = [..    .. 
-00000050: 2020 2023 2027 6e74 765f 7479 7065 2720     # 'ntv_type' 
-00000060: 6973 2074 6865 2074 7970 6520 6f66 2074  is the type of t
-00000070: 6865 2064 6174 6120 0d0a 2020 2020 226e  he data ..    "n
-00000080: 7476 5f74 7970 6522 2c20 0d0a 2020 2020  tv_type", ..    
-00000090: 0d0a 2020 2020 2320 2761 6464 5f74 7970  ..    # 'add_typ
-000000a0: 6527 2069 7320 7468 6520 6164 6469 7469  e' is the additi
-000000b0: 6f6e 616c 2064 6174 6120 6164 6465 6420  onal data added 
-000000c0: 746f 2074 6865 206e 6461 7272 6179 206f  to the ndarray o
-000000d0: 626a 6563 740d 0a20 2020 2022 6164 645f  bject..    "add_
-000000e0: 7479 7065 222c 200d 0a20 2020 200d 0a20  type", ..    .. 
-000000f0: 2020 2023 2027 6474 7970 6527 2069 7320     # 'dtype' is 
-00000100: 7573 6564 2074 6f20 6465 6669 6e65 2074  used to define t
-00000110: 6865 2064 7479 7065 206f 6620 7468 6520  he dtype of the 
-00000120: 6e64 6172 7261 792c 2069 6620 276e 756c  ndarray, if 'nul
-00000130: 6c27 204e 756d 5079 2063 686f 6f73 6520  l' NumPy choose 
-00000140: 7468 6520 6474 7970 650d 0a20 2020 2022  the dtype..    "
-00000150: 6474 7970 6522 5d0d 0a0d 0a23 2064 6566  dtype"]....# def
-00000160: 696e 6520 7468 6520 7479 7065 7320 7769  ine the types wi
-00000170: 7468 2061 204e 756d 5079 2063 6f6e 7665  th a NumPy conve
-00000180: 7273 696f 6e0d 0a74 7970 6573 2020 203d  rsion..types   =
-00000190: 205b 0d0a 0d0a 2020 2020 2320 7769 7468   [....    # with
-000001a0: 6f75 7420 6e74 765f 7479 7065 200d 0a20  out ntv_type .. 
-000001b0: 2020 2023 2020 2020 2064 7479 7065 2069     #     dtype i
-000001c0: 7320 3a20 2769 6e74 7878 272c 2027 666c  s : 'intxx', 'fl
-000001d0: 6f61 7478 7827 2c20 2762 6f6f 6c65 616e  oatxx', 'boolean
-000001e0: 272c 200d 0a20 2020 2023 2020 2020 2020  ', ..    #      
-000001f0: 2020 2020 2020 2020 2020 6f72 2027 6f62            or 'ob
-00000200: 6a65 6374 2720 286a 736f 6e2d 6172 7261  ject' (json-arra
-00000210: 792c 206a 736f 6e2d 6f62 6a65 6374 290d  y, json-object).
-00000220: 0a20 2020 205b 2222 2c09 0920 2020 2022  .    ["",..    "
-00000230: 6a73 6f6e 222c 2020 2020 206e 756c 6c20  json",     null 
-00000240: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-00000250: 2c0d 0a0d 0a20 2020 2023 2077 6974 6820  ,....    # with 
-00000260: 6e74 765f 7479 7065 206f 6e6c 7920 696e  ntv_type only in
-00000270: 206a 736f 6e20 6461 7461 2028 6e6f 7420   json data (not 
-00000280: 6e75 6d62 6572 7329 2020 2020 0d0a 2020  numbers)    ..  
-00000290: 2020 5b22 6461 7465 222c 0920 2020 206e    ["date",.    n
-000002a0: 756c 6c2c 0920 2020 2022 6461 7465 7469  ull,.    "dateti
-000002b0: 6d65 3634 5b44 5d22 2020 2020 205d 2c20  me64[D]"     ], 
-000002c0: 0d0a 2020 2020 5b22 7965 6172 6d6f 6e74  ..    ["yearmont
-000002d0: 6822 2c20 2020 6e75 6c6c 2c09 2020 2020  h",   null,.    
-000002e0: 2264 6174 6574 696d 6536 345b 4d5d 2220  "datetime64[M]" 
-000002f0: 2020 2020 5d2c 200d 0a20 2020 205b 2279      ], ..    ["y
-00000300: 6561 7222 2c09 2020 2020 6e75 6c6c 2c09  ear",.    null,.
-00000310: 2020 2020 2264 6174 6574 696d 6536 345b      "datetime64[
-00000320: 595d 2220 2020 2020 5d2c 0d0a 2020 2020  Y]"     ],..    
-00000330: 5b22 7374 7269 6e67 222c 0920 2020 206e  ["string",.    n
-00000340: 756c 6c2c 0920 2020 2022 7374 7222 2020  ull,.    "str"  
-00000350: 2020 2020 2020 2020 2020 2020 205d 2c0d               ],.
-00000360: 0a0d 0a20 2020 2023 2077 6974 6820 6e74  ...    # with nt
-00000370: 765f 7479 7065 206f 6e6c 7920 696e 206a  v_type only in j
-00000380: 736f 6e20 6461 7461 2061 6e64 2077 6974  son data and wit
-00000390: 6820 4e54 5674 7970 6520 6578 7465 6e73  h NTVtype extens
-000003a0: 696f 6e20 286e 6f74 206e 756d 6265 7273  ion (not numbers
-000003b0: 2920 2020 200d 0a20 2020 205b 2264 6174  )    ..    ["dat
-000003c0: 6574 696d 6522 2c09 6e75 6c6c 2c09 2020  etime",.null,.  
-000003d0: 2020 2264 6174 6574 696d 6536 345b 735d    "datetime64[s]
-000003e0: 2220 2020 2020 5d2c 0d0a 2020 2020 5b22  "     ],..    ["
-000003f0: 7469 6d65 6465 6c74 6122 2c09 6e75 6c6c  timedelta",.null
-00000400: 2c09 2020 2020 2274 696d 6564 656c 7461  ,.    "timedelta
-00000410: 3634 5b73 5d22 2020 2020 5d2c 0d0a 0d0a  64[s]"    ],....
-00000420: 2020 2020 2320 7769 7468 206e 7476 5f74      # with ntv_t
-00000430: 7970 6520 6f6e 6c79 2069 6e20 6a73 6f6e  ype only in json
-00000440: 2064 6174 6120 286e 756d 6265 7273 2061   data (numbers a
-00000450: 6e64 2062 7974 6573 2920 2020 200d 0a20  nd bytes)    .. 
-00000460: 2020 205b 2266 6c6f 6174 3136 222c 0920     ["float16",. 
-00000470: 2020 206e 756c 6c2c 0920 2020 2022 666c     null,.    "fl
-00000480: 6f61 7431 3622 2020 2020 2020 2020 2020  oat16"          
-00000490: 205d 2c0d 0a20 2020 205b 2266 6c6f 6174   ],..    ["float
-000004a0: 3332 222c 0920 2020 206e 756c 6c2c 0920  32",.    null,. 
-000004b0: 2020 2022 666c 6f61 7433 3222 2020 2020     "float32"    
-000004c0: 2020 2020 2020 205d 2c0d 0a20 2020 205b         ],..    [
-000004d0: 2266 6c6f 6174 3634 222c 0920 2020 206e  "float64",.    n
-000004e0: 756c 6c2c 0920 2020 2022 666c 6f61 7436  ull,.    "float6
-000004f0: 3422 2020 2020 2020 2020 2020 205d 2c0d  4"           ],.
-00000500: 0a20 2020 205b 2266 6c6f 6174 3936 222c  .    ["float96",
-00000510: 0920 2020 206e 756c 6c2c 0920 2020 2022  .    null,.    "
-00000520: 666c 6f61 7439 3622 2020 2020 2020 2020  float96"        
-00000530: 2020 205d 2c0d 0a20 2020 205b 2266 6c6f     ],..    ["flo
-00000540: 6174 3132 3822 2c20 2020 206e 756c 6c2c  at128",    null,
-00000550: 0920 2020 2022 666c 6f61 7431 3238 2220  .    "float128" 
-00000560: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
-00000570: 205b 2275 696e 7438 222c 0920 2020 206e   ["uint8",.    n
-00000580: 756c 6c2c 0920 2020 2022 7569 6e74 3822  ull,.    "uint8"
-00000590: 2020 2020 2020 2020 2020 2020 205d 2c0d               ],.
-000005a0: 0a20 2020 205b 2275 696e 7431 3622 2c09  .    ["uint16",.
-000005b0: 2020 2020 6e75 6c6c 2c09 2020 2020 2275      null,.    "u
-000005c0: 696e 7431 3622 2020 2020 2020 2020 2020  int16"          
-000005d0: 2020 5d2c 0d0a 2020 2020 5b22 7569 6e74    ],..    ["uint
-000005e0: 3332 222c 0920 2020 206e 756c 6c2c 0920  32",.    null,. 
-000005f0: 2020 2022 7569 6e74 3332 2220 2020 2020     "uint32"     
-00000600: 2020 2020 2020 205d 2c0d 0a20 2020 205b         ],..    [
-00000610: 2275 696e 7436 3422 2c09 2020 2020 6e75  "uint64",.    nu
-00000620: 6c6c 2c20 0920 2020 2022 7569 6e74 3634  ll, .    "uint64
-00000630: 2220 2020 2020 2020 2020 2020 205d 2c0d  "            ],.
-00000640: 0a20 2020 205b 2269 6e74 3822 2c09 2020  .    ["int8",.  
-00000650: 2020 6e75 6c6c 2c09 2020 2020 2269 6e74    null,.    "int
-00000660: 3822 2020 2020 2020 2020 2020 2020 2020  8"              
-00000670: 5d2c 0d0a 2020 2020 5b22 696e 7431 3622  ],..    ["int16"
-00000680: 2c09 2020 2020 6e75 6c6c 2c09 2020 2020  ,.    null,.    
-00000690: 2269 6e74 3136 2220 2020 2020 2020 2020  "int16"         
-000006a0: 2020 2020 5d2c 0d0a 2020 2020 5b22 696e      ],..    ["in
-000006b0: 7433 3222 2c09 2020 2020 6e75 6c6c 2c09  t32",.    null,.
-000006c0: 2020 2020 2269 6e74 3332 2220 2020 2020      "int32"     
-000006d0: 2020 2020 2020 2020 5d2c 0d0a 2020 2020          ],..    
-000006e0: 5b22 696e 7436 3422 2c20 2020 2020 2020  ["int64",       
-000006f0: 6e75 6c6c 2c20 2020 0922 696e 7436 3422  null,   ."int64"
-00000700: 2020 2020 2020 2020 2020 2020 205d 2c0d               ],.
-00000710: 0a20 2020 205b 2262 6f6f 6c65 616e 222c  .    ["boolean",
-00000720: 0920 2020 206e 756c 6c2c 2020 2009 2262  .    null,   ."b
-00000730: 6f6f 6c22 2020 2020 2020 2020 2020 2020  ool"            
-00000740: 2020 5d2c 0d0a 2020 2020 5b22 6261 7365    ],..    ["base
-00000750: 3136 222c 0920 2020 206e 756c 6c2c 2020  16",.    null,  
-00000760: 2009 2262 7974 6573 2220 2020 2020 2020   ."bytes"       
-00000770: 2020 2020 2020 5d2c 0d0a 0d0a 2020 2020        ],....    
-00000780: 2320 7769 7468 206e 7476 5f74 7970 6520  # with ntv_type 
-00000790: 636f 6e76 6572 7465 6420 696e 206f 626a  converted in obj
-000007a0: 6563 7420 6474 7970 6520 2873 7461 6e64  ect dtype (stand
-000007b0: 6172 6420 7079 7468 6f6e 2074 7970 6529  ard python type)
-000007c0: 0d0a 2020 2020 5b22 7469 6d65 222c 0920  ..    ["time",. 
-000007d0: 2020 206e 756c 6c2c 0920 2020 2022 6f62     null,.    "ob
-000007e0: 6a65 6374 2220 2020 2020 2020 2020 2020  ject"           
-000007f0: 205d 2c0d 0a20 2020 205b 2261 7272 6179   ],..    ["array
-00000800: 222c 0920 2020 206e 756c 6c2c 0920 2020  ",.    null,.   
-00000810: 2022 6f62 6a65 6374 2220 2020 2020 2020   "object"       
-00000820: 2020 2020 205d 2c0d 0a20 2020 205b 226f       ],..    ["o
-00000830: 626a 6563 7422 2c09 2020 2020 6e75 6c6c  bject",.    null
-00000840: 2c09 2020 2020 226f 626a 6563 7422 2020  ,.    "object"  
-00000850: 2020 2020 2020 2020 2020 5d2c 0d0a 2020            ],..  
-00000860: 2020 5b22 6e75 6c6c 222c 0920 2020 206e    ["null",.    n
-00000870: 756c 6c2c 2009 2020 2020 226f 626a 6563  ull, .    "objec
-00000880: 7422 2020 2020 2020 2020 2020 2020 5d2c  t"            ],
-00000890: 0d0a 2020 2020 5b22 6465 6369 6d61 6c36  ..    ["decimal6
-000008a0: 3422 2c20 2020 6e75 6c6c 2c20 0920 2020  4",   null, .   
-000008b0: 2022 6f62 6a65 6374 2220 2020 2020 2020   "object"       
-000008c0: 2020 2020 205d 2c0d 0a0d 0a20 2020 2023       ],....    #
-000008d0: 2077 6974 6820 6e74 765f 7479 7065 2063   with ntv_type c
-000008e0: 6f6e 7665 7274 6564 2069 6e20 6f62 6a65  onverted in obje
-000008f0: 6374 2064 7479 7065 2028 7079 7468 6f6e  ct dtype (python
-00000900: 206f 626a 6563 7420 290d 0a20 2020 205b   object )..    [
-00000910: 226e 6461 7272 6179 222c 2020 2020 206e  "ndarray",     n
-00000920: 756c 6c2c 2009 2020 2020 226f 626a 6563  ull, .    "objec
-00000930: 7422 2020 2020 2020 2020 2020 2020 5d2c  t"            ],
-00000940: 0d0a 2020 2020 5b22 6e61 7272 6179 222c  ..    ["narray",
-00000950: 2020 2020 2020 6e75 6c6c 2c20 0920 2020        null, .   
-00000960: 2022 6f62 6a65 6374 2220 2020 2020 2020   "object"       
-00000970: 2020 2020 205d 2c0d 0a20 2020 205b 226e       ],..    ["n
-00000980: 7476 222c 0920 2020 2020 2020 206e 756c  tv",.        nul
-00000990: 6c2c 0920 2020 2022 6f62 6a65 6374 2220  l,.    "object" 
-000009a0: 2020 2020 2020 2020 2020 205d 2c0d 0a20             ],.. 
-000009b0: 2020 205b 2270 6f69 6e74 222c 0920 2020     ["point",.   
-000009c0: 206e 756c 6c2c 2020 2009 226f 626a 6563   null,   ."objec
-000009d0: 7422 2020 2020 2020 2020 2020 2020 5d2c  t"            ],
-000009e0: 0d0a 2020 2020 5b22 6c69 6e65 222c 0920  ..    ["line",. 
-000009f0: 2020 206e 756c 6c2c 0920 2020 2022 6f62     null,.    "ob
-00000a00: 6a65 6374 2220 2020 2020 2020 2020 2020  ject"           
-00000a10: 205d 2c0d 0a20 2020 205b 2270 6f6c 7967   ],..    ["polyg
-00000a20: 6f6e 222c 0920 2020 206e 756c 6c2c 0920  on",.    null,. 
-00000a30: 2020 2022 6f62 6a65 6374 2220 2020 2020     "object"     
-00000a40: 2020 2020 2020 205d 2c0d 0a20 2020 205b         ],..    [
-00000a50: 2266 6965 6c64 222c 0920 2020 206e 756c  "field",.    nul
-00000a60: 6c2c 0920 2020 2022 6f62 6a65 6374 2220  l,.    "object" 
-00000a70: 2020 2020 2020 2020 2020 205d 2c0d 0a20             ],.. 
-00000a80: 2020 205b 2274 6162 222c 0920 2020 2020     ["tab",.     
-00000a90: 2020 206e 756c 6c2c 0920 2020 2022 6f62     null,.    "ob
-00000aa0: 6a65 6374 2220 2020 2020 2020 2020 2020  ject"           
-00000ab0: 205d 2c0d 0a0d 0a20 2020 2023 2077 6974   ],....    # wit
-00000ac0: 6820 6e74 765f 7479 7065 2069 6e20 6164  h ntv_type in ad
-00000ad0: 645f 7479 7065 2061 6e64 2069 6e20 6a73  d_type and in js
-00000ae0: 6f6e 2064 6174 6120 286e 756d 6265 7273  on data (numbers
-00000af0: 290d 0a20 2020 205b 226a 736f 6e22 2c09  )..    ["json",.
-00000b00: 2020 2020 226a 736f 6e22 2c20 0922 6f62      "json", ."ob
-00000b10: 6a65 6374 2220 2020 2020 2020 2020 2020  ject"           
-00000b20: 205d 2c0d 0a20 2020 205b 226e 756d 6265   ],..    ["numbe
-00000b30: 7222 2c09 2020 2020 226e 756d 6265 7222  r",.    "number"
-00000b40: 2c09 6e75 6c6c 2020 2020 2020 2020 2020  ,.null          
-00000b50: 2020 2020 2020 5d2c 0d0a 2020 2020 235b        ],..    #[
-00000b60: 226e 756d 6265 7222 2c09 2020 2020 226e  "number",.    "n
-00000b70: 756d 6265 7222 2c09 226f 626a 6563 7422  umber",."object"
-00000b80: 2020 2020 2020 2020 2020 2020 5d2c 0d0a              ],..
-00000b90: 2020 2020 5b22 666c 6f61 7422 2c09 2020      ["float",.  
-00000ba0: 2020 2266 6c6f 6174 222c 0922 666c 6f61    "float",."floa
-00000bb0: 7422 2020 2020 2020 2020 2020 2020 205d  t"             ]
-00000bc0: 2c0d 0a20 2020 205b 2269 6e74 222c 0920  ,..    ["int",. 
-00000bd0: 2020 2020 2020 2022 696e 7422 2c09 2020         "int",.  
-00000be0: 2020 2269 6e74 2220 2020 2020 2020 2020    "int"         
-00000bf0: 2020 2020 2020 5d2c 0d0a 2020 2020 5b22        ],..    ["
-00000c00: 6d6f 6e74 6822 2c09 2020 2020 226d 6f6e  month",.    "mon
-00000c10: 7468 222c 0922 696e 7422 2020 2020 2020  th",."int"      
-00000c20: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
-00000c30: 205b 2264 6179 222c 0920 2020 2020 2020   ["day",.       
-00000c40: 2022 6461 7922 2c09 2020 2020 2269 6e74   "day",.    "int
-00000c50: 2220 2020 2020 2020 2020 2020 2020 2020  "               
-00000c60: 5d2c 0d0a 2020 2020 5b22 7764 6179 222c  ],..    ["wday",
-00000c70: 0920 2020 2022 7764 6179 222c 0920 2020  .    "wday",.   
-00000c80: 2022 696e 7422 2020 2020 2020 2020 2020   "int"          
-00000c90: 2020 2020 205d 2c0d 0a20 2020 205b 2279       ],..    ["y
-00000ca0: 6461 7922 2c09 2020 2020 2279 6461 7922  day",.    "yday"
-00000cb0: 2c09 2020 2020 2269 6e74 2220 2020 2020  ,.    "int"     
-00000cc0: 2020 2020 2020 2020 2020 5d2c 0d0a 2020            ],..  
-00000cd0: 2020 5b22 7765 656b 222c 0920 2020 2022    ["week",.    "
-00000ce0: 7765 656b 222c 0920 2020 2022 696e 7422  week",.    "int"
-00000cf0: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-00000d00: 2c0d 0a20 2020 205b 2268 6f75 7222 2c09  ,..    ["hour",.
-00000d10: 2020 2020 2268 6f75 7222 2c09 2020 2020      "hour",.    
-00000d20: 2269 6e74 2220 2020 2020 2020 2020 2020  "int"           
-00000d30: 2020 2020 5d2c 0d0a 2020 2020 5b22 6d69      ],..    ["mi
-00000d40: 6e75 7465 222c 0920 2020 2022 6d69 6e75  nute",.    "minu
-00000d50: 7465 222c 0922 696e 7422 2020 2020 2020  te",."int"      
-00000d60: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
-00000d70: 205b 2273 6563 6f6e 6422 2c09 2020 2020   ["second",.    
-00000d80: 2273 6563 6f6e 6422 2c09 2269 6e74 2220  "second",."int" 
-00000d90: 2020 2020 2020 2020 2020 2020 2020 5d2c                ],
-00000da0: 2020 2020 0d0a 2020 2020 0d0a 2020 2020      ..    ..    
-00000db0: 2320 7769 7468 206e 7476 5f74 7970 6520  # with ntv_type 
-00000dc0: 696e 2061 6464 5f74 7970 6520 616e 6420  in add_type and 
-00000dd0: 696e 206a 736f 6e20 6461 7461 2028 6e6f  in json data (no
-00000de0: 7420 6e75 6d62 6572 7329 0d0a 2020 2020  t numbers)..    
-00000df0: 5b22 6269 6e61 7279 222c 0920 2020 2022  ["binary",.    "
-00000e00: 6269 6e61 7279 222c 2020 0922 7374 7222  binary",  ."str"
-00000e10: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-00000e20: 2c0d 0a20 2020 205b 2262 6173 6533 3222  ,..    ["base32"
-00000e30: 2c09 2020 2020 2262 6173 6533 3222 2c09  ,.    "base32",.
-00000e40: 2273 7472 2220 2020 2020 2020 2020 2020  "str"           
-00000e50: 2020 2020 5d2c 0d0a 2020 2020 5b22 6261      ],..    ["ba
-00000e60: 7365 3634 222c 0920 2020 2022 6261 7365  se64",.    "base
-00000e70: 3634 222c 0922 7374 7222 2020 2020 2020  64",."str"      
-00000e80: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
-00000e90: 205b 2270 6572 696f 6422 2c09 2020 2020   ["period",.    
-00000ea0: 2270 6572 696f 6422 2c09 2273 7472 2220  "period",."str" 
-00000eb0: 2020 2020 2020 2020 2020 2020 2020 5d2c                ],
-00000ec0: 0d0a 2020 2020 5b22 6475 7261 7469 6f6e  ..    ["duration
-00000ed0: 222c 2020 2020 2264 7572 6174 696f 6e22  ",    "duration"
-00000ee0: 2c09 2273 7472 2220 2020 2020 2020 2020  ,."str"         
-00000ef0: 2020 2020 2020 5d2c 0d0a 2020 2020 5b22        ],..    ["
-00000f00: 6a70 6f69 6e74 6572 222c 2020 2020 226a  jpointer",    "j
-00000f10: 706f 696e 7465 7222 2c09 2273 7472 2220  pointer",."str" 
-00000f20: 2020 2020 2020 2020 2020 2020 2020 5d2c                ],
-00000f30: 0d0a 2020 2020 5b22 7572 6922 2c09 2020  ..    ["uri",.  
-00000f40: 2020 2020 2020 2275 7269 222c 0920 2020        "uri",.   
-00000f50: 2022 7374 7222 2020 2020 2020 2020 2020   "str"          
-00000f60: 2020 2020 205d 2c0d 0a20 2020 205b 2275       ],..    ["u
-00000f70: 7269 7265 6622 2c09 2020 2020 2275 7269  riref",.    "uri
-00000f80: 7265 6622 2c09 2273 7472 2220 2020 2020  ref",."str"     
-00000f90: 2020 2020 2020 2020 2020 5d2c 2020 2020            ],    
-00000fa0: 0d0a 2020 2020 5b22 6972 6922 2c09 2020  ..    ["iri",.  
-00000fb0: 2020 2020 2020 2269 7269 222c 0920 2020        "iri",.   
-00000fc0: 2022 7374 7222 2020 2020 2020 2020 2020   "str"          
-00000fd0: 2020 2020 205d 2c0d 0a20 2020 205b 2269       ],..    ["i
-00000fe0: 7269 7265 6622 2c09 2020 2020 2269 7269  riref",.    "iri
-00000ff0: 7265 6622 2c09 2273 7472 2220 2020 2020  ref",."str"     
-00001000: 2020 2020 2020 2020 2020 5d2c 0d0a 2020            ],..  
-00001010: 2020 5b22 656d 6169 6c22 2c09 2020 2020    ["email",.    
-00001020: 2265 6d61 696c 222c 0922 7374 7222 2020  "email",."str"  
-00001030: 2020 2020 2020 2020 2020 2020 205d 2c0d               ],.
-00001040: 0a20 2020 205b 2272 6567 6578 222c 0920  .    ["regex",. 
-00001050: 2020 2022 7265 6765 7822 2c09 2273 7472     "regex",."str
-00001060: 2220 2020 2020 2020 2020 2020 2020 2020  "               
-00001070: 5d2c 0d0a 2020 2020 5b22 686f 7374 6e61  ],..    ["hostna
-00001080: 6d65 222c 2020 2020 2268 6f73 746e 616d  me",    "hostnam
-00001090: 6522 2c09 2273 7472 2220 2020 2020 2020  e",."str"       
-000010a0: 2020 2020 2020 2020 5d2c 0d0a 2020 2020          ],..    
-000010b0: 5b22 6970 7634 222c 0920 2020 2022 6970  ["ipv4",.    "ip
-000010c0: 7634 222c 0920 2020 2022 7374 7222 2020  v4",.    "str"  
-000010d0: 2020 2020 2020 2020 2020 2020 205d 2c0d               ],.
-000010e0: 0a20 2020 205b 2269 7076 3622 2c09 2020  .    ["ipv6",.  
-000010f0: 2020 2269 7076 3622 2c09 2020 2020 2273    "ipv6",.    "s
-00001100: 7472 2220 2020 2020 2020 2020 2020 2020  tr"             
-00001110: 2020 5d2c 0d0a 2020 2020 5b22 6669 6c65    ],..    ["file
-00001120: 222c 0920 2020 2022 6669 6c65 222c 0920  ",.    "file",. 
-00001130: 2020 2022 7374 7222 2020 2020 2020 2020     "str"        
-00001140: 2020 2020 2020 205d 2c0d 0a20 2020 205b         ],..    [
-00001150: 2267 656f 6a73 6f6e 222c 0920 2020 2022  "geojson",.    "
-00001160: 6765 6f6a 736f 6e22 2c09 2273 7472 2220  geojson",."str" 
-00001170: 2020 2020 2020 2020 2020 2020 2020 5d2c                ],
-00001180: 0d0a 2020 2020 0d0a 2020 2020 2320 7769  ..    ..    # wi
-00001190: 7468 206e 7476 5f74 7970 6520 636f 6e76  th ntv_type conv
-000011a0: 6572 7465 6420 696e 206f 626a 6563 7420  erted in object 
-000011b0: 6474 7970 6520 2870 7974 686f 6e20 7479  dtype (python ty
-000011c0: 7065 290d 0a20 2020 205b 2267 656f 6d65  pe)..    ["geome
-000011d0: 7472 7922 2c20 2020 2022 6765 6f6d 6574  try",    "geomet
-000011e0: 7279 222c 0922 6f62 6a65 6374 2220 2020  ry",."object"   
-000011f0: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
-00001200: 205b 2274 696d 6561 7272 6179 222c 0922   ["timearray",."
-00001210: 7469 6d65 6172 7261 7922 2c22 6f62 6a65  timearray","obje
-00001220: 6374 2220 2020 2020 2020 2020 2020 205d  ct"            ]
-00001230: 0d0a 2020 2020 5d0d 0a0d 0a23 2064 6566  ..    ]....# def
-00001240: 696e 6520 7468 6520 7479 7065 7320 7769  ine the types wi
-00001250: 7468 2061 204e 5456 2063 6f6e 7665 7273  th a NTV convers
-00001260: 696f 6e20 2827 6f74 6865 7274 7970 6527  ion ('othertype'
-00001270: 2069 7320 6e6f 7420 7573 6564 290d 0a6f   is not used)..o
-00001280: 7468 6572 7479 7065 203d 205b 0d0a 2020  thertype = [..  
-00001290: 2020 5b22 6461 7422 2c09 2020 2020 2020    ["dat",.      
-000012a0: 2020 2020 2020 2264 6174 222c 0920 2020        "dat",.   
-000012b0: 2020 2020 2022 6f62 6a65 6374 2220 2020       "object"   
-000012c0: 205d 2c0d 0a20 2020 205b 226d 756c 7469   ],..    ["multi
-000012d0: 706f 696e 7422 2c09 2020 2020 226d 756c  point",.    "mul
-000012e0: 7469 706f 696e 7422 2c20 2020 226f 626a  tipoint",   "obj
-000012f0: 6563 7422 2020 2020 5d2c 0d0a 2020 2020  ect"    ],..    
-00001300: 5b22 6d75 6c74 696c 696e 6522 2c09 2020  ["multiline",.  
-00001310: 2020 226d 756c 7469 6c69 6e65 222c 2020    "multiline",  
-00001320: 2020 226f 626a 6563 7422 2020 2020 5d2c    "object"    ],
-00001330: 0d0a 2020 2020 5b22 6d75 6c74 6970 6f6c  ..    ["multipol
-00001340: 7967 6f6e 222c 0922 6d75 6c74 6970 6f6c  ygon",."multipol
-00001350: 7967 6f6e 222c 0922 6f62 6a65 6374 2220  ygon",."object" 
-00001360: 2020 205d 2c0d 0a20 2020 205b 2262 6f78     ],..    ["box
-00001370: 222c 0920 2020 2020 2020 2020 2020 2022  ",.            "
-00001380: 626f 7822 2c09 2020 2020 2020 2020 226f  box",.        "o
-00001390: 626a 6563 7422 2020 2020 5d2c 0d0a 2020  bject"    ],..  
-000013a0: 2020 5b22 636f 6465 6f6c 6322 2c09 2020    ["codeolc",.  
-000013b0: 2020 2020 2020 2263 6f64 656f 6c63 222c        "codeolc",
-000013c0: 0920 2020 2022 6f62 6a65 6374 2220 2020  .    "object"   
-000013d0: 205d 2c0d 0a20 2020 205b 2272 6f77 222c   ],..    ["row",
-000013e0: 0920 2020 2020 2020 2020 2020 2022 726f  .            "ro
-000013f0: 7722 2c09 2020 2020 2020 2020 226f 626a  w",.        "obj
-00001400: 6563 7422 2020 2020 5d0d 0a20 2020 205d  ect"    ]..    ]
-00001410: 0d0a 0d0a 2320 7265 706c 6163 6520 285c  ....# replace (\
-00001420: 772b 2920 2d3e 2022 2431 222c 0d0a       w+) -> "$1",..
+00000040: 756d 6e20 3d20 5b0d 0a0d 0a20 2020 2023  umn = [....    #
+00000050: 2027 6e74 765f 7479 7065 2720 6973 2074   'ntv_type' is t
+00000060: 6865 2074 7970 6520 6f66 2074 6865 2064  he type of the d
+00000070: 6174 610d 0a20 2020 2022 6e74 765f 7479  ata..    "ntv_ty
+00000080: 7065 222c 0d0a 0d0a 2020 2020 2320 2761  pe",....    # 'a
+00000090: 6464 5f74 7970 6527 2069 7320 7468 6520  dd_type' is the 
+000000a0: 6164 6469 7469 6f6e 616c 2064 6174 6120  additional data 
+000000b0: 6164 6465 6420 746f 2074 6865 206e 6461  added to the nda
+000000c0: 7272 6179 206f 626a 6563 740d 0a20 2020  rray object..   
+000000d0: 2022 6164 645f 7479 7065 222c 0d0a 0d0a   "add_type",....
+000000e0: 2020 2020 2320 2764 7479 7065 2720 6973      # 'dtype' is
+000000f0: 2075 7365 6420 746f 2064 6566 696e 6520   used to define 
+00000100: 7468 6520 6474 7970 6520 6f66 2074 6865  the dtype of the
+00000110: 206e 6461 7272 6179 2c20 6966 2027 6e75   ndarray, if 'nu
+00000120: 6c6c 2720 4e75 6d50 7920 6368 6f6f 7365  ll' NumPy choose
+00000130: 2074 6865 2064 7479 7065 0d0a 2020 2020   the dtype..    
+00000140: 2264 7479 7065 225d 0d0a 0d0a 2320 6465  "dtype"]....# de
+00000150: 6669 6e65 2074 6865 2074 7970 6573 2077  fine the types w
+00000160: 6974 6820 6120 4e75 6d50 7920 636f 6e76  ith a NumPy conv
+00000170: 6572 7369 6f6e 0d0a 7479 7065 7320 2020  ersion..types   
+00000180: 3d20 5b0d 0a0d 0a20 2020 2023 2077 6974  = [....    # wit
+00000190: 686f 7574 206e 7476 5f74 7970 650d 0a20  hout ntv_type.. 
+000001a0: 2020 2023 2020 2020 2064 7479 7065 2069     #     dtype i
+000001b0: 7320 3a20 2769 6e74 7878 272c 2027 666c  s : 'intxx', 'fl
+000001c0: 6f61 7478 7827 2c20 2762 6f6f 6c65 616e  oatxx', 'boolean
+000001d0: 272c 0d0a 2020 2020 2320 2020 2020 2020  ',..    #       
+000001e0: 2020 2020 2020 2020 206f 7220 276f 626a           or 'obj
+000001f0: 6563 7427 2028 6a73 6f6e 2d61 7272 6179  ect' (json-array
+00000200: 2c20 6a73 6f6e 2d6f 626a 6563 7429 0d0a  , json-object)..
+00000210: 2020 2020 5b22 222c 0909 2020 2020 226a      ["",..    "j
+00000220: 736f 6e22 2c20 2020 2020 6e75 6c6c 2020  son",     null  
+00000230: 2020 2020 2020 2020 2020 2020 2020 5d2c                ],
+00000240: 0d0a 0d0a 2020 2020 2320 7769 7468 206e  ....    # with n
+00000250: 7476 5f74 7970 6520 6f6e 6c79 2069 6e20  tv_type only in 
+00000260: 6a73 6f6e 2064 6174 6120 286e 6f74 206e  json data (not n
+00000270: 756d 6265 7273 290d 0a20 2020 205b 2264  umbers)..    ["d
+00000280: 6174 6522 2c09 2020 2020 6e75 6c6c 2c09  ate",.    null,.
+00000290: 2020 2020 2264 6174 6574 696d 6536 345b      "datetime64[
+000002a0: 445d 2220 2020 2020 5d2c 0d0a 2020 2020  D]"     ],..    
+000002b0: 5b22 7965 6172 6d6f 6e74 6822 2c20 2020  ["yearmonth",   
+000002c0: 6e75 6c6c 2c09 2020 2020 2264 6174 6574  null,.    "datet
+000002d0: 696d 6536 345b 4d5d 2220 2020 2020 5d2c  ime64[M]"     ],
+000002e0: 0d0a 2020 2020 5b22 7965 6172 222c 0920  ..    ["year",. 
+000002f0: 2020 206e 756c 6c2c 0920 2020 2022 6461     null,.    "da
+00000300: 7465 7469 6d65 3634 5b59 5d22 2020 2020  tetime64[Y]"    
+00000310: 205d 2c0d 0a20 2020 205b 2273 7472 696e   ],..    ["strin
+00000320: 6722 2c09 2020 2020 6e75 6c6c 2c09 2020  g",.    null,.  
+00000330: 2020 2273 7472 2220 2020 2020 2020 2020    "str"         
+00000340: 2020 2020 2020 5d2c 0d0a 0d0a 2020 2020        ],....    
+00000350: 2320 7769 7468 206e 7476 5f74 7970 6520  # with ntv_type 
+00000360: 6f6e 6c79 2069 6e20 6a73 6f6e 2064 6174  only in json dat
+00000370: 6120 616e 6420 7769 7468 204e 5456 7479  a and with NTVty
+00000380: 7065 2065 7874 656e 7369 6f6e 2028 6e6f  pe extension (no
+00000390: 7420 6e75 6d62 6572 7329 0d0a 2020 2020  t numbers)..    
+000003a0: 5b22 6461 7465 7469 6d65 222c 096e 756c  ["datetime",.nul
+000003b0: 6c2c 0920 2020 2022 6461 7465 7469 6d65  l,.    "datetime
+000003c0: 3634 5b73 5d22 2020 2020 205d 2c0d 0a20  64[s]"     ],.. 
+000003d0: 2020 205b 2274 696d 6564 656c 7461 222c     ["timedelta",
+000003e0: 096e 756c 6c2c 0920 2020 2022 7469 6d65  .null,.    "time
+000003f0: 6465 6c74 6136 345b 735d 2220 2020 205d  delta64[s]"    ]
+00000400: 2c0d 0a0d 0a20 2020 2023 2077 6974 6820  ,....    # with 
+00000410: 6e74 765f 7479 7065 206f 6e6c 7920 696e  ntv_type only in
+00000420: 206a 736f 6e20 6461 7461 2028 6e75 6d62   json data (numb
+00000430: 6572 7320 616e 6420 6279 7465 7329 0d0a  ers and bytes)..
+00000440: 2020 2020 5b22 666c 6f61 7431 3622 2c09      ["float16",.
+00000450: 2020 2020 6e75 6c6c 2c09 2020 2020 2266      null,.    "f
+00000460: 6c6f 6174 3136 2220 2020 2020 2020 2020  loat16"         
+00000470: 2020 5d2c 0d0a 2020 2020 5b22 666c 6f61    ],..    ["floa
+00000480: 7433 3222 2c09 2020 2020 6e75 6c6c 2c09  t32",.    null,.
+00000490: 2020 2020 2266 6c6f 6174 3332 2220 2020      "float32"   
+000004a0: 2020 2020 2020 2020 5d2c 0d0a 2020 2020          ],..    
+000004b0: 5b22 666c 6f61 7436 3422 2c09 2020 2020  ["float64",.    
+000004c0: 6e75 6c6c 2c09 2020 2020 2266 6c6f 6174  null,.    "float
+000004d0: 3634 2220 2020 2020 2020 2020 2020 5d2c  64"           ],
+000004e0: 0d0a 2020 2020 5b22 666c 6f61 7439 3622  ..    ["float96"
+000004f0: 2c09 2020 2020 6e75 6c6c 2c09 2020 2020  ,.    null,.    
+00000500: 2266 6c6f 6174 3936 2220 2020 2020 2020  "float96"       
+00000510: 2020 2020 5d2c 0d0a 2020 2020 5b22 666c      ],..    ["fl
+00000520: 6f61 7431 3238 222c 2020 2020 6e75 6c6c  oat128",    null
+00000530: 2c09 2020 2020 2266 6c6f 6174 3132 3822  ,.    "float128"
+00000540: 2020 2020 2020 2020 2020 5d2c 0d0a 2020            ],..  
+00000550: 2020 5b22 7569 6e74 3822 2c09 2020 2020    ["uint8",.    
+00000560: 6e75 6c6c 2c09 2020 2020 2275 696e 7438  null,.    "uint8
+00000570: 2220 2020 2020 2020 2020 2020 2020 5d2c  "             ],
+00000580: 0d0a 2020 2020 5b22 7569 6e74 3136 222c  ..    ["uint16",
+00000590: 0920 2020 206e 756c 6c2c 0920 2020 2022  .    null,.    "
+000005a0: 7569 6e74 3136 2220 2020 2020 2020 2020  uint16"         
+000005b0: 2020 205d 2c0d 0a20 2020 205b 2275 696e     ],..    ["uin
+000005c0: 7433 3222 2c09 2020 2020 6e75 6c6c 2c09  t32",.    null,.
+000005d0: 2020 2020 2275 696e 7433 3222 2020 2020      "uint32"    
+000005e0: 2020 2020 2020 2020 5d2c 0d0a 2020 2020          ],..    
+000005f0: 5b22 7569 6e74 3634 222c 0920 2020 206e  ["uint64",.    n
+00000600: 756c 6c2c 2009 2020 2020 2275 696e 7436  ull, .    "uint6
+00000610: 3422 2020 2020 2020 2020 2020 2020 5d2c  4"            ],
+00000620: 0d0a 2020 2020 5b22 696e 7438 222c 0920  ..    ["int8",. 
+00000630: 2020 206e 756c 6c2c 0920 2020 2022 696e     null,.    "in
+00000640: 7438 2220 2020 2020 2020 2020 2020 2020  t8"             
+00000650: 205d 2c0d 0a20 2020 205b 2269 6e74 3136   ],..    ["int16
+00000660: 222c 0920 2020 206e 756c 6c2c 0920 2020  ",.    null,.   
+00000670: 2022 696e 7431 3622 2020 2020 2020 2020   "int16"        
+00000680: 2020 2020 205d 2c0d 0a20 2020 205b 2269       ],..    ["i
+00000690: 6e74 3332 222c 0920 2020 206e 756c 6c2c  nt32",.    null,
+000006a0: 0920 2020 2022 696e 7433 3222 2020 2020  .    "int32"    
+000006b0: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
+000006c0: 205b 2269 6e74 3634 222c 2020 2020 2020   ["int64",      
+000006d0: 206e 756c 6c2c 2020 2009 2269 6e74 3634   null,   ."int64
+000006e0: 2220 2020 2020 2020 2020 2020 2020 5d2c  "             ],
+000006f0: 0d0a 2020 2020 5b22 626f 6f6c 6561 6e22  ..    ["boolean"
+00000700: 2c09 2020 2020 6e75 6c6c 2c20 2020 0922  ,.    null,   ."
+00000710: 626f 6f6c 2220 2020 2020 2020 2020 2020  bool"           
+00000720: 2020 205d 2c0d 0a20 2020 205b 2262 6173     ],..    ["bas
+00000730: 6531 3622 2c09 2020 2020 6e75 6c6c 2c20  e16",.    null, 
+00000740: 2020 0922 6279 7465 7322 2020 2020 2020    ."bytes"      
+00000750: 2020 2020 2020 205d 2c0d 0a0d 0a20 2020         ],....   
+00000760: 2023 2077 6974 6820 6e74 765f 7479 7065   # with ntv_type
+00000770: 2063 6f6e 7665 7274 6564 2069 6e20 6f62   converted in ob
+00000780: 6a65 6374 2064 7479 7065 2028 7374 616e  ject dtype (stan
+00000790: 6461 7264 2070 7974 686f 6e20 7479 7065  dard python type
+000007a0: 290d 0a20 2020 205b 2274 696d 6522 2c09  )..    ["time",.
+000007b0: 2020 2020 6e75 6c6c 2c09 2020 2020 226f      null,.    "o
+000007c0: 626a 6563 7422 2020 2020 2020 2020 2020  bject"          
+000007d0: 2020 5d2c 0d0a 2020 2020 5b22 6172 7261    ],..    ["arra
+000007e0: 7922 2c09 2020 2020 6e75 6c6c 2c09 2020  y",.    null,.  
+000007f0: 2020 226f 626a 6563 7422 2020 2020 2020    "object"      
+00000800: 2020 2020 2020 5d2c 0d0a 2020 2020 5b22        ],..    ["
+00000810: 6f62 6a65 6374 222c 0920 2020 206e 756c  object",.    nul
+00000820: 6c2c 0920 2020 2022 6f62 6a65 6374 2220  l,.    "object" 
+00000830: 2020 2020 2020 2020 2020 205d 2c0d 0a20             ],.. 
+00000840: 2020 205b 226e 756c 6c22 2c09 2020 2020     ["null",.    
+00000850: 6e75 6c6c 2c20 0920 2020 2022 6f62 6a65  null, .    "obje
+00000860: 6374 2220 2020 2020 2020 2020 2020 205d  ct"            ]
+00000870: 2c0d 0a20 2020 205b 2264 6563 696d 616c  ,..    ["decimal
+00000880: 3634 222c 2020 206e 756c 6c2c 2009 2020  64",   null, .  
+00000890: 2020 226f 626a 6563 7422 2020 2020 2020    "object"      
+000008a0: 2020 2020 2020 5d2c 0d0a 0d0a 2020 2020        ],....    
+000008b0: 2320 7769 7468 206e 7476 5f74 7970 6520  # with ntv_type 
+000008c0: 636f 6e76 6572 7465 6420 696e 206f 626a  converted in obj
+000008d0: 6563 7420 6474 7970 6520 2870 7974 686f  ect dtype (pytho
+000008e0: 6e20 6f62 6a65 6374 2029 0d0a 2020 2020  n object )..    
+000008f0: 5b22 6e64 6172 7261 7922 2c20 2020 2020  ["ndarray",     
+00000900: 6e75 6c6c 2c20 0920 2020 2022 6f62 6a65  null, .    "obje
+00000910: 6374 2220 2020 2020 2020 2020 2020 205d  ct"            ]
+00000920: 2c0d 0a20 2020 205b 226e 6172 7261 7922  ,..    ["narray"
+00000930: 2c20 2020 2020 206e 756c 6c2c 2009 2020  ,      null, .  
+00000940: 2020 226f 626a 6563 7422 2020 2020 2020    "object"      
+00000950: 2020 2020 2020 5d2c 0d0a 2020 2020 5b22        ],..    ["
+00000960: 6e74 7622 2c09 2020 2020 2020 2020 6e75  ntv",.        nu
+00000970: 6c6c 2c09 2020 2020 226f 626a 6563 7422  ll,.    "object"
+00000980: 2020 2020 2020 2020 2020 2020 5d2c 0d0a              ],..
+00000990: 2020 2020 5b22 706f 696e 7422 2c09 2020      ["point",.  
+000009a0: 2020 6e75 6c6c 2c20 2020 0922 6f62 6a65    null,   ."obje
+000009b0: 6374 2220 2020 2020 2020 2020 2020 205d  ct"            ]
+000009c0: 2c0d 0a20 2020 205b 226c 696e 6522 2c09  ,..    ["line",.
+000009d0: 2020 2020 6e75 6c6c 2c09 2020 2020 226f      null,.    "o
+000009e0: 626a 6563 7422 2020 2020 2020 2020 2020  bject"          
+000009f0: 2020 5d2c 0d0a 2020 2020 5b22 706f 6c79    ],..    ["poly
+00000a00: 676f 6e22 2c09 2020 2020 6e75 6c6c 2c09  gon",.    null,.
+00000a10: 2020 2020 226f 626a 6563 7422 2020 2020      "object"    
+00000a20: 2020 2020 2020 2020 5d2c 0d0a 2020 2020          ],..    
+00000a30: 5b22 6669 656c 6422 2c09 2020 2020 6e75  ["field",.    nu
+00000a40: 6c6c 2c09 2020 2020 226f 626a 6563 7422  ll,.    "object"
+00000a50: 2020 2020 2020 2020 2020 2020 5d2c 0d0a              ],..
+00000a60: 2020 2020 5b22 7461 6222 2c09 2020 2020      ["tab",.    
+00000a70: 2020 2020 6e75 6c6c 2c09 2020 2020 226f      null,.    "o
+00000a80: 626a 6563 7422 2020 2020 2020 2020 2020  bject"          
+00000a90: 2020 5d2c 0d0a 0d0a 2020 2020 2320 7769    ],....    # wi
+00000aa0: 7468 206e 7476 5f74 7970 6520 696e 2061  th ntv_type in a
+00000ab0: 6464 5f74 7970 6520 616e 6420 696e 206a  dd_type and in j
+00000ac0: 736f 6e20 6461 7461 2028 6e75 6d62 6572  son data (number
+00000ad0: 7329 0d0a 2020 2020 5b22 6a73 6f6e 222c  s)..    ["json",
+00000ae0: 0920 2020 2022 6a73 6f6e 222c 2009 226f  .    "json", ."o
+00000af0: 626a 6563 7422 2020 2020 2020 2020 2020  bject"          
+00000b00: 2020 5d2c 0d0a 2020 2020 5b22 6e75 6d62    ],..    ["numb
+00000b10: 6572 222c 0920 2020 2022 6e75 6d62 6572  er",.    "number
+00000b20: 222c 096e 756c 6c20 2020 2020 2020 2020  ",.null         
+00000b30: 2020 2020 2020 205d 2c0d 0a20 2020 2023         ],..    #
+00000b40: 5b22 6e75 6d62 6572 222c 0920 2020 2022  ["number",.    "
+00000b50: 6e75 6d62 6572 222c 0922 6f62 6a65 6374  number",."object
+00000b60: 2220 2020 2020 2020 2020 2020 205d 2c0d  "            ],.
+00000b70: 0a20 2020 205b 2266 6c6f 6174 222c 0920  .    ["float",. 
+00000b80: 2020 2022 666c 6f61 7422 2c09 2266 6c6f     "float",."flo
+00000b90: 6174 2220 2020 2020 2020 2020 2020 2020  at"             
+00000ba0: 5d2c 0d0a 2020 2020 5b22 696e 7422 2c09  ],..    ["int",.
+00000bb0: 2020 2020 2020 2020 2269 6e74 222c 0920          "int",. 
+00000bc0: 2020 2022 696e 7422 2020 2020 2020 2020     "int"        
+00000bd0: 2020 2020 2020 205d 2c0d 0a20 2020 205b         ],..    [
+00000be0: 226d 6f6e 7468 222c 0920 2020 2022 6d6f  "month",.    "mo
+00000bf0: 6e74 6822 2c09 2269 6e74 2220 2020 2020  nth",."int"     
+00000c00: 2020 2020 2020 2020 2020 5d2c 0d0a 2020            ],..  
+00000c10: 2020 5b22 6461 7922 2c09 2020 2020 2020    ["day",.      
+00000c20: 2020 2264 6179 222c 0920 2020 2022 696e    "day",.    "in
+00000c30: 7422 2020 2020 2020 2020 2020 2020 2020  t"              
+00000c40: 205d 2c0d 0a20 2020 205b 2277 6461 7922   ],..    ["wday"
+00000c50: 2c09 2020 2020 2277 6461 7922 2c09 2020  ,.    "wday",.  
+00000c60: 2020 2269 6e74 2220 2020 2020 2020 2020    "int"         
+00000c70: 2020 2020 2020 5d2c 0d0a 2020 2020 5b22        ],..    ["
+00000c80: 7964 6179 222c 0920 2020 2022 7964 6179  yday",.    "yday
+00000c90: 222c 0920 2020 2022 696e 7422 2020 2020  ",.    "int"    
+00000ca0: 2020 2020 2020 2020 2020 205d 2c0d 0a20             ],.. 
+00000cb0: 2020 205b 2277 6565 6b22 2c09 2020 2020     ["week",.    
+00000cc0: 2277 6565 6b22 2c09 2020 2020 2269 6e74  "week",.    "int
+00000cd0: 2220 2020 2020 2020 2020 2020 2020 2020  "               
+00000ce0: 5d2c 0d0a 2020 2020 5b22 686f 7572 222c  ],..    ["hour",
+00000cf0: 0920 2020 2022 686f 7572 222c 0920 2020  .    "hour",.   
+00000d00: 2022 696e 7422 2020 2020 2020 2020 2020   "int"          
+00000d10: 2020 2020 205d 2c0d 0a20 2020 205b 226d       ],..    ["m
+00000d20: 696e 7574 6522 2c09 2020 2020 226d 696e  inute",.    "min
+00000d30: 7574 6522 2c09 2269 6e74 2220 2020 2020  ute",."int"     
+00000d40: 2020 2020 2020 2020 2020 5d2c 0d0a 2020            ],..  
+00000d50: 2020 5b22 7365 636f 6e64 222c 0920 2020    ["second",.   
+00000d60: 2022 7365 636f 6e64 222c 0922 696e 7422   "second",."int"
+00000d70: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+00000d80: 2c0d 0a0d 0a20 2020 2023 2077 6974 6820  ,....    # with 
+00000d90: 6e74 765f 7479 7065 2069 6e20 6164 645f  ntv_type in add_
+00000da0: 7479 7065 2061 6e64 2069 6e20 6a73 6f6e  type and in json
+00000db0: 2064 6174 6120 286e 6f74 206e 756d 6265   data (not numbe
+00000dc0: 7273 290d 0a20 2020 205b 2262 696e 6172  rs)..    ["binar
+00000dd0: 7922 2c09 2020 2020 2262 696e 6172 7922  y",.    "binary"
+00000de0: 2c20 2009 2273 7472 2220 2020 2020 2020  ,  ."str"       
+00000df0: 2020 2020 2020 2020 5d2c 0d0a 2020 2020          ],..    
+00000e00: 5b22 6261 7365 3332 222c 0920 2020 2022  ["base32",.    "
+00000e10: 6261 7365 3332 222c 0922 7374 7222 2020  base32",."str"  
+00000e20: 2020 2020 2020 2020 2020 2020 205d 2c0d               ],.
+00000e30: 0a20 2020 205b 2262 6173 6536 3422 2c09  .    ["base64",.
+00000e40: 2020 2020 2262 6173 6536 3422 2c09 2273      "base64",."s
+00000e50: 7472 2220 2020 2020 2020 2020 2020 2020  tr"             
+00000e60: 2020 5d2c 0d0a 2020 2020 5b22 7065 7269    ],..    ["peri
+00000e70: 6f64 222c 0920 2020 2022 7065 7269 6f64  od",.    "period
+00000e80: 222c 0922 7374 7222 2020 2020 2020 2020  ",."str"        
+00000e90: 2020 2020 2020 205d 2c0d 0a20 2020 205b         ],..    [
+00000ea0: 2264 7572 6174 696f 6e22 2c20 2020 2022  "duration",    "
+00000eb0: 6475 7261 7469 6f6e 222c 0922 7374 7222  duration",."str"
+00000ec0: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+00000ed0: 2c0d 0a20 2020 205b 226a 706f 696e 7465  ,..    ["jpointe
+00000ee0: 7222 2c20 2020 2022 6a70 6f69 6e74 6572  r",    "jpointer
+00000ef0: 222c 0922 7374 7222 2020 2020 2020 2020  ",."str"        
+00000f00: 2020 2020 2020 205d 2c0d 0a20 2020 205b         ],..    [
+00000f10: 2275 7269 222c 0920 2020 2020 2020 2022  "uri",.        "
+00000f20: 7572 6922 2c09 2020 2020 2273 7472 2220  uri",.    "str" 
+00000f30: 2020 2020 2020 2020 2020 2020 2020 5d2c                ],
+00000f40: 0d0a 2020 2020 5b22 7572 6972 6566 222c  ..    ["uriref",
+00000f50: 0920 2020 2022 7572 6972 6566 222c 0922  .    "uriref",."
+00000f60: 7374 7222 2020 2020 2020 2020 2020 2020  str"            
+00000f70: 2020 205d 2c0d 0a20 2020 205b 2269 7269     ],..    ["iri
+00000f80: 222c 0920 2020 2020 2020 2022 6972 6922  ",.        "iri"
+00000f90: 2c09 2020 2020 2273 7472 2220 2020 2020  ,.    "str"     
+00000fa0: 2020 2020 2020 2020 2020 5d2c 0d0a 2020            ],..  
+00000fb0: 2020 5b22 6972 6972 6566 222c 0920 2020    ["iriref",.   
+00000fc0: 2022 6972 6972 6566 222c 0922 7374 7222   "iriref",."str"
+00000fd0: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+00000fe0: 2c0d 0a20 2020 205b 2265 6d61 696c 222c  ,..    ["email",
+00000ff0: 0920 2020 2022 656d 6169 6c22 2c09 2273  .    "email",."s
+00001000: 7472 2220 2020 2020 2020 2020 2020 2020  tr"             
+00001010: 2020 5d2c 0d0a 2020 2020 5b22 7265 6765    ],..    ["rege
+00001020: 7822 2c09 2020 2020 2272 6567 6578 222c  x",.    "regex",
+00001030: 0922 7374 7222 2020 2020 2020 2020 2020  ."str"          
+00001040: 2020 2020 205d 2c0d 0a20 2020 205b 2268       ],..    ["h
+00001050: 6f73 746e 616d 6522 2c20 2020 2022 686f  ostname",    "ho
+00001060: 7374 6e61 6d65 222c 0922 7374 7222 2020  stname",."str"  
+00001070: 2020 2020 2020 2020 2020 2020 205d 2c0d               ],.
+00001080: 0a20 2020 205b 2269 7076 3422 2c09 2020  .    ["ipv4",.  
+00001090: 2020 2269 7076 3422 2c09 2020 2020 2273    "ipv4",.    "s
+000010a0: 7472 2220 2020 2020 2020 2020 2020 2020  tr"             
+000010b0: 2020 5d2c 0d0a 2020 2020 5b22 6970 7636    ],..    ["ipv6
+000010c0: 222c 0920 2020 2022 6970 7636 222c 0920  ",.    "ipv6",. 
+000010d0: 2020 2022 7374 7222 2020 2020 2020 2020     "str"        
+000010e0: 2020 2020 2020 205d 2c0d 0a20 2020 205b         ],..    [
+000010f0: 2266 696c 6522 2c09 2020 2020 2266 696c  "file",.    "fil
+00001100: 6522 2c09 2020 2020 2273 7472 2220 2020  e",.    "str"   
+00001110: 2020 2020 2020 2020 2020 2020 5d2c 0d0a              ],..
+00001120: 2020 2020 5b22 6765 6f6a 736f 6e22 2c09      ["geojson",.
+00001130: 2020 2020 2267 656f 6a73 6f6e 222c 0922      "geojson",."
+00001140: 7374 7222 2020 2020 2020 2020 2020 2020  str"            
+00001150: 2020 205d 2c0d 0a0d 0a20 2020 2023 2077     ],....    # w
+00001160: 6974 6820 6e74 765f 7479 7065 2063 6f6e  ith ntv_type con
+00001170: 7665 7274 6564 2069 6e20 6f62 6a65 6374  verted in object
+00001180: 2064 7479 7065 2028 7079 7468 6f6e 2074   dtype (python t
+00001190: 7970 6529 0d0a 2020 2020 5b22 6765 6f6d  ype)..    ["geom
+000011a0: 6574 7279 222c 2020 2020 2267 656f 6d65  etry",    "geome
+000011b0: 7472 7922 2c09 226f 626a 6563 7422 2020  try",."object"  
+000011c0: 2020 2020 2020 2020 2020 5d2c 0d0a 2020            ],..  
+000011d0: 2020 5b22 7469 6d65 6172 7261 7922 2c09    ["timearray",.
+000011e0: 2274 696d 6561 7272 6179 222c 226f 626a  "timearray","obj
+000011f0: 6563 7422 2020 2020 2020 2020 2020 2020  ect"            
+00001200: 5d0d 0a20 2020 205d 0d0a 0d0a 2320 6465  ]..    ]....# de
+00001210: 6669 6e65 2074 6865 2074 7970 6573 2077  fine the types w
+00001220: 6974 6820 6120 4e54 5620 636f 6e76 6572  ith a NTV conver
+00001230: 7369 6f6e 2028 276f 7468 6572 7479 7065  sion ('othertype
+00001240: 2720 6973 206e 6f74 2075 7365 6429 0d0a  ' is not used)..
+00001250: 6f74 6865 7274 7970 6520 3d20 5b0d 0a20  othertype = [.. 
+00001260: 2020 205b 2264 6174 222c 0920 2020 2020     ["dat",.     
+00001270: 2020 2020 2020 2022 6461 7422 2c09 2020         "dat",.  
+00001280: 2020 2020 2020 226f 626a 6563 7422 2020        "object"  
+00001290: 2020 5d2c 0d0a 2020 2020 5b22 6d75 6c74    ],..    ["mult
+000012a0: 6970 6f69 6e74 222c 0920 2020 2022 6d75  ipoint",.    "mu
+000012b0: 6c74 6970 6f69 6e74 222c 2020 2022 6f62  ltipoint",   "ob
+000012c0: 6a65 6374 2220 2020 205d 2c0d 0a20 2020  ject"    ],..   
+000012d0: 205b 226d 756c 7469 6c69 6e65 222c 0920   ["multiline",. 
+000012e0: 2020 2022 6d75 6c74 696c 696e 6522 2c20     "multiline", 
+000012f0: 2020 2022 6f62 6a65 6374 2220 2020 205d     "object"    ]
+00001300: 2c0d 0a20 2020 205b 226d 756c 7469 706f  ,..    ["multipo
+00001310: 6c79 676f 6e22 2c09 226d 756c 7469 706f  lygon",."multipo
+00001320: 6c79 676f 6e22 2c09 226f 626a 6563 7422  lygon",."object"
+00001330: 2020 2020 5d2c 0d0a 2020 2020 5b22 626f      ],..    ["bo
+00001340: 7822 2c09 2020 2020 2020 2020 2020 2020  x",.            
+00001350: 2262 6f78 222c 0920 2020 2020 2020 2022  "box",.        "
+00001360: 6f62 6a65 6374 2220 2020 205d 2c0d 0a20  object"    ],.. 
+00001370: 2020 205b 2263 6f64 656f 6c63 222c 0920     ["codeolc",. 
+00001380: 2020 2020 2020 2022 636f 6465 6f6c 6322         "codeolc"
+00001390: 2c09 2020 2020 226f 626a 6563 7422 2020  ,.    "object"  
+000013a0: 2020 5d2c 0d0a 2020 2020 5b22 726f 7722    ],..    ["row"
+000013b0: 2c09 2020 2020 2020 2020 2020 2020 2272  ,.            "r
+000013c0: 6f77 222c 0920 2020 2020 2020 2022 6f62  ow",.        "ob
+000013d0: 6a65 6374 2220 2020 205d 0d0a 2020 2020  ject"    ]..    
+000013e0: 5d0d 0a0d 0a23 2072 6570 6c61 6365 2028  ]....# replace (
+000013f0: 5c77 2b29 202d 3e20 2224 3122 2c0d 0a    \w+) -> "$1",..
```

### Comparing `ntv_numpy-0.2.1/ntv_numpy/numpy_ntv_connector.py` & `ntv_numpy-0.2.2/ntv_numpy/numpy_ntv_connector.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,181 +14,204 @@
 
 It contains the child classes of `NTV.json_ntv.ntv.NtvConnector` abstract class:
     - `NarrayConnec`: 'narray' connector for np.ndarray data
     - `NdarrayConnec`: 'ndarray'   connector for Ndarray data
     - `XndarrayConnec`: 'xndarray' connector for Xndarray data
     - `XdatasetConnec`: 'xdataset' connector for Xdataset data
 """
+
 from json_ntv import NtvConnector
 
 from ntv_numpy.ndarray import Ndarray
 from ntv_numpy.xndarray import Xndarray
 from ntv_numpy.xdataset import Xdataset
 
 
 class NarrayConnec(NtvConnector):
+    """NTV connector for Numpy ndarray."""
 
-    '''NTV connector for Numpy ndarray.'''
-
-    clas_obj = 'ndarray'
-    clas_typ = 'narray'
+    clas_obj = "ndarray"
+    clas_typ = "narray"
 
     @staticmethod
     def to_obj_ntv(ntv_value, **kwargs):
-        ''' convert json ntv_value into a np.ndarray.
+        """convert json ntv_value into a np.ndarray.
 
         *Parameters*
 
         - **convert** : boolean (default True) - If True, convert json data with
-        non Numpy ntv_type into data with python type'''
+        non Numpy ntv_type into data with python type"""
         return Ndarray.read_json(ntv_value, **kwargs).darray
 
     @staticmethod
     def to_json_ntv(value, name=None, typ=None, **kwargs):
-        ''' convert a np.ndarray (value, name, type) into NTV json (json-value, name, ntv_type).
+        """convert a np.ndarray (value, name, type) into NTV json (json-value, name, ntv_type).
 
         *Parameters*
 
         - **typ** : string (default None) - ntv_type of the np.ndarray object,
         - **name** : string (default None) - name of the ndarray object
         - **value** : np.ndarray value
         - **noshape** : Boolean (default True) - if True, without shape if dim < 1
         - **notype** : Boolean (default False) - including data type if False
         - **novalue** : Boolean (default False) - including value if False
         - **format** : string (default 'full') - representation format of the ndarray,
         - **encoded** : Boolean (default False) - json-value if False else json-text
         - **header** : Boolean (default True) - including ndarray type
-        '''
-        option = {'format': 'full', 'header': True, 'encoded': False,
-                  'notype': False, 'noshape': True, 'novalue': False} | kwargs
-        if not option['format'] in ['full', 'complete']:
-            option['noshape'] = False
-        option['header'] = False
-        return (Ndarray(value).to_json(**option), name, 'narray')
+        """
+        option = {
+            "format": "full",
+            "header": True,
+            "encoded": False,
+            "notype": False,
+            "noshape": True,
+            "novalue": False,
+        } | kwargs
+        if option["format"] not in ["full", "complete"]:
+            option["noshape"] = False
+        option["header"] = False
+        return (Ndarray(value).to_json(**option), name, "narray")
 
 
 class NdarrayConnec(NtvConnector):
+    """NTV connector for Ndarray."""
 
-    '''NTV connector for Ndarray.'''
-
-    clas_obj = 'Ndarray'
-    clas_typ = 'ndarray'
+    clas_obj = "Ndarray"
+    clas_typ = "ndarray"
 
     @staticmethod
     def to_obj_ntv(ntv_value, **kwargs):
-        ''' convert json ntv_value into a Ndarray.
+        """convert json ntv_value into a Ndarray.
 
         *Parameters*
 
         - **convert** : boolean (default True) - If True, convert json data with
-        non-Numpy ntv_type into data with python type'''
+        non-Numpy ntv_type into data with python type"""
         return Ndarray.read_json(ntv_value, **kwargs)
 
     @staticmethod
     def to_json_ntv(value, name=None, typ=None, **kwargs):
-        ''' convert a Ndarray (value, name, type) into NTV json (json-value, name, ntv_type).
+        """convert a Ndarray (value, name, type) into NTV json (json-value, name, ntv_type).
 
         *Parameters*
 
         - **typ** : string (default None) - ntv_type of the ndarray object,
         - **name** : string (default None) - name of the ndarray object
         - **value** : Ndarray value (or np.ndarray value)
         - **noshape** : Boolean (default True) - if True, without shape if dim < 1
         - **notype** : Boolean (default False) - including data type if False
         - **novalue** : Boolean (default False) - including value if False
         - **format** : string (default 'full') - representation format of the ndarray,
         - **encoded** : Boolean (default False) - json-value if False else json-text
         - **header** : Boolean (default True) - including ndarray type
-        '''
-        option = {'format': 'full', 'header': True, 'encoded': False,
-                  'notype': False, 'noshape': True, 'novalue': False} | kwargs
-        if not option['format'] in ['full', 'complete']:
-            option['noshape'] = False
-        return (Ndarray(value).to_json(**option), name, 'ndarray')
+        """
+        option = {
+            "format": "full",
+            "header": True,
+            "encoded": False,
+            "notype": False,
+            "noshape": True,
+            "novalue": False,
+        } | kwargs
+        if option["format"] not in ["full", "complete"]:
+            option["noshape"] = False
+        return (Ndarray(value).to_json(**option), name, "ndarray")
 
 
 class XndarrayConnec(NtvConnector):
+    """NTV connector for Xndarray."""
 
-    '''NTV connector for Xndarray.'''
-
-    clas_obj = 'Xndarray'
-    clas_typ = 'xndarray'
+    clas_obj = "Xndarray"
+    clas_typ = "xndarray"
 
     @staticmethod
     def to_obj_ntv(ntv_value, **kwargs):
-        ''' convert json ntv_value into a Xndarray.
+        """convert json ntv_value into a Xndarray.
 
         *Parameters*
 
         - **convert** : boolean (default True) - If True, convert json data with
         non-umpy ntv_type into Xndarray with python type
-        '''
+        """
         print(ntv_value)
         return Xndarray.read_json(ntv_value, **kwargs)
 
     @staticmethod
     def to_json_ntv(value, name=None, typ=None, **kwargs):
-        ''' convert a Xndarray (value) into NTV json (json-value, name, ntv_type).
+        """convert a Xndarray (value) into NTV json (json-value, name, ntv_type).
 
         *Parameters*
 
         - **typ** : string (default None) - not used,
         - **name** : string (default None) - not used
         - **value** : Xndarray values
         - **encoded** : Boolean (default False) - json-value if False else json-text
         - **header** : Boolean (default True) - including xndarray type
         - **notype** : Boolean (default False) - including data type if False
         - **novalue** : Boolean (default False) - including value if False
         - **noshape** : Boolean (default True) - if True, without shape if dim < 1
         - **format** : string (default 'full') - representation format of the ndarray,
         - **extension** : string (default None) - type extension
-        '''
-        option = {'notype': False, 'extension': None, 'format': 'full',
-                  'noshape': True, 'header': True, 'encoded': False,
-                  'novalue': False, 'noname': False} | kwargs
-        if not option['format'] in ['full', 'complete']:
-            option['noshape'] = False
-        return (value.to_json(**option), name, 'xndarray')
+        """
+        option = {
+            "notype": False,
+            "extension": None,
+            "format": "full",
+            "noshape": True,
+            "header": True,
+            "encoded": False,
+            "novalue": False,
+            "noname": False,
+        } | kwargs
+        if option["format"] not in ["full", "complete"]:
+            option["noshape"] = False
+        return (value.to_json(**option), name, "xndarray")
 
 
 class XdatasetConnec(NtvConnector):
+    """NTV connector for Xdataset."""
 
-    '''NTV connector for Xdataset.'''
-
-    clas_obj = 'Xdataset'
-    clas_typ = 'xdataset'
+    clas_obj = "Xdataset"
+    clas_typ = "xdataset"
 
     @staticmethod
     def to_obj_ntv(ntv_value, **kwargs):  # reindex=True, decode_str=False):
-        ''' convert json ntv_value into a Xdataset.
+        """convert json ntv_value into a Xdataset.
 
         *Parameters*
 
         - **convert** : boolean (default True) - If True, convert json data with
         non-Numpy ntv_type into Xdataset with python type
-        '''
+        """
         return Xdataset.read_json(ntv_value, **kwargs)
 
     @staticmethod
     def to_json_ntv(value, name=None, typ=None, **kwargs):
-        ''' convert a Xdataset (value) into NTV json (json-value, name, ntv_type).
+        """convert a Xdataset (value) into NTV json (json-value, name, ntv_type).
 
         *Parameters*
 
         - **typ** : string (default None) - not used,
         - **name** : string (default None) - not used
         - **value** : Xdataset entity
         - **encoded** : Boolean (default False) - json value if False else json text
         - **header** : Boolean (default True) - including 'xdataset' type
         - **notype** : list of Boolean (default list of None) - including data type if False
         - **novalue** : Boolean (default False) - including value if False
         - **noshape** : Boolean (default False) - if True, without shape if dim < 1
         - **format** : list of string (default list of 'full') - representation format
         of the np.ndarray,
-        '''
-        option = {'notype': False, 'extension': None, 'format': 'full',
-                  'noshape': True, 'header': True, 'encoded': False,
-                  'novalue': False, 'noname': False} | kwargs
-        if not option['format'] in ['full', 'complete']:
-            option['noshape'] = False
-        option['noname'] = True
-        return (value.to_json(**option), name, 'xdataset')
+        """
+        option = {
+            "notype": False,
+            "extension": None,
+            "format": "full",
+            "noshape": True,
+            "header": True,
+            "encoded": False,
+            "novalue": False,
+            "noname": False,
+        } | kwargs
+        if option["format"] not in ["full", "complete"]:
+            option["noshape"] = False
+        option["noname"] = True
+        return (value.to_json(**option), name, "xdataset")
```

### Comparing `ntv_numpy-0.2.1/ntv_numpy/xconnector.py` & `ntv_numpy-0.2.2/ntv_numpy/xconnector.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,221 +13,255 @@
 
 
 For more information, see the
 [user guide](https://loco-philippe.github.io/ntv-numpy/docs/user_guide.html)
  or the [github repository](https://github.com/loco-philippe/ntv-numpy).
 """
 
-
 import xarray as xr
 import scipp as sc
 import pandas as pd
 import numpy as np
 from astropy import wcs
 from astropy.nddata import NDData
 from astropy.nddata.nduncertainty import StdDevUncertainty, VarianceUncertainty
 from astropy.nddata.nduncertainty import InverseVariance
 from ntv_numpy.ndarray import Nutil, Ndarray
 from ntv_numpy.xndarray import Xndarray
 
 
 class AstropyNDDataConnec:
-    ''' NDData interface with two static methods ximport and xexport'''
+    """NDData interface with two static methods ximport and xexport"""
 
     @staticmethod
     def xexport(xdt, **kwargs):
-        '''return a NDData from a Xdataset'''
-        data = xdt['data'].ndarray
-        mask = xdt['data.mask'].ndarray
-        unit = xdt['data'].nda.ntvtype.extension
-        uncert = xdt['data.uncertainty'].ndarray
-        typ_u = xdt['data.uncertainty'].nda.ntvtype.extension
+        """return a NDData from a Xdataset"""
+        data = xdt["data"].ndarray
+        mask = xdt["data.mask"].ndarray
+        unit = xdt["data"].nda.ntvtype.extension
+        uncert = xdt["data.uncertainty"].ndarray
+        typ_u = xdt["data.uncertainty"].nda.ntvtype.extension
         match typ_u:
-            case 'std':
+            case "std":
                 uncertainty = StdDevUncertainty(uncert)
-            case 'var':
+            case "var":
                 uncertainty = VarianceUncertainty(uncert)
-            case 'inv':
+            case "inv":
                 uncertainty = InverseVariance(uncert)
             case _:
                 uncertainty = uncert
-        meta = xdt['meta'].meta | {'name': xdt.name}
-        wcs_dic = xdt['wcs'].meta
-        psf = xdt['psf'].ndarray
-        return NDData(data, mask=mask, unit=unit, uncertainty=uncertainty,
-                      meta=meta, wcs=wcs.WCS(wcs_dic), psf=psf)
+        meta = xdt["meta"].meta | {"name": xdt.name}
+        wcs_dic = xdt["wcs"].meta
+        psf = xdt["psf"].ndarray
+        return NDData(
+            data,
+            mask=mask,
+            unit=unit,
+            uncertainty=uncertainty,
+            meta=meta,
+            wcs=wcs.WCS(wcs_dic),
+            psf=psf,
+        )
 
     @staticmethod
     def ximport(ndd, Xclass, **kwargs):
-        '''return a Xdataset from a astropy.NDData'''
+        """return a Xdataset from a astropy.NDData"""
         xnd = []
-        name = 'no_name'
+        name = "no_name"
         unit = ndd.unit.to_string() if ndd.unit is not None else None
         ntv_type = Nutil.ntv_type(ndd.data.dtype.name, ext=unit)
-        xnd += [Xndarray('data', nda=Ndarray(ndd.data, ntv_type=ntv_type))]
+        xnd += [Xndarray("data", nda=Ndarray(ndd.data, ntv_type=ntv_type))]
         if ndd.meta:
-            meta = {key: val for key, val in ndd.meta.items() if key != 'name'}
-            name = ndd.meta.get('name', 'no_name')
-            xnd += [Xndarray('meta', meta=meta)]
+            meta = {key: val for key, val in ndd.meta.items() if key != "name"}
+            name = ndd.meta.get("name", "no_name")
+            xnd += [Xndarray("meta", meta=meta)]
         if ndd.wcs:
-            xnd += [Xndarray('wcs', meta=dict(ndd.wcs.to_header()))]
+            xnd += [Xndarray("wcs", meta=dict(ndd.wcs.to_header()))]
         if ndd.psf is not None:
-            xnd += [Xndarray('psf', nda=Ndarray(ndd.psf, ntv_type=ntv_type))]
+            xnd += [Xndarray("psf", nda=Ndarray(ndd.psf, ntv_type=ntv_type))]
         if ndd.mask is not None:
-            xnd += [Xndarray('data.mask', nda=ndd.mask)]
+            xnd += [Xndarray("data.mask", nda=ndd.mask)]
         if ndd.uncertainty is not None:
             typ_u = ndd.uncertainty.__class__.__name__[:3].lower()
-            ntv_type = Nutil.ntv_type(
-                ndd.uncertainty.array.dtype.name, ext=typ_u)
+            ntv_type = Nutil.ntv_type(ndd.uncertainty.array.dtype.name, ext=typ_u)
             nda = Ndarray(ndd.uncertainty.array, ntv_type=ntv_type)
-            xnd += [Xndarray('data.uncertainty', nda=nda)]
+            xnd += [Xndarray("data.uncertainty", nda=nda)]
         return Xclass(xnd, name).to_canonical()
 
 
 class PandasConnec:
-    ''' pandas.DataFrame interface with two static methods ximport and xexport'''
+    """pandas.DataFrame interface with two static methods ximport and xexport"""
 
     @staticmethod
     def xexport(xdt, **kwargs):
-        '''return a pd.DataFrame from a Xdataset
+        """return a pd.DataFrame from a Xdataset
 
         *Parameters*
 
         - **ntv_type**: Boolean (default True) - if False use full_name else json_name
         - **info**: Boolean (default True) - if True add xdt.info in DataFrame.attrs
         - **dims**: list of string (default None) - order of dimensions full_name to apply
-        '''
-        opt = {'ntv_type': True, 'info': True, 'dims': None} | kwargs
-        dic_name = {name: xdt[name].json_name if opt['ntv_type'] else xdt[name].full_name
-                    for name in xdt.names}
-        dims = xdt.dimensions if not opt['dims'] else tuple(opt['dims'])
-        fields = (xdt.group(dims) + xdt.group(xdt.coordinates) +
-                  xdt.group(xdt.data_vars) + xdt.uniques)
-        fields += tuple(nam for nam in xdt.group(xdt.data_arrays)
-                        if len(xdt[nam]) == xdt.length)
+        - **index**: Boolean (default True) - if True, dimensions are translated into indexes
+        """
+        opt = {"ntv_type": True, "info": True, "index": True, "dims": None} | kwargs
+        dic_name = {
+            name: xdt[name].json_name if opt["ntv_type"] else xdt[name].full_name
+            for name in xdt.names
+        }
+        dims = xdt.dimensions if not opt["dims"] else tuple(opt["dims"])
+        fields = (
+            xdt.group(dims)
+            + xdt.group(xdt.coordinates)
+            + xdt.group(xdt.data_vars)
+            + xdt.uniques
+        )
+        fields += tuple(
+            nam for nam in xdt.group(xdt.data_arrays) if len(xdt[nam]) == xdt.length
+        )
         fields_array = tuple(var for var in fields if not xdt[var].uri)
-        dic_series = {dic_name[name]: PandasConnec._to_np_series(xdt, name, dims)
-                      for name in fields_array}
+        dic_series = {
+            dic_name[name]: PandasConnec._to_np_series(xdt, name, dims)
+            for name in fields_array
+        }
         dfr = pd.DataFrame(dic_series)
         index = [dic_name[name] for name in dims]
-        if index:
+        if index and opt["index"]:
             dfr = dfr.set_index(index)
-        if opt['info']:
-            dfr.attrs |= {'info': xdt.tab_info}
-            dfr.attrs |= {'metadata': {
-                name: xdt[name].meta for name in xdt.metadata}}
+        if opt["info"]:
+            dfr.attrs |= {"info": xdt.tab_info}
+            dfr.attrs |= {"metadata": {name: xdt[name].meta for name in xdt.metadata}}
             fields_uri = [var for var in fields if var not in fields_array]
-            fields_other = [nam for nam in xdt.group(xdt.data_arrays)
-                            if len(xdt[nam]) != xdt.length]
+            fields_other = [
+                nam for nam in xdt.group(xdt.data_arrays) if len(xdt[nam]) != xdt.length
+            ]
             if fields_uri:
-                dfr.attrs |= {'fields': {nam: xdt[nam].to_json(noname=True,)
-                                         for nam in fields_uri + fields_other}}
+                dfr.attrs |= {
+                    "fields": {
+                        nam: xdt[nam].to_json(
+                            noname=True,
+                        )
+                        for nam in fields_uri + fields_other
+                    }
+                }
             if xdt.name:
-                dfr.attrs |= {'name': xdt.name}
+                dfr.attrs |= {"name": xdt.name}
         return dfr
 
     @staticmethod
     def ximport(df, Xclass, **kwargs):
-        '''return a Xdataset from a pd.DataFrame
+        """return a Xdataset from a pd.DataFrame
 
         *Parameters*
 
         - dims: list of string (default None) - order of dimensions to apply
-        '''
-        opt = {'dims': None} | kwargs
+        """
+        opt = {"dims": None} | kwargs
         xnd = []
         dfr = df.reset_index()
-        if 'index' in dfr.columns and 'index' not in df.columns:
-            del dfr['index']
-        df_names = {Nutil.split_json_name(j_name)[0]: j_name
-                    for j_name in dfr.columns}
-        df_ntv_types = {Nutil.split_json_name(j_name)[0]:
-                        Nutil.split_json_name(j_name)[1] for j_name in dfr.columns}
+        if "index" in dfr.columns and "index" not in df.columns:
+            del dfr["index"]
+        df_names = {Nutil.split_json_name(j_name)[0]: j_name for j_name in dfr.columns}
+        df_ntv_types = {
+            Nutil.split_json_name(j_name)[0]: Nutil.split_json_name(j_name)[1]
+            for j_name in dfr.columns
+        }
         dfr.columns = [Nutil.split_json_name(name)[0] for name in dfr.columns]
-        if dfr.attrs.get('metadata'):
-            for name, meta in dfr.attrs['metadata'].items():
+        if dfr.attrs.get("metadata"):
+            for name, meta in dfr.attrs["metadata"].items():
                 xnd += [Xndarray.read_json({name: meta})]
-        if dfr.attrs.get('fields'):
-            for name, jsn in dfr.attrs['fields'].items():
+        if dfr.attrs.get("fields"):
+            for name, jsn in dfr.attrs["fields"].items():
                 xnd += [Xndarray.read_json({name: jsn})]
-        if dfr.attrs.get('info'):
-            dimensions = dfr.attrs['info']['dimensions']
-            data = dfr.attrs['info']['data']
+        if dfr.attrs.get("info"):
+            dimensions = dfr.attrs["info"]["dimensions"]
+            data = dfr.attrs["info"]["data"]
         else:
-            dimensions, data = PandasConnec._ximport_analysis(dfr, opt['dims'])
-        shape_dfr = [data[dim]['shape'][0]
-                     for dim in dimensions] if dimensions else len(dfr)
+            dimensions, data = PandasConnec._ximport_analysis(dfr, opt["dims"])
+        shape_dfr = (
+            [data[dim]["shape"][0] for dim in dimensions] if dimensions else len(dfr)
+        )
         dfr = dfr.sort_values(dimensions)
         for name in df_names:
-            xnd += [PandasConnec._ximport_series(data, name, dfr, dimensions,
-                                                 shape_dfr, df_ntv_types, **opt)]
-        return Xclass(xnd, dfr.attrs.get('name')).to_canonical()
+            xnd += [
+                PandasConnec._ximport_series(
+                    data, name, dfr, dimensions, shape_dfr, df_ntv_types, **opt
+                )
+            ]
+        return Xclass(xnd, dfr.attrs.get("name")).to_canonical()
 
     @staticmethod
     def _ximport_analysis(dfr, opt_dims):
-        '''return data and dimensions from analysis module
+        """return data and dimensions from analysis module
         - opt_dims: partition to apply
-        - dfr: dataframe to analyse'''
+        - dfr: dataframe to analyse"""
         dfr_idx = list(dfr.index.names)
         opt_dims = dfr_idx if dfr_idx != [None] else opt_dims
         ana = dfr.npd.analysis(distr=True)
-        partition = ana.field_partition(partition=opt_dims, mode='id')
+        partition = ana.field_partition(partition=opt_dims, mode="id")
         part_rel = ana.relation_partition(partition=opt_dims, noroot=True)
-        part_dim = ana.relation_partition(
-            partition=opt_dims, noroot=True, primary=True)
-        dimensions = partition['primary']
+        part_dim = ana.relation_partition(partition=opt_dims, noroot=True, primary=True)
+        dimensions = partition["primary"]
         len_fields = {fld.idfield: fld.lencodec for fld in ana.fields}
-        data = {fld.idfield: {
-            'shape': [len_fields[dim] for dim in part_dim[fld.idfield]] if part_dim else [],
-            'links': part_rel[fld.idfield] if part_rel else []} for fld in ana.fields}
+        data = {
+            fld.idfield: {
+                "shape": [len_fields[dim] for dim in part_dim[fld.idfield]]
+                if part_dim
+                else [],
+                "links": part_rel[fld.idfield] if part_rel else [],
+            }
+            for fld in ana.fields
+        }
         for json_name in data:
-            if not data[json_name]['shape']:
+            if not data[json_name]["shape"]:
                 name = Nutil.split_name(Nutil.split_json_name(json_name)[0])[0]
-                p_name = [js_name for js_name in data
-                          if Nutil.split_json_name(js_name)[0] == name][0]
-                data[json_name]['shape'] = data[p_name]['shape']
+                p_name = [
+                    js_name
+                    for js_name in data
+                    if Nutil.split_json_name(js_name)[0] == name
+                ][0]
+                data[json_name]["shape"] = data[p_name]["shape"]
         return (dimensions, data)
 
     @staticmethod
     def _ximport_series(data, name, dfr, dimensions, shape_dfr, df_ntv_types, **opt):
-        '''return a Xndarray from a Series of a pd.DataFrame'''
-        if data[name].get('xtype') == 'meta':  # or len(dfr[name].unique()) == 1:
+        """return a Xndarray from a Series of a pd.DataFrame"""
+        if data[name].get("xtype") == "meta":  # or len(dfr[name].unique()) == 1:
             return Xndarray(name, meta=dfr[name].iloc[0])
-        meta = data[name].get('meta')
+        meta = data[name].get("meta")
         ntv_type = df_ntv_types[name]
         if len(dfr[name].unique()) == 1:
-            nda = Ndarray(np.array(dfr[name].iloc[0]),
-                          ntv_type=ntv_type, str_uri=False)
+            nda = Ndarray(np.array(dfr[name].iloc[0]), ntv_type=ntv_type, str_uri=False)
             nda.set_shape([1])
             return Xndarray(name, nda=nda, meta=meta)
         if not dimensions:
             nda = Ndarray(np.array(dfr[name]), ntv_type=ntv_type)
             return Xndarray(name, nda=nda, meta=meta)
         dims = []
         PandasConnec._get_dims(dims, name, data, dimensions)
         if not dims:
             p_name, add_name = Nutil.split_name(name)
             if add_name:
                 PandasConnec._get_dims(dims, p_name, data, dimensions)
-        np_array = PandasConnec._from_series(dfr, name, shape_dfr,
-                                             dimensions, dims, opt['dims'])
-        shape = data[name].get('shape', [len(dfr)])
+        np_array = PandasConnec._from_series(
+            dfr, name, shape_dfr, dimensions, dims, opt["dims"]
+        )
+        shape = data[name].get("shape", [len(dfr)])
         nda = Ndarray(np_array, ntv_type, shape)
-        links = data[name].get('links')
+        links = data[name].get("links")
         return Xndarray(name, nda=nda, links=links if links else dims, meta=meta)
 
     @staticmethod
     def _to_np_series(xdt, name, dims):
-        '''return a np.ndarray from the Xndarray of xdt defined by his name
+        """return a np.ndarray from the Xndarray of xdt defined by his name
 
         *parameters*
 
         - **xdt**: Xdataset - data to convert in a pd.DataFrame
         - **name**: string - full_name of the Xndarray to convert
-        - **dims**: list of string - order of dimensions full_name to apply'''
+        - **dims**: list of string - order of dimensions full_name to apply"""
         if name in xdt.uniques:
             return np.array([xdt[name].darray[0]] * xdt.length)
         if xdt[name].shape == [xdt.length]:
             return xdt[name].darray
         n_shape = {nam: len(xdt[nam]) for nam in dims}
         dim_name = xdt.dims(name)
         if not set(dim_name) <= set(dims):
@@ -241,353 +275,382 @@
         shap = [n_shape[nam] for nam in tab_name]
         order = [dims.index(nam) for nam in tab_name]
         arr = xdt[name].darray
         return Nutil.extend_array(arr, til, shap, order)
 
     @staticmethod
     def _from_series(dfr, name, shape, dims, links, new_dims=None):
-        '''return a flattened np.ndarray from the pd.Series of dfr defined by his name
+        """return a flattened np.ndarray from the pd.Series of dfr defined by his name
 
         *parameters*
 
         - dfr: DataFrame - data to convert in Xdataset
         - name: string - name of the Series (full_name or json_name)
         - shape: shape of the Xdataset
         - dims: list of string - list of name of dimensions
         - links: list of string - list of linked Series
         - new_dims: list of string (default None) - new order of dims
-        '''
+        """
         if not links:
             return np.array(dfr[name])
         old_order = list(range(len(dims)))
         new_dims = new_dims if new_dims else dims
-        order = [dims.index(dim)
-                 for dim in new_dims] if new_dims else old_order
+        order = [dims.index(dim) for dim in new_dims] if new_dims else old_order
         idx = [0] * len(dims)
         for nam in links:
             idx[new_dims.index(nam)] = slice(shape[dims.index(nam)])
-        xar = np.moveaxis(np.array(dfr[name]).reshape(shape),
-                          old_order, order)[tuple(idx)]
+        xar = np.moveaxis(np.array(dfr[name]).reshape(shape), old_order, order)[
+            tuple(idx)
+        ]
         if not links:
             return xar.flatten()
         lnk = [nam for nam in new_dims if nam in links]
         shape_lnk = [shape[dims.index(nam)] for nam in lnk]
         xar = xar.reshape(shape_lnk)
         old_order = list(range(len(links)))
         order = [lnk.index(dim) for dim in links]
         return np.moveaxis(xar, old_order, order).flatten()
 
     @staticmethod
     def _get_dims(dims, name, data, dimensions):
-        '''add names of dimensions into dims'''
+        """add names of dimensions into dims"""
         if not name:
             return
         if name in dimensions:
             dims += [name]
         else:
-            if 'links' not in data[name]:
+            if "links" not in data[name]:
                 return
-            for nam in data[name]['links']:
+            for nam in data[name]["links"]:
                 PandasConnec._get_dims(dims, nam, data, dimensions)
 
 
 class XarrayConnec:
-    ''' Xarray interface with two static methods ximport and xexport'''
+    """Xarray interface with two static methods ximport and xexport"""
 
     @staticmethod
     def xexport(xdt, **kwargs):
-        '''return a xr.DataArray or a xr.Dataset from a Xdataset
+        """return a xr.DataArray or a xr.Dataset from a Xdataset
 
         *Parameters*
 
         - **dataset** : Boolean (default True) - if False and a single data_var,
         return a xr.DataArray
         - **info** : Boolean (default True) - if True, add json representation
         of 'relative' Xndarrays and 'data_arrays' Xndarrays in attrs
-        '''
-        option = {'dataset': True, 'info': True} | kwargs
+        """
+        option = {"dataset": True, "info": True} | kwargs
         coords = XarrayConnec._to_xr_vars(
-            xdt, xdt.dimensions + xdt.coordinates + xdt.uniques)
+            xdt, xdt.dimensions + xdt.coordinates + xdt.uniques
+        )
         coords |= XarrayConnec._to_xr_vars(xdt, xdt.additionals)
         attrs = XarrayConnec._to_xr_attrs(xdt, **option)
-        if len(xdt.data_vars) == 1 and not option['dataset']:
+        if len(xdt.data_vars) == 1 and not option["dataset"]:
             var_name = xdt.data_vars[0]
             data = xdt.to_ndarray(var_name)
             dims = xdt.dims(var_name)
-            attrs |= {'ntv_type': xdt[var_name].nda.ntv_type}
+            attrs |= {"ntv_type": xdt[var_name].nda.ntv_type}
             attrs |= xdt[var_name].meta if xdt[var_name].meta else {}
-            name = var_name if var_name != 'data' else None
-            xrd = xr.DataArray(data=data, coords=coords, dims=dims, attrs=attrs,
-                               name=name)
+            name = var_name if var_name != "data" else None
+            xrd = xr.DataArray(
+                data=data, coords=coords, dims=dims, attrs=attrs, name=name
+            )
         else:
             data_vars = XarrayConnec._to_xr_vars(xdt, xdt.data_vars)
             xrd = xr.Dataset(data_vars, coords=coords, attrs=attrs)
         for unic in xdt.uniques:
-            xrd[unic].attrs |= {'ntv_type': xdt[unic].ntv_type} | (
-                xdt[unic].meta if xdt[unic].meta else {})
+            xrd[unic].attrs |= {"ntv_type": xdt[unic].ntv_type} | (
+                xdt[unic].meta if xdt[unic].meta else {}
+            )
         return xrd
 
     @staticmethod
     def ximport(xar, Xclass, **kwargs):
-        '''return a Xdataset from a xr.DataArray or a xr.Dataset'''
+        """return a Xdataset from a xr.DataArray or a xr.Dataset"""
         xnd = []
         if xar.attrs:
-            attrs = {k: v for k, v in xar.attrs.items() if k not in [
-                'name', 'ntv_type']}
+            attrs = {
+                k: v for k, v in xar.attrs.items() if k not in ["name", "ntv_type"]
+            }
             for name, meta in attrs.items():
                 if isinstance(meta, list):
                     xnd += [Xndarray.read_json({name: meta})]
                 else:
                     xnd += [Xndarray(name, meta=meta)]
         for coord in xar.coords:
             xnd += [XarrayConnec._var_xr_to_xnd(xar.coords[coord])]
-            if list(xar.coords[coord].dims) == list(xar.dims) and isinstance(xar, xr.Dataset):
+            if list(xar.coords[coord].dims) == list(xar.dims) and isinstance(
+                xar, xr.Dataset
+            ):
                 xnd[-1].links = [list(xar.data_vars)[0]]
         if isinstance(xar, xr.DataArray):
-            var = XarrayConnec._var_xr_to_xnd(
-                xar, name='data', add_attrs=False)
-            xnd += [XarrayConnec._var_xr_to_xnd(xar,
-                                                name='data', add_attrs=False)]
-            xdt = Xclass(xnd, xar.attrs.get('name'))
+            var = XarrayConnec._var_xr_to_xnd(xar, name="data", add_attrs=False)
+            xnd += [XarrayConnec._var_xr_to_xnd(xar, name="data", add_attrs=False)]
+            xdt = Xclass(xnd, xar.attrs.get("name"))
             for var in xdt.data_vars:
                 if var != xar.name and xar.name:
                     xdt[var].links = [xar.name]
             return xdt.to_canonical()
         for var in xar.data_vars:
             xnd += [XarrayConnec._var_xr_to_xnd(xar.data_vars[var])]
-        return Xclass(xnd, xar.attrs.get('name')).to_canonical()
+        return Xclass(xnd, xar.attrs.get("name")).to_canonical()
 
     @staticmethod
     def _var_xr_to_xnd(var, name=None, add_attrs=True):
-        '''return a Xndarray from a Xarray variable
+        """return a Xndarray from a Xarray variable
 
         *Parameters*
 
         - **var** : Xarray variable to convert in Xndarray,
         - **name** : string (default None) - default name if var have no name,
         - **add_attrs** : boolean (default True) - if False, attrs are not converted
-        '''
+        """
         full_name = var.name if var.name else name
         name = Nutil.split_name(full_name)[0]
         dims = None if var.dims == (name,) or var.size == 1 else list(var.dims)
-        ntv_type = var.attrs.get('ntv_type')
+        ntv_type = var.attrs.get("ntv_type")
         nda = var.values
         nda = nda.reshape(1) if not nda.shape else nda
-        if nda.dtype.name == 'datetime64[ns]' and ntv_type:
+        if nda.dtype.name == "datetime64[ns]" and ntv_type:
             nda = Nutil.convert(ntv_type, nda, tojson=False)
-        attrs = {k: v for k, v in var.attrs.items()
-                 if k not in ['ntv_type', 'name']} if add_attrs else {}
+        attrs = (
+            {k: v for k, v in var.attrs.items() if k not in ["ntv_type", "name"]}
+            if add_attrs
+            else {}
+        )
         return Xndarray(full_name, Ndarray(nda, ntv_type), dims, attrs)
 
     @staticmethod
     def _to_xr_attrs(xdt, **option):
-        '''return a dict with attributes from a Xdataset
+        """return a dict with attributes from a Xdataset
 
         *Parameters*
 
         - **info** : Boolean  if True, add json representation of 'relative'
         Xndarrays and 'data_arrays' Xndarrays in attrs
-        '''
+        """
         attrs = {meta: xdt[meta].meta for meta in xdt.metadata}
-        attrs |= {'name': xdt.name} if xdt.name else {}
-        if option['info']:
+        attrs |= {"name": xdt.name} if xdt.name else {}
+        if option["info"]:
             for name in xdt.names:
-                if xdt[name].mode == 'relative':
+                if xdt[name].mode == "relative":
                     attrs |= xdt[name].to_json(header=False)
             for name in xdt.data_arrays:
                 attrs |= xdt[name].to_json(header=False)
         return attrs
 
     @staticmethod
     def _to_xr_coord(xdt, name):
-        '''return a dict with Xarray attributes from a Xndarray defined by his name'''
+        """return a dict with Xarray attributes from a Xndarray defined by his name"""
         data = xdt.to_ndarray(name)
         if name in xdt.uniques:
             return {name: data[0]}
         if name in xdt.additionals and not xdt[name].links:
             data = data.reshape(xdt.shape_dims(xdt[name].name))
         dims = tuple(xdt.dims(name)) if xdt.dims(name) else (xdt[name].name)
-        meta = {'ntv_type': xdt[name].ntv_type} | (
-            xdt[name].meta if xdt[name].meta else {})
+        meta = {"ntv_type": xdt[name].ntv_type} | (
+            xdt[name].meta if xdt[name].meta else {}
+        )
         return {name: (dims, data, meta)}
 
     @staticmethod
     def _to_xr_vars(xdt, list_names):
-        '''return a dict with Xarray attributes from a list of Xndarray names'''
+        """return a dict with Xarray attributes from a list of Xndarray names"""
         arg_vars = {}
-        valid_names = [
-            nam for nam in list_names if xdt[nam].mode == 'absolute']
+        valid_names = [nam for nam in list_names if xdt[nam].mode == "absolute"]
         for xnd_name in valid_names:
             arg_vars |= XarrayConnec._to_xr_coord(xdt, xnd_name)
         for name in list_names:
-            if xdt[name].xtype == 'meta':
+            if xdt[name].xtype == "meta":
                 arg_vars |= {name: xdt[name].meta}
         return arg_vars
 
     @staticmethod
     def _xr_add_type(xar):
-        '''add 'ntv_type' as attribute for a xr.DataArray'''
-        if isinstance(xar, xr.DataArray) and 'ntv_type' not in xar.attrs:
-            xar.attrs |= {'ntv_type': Nutil.ntv_type(xar.data.dtype.name)}
+        """add 'ntv_type' as attribute for a xr.DataArray"""
+        if isinstance(xar, xr.DataArray) and "ntv_type" not in xar.attrs:
+            xar.attrs |= {"ntv_type": Nutil.ntv_type(xar.data.dtype.name)}
             return
         for coord in xar.coords:
             XarrayConnec._xr_add_type(coord)
         for var in xar.data_vars:
             XarrayConnec._xr_add_type(var)
         return
 
 
 class ScippConnec:
-    ''' Scipp interface with two static methods ximport and xexport'''
+    """Scipp interface with two static methods ximport and xexport"""
 
-    SCTYPE_DTYPE = {'string': 'str'}
+    SCTYPE_DTYPE = {"string": "str"}
 
     @staticmethod
     def xexport(xdt, **kwargs):
-        '''return a sc.DataArray or a sc.Dataset from a xdataset
+        """return a sc.DataArray or a sc.Dataset from a xdataset
 
         *Parameters*
 
         - **dataset** : Boolean (default True) - if False and a single data_var,
         return a DataArray
         - **info** : Boolean (default True) - if True return a DataGroup with
         metadata and data_arrays
         - **ntv_type** : Boolean (default True) - if True add ntv-type to the name
-        '''
-        option = {'dataset': True, 'info': True,
-                  'ntv_type': True} | kwargs
-        coords = dict([ScippConnec._to_scipp_var(xdt, name, **option)
-                       for name in xdt.coordinates + xdt.dimensions + xdt.uniques
-                       if xdt[name].mode == 'absolute'])
-        scd = sc.Dataset(dict([ScippConnec._to_sc_dataarray(xdt, name, coords, **option)
-                               for name in xdt.data_vars
-                               if xdt[name].mode == 'absolute']))
-        scd = scd if option['dataset'] else scd[list(scd)[0]]
-        if not option['info']:
+        """
+        option = {"dataset": True, "info": True, "ntv_type": True} | kwargs
+        coords = dict(
+            [
+                ScippConnec._to_scipp_var(xdt, name, **option)
+                for name in xdt.coordinates + xdt.dimensions + xdt.uniques
+                if xdt[name].mode == "absolute"
+            ]
+        )
+        scd = sc.Dataset(
+            dict(
+                [
+                    ScippConnec._to_sc_dataarray(xdt, name, coords, **option)
+                    for name in xdt.data_vars
+                    if xdt[name].mode == "absolute"
+                ]
+            )
+        )
+        scd = scd if option["dataset"] else scd[list(scd)[0]]
+        if not option["info"]:
             return scd
-        sc_name = xdt.name if xdt.name else 'no_name'
+        sc_name = xdt.name if xdt.name else "no_name"
         return sc.DataGroup({sc_name: scd} | ScippConnec._to_scipp_grp(xdt, **option))
 
     @staticmethod
     def ximport(sc_obj, Xclass, **kwargs):
-        '''return a xdataset from a scipp object DataArray, Dataset or DataGroup'''
+        """return a xdataset from a scipp object DataArray, Dataset or DataGroup"""
         xnd = []
         scd = sc_obj
         xnd_name = None
         if isinstance(sc_obj, sc.DataGroup):
             for obj in sc_obj:
                 if isinstance(sc_obj[obj], (sc.Dataset, sc.DataArray)):
                     scd = sc_obj[obj]
                     xnd_name = obj
                     break
         if isinstance(scd, sc.DataArray):
-            scd = sc.Dataset({(scd.name if scd.name else 'no_name'): scd})
+            scd = sc.Dataset({(scd.name if scd.name else "no_name"): scd})
         if isinstance(scd, sc.Dataset):
             for coord in scd.coords:
-                xnd += ScippConnec._var_sc_to_xnd(
-                    scd.coords[coord], scd, coord)
+                xnd += ScippConnec._var_sc_to_xnd(scd.coords[coord], scd, coord)
             for var in scd:
                 for mask in scd[var].masks:
                     m_var = Nutil.split_json_name(var)[0]
                     xnd += ScippConnec._var_sc_to_xnd(
-                        scd[var].masks[mask], scd, mask, m_var)
+                        scd[var].masks[mask], scd, mask, m_var
+                    )
                 xnd += ScippConnec._var_sc_to_xnd(scd[var].data, scd, var)
         if isinstance(sc_obj, sc.DataGroup):
             xnd = ScippConnec._grp_sc_to_xnd(sc_obj, xnd)
         return Xclass(xnd, xnd_name).to_canonical()
 
     @staticmethod
     def _grp_sc_to_xnd(sc_obj, xnd):
-        '''return a list of Xndarray from a scipp variable'''
+        """return a list of Xndarray from a scipp variable"""
         dic_xnd = {xar.name: xar for xar in xnd}
         for obj in sc_obj:
             name, add_name = Nutil.split_name(obj)
             match [name, add_name, sc_obj[obj]]:
                 case [name, None, list()]:
                     xnd += [Xndarray.read_json({name: sc_obj[obj]})]
                 case [name, add_name, sc.Variable()]:
-                    xnd += ScippConnec._var_sc_to_xnd(
-                        sc_obj[obj], None, add_name, name)
+                    xnd += ScippConnec._var_sc_to_xnd(sc_obj[obj], None, add_name, name)
                 case [name, _, dict() | str() | list()] if name in dic_xnd:
                     if dic_xnd[name].meta:
                         dic_xnd[name].meta |= sc_obj[obj]
                     else:
                         dic_xnd[name].meta = sc_obj[obj]
                 case [name, _, dict() | str() | list()]:
                     xnd += [Xndarray.read_json({name: sc_obj[obj]})]
-                case [_, _, _]: ...
+                case [_, _, _]:
+                    ...
         return xnd
 
     @staticmethod
-    def _var_sc_to_xnd(scv, scd=None, sc_name='', var=None):
-        '''return a list of Xndarray from a scipp variable
+    def _var_sc_to_xnd(scv, scd=None, sc_name="", var=None):
+        """return a list of Xndarray from a scipp variable
         - scd : scipp dataset
         - scv : scipp variable
         - var : name
-        - sc_name : scipp name'''
+        - sc_name : scipp name"""
         l_xnda = []
-        unit = scv.unit.name if scv.unit and scv.unit not in [
-            'dimensionless', 'ns'] else ''
+        unit = (
+            scv.unit.name
+            if scv.unit and scv.unit not in ["dimensionless", "ns"]
+            else ""
+        )
         ext_name, typ1 = Nutil.split_json_name(sc_name, True)
         var_name, typ2 = Nutil.split_json_name(var, True)
-        full_name = var_name + \
-            ('.' if var_name and ext_name else '') + ext_name
+        full_name = var_name + ("." if var_name and ext_name else "") + ext_name
         ntv_type_base = typ1 + typ2
-        ntv_type = ntv_type_base + ('[' + unit + ']' if unit else '')
+        ntv_type = ntv_type_base + ("[" + unit + "]" if unit else "")
         links = [Nutil.split_json_name(jsn)[0] for jsn in scv.dims]
         if scd is not None and sc_name in scd.coords and scv.dims == scd.dims:
             links = [Nutil.split_json_name(list(scd)[0])[0]]
         if scv.variances is not None:
             nda = Ndarray(scv.variances, ntv_type_base)
-            l_xnda.append(Xndarray(full_name + '.variance', nda, links))
+            l_xnda.append(Xndarray(full_name + ".variance", nda, links))
         nda = Ndarray(scv.values, ntv_type, str_uri=False)
         shape = scv.shape if scv.shape else (1,)
         nda.set_shape(shape)
         l_xnda.append(Xndarray(full_name, nda, links))
         return l_xnda
 
     @staticmethod
     def _to_sc_dataarray(xdt, name, coords, **option):
-        '''return a scipp.DataArray from a xdataset.global_var defined by his name'''
+        """return a scipp.DataArray from a xdataset.global_var defined by his name"""
         scipp_name, data = ScippConnec._to_scipp_var(xdt, name, **option)
-        masks = dict([ScippConnec._to_scipp_var(xdt, nam, **option)
-                     for nam in set(xdt.group(name)) & set(xdt.masks)])
+        masks = dict(
+            [
+                ScippConnec._to_scipp_var(xdt, nam, **option)
+                for nam in set(xdt.group(name)) & set(xdt.masks)
+            ]
+        )
         return (scipp_name, sc.DataArray(data, coords=coords, masks=masks))
 
     @staticmethod
     def _to_scipp_grp(xdt, **option):
-        '''return a dict with metadata, data-array and data_add from a xdataset'''
+        """return a dict with metadata, data-array and data_add from a xdataset"""
         grp = {}
-        grp |= dict([ScippConnec._to_scipp_var(xdt, name, **option)
-                     for name in xdt.data_add + xdt.data_arrays
-                     if xdt[name].add_name != 'variance'])
-        opt_mask = option | {'grp_mask': True}
-        grp |= dict([ScippConnec._to_scipp_var(xdt, name, **opt_mask)
-                     for name in xdt.masks
-                     if xdt[name].name in xdt.names and xdt[name].name not in xdt.data_vars])
-        grp |= {name + '.meta': xdt[name].meta for name in xdt.names
-                if xdt[name].meta}
+        grp |= dict(
+            [
+                ScippConnec._to_scipp_var(xdt, name, **option)
+                for name in xdt.data_add + xdt.data_arrays
+                if xdt[name].add_name != "variance"
+            ]
+        )
+        opt_mask = option | {"grp_mask": True}
+        grp |= dict(
+            [
+                ScippConnec._to_scipp_var(xdt, name, **opt_mask)
+                for name in xdt.masks
+                if xdt[name].name in xdt.names and xdt[name].name not in xdt.data_vars
+            ]
+        )
+        grp |= {name + ".meta": xdt[name].meta for name in xdt.names if xdt[name].meta}
         for name in xdt.names:
-            if xdt[name].mode == 'relative':
+            if xdt[name].mode == "relative":
                 grp |= xdt[name].to_json(header=False)
         return grp
 
     @staticmethod
     def _to_scipp_var(xdt, name, **kwargs):
-        '''return a scipp.Variable from a Xndarray defined by his name'''
-        option = {'grp_mask': False, 'ntv_type': True} | kwargs
+        """return a scipp.Variable from a Xndarray defined by his name"""
+        option = {"grp_mask": False, "ntv_type": True} | kwargs
         simple_type, unit = Nutil.split_type(xdt[name].ntv_type)
-        unit = unit if unit else ''
+        unit = unit if unit else ""
         add_name = Nutil.split_name(name)[1]
-        new_n = add_name if name in xdt.masks and not option['grp_mask'] else name
-        opt_n = option['ntv_type']
-        scipp_name = new_n + (':' + simple_type if opt_n else '')
+        new_n = add_name if name in xdt.masks and not option["grp_mask"] else name
+        opt_n = option["ntv_type"]
+        scipp_name = new_n + (":" + simple_type if opt_n else "")
         if name in xdt.uniques:
             return (scipp_name, sc.scalar(xdt[name].darray[0], unit=unit))
-        vari_name = name + '.variance'
+        vari_name = name + ".variance"
         variances = xdt[vari_name].darray if vari_name in xdt.names else None
-        dims = xdt.dims(name, opt_n) if xdt.dims(
-            name, opt_n) else [xdt[name].name]
-        var = sc.array(dims=['flat'], values=xdt.to_darray(
-            name), variances=variances, unit=unit)
-        var = sc.fold(var, dim='flat', sizes=dict(zip(dims, xdt[name].shape)))
+        dims = xdt.dims(name, opt_n) if xdt.dims(name, opt_n) else [xdt[name].name]
+        var = sc.array(
+            dims=["flat"], values=xdt.to_darray(name), variances=variances, unit=unit
+        )
+        var = sc.fold(var, dim="flat", sizes=dict(zip(dims, xdt[name].shape)))
         return (scipp_name, var)
```

### Comparing `ntv_numpy-0.2.1/ntv_numpy/xndarray.py` & `ntv_numpy-0.2.2/ntv_numpy/xndarray.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import json
 from json_ntv import Ntv
 from ntv_numpy.ndarray import Ndarray, Nutil, NdarrayError
 
 
 class Xndarray:
-    ''' Representation of a labelled multidimensional Array
+    """Representation of a labelled multidimensional Array
 
     *Attributes :*
     - **name** :  string - name of the Xndarray
     - **add_name** :  string - additional name of the Xndarray
     - **nda**: Ndarray - ndarray data
     - **links**: list of string - links to other Xndarray
     - **meta** : JsonValue - informations
@@ -39,222 +39,242 @@
     - `full_name`
     - `json_name`
 
     *methods*
     - `to_json`
     - `read_json (static method)`
     - `set_ndarray`
-    '''
+    """
 
-    def __init__(self, full_name, nda=None, links=None,
-                 meta=None):
-        '''Xndarray constructor.
+    def __init__(self, full_name, nda=None, links=None, meta=None):
+        """Xndarray constructor.
 
         *Parameters*
 
         - **full_name**: string (default None) - name with additional name
         - **nda** : Ndarray (default None) - data
         - **links**: List of string (default None) - dims or other names of associated Xndarray
         - **ntv_type**: string (default None) - ntv_type to apply to data
         - **meta**: dict (default None) - information
-        '''
+        """
         if isinstance(full_name, Xndarray):
             self.name = full_name.name
             self.add_name = full_name.add_name
             self.nda = full_name.nda
             self.links = full_name.links
             self.meta = full_name.meta
             return
         self.name, self.add_name = Nutil.split_name(full_name)
         self.nda = Ndarray(nda) if nda is not None else None
         self.links = links if links else None
         self.meta = meta if meta else None
         if self.meta is None and self.nda is None:
-            raise NdarrayError('A Xndarray has to have metadata or Ndarray')
+            raise NdarrayError("A Xndarray has to have metadata or Ndarray")
 
     def __repr__(self):
-        '''return classname and number of value'''
-        return self.__class__.__name__ + '[' + self.full_name + ']'
+        """return classname and number of value"""
+        return self.__class__.__name__ + "[" + self.full_name + "]"
 
     def __str__(self):
-        '''return json string format'''
+        """return json string format"""
         return json.dumps(self.to_json())
 
     def __eq__(self, other):
-        ''' equal if attributes are equal'''
+        """equal if attributes are equal"""
         if self.name != other.name or self.add_name != other.add_name:
             return False
         if self.links != other.links or self.meta != other.meta:
             return False
         if self.nda is None and other.nda is None:
             return True
         if self.nda is None or other.nda is None:
             return False
         return self.nda == other.nda
 
     def __len__(self):
-        ''' len of ndarray'''
+        """len of ndarray"""
         return len(self.nda) if self.nda is not None else 0
 
     def __contains__(self, item):
-        ''' item of ndarray values'''
+        """item of ndarray values"""
         return item in self.nda if self.nda is not None else None
 
     def __getitem__(self, ind):
-        ''' return ndarray value item'''
+        """return ndarray value item"""
         if self.nda is None:
             return None
         if isinstance(ind, tuple):
             return [self.nda[i] for i in ind]
         return self.nda[ind]
 
     def __copy__(self):
-        ''' Copy all the data '''
+        """Copy all the data"""
         return self.__class__(self)
 
     @property
     def darray(self):
-        '''return the darray of the ndarray'''
+        """return the darray of the ndarray"""
         return self.nda.darray if self.nda is not None else None
 
     @property
     def ndarray(self):
-        '''return the darray of the ndarray'''
+        """return the darray of the ndarray"""
         return self.nda.ndarray if self.nda is not None else None
 
     @property
     def uri(self):
-        '''return the uri of the ndarray'''
+        """return the uri of the ndarray"""
         return self.nda.uri if self.nda is not None else None
 
     @property
     def shape(self):
-        '''return the shape of the ndarray'''
+        """return the shape of the ndarray"""
         return self.nda.shape if self.nda is not None else None
 
     @property
     def ntv_type(self):
-        '''return the ntv_type of the ndarray'''
+        """return the ntv_type of the ndarray"""
         return self.nda.ntv_type if self.nda is not None else None
 
     @property
     def mode(self):
-        '''return the mode of the ndarray'''
-        return self.nda.mode if self.nda is not None else 'undefined'
+        """return the mode of the ndarray"""
+        return self.nda.mode if self.nda is not None else "undefined"
 
     @property
     def info(self):
-        ''' infos of the Xndarray'''
-        inf = {'name': self.full_name}
-        inf['length'] = len(self)
+        """infos of the Xndarray"""
+        inf = {"name": self.full_name}
+        inf["length"] = len(self)
         if self.nda:
-            inf['mode'] = self.mode
-            inf['ntvtype'] = self.ntv_type
-            inf['shape'] = self.shape
-        inf['uri'] = self.uri
-        inf['meta'] = self.meta
-        inf['xtype'] = self.xtype
-        inf['links'] = self.links
+            inf["mode"] = self.mode
+            inf["ntvtype"] = self.ntv_type
+            inf["shape"] = self.shape
+        inf["uri"] = self.uri
+        inf["meta"] = self.meta
+        inf["xtype"] = self.xtype
+        inf["links"] = self.links
         return {key: val for key, val in inf.items() if val}
 
     @property
     def xtype(self):
-        '''nature of the Xndarray (undefined, namedarray, variable, additional,
-        meta, inconsistent)'''
+        """nature of the Xndarray (undefined, namedarray, variable, additional,
+        meta, inconsistent)"""
         match [self.links, self.add_name, self.mode]:
-            case [_, _, 'inconsistent']:
-                return 'inconsistent'
-            case [_, _, 'undefined']:
-                return 'meta'
-            case [None, '', _]:
-                return 'namedarray'
-            case [_, '', _]:
-                return 'variable'
+            case [_, _, "inconsistent"]:
+                return "inconsistent"
+            case [_, _, "undefined"]:
+                return "meta"
+            case [None, "", _]:
+                return "namedarray"
+            case [_, "", _]:
+                return "variable"
             case [_, str(), _]:
-                return 'additional'
+                return "additional"
             case _:
-                return 'inconsistent'
+                return "inconsistent"
 
     @property
     def full_name(self):
-        '''concatenation of name and additional name'''
-        add_name = '.' + self.add_name if self.add_name else ''
+        """concatenation of name and additional name"""
+        add_name = "." + self.add_name if self.add_name else ""
         return self.name + add_name
 
     @property
     def json_name(self):
-        '''concatenation of full_name and ntv_type'''
-        add_ntv_type = ':' + self.ntv_type if self.ntv_type else ''
+        """concatenation of full_name and ntv_type"""
+        add_ntv_type = ":" + self.ntv_type if self.ntv_type else ""
         return self.full_name + add_ntv_type
 
     @staticmethod
     def read_json(jsn, **kwargs):
-        ''' convert json data into a Xndarray.
+        """convert json data into a Xndarray.
 
         *Parameters*
 
         - **convert** : boolean (default True) - If True, convert json data with
         non Numpy ntv_type into data with python type
-        '''
-        option = {'convert': True} | kwargs
+        """
+        option = {"convert": True} | kwargs
         jso = json.loads(jsn) if isinstance(jsn, str) else jsn
         value, full_name = Ntv.decode_json(jso)[:2]
 
         meta = links = nda = None
         match value:
-            case str(meta) | dict(meta): ...
-            case [list(nda)]: ...
-            case [list(nda), list(links)]: ...
-            case [list(nda), dict(meta)] | [list(nda), str(meta)]: ...
-            case [list(nda), list(links), dict(meta)]: ...
-            case [list(nda), list(links), str(meta)]: ...
+            case str(meta) | dict(meta):
+                ...
+            case [list(nda)]:
+                ...
+            case [list(nda), list(links)]:
+                ...
+            case [list(nda), dict(meta)] | [list(nda), str(meta)]:
+                ...
+            case [list(nda), list(links), dict(meta)]:
+                ...
+            case [list(nda), list(links), str(meta)]:
+                ...
             case _:
                 return None
         nda = Ndarray.read_json(nda, **option) if nda else None
         return Xndarray(full_name, links=links, meta=meta, nda=nda)
 
     def set_ndarray(self, ndarray, nda_uri=True):
-        '''set a new ndarray (nda) and return the result (True, False)
+        """set a new ndarray (nda) and return the result (True, False)
 
         *Parameters*
 
         - **ndarray** : string, list, np.ndarray, Ndarray - data to include
         - **nda_uri** : boolean (default True) - if True, existing shape and
-        ntv_type are not updated (but are created if not existing)'''
+        ntv_type are not updated (but are created if not existing)"""
         ndarray = Ndarray(ndarray)
         if self.nda is not None:
             return self.nda.update(ndarray, nda_uri=nda_uri)
         self.nda = ndarray
         return True
 
     def to_json(self, **kwargs):
-        ''' convert a Xndarray into json-value.
+        """convert a Xndarray into json-value.
 
         *Parameters*
 
         - **encoded** : Boolean (default False) - json-value if False else json-text
         - **header** : Boolean (default True) - including xndarray type
         - **noname** : Boolean (default False) - including data type and name if False
         - **notype** : Boolean (default False) - including data type if False
         - **novalue** : Boolean (default False) - including value if False
         - **noshape** : Boolean (default True) - if True, without shape if dim < 1
         - **format** : string (default 'full') - representation format of the ndarray,
         - **extension** : string (default None) - type extension
-        '''
-        option = {'notype': False, 'format': 'full',
-                  'noshape': True, 'header': True, 'encoded': False,
-                  'novalue': False, 'noname': False} | kwargs
-        if not option['format'] in ['full', 'complete']:
-            option['noshape'] = False
-        opt_nda = option | {'header': False}
+        """
+        option = {
+            "notype": False,
+            "format": "full",
+            "noshape": True,
+            "header": True,
+            "encoded": False,
+            "novalue": False,
+            "noname": False,
+        } | kwargs
+        if option["format"] not in ["full", "complete"]:
+            option["noshape"] = False
+        opt_nda = option | {"header": False}
         nda_str = self.nda.to_json(**opt_nda) if self.nda is not None else None
         lis = [nda_str, self.links, self.meta]
         lis = [val for val in lis if val is not None]
-        return Nutil.json_ntv(None if option['noname'] else self.full_name,
-                              None if option['noname'] else 'xndarray',
-                              lis[0] if lis == [self.meta] else lis,
-                              header=option['header'], encoded=option['encoded'])
+        return Nutil.json_ntv(
+            None if option["noname"] else self.full_name,
+            None if option["noname"] else "xndarray",
+            lis[0] if lis == [self.meta] else lis,
+            header=option["header"],
+            encoded=option["encoded"],
+        )
 
     def _to_json(self):
-        '''return dict of attributes'''
-        return {'name': self.name, 'ntv_type': self.ntv_type, 'uri': self.uri,
-                'nda': self.nda, 'meta': self.meta, 'links': self.links}
+        """return dict of attributes"""
+        return {
+            "name": self.name,
+            "ntv_type": self.ntv_type,
+            "uri": self.uri,
+            "nda": self.nda,
+            "meta": self.meta,
+            "links": self.links,
+        }
```

### Comparing `ntv_numpy-0.2.1/ntv_numpy.egg-info/PKG-INFO` & `ntv_numpy-0.2.2/ntv_numpy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntv_numpy
-Version: 0.2.1
+Version: 0.2.2
 Summary: NTV-NumPy : A multidimensional semantic, compact and reversible format for interoperability
 Home-page: https://github.com/loco-philippe/ntv-numpy/blob/main/README.md
 Author: Philippe Thomy
 Author-email: philippe@loco-labs.io
 Keywords: numpy,JSON-NTV,semantic JSON,development,environmental data,multidimensional
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -67,26 +67,26 @@
 ```python
 In [1]: example = {
                 'example:xdataset': {
                         'var1': [['float[kg]', [2, 2], [10.1, 0.4, 3.4, 8.2]], ['x', 'y']],
                         'var1.variance': [[[2, 2], [0.1, 0.2, 0.3, 0.4]]],
                         'var1.mask1': [[[True, False]], ['x']],
                         'var1.mask2': [[[2, 2], [True, False, False, True]]],
-                
-                        'var2': [['var2.ntv'], ['x', 'y']],    
-                        
+
+                        'var2': [['var2.ntv'], ['x', 'y']],
+
                         'x': [['string', ['23F0AE', '578B98']], {'test': 21}],
                         'y': [['date', ['2021-01-01', '2022-02-02']]],
-                        
+
                         'ranking': [['month', [2, 2], [1, 2, 3, 4]], ['var1']],
                         'z': [['float', [10, 20]], ['x']],
                         'z.uncertainty': [[[0.1, 0.2]]],
-                        
+
                         'z_bis': [[['z1_bis', 'z2_bis']]],
-                
+
                         'info': {'path': 'https://github.com/loco-philippe/ntv-numpy/tree/main/example/',
                         'location': [['string', ['paris']]]}
                 }
         }
 
 In [2]: from ntv_numpy import Xdataset
 
@@ -151,28 +151,28 @@
 
 ### Pandas interoperability
 
 ```python
 In [6]: x_dataframe = x_example.to_dataframe()
         print(x_example.to_dataframe(json_name=False))
         print(x_xarray)
-Out[6]: 
+Out[6]:
                    ranking     z  z.uncertainty  var1  var1.mask1  var1.mask2  \
-x      y                                                                        
-23F0AE 2021-01-01        1  10.0            0.1  10.1        True        True   
-       2022-02-02        2  10.0            0.1   0.4        True       False   
-578B98 2021-01-01        3  20.0            0.2   3.4       False       False   
-       2022-02-02        4  20.0            0.2   8.2       False        True   
-
-                   var1.variance location  
-x      y                                   
-23F0AE 2021-01-01            0.1    paris  
-       2022-02-02            0.2    paris  
-578B98 2021-01-01            0.3    paris  
-       2022-02-02            0.4    paris 
+x      y
+23F0AE 2021-01-01        1  10.0            0.1  10.1        True        True
+       2022-02-02        2  10.0            0.1   0.4        True       False
+578B98 2021-01-01        3  20.0            0.2   3.4       False       False
+       2022-02-02        4  20.0            0.2   8.2       False        True
+
+                   var1.variance location
+x      y
+23F0AE 2021-01-01            0.1    paris
+       2022-02-02            0.2    paris
+578B98 2021-01-01            0.3    paris
+       2022-02-02            0.4    paris
 ```
 
 Reversibility:
 
 ```python
 In [7]: x_example_pd = Xdataset.from_dataframe(x_dataframe)
         x_example_pd == x_example_xr == x_example_json == x_example
@@ -218,17 +218,17 @@
                         'wcs':  {'WCSAXES': 2, 'CRPIX1': 2048.0, 'CRPIX2': 1024.0, 'PC1_1': 1.2905625619716e-05,
                                 'PC1_2': 5.9530912331034e-06, 'PC2_1': 5.0220581265601e-06, 'PC2_2': -1.2644774105568e-05,
                                 'CDELT1': 1.0, 'CDELT2': 1.0, 'CUNIT1': 'deg', 'CUNIT2': 'deg', 'CTYPE1': 'RA---TAN',
                                 'CTYPE2': 'DEC--TAN', 'CRVAL1': 5.63056810618, 'CRVAL2': -72.05457184279, 'LONPOLE': 180.0,
                                 'LATPOLE': -72.05457184279, 'WCSNAME': 'IDC_qbu1641sj', 'MJDREF': 0.0, 'RADESYS': 'ICRS'},
                         'psf': [['float[erg/s]', [1,2,3,4]]]
                 }
-        } 
+        }
         n_example = Xdataset.read_json(example)
-        n_example.info 
+        n_example.info
 Out[1]: {'name': 'example',
         'xtype': 'group',
         'data_arrays': ['data', 'psf'],
         'additionals': ['data.mask', 'data.uncertainty'],
         'metadata': ['meta', 'wcs'],
         'validity': 'valid',
         'width': 6}
@@ -255,26 +255,26 @@
 ```python
 In [1]: example = {
                 'example:xdataset': {
                         'var1': [['float[kg]', [2, 2], 'var1.ntv'], ['x', 'y']],
                         'var1.variance': [[[2, 2], 'var1_variance.ntv']],
                         'var1.mask1': [['var1_mask1.ntv'], ['x']],
                         'var1.mask2': [[[2, 2], 'var1_mask2.ntv']],
-                
-                        'var2': [['var2.ntv'], ['x', 'y']],    
-                        
+
+                        'var2': [['var2.ntv'], ['x', 'y']],
+
                         'x': [['x.ntv'], {'test': 21}],
                         'y': [['date', 'y.ntv']],
-                        
+
                         'ranking': [['month', [2, 2], 'ranking.ntv'], ['var1']],
                         'z': [['float', 'z.ntv'], ['x']],
                         'z.uncertainty': [['z_uncertainty.ntv']],
-                        
+
                         'z_bis': [['z_bis.ntv']],
-                
+
                         'info': {'path': 'https://github.com/loco-philippe/ntv-numpy/tree/main/example/'}
                 }
         }
 ```
 
 The complete example can be rebuild with loading data (path + file name).
```

### Comparing `ntv_numpy-0.2.1/setup.py` & `ntv_numpy-0.2.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,26 +7,27 @@
 from setuptools import setup, find_packages
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="ntv_numpy",
-    version="0.2.1",
+    version="0.2.2",
     description="NTV-NumPy : A multidimensional semantic, compact and reversible format for interoperability",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/loco-philippe/ntv-numpy/blob/main/README.md",
     author="Philippe Thomy",
     author_email="philippe@loco-labs.io",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3"],
+        "Programming Language :: Python :: 3",
+    ],
     keywords="numpy, JSON-NTV, semantic JSON, development, environmental data, multidimensional",
-    packages=find_packages(include=['ntv_numpy', 'ntv_numpy.*']),
-    package_data={'ntv_numpy': ['*.ini']},
+    packages=find_packages(include=["ntv_numpy", "ntv_numpy.*"]),
+    package_data={"ntv_numpy": ["*.ini"]},
     python_requires=">=3.10, <4",
-    install_requires=['json_ntv', 'numpy', 'shapely']
+    install_requires=["json_ntv", "numpy", "shapely"],
 )
```

