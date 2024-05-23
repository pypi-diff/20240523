# Comparing `tmp/giverny-2.2.6.tar.gz` & `tmp/giverny-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giverny-2.2.6.tar", max compression
+gzip compressed data, was "giverny-2.2.7.tar", max compression
```

## Comparing `giverny-2.2.6.tar` & `giverny-2.2.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2024-05-15 20:29:21.051224 giverny-2.2.6/LICENSE.txt
--rw-r--r--   0        0        0      880 2024-05-16 23:39:59.828172 giverny-2.2.6/pyproject.toml
--rw-r--r--   0        0        0     2654 2024-05-15 20:29:21.067688 giverny-2.2.6/README.md
--rw-r--r--   0        0        0        0 2024-05-15 20:29:21.153138 giverny-2.2.6/src/giverny/__init__.py
--rw-r--r--   0        0        0   115748 2024-05-15 20:29:21.120913 giverny-2.2.6/src/giverny/turbulence_dataset.py
--rw-r--r--   0        0        0        0 2024-05-15 20:29:21.273182 giverny-2.2.6/src/giverny/turbulence_gizmos/__init__.py
--rw-r--r--   0        0        0    69836 2024-05-15 20:29:21.183536 giverny-2.2.6/src/giverny/turbulence_gizmos/basic_gizmos.py
--rw-r--r--   0        0        0     2690 2024-05-15 20:29:21.204673 giverny-2.2.6/src/giverny/turbulence_gizmos/constants.py
--rw-r--r--   0        0        0     5511 2024-05-15 20:29:21.224535 giverny-2.2.6/src/giverny/turbulence_gizmos/getCutout.py
--rw-r--r--   0        0        0     4571 2024-05-15 20:29:21.241042 giverny-2.2.6/src/giverny/turbulence_gizmos/getData.py
--rw-r--r--   0        0        0    54312 2024-05-15 20:29:21.261929 giverny-2.2.6/src/giverny/turbulence_gizmos/variable_dy_grid_ys.py
--rw-r--r--   0        0        0    38365 2024-05-15 20:29:21.093506 giverny-2.2.6/src/giverny/turbulence_toolkit.py
--rw-r--r--   0        0        0       21 2024-05-15 20:29:21.139426 giverny-2.2.6/src/giverny/version.py
--rw-r--r--   0        0        0     3802 1970-01-01 00:00:00.000000 giverny-2.2.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-23 03:31:14.842901 giverny-2.2.7/LICENSE.txt
+-rw-r--r--   0        0        0      880 2024-05-23 03:23:30.557647 giverny-2.2.7/pyproject.toml
+-rw-r--r--   0        0        0     2654 2024-05-23 03:31:14.858484 giverny-2.2.7/README.md
+-rw-r--r--   0        0        0        0 2024-05-23 03:31:14.918219 giverny-2.2.7/src/giverny/__init__.py
+-rw-r--r--   0        0        0   115748 2024-05-23 03:31:14.898514 giverny-2.2.7/src/giverny/turbulence_dataset.py
+-rw-r--r--   0        0        0        0 2024-05-23 03:31:15.020161 giverny-2.2.7/src/giverny/turbulence_gizmos/__init__.py
+-rw-r--r--   0        0        0    69541 2024-05-23 03:31:14.942426 giverny-2.2.7/src/giverny/turbulence_gizmos/basic_gizmos.py
+-rw-r--r--   0        0        0     2690 2024-05-23 03:31:14.956288 giverny-2.2.7/src/giverny/turbulence_gizmos/constants.py
+-rw-r--r--   0        0        0     5511 2024-05-23 03:31:14.967238 giverny-2.2.7/src/giverny/turbulence_gizmos/getCutout.py
+-rw-r--r--   0        0        0     4571 2024-05-23 03:31:14.983456 giverny-2.2.7/src/giverny/turbulence_gizmos/getData.py
+-rw-r--r--   0        0        0    54312 2024-05-23 03:31:15.007644 giverny-2.2.7/src/giverny/turbulence_gizmos/variable_dy_grid_ys.py
+-rw-r--r--   0        0        0    38365 2024-05-23 03:31:14.878889 giverny-2.2.7/src/giverny/turbulence_toolkit.py
+-rw-r--r--   0        0        0       21 2024-05-23 03:31:14.910154 giverny-2.2.7/src/giverny/version.py
+-rw-r--r--   0        0        0     3802 1970-01-01 00:00:00.000000 giverny-2.2.7/PKG-INFO
```

### Comparing `giverny-2.2.6/LICENSE.txt` & `giverny-2.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `giverny-2.2.6/pyproject.toml` & `giverny-2.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "giverny"
-version = "2.2.6"
+version = "2.2.7"
 description = "codebase to query the Johns Hopkins Turbulence Database (JHTDB) datasets"
 authors = ["Johns Hopkins Turbulence Database Group"]
 license = "LICENSE.txt"
 readme = "README.md"
 
 [[tool.poetry.packages]]
 include = "giverny"
```

### Comparing `giverny-2.2.6/README.md` & `giverny-2.2.7/README.md`

 * *Files identical despite different names*

### Comparing `giverny-2.2.6/src/giverny/turbulence_dataset.py` & `giverny-2.2.7/src/giverny/turbulence_dataset.py`

 * *Files identical despite different names*

### Comparing `giverny-2.2.6/src/giverny/turbulence_gizmos/basic_gizmos.py` & `giverny-2.2.7/src/giverny/turbulence_gizmos/basic_gizmos.py`

 * *Files 0% similar despite different names*

```diff
@@ -672,23 +672,23 @@
         'transition_bl': 'transitionbl'
     }[dataset_title]
 
 def get_value_names():
     # map of the value names for each variable, e.g. "ux" is the x-component of the velocity. 'vel': velocity, 'pr': pressure,
     # 'en': energy, 'temp': temperature, 'frc': force, 'mgnt': magnetic field, 'ptnt': vector potential, 'dnst': density, 'pst': position.
     return {
-        'vel':{1:'ux', 2:'uy', 3:'uz'},
-        'pr':{1:'p'},
-        'en':{1:'e'},
-        'temp':{1:'t'},
-        'frc':{1:'fx', 2:'fy', 3:'fz'},
-        'mgnt':{1:'bx', 2:'by', 3:'bz'},
-        'ptnt':{1:'ax', 2:'ay', 3:'az'},
-        'dnst':{1:'rho'},
-        'pst':{1:'x', 2:'y', 3:'z'}
+        'vel':{0:'ux', 1:'uy', 2:'uz'},
+        'pr':{0:'p'},
+        'en':{0:'e'},
+        'temp':{0:'t'},
+        'frc':{0:'fx', 1:'fy', 2:'fz'},
+        'mgnt':{0:'bx', 1:'by', 2:'bz'},
+        'ptnt':{0:'ax', 1:'ay', 2:'az'},
+        'dnst':{0:'rho'},
+        'pst':{0:'x', 1:'y', 2:'z'}
     }
 
 def get_num_values_per_datapoint(variable_id):
     # get the number of values per datapoint for the user-specified variable.
     return {
         'vel':3,
         'pr':1,
@@ -842,18 +842,14 @@
 """
 processing gizmos.
 """
 def assemble_axis_data(axes_data):
     # assemble all of the axis data together into one numpy array.
     return np.array(axes_data, dtype = np.ndarray)
 
-def convert_to_0_based_value(value):
-    # convert the 1-based value to a 0-based value.
-    return value - 1
-
 def get_axes_ranges_num_datapoints(axes_ranges):
     # number of datapoints along each axis.
     return axes_ranges[:, 1] - axes_ranges[:, 0] + 1
 
 def convert_to_0_based_ranges(dataset_title, axes_ranges):
     """
     convert the axes ranges to 0-based indices (giverny datasets) from 1-based user input. indices are left as 1-based for pyJHTDB datasets.
@@ -1012,15 +1008,15 @@
     with open(cube.output_path.joinpath(output_filename + '.xmf'), 'w') as output_file:
         output_file.write(output_str)
     
     print('\nfiles written successfully.')
     print('-----')
     sys.stdout.flush()
 
-def contour_plot(cube, value_index_original, cutout_data, plot_ranges, axes_ranges, strides, output_filename,
+def contour_plot(cube, value_index, cutout_data, plot_ranges, axes_ranges, strides, output_filename,
                 colormap = 'inferno'):
     """
     create a contour plot from the getCutout output.
     """
     # dictionaries.
     # -----
     variable = cube.var_name
@@ -1036,16 +1032,16 @@
     
     # exception handling.
     # -----
     # check that the user-input x-, y-, and z-axis plot ranges are all specified correctly as [minimum, maximum] integer values.
     check_axes_ranges(dataset_title, plot_ranges)
     
     # check that the user specified a valid value index.
-    if value_index_original not in value_name_map[variable_id]:
-        raise Exception(f"{value_index_original} is not a valid value_index: {list(value_name_map[variable_id].keys())}")
+    if value_index not in value_name_map[variable_id]:
+        raise Exception(f"{value_index} is not a valid value_index: {list(value_name_map[variable_id].keys())}")
         
     # transposed minimum and maximum arrays for both plot_ranges and axes_ranges.
     plot_ranges_min = plot_ranges[:, 0]
     plot_ranges_max = plot_ranges[:, 1]
     
     axes_min = axes_ranges[:, 0]
     axes_max = axes_ranges[:, 1]
@@ -1077,19 +1073,16 @@
 
     # generate the plot.
     print('generating contour plot...')
     print('-----')
     sys.stdout.flush()
     
     # -----
-    # convert the 1-based value_index_original to a 0-based index for python.
-    value_index = convert_to_0_based_value(value_index_original)
-    
     # name of the value that is being plotted.
-    value_name = value_name_map[variable_id][value_index_original]
+    value_name = value_name_map[variable_id][value_index]
     
     # get the formatted dataset title for use in the plot title.
     output_dataset_title = get_output_title(dataset_title)
     
     # specify the subset (or full) axes ranges to use for plotting. cutout_data is of the format [z-range, y-range, x-range, output value index].
     if dataset_title in ['sabl2048low', 'sabl2048high'] and variable == 'velocity':
         # zcoor_uv are the default z-axis coordinates for the 'velocity' variable of the 'sabl' datasets.
```

### Comparing `giverny-2.2.6/src/giverny/turbulence_gizmos/constants.py` & `giverny-2.2.7/src/giverny/turbulence_gizmos/constants.py`

 * *Files identical despite different names*

### Comparing `giverny-2.2.6/src/giverny/turbulence_gizmos/getCutout.py` & `giverny-2.2.7/src/giverny/turbulence_gizmos/getCutout.py`

 * *Files identical despite different names*

### Comparing `giverny-2.2.6/src/giverny/turbulence_gizmos/getData.py` & `giverny-2.2.7/src/giverny/turbulence_gizmos/getData.py`

 * *Files identical despite different names*

### Comparing `giverny-2.2.6/src/giverny/turbulence_gizmos/variable_dy_grid_ys.py` & `giverny-2.2.7/src/giverny/turbulence_gizmos/variable_dy_grid_ys.py`

 * *Files identical despite different names*

### Comparing `giverny-2.2.6/src/giverny/turbulence_toolkit.py` & `giverny-2.2.7/src/giverny/turbulence_toolkit.py`

 * *Files identical despite different names*

### Comparing `giverny-2.2.6/PKG-INFO` & `giverny-2.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giverny
-Version: 2.2.6
+Version: 2.2.7
 Summary: codebase to query the Johns Hopkins Turbulence Database (JHTDB) datasets
 License: LICENSE.txt
 Author: Johns Hopkins Turbulence Database Group
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

