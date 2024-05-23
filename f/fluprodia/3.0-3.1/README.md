# Comparing `tmp/fluprodia-3.0.tar.gz` & `tmp/fluprodia-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluprodia-3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fluprodia-3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fluprodia-3.0.tar` & `fluprodia-3.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1649 2023-12-04 07:14:52.003443 fluprodia-3.0/CHANGELOG.rst
--rw-r--r--   0        0        0     2210 2023-12-07 17:42:54.221123 fluprodia-3.0/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1111 2022-12-02 16:23:35.372137 fluprodia-3.0/LICENSE
--rw-r--r--   0        0        0     5098 2023-12-07 17:50:21.823631 fluprodia-3.0/README.rst
--rw-r--r--   0        0        0     4912 2024-04-26 18:04:02.394957 fluprodia-3.0/docs/README.rst
--rw-r--r--   0        0        0    29585 2023-12-07 14:17:42.348154 fluprodia-3.0/docs/_static/images/logo_fluprodia_small.svg
--rw-r--r--   0        0        0    29828 2023-12-07 15:13:58.835502 fluprodia-3.0/docs/_static/images/logo_fluprodia_small_darkmode.svg
--rw-r--r--   0        0        0       29 2022-12-02 16:23:35.372137 fluprodia-3.0/docs/authors.rst
--rw-r--r--   0        0        0       31 2022-12-02 16:23:35.372137 fluprodia-3.0/docs/changelog.rst
--rw-r--r--   0        0        0     3699 2023-12-07 15:05:54.136759 fluprodia-3.0/docs/conf.py
--rw-r--r--   0        0        0       34 2022-12-02 16:23:35.372137 fluprodia-3.0/docs/contributing.rst
--rw-r--r--   0        0        0      262 2023-12-07 17:27:46.148538 fluprodia-3.0/docs/index.rst
--rw-r--r--   0        0        0     2496 2023-12-07 17:26:35.831705 fluprodia-3.0/docs/installation.rst
--rw-r--r--   0        0        0   216190 2023-12-04 18:23:26.492658 fluprodia-3.0/docs/reference/_images/Ts_R290_isolines.svg
--rw-r--r--   0        0        0   212552 2023-12-04 18:23:27.021556 fluprodia-3.0/docs/reference/_images/Ts_R290_pressure_loss.svg
--rw-r--r--   0        0        0   125924 2023-12-04 18:23:14.901351 fluprodia-3.0/docs/reference/_images/Ts_diagram.svg
--rw-r--r--   0        0        0   126103 2023-12-07 17:43:37.844787 fluprodia-3.0/docs/reference/_images/Ts_diagram_H2O.svg
--rw-r--r--   0        0        0   128714 2023-12-04 18:23:34.815330 fluprodia-3.0/docs/reference/_images/Ts_diagram_states.svg
--rw-r--r--   0        0        0   108148 2023-12-04 18:23:23.933735 fluprodia-3.0/docs/reference/_images/logph_R290_full.svg
--rw-r--r--   0        0        0   140191 2023-12-04 18:23:25.801304 fluprodia-3.0/docs/reference/_images/logph_R290_isolines.svg
--rw-r--r--   0        0        0   152726 2023-12-04 18:23:24.464968 fluprodia-3.0/docs/reference/_images/logph_R290_zoomed.svg
--rw-r--r--   0        0        0   162597 2023-12-04 18:23:24.980806 fluprodia-3.0/docs/reference/_images/logph_R290_zoomed_temperature_labels.svg
--rw-r--r--   0        0        0   108148 2023-12-04 18:23:15.312340 fluprodia-3.0/docs/reference/_images/logph_diagram.svg
--rw-r--r--   0        0        0   147439 2023-12-07 17:43:37.040465 fluprodia-3.0/docs/reference/_images/logph_diagram_H2O.svg
--rw-r--r--   0        0        0   104299 2023-12-07 17:43:43.932762 fluprodia-3.0/docs/reference/_images/logph_diagram_R290.svg
--rw-r--r--   0        0        0    99930 2023-12-04 18:23:34.396119 fluprodia-3.0/docs/reference/_images/logph_diagram_states.svg
--rw-r--r--   0        0        0      122 2022-12-02 16:23:35.441359 fluprodia-3.0/docs/reference/index.rst
--rw-r--r--   0        0        0       77 2023-12-07 17:32:15.145820 fluprodia-3.0/docs/requirements.txt
--rw-r--r--   0        0        0    17737 2024-04-26 18:06:06.705823 fluprodia-3.0/docs/usage.rst
--rw-r--r--   0        0        0     2073 2024-04-26 18:08:25.017418 fluprodia-3.0/pyproject.toml
--rw-r--r--   0        0        0      196 2024-04-26 18:08:50.950992 fluprodia-3.0/src/fluprodia/__init__.py
--rw-r--r--   0        0        0    42960 2024-04-26 18:06:35.273273 fluprodia-3.0/src/fluprodia/fluid_property_diagram.py
--rw-r--r--   0        0        0       80 2022-12-02 16:23:35.441359 fluprodia-3.0/tests/test_fluprodia.py
--rw-r--r--   0        0        0     6497 1970-01-01 00:00:00.000000 fluprodia-3.0/PKG-INFO
+-rw-r--r--   0        0        0     1913 2024-05-23 17:47:09.900018 fluprodia-3.1/CHANGELOG.rst
+-rw-r--r--   0        0        0     2210 2023-12-07 17:42:54.221123 fluprodia-3.1/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1111 2022-12-02 16:23:35.372137 fluprodia-3.1/LICENSE
+-rw-r--r--   0        0        0     5098 2023-12-07 17:50:21.823631 fluprodia-3.1/README.rst
+-rw-r--r--   0        0        0     4912 2024-04-26 18:04:02.394957 fluprodia-3.1/docs/README.rst
+-rw-r--r--   0        0        0    29585 2023-12-07 14:17:42.348154 fluprodia-3.1/docs/_static/images/logo_fluprodia_small.svg
+-rw-r--r--   0        0        0    29828 2023-12-07 15:13:58.835502 fluprodia-3.1/docs/_static/images/logo_fluprodia_small_darkmode.svg
+-rw-r--r--   0        0        0       29 2022-12-02 16:23:35.372137 fluprodia-3.1/docs/authors.rst
+-rw-r--r--   0        0        0       31 2022-12-02 16:23:35.372137 fluprodia-3.1/docs/changelog.rst
+-rw-r--r--   0        0        0     3699 2023-12-07 15:05:54.136759 fluprodia-3.1/docs/conf.py
+-rw-r--r--   0        0        0       34 2022-12-02 16:23:35.372137 fluprodia-3.1/docs/contributing.rst
+-rw-r--r--   0        0        0      262 2023-12-07 17:27:46.148538 fluprodia-3.1/docs/index.rst
+-rw-r--r--   0        0        0     2496 2023-12-07 17:26:35.831705 fluprodia-3.1/docs/installation.rst
+-rw-r--r--   0        0        0   216190 2023-12-04 18:23:26.492658 fluprodia-3.1/docs/reference/_images/Ts_R290_isolines.svg
+-rw-r--r--   0        0        0   212552 2023-12-04 18:23:27.021556 fluprodia-3.1/docs/reference/_images/Ts_R290_pressure_loss.svg
+-rw-r--r--   0        0        0   125924 2023-12-04 18:23:14.901351 fluprodia-3.1/docs/reference/_images/Ts_diagram.svg
+-rw-r--r--   0        0        0   126103 2023-12-07 17:43:37.844787 fluprodia-3.1/docs/reference/_images/Ts_diagram_H2O.svg
+-rw-r--r--   0        0        0   128714 2023-12-04 18:23:34.815330 fluprodia-3.1/docs/reference/_images/Ts_diagram_states.svg
+-rw-r--r--   0        0        0   108148 2023-12-04 18:23:23.933735 fluprodia-3.1/docs/reference/_images/logph_R290_full.svg
+-rw-r--r--   0        0        0   140191 2023-12-04 18:23:25.801304 fluprodia-3.1/docs/reference/_images/logph_R290_isolines.svg
+-rw-r--r--   0        0        0   152726 2023-12-04 18:23:24.464968 fluprodia-3.1/docs/reference/_images/logph_R290_zoomed.svg
+-rw-r--r--   0        0        0   162597 2023-12-04 18:23:24.980806 fluprodia-3.1/docs/reference/_images/logph_R290_zoomed_temperature_labels.svg
+-rw-r--r--   0        0        0   108148 2023-12-04 18:23:15.312340 fluprodia-3.1/docs/reference/_images/logph_diagram.svg
+-rw-r--r--   0        0        0   147439 2023-12-07 17:43:37.040465 fluprodia-3.1/docs/reference/_images/logph_diagram_H2O.svg
+-rw-r--r--   0        0        0   104299 2023-12-07 17:43:43.932762 fluprodia-3.1/docs/reference/_images/logph_diagram_R290.svg
+-rw-r--r--   0        0        0    99930 2023-12-04 18:23:34.396119 fluprodia-3.1/docs/reference/_images/logph_diagram_states.svg
+-rw-r--r--   0        0        0      122 2022-12-02 16:23:35.441359 fluprodia-3.1/docs/reference/index.rst
+-rw-r--r--   0        0        0       77 2023-12-07 17:32:15.145820 fluprodia-3.1/docs/requirements.txt
+-rw-r--r--   0        0        0    17737 2024-04-26 18:06:06.705823 fluprodia-3.1/docs/usage.rst
+-rw-r--r--   0        0        0     2073 2024-04-26 18:08:25.017418 fluprodia-3.1/pyproject.toml
+-rw-r--r--   0        0        0      196 2024-05-23 17:47:15.822410 fluprodia-3.1/src/fluprodia/__init__.py
+-rw-r--r--   0        0        0    42989 2024-05-23 17:47:41.955352 fluprodia-3.1/src/fluprodia/fluid_property_diagram.py
+-rw-r--r--   0        0        0       80 2022-12-02 16:23:35.441359 fluprodia-3.1/tests/test_fluprodia.py
+-rw-r--r--   0        0        0     6497 1970-01-01 00:00:00.000000 fluprodia-3.1/PKG-INFO
```

### Comparing `fluprodia-3.0/CHANGELOG.rst` & `fluprodia-3.1/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,26 @@
 
 Changelog
 =========
 
+v3.1 (May, 23, 2024)
+--------------------
+
+* The `draw_isolines` method is now compatible with matplotlib darkmode style.
+
+v3.0 (April, 26, 2024)
+----------------------
+
+* You can export the underlying data of your diagram using the `to_json` method.
+
 v2.0 (November, 22, 2023)
 -------------------------
+
 * The API changed in a way, that you have to create the figure and axes
-  externally using matplolib. These are then passed to the `draw_isolines`
+  externally using matplotlib. These are then passed to the `draw_isolines`
   method. See the README or in the examples for the new API version.
 
 v1.6 (December, 02, 2022)
 -------------------------
 
 * Remove upper Python version limit.
 
@@ -24,15 +35,15 @@
 
 * Add kPa to pressure unit system.
 * Fix TESPy API calls in the example usage.
 
 v1.3 (January, 7, 2021)
 -----------------------
 
-* Reduce the number of datappoints for isolines to 200 for faster performance.
+* Reduce the number of datapoints for isolines to 200 for faster performance.
 
 v1.2 (December, 8, 2020)
 ------------------------
 
 * Fix minimum volume value for iterators.
 
 v1.1 (November, 10, 2020)
```

### Comparing `fluprodia-3.0/CONTRIBUTING.rst` & `fluprodia-3.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `fluprodia-3.0/LICENSE` & `fluprodia-3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fluprodia-3.0/README.rst` & `fluprodia-3.1/README.rst`

 * *Files identical despite different names*

### Comparing `fluprodia-3.0/docs/README.rst` & `fluprodia-3.1/docs/README.rst`

 * *Files identical despite different names*

### Comparing `fluprodia-3.0/docs/_static/images/logo_fluprodia_small.svg` & `fluprodia-3.1/docs/_static/images/logo_fluprodia_small.svg`

 * *Files identical despite different names*

### Comparing `fluprodia-3.0/docs/_static/images/logo_fluprodia_small_darkmode.svg` & `fluprodia-3.1/docs/_static/images/logo_fluprodia_small_darkmode.svg`

 * *Files identical despite different names*

### Comparing `fluprodia-3.0/docs/conf.py` & `fluprodia-3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fluprodia-3.0/docs/installation.rst` & `fluprodia-3.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `fluprodia-3.0/docs/reference/_images/Ts_R290_isolines.svg` & `fluprodia-3.1/docs/reference/_images/Ts_R290_isolines.svg`

 * *Files identical despite different names*

### Comparing `fluprodia-3.0/docs/reference/_images/Ts_R290_pressure_loss.svg` & `fluprodia-3.1/docs/reference/_images/Ts_R290_pressure_loss.svg`

 * *Files identical despite different names*

### Comparing `fluprodia-3.0/docs/reference/_images/Ts_diagram.svg` & `fluprodia-3.1/docs/reference/_images/Ts_diagram.svg`

 * *Files identical despite different names*

### Comparing `fluprodia-3.0/docs/reference/_images/Ts_diagram_H2O.svg` & `fluprodia-3.1/docs/reference/_images/Ts_diagram_H2O.svg`

 * *Files identical despite different names*

### Comparing `fluprodia-3.0/docs/reference/_images/Ts_diagram_states.svg` & `fluprodia-3.1/docs/reference/_images/Ts_diagram_states.svg`

 * *Files identical despite different names*

### Comparing `fluprodia-3.0/docs/reference/_images/logph_R290_full.svg` & `fluprodia-3.1/docs/reference/_images/logph_R290_full.svg`

 * *Files identical despite different names*

### Comparing `fluprodia-3.0/docs/reference/_images/logph_R290_isolines.svg` & `fluprodia-3.1/docs/reference/_images/logph_R290_isolines.svg`

 * *Files identical despite different names*

### Comparing `fluprodia-3.0/docs/reference/_images/logph_R290_zoomed.svg` & `fluprodia-3.1/docs/reference/_images/logph_R290_zoomed.svg`

 * *Files identical despite different names*

### Comparing `fluprodia-3.0/docs/reference/_images/logph_R290_zoomed_temperature_labels.svg` & `fluprodia-3.1/docs/reference/_images/logph_R290_zoomed_temperature_labels.svg`

 * *Files identical despite different names*

### Comparing `fluprodia-3.0/docs/reference/_images/logph_diagram.svg` & `fluprodia-3.1/docs/reference/_images/logph_diagram.svg`

 * *Files identical despite different names*

### Comparing `fluprodia-3.0/docs/reference/_images/logph_diagram_H2O.svg` & `fluprodia-3.1/docs/reference/_images/logph_diagram_H2O.svg`

 * *Files identical despite different names*

### Comparing `fluprodia-3.0/docs/reference/_images/logph_diagram_R290.svg` & `fluprodia-3.1/docs/reference/_images/logph_diagram_R290.svg`

 * *Files identical despite different names*

### Comparing `fluprodia-3.0/docs/reference/_images/logph_diagram_states.svg` & `fluprodia-3.1/docs/reference/_images/logph_diagram_states.svg`

 * *Files identical despite different names*

### Comparing `fluprodia-3.0/docs/usage.rst` & `fluprodia-3.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `fluprodia-3.0/pyproject.toml` & `fluprodia-3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fluprodia-3.0/src/fluprodia/fluid_property_diagram.py` & `fluprodia-3.1/src/fluprodia/fluid_property_diagram.py`

 * *Files 2% similar despite different names*

```diff
@@ -480,36 +480,39 @@
                 alpha = 90
             else:
                 alpha = -90
         elif y[idx] - y[idx - 1] == 0:
             alpha = 0
         else:
             if ax.get_xscale() == 'log':
-                x_scaled = (np.log(x[idx]) - np.log(x[idx - 1])) * (
-                    width / (np.log(x_max) - np.log(x_min)))
+                x_scaled = (
+                    (np.log(x[idx]) - np.log(x[idx - 1]))
+                    * (width / (np.log(x_max) - np.log(x_min)))
+                )
             else:
-                x_scaled = (x[idx] - x[idx - 1]) * (
-                    width / (x_max - x_min))
+                x_scaled = (x[idx] - x[idx - 1]) * (width / (x_max - x_min))
 
             if ax.get_yscale() == 'log':
-                y_scaled = (np.log(y[idx]) - np.log(y[idx - 1])) * (
-                    height / (np.log(y_max) - np.log(y_min)))
+                y_scaled = (
+                    (np.log(y[idx]) - np.log(y[idx - 1]))
+                    * (height / (np.log(y_max) - np.log(y_min)))
+                )
             else:
-                y_scaled = (y[idx] - y[idx - 1]) * (
-                    height / (y_max - y_min))
+                y_scaled = (y[idx] - y[idx - 1]) * (height / (y_max - y_min))
 
             alpha = np.arctan(y_scaled / x_scaled) / (2 * np.pi) * 360
 
         unit = _beautiful_unit_string(self.units[property])
 
-        txt = str(isoline) + ' ' + unit
+        txt = f'{isoline} {unit}'
+        text_bg_color = ax.get_facecolor()
         ax.text(
             x[idx], y[idx], txt, fontsize=5,
             rotation=alpha, va='center', ha='center',
-            bbox=dict(facecolor='white', edgecolor='white', pad=0.0)
+            bbox=dict(facecolor=text_bg_color, edgecolor=text_bg_color, pad=0.0)
         )
 
     def calc_isolines(self):
         """Calculate all isolines."""
         self._isobaric()
         self._isochoric()
         self._isoquality()
@@ -622,15 +625,15 @@
         }
 
         directory = os.path.dirname(path)
         if directory != "" and not os.path.exists(directory):
             os.makedirs(directory)
 
         with open(path, "w", encoding="utf-8") as f:
-            f.write(json.dumps(data, indent=2))
+            json.dump(data, f, indent=2)
 
     def calc_individual_isoline(
             self, isoline_property=None,
             isoline_value=None,
             isoline_value_end=None,
             starting_point_property=None, ending_point_property=None,
             starting_point_value=None, ending_point_value=None):
@@ -1134,18 +1137,16 @@
                 )
 
                 if len(indices) == 0:
                     continue
 
                 gap = np.where(np.diff(indices) > 1)[0]
                 if len(gap) > 0:
-                    indices = np.insert(
-                        indices, gap + 1, indices[gap] + 1)
-                    indices = np.insert(
-                        indices, gap + 2, indices[gap + 2] - 1)
+                    indices = np.insert(indices, gap + 1, indices[gap] + 1)
+                    indices = np.insert(indices, gap + 2, indices[gap + 2] - 1)
 
                 if indices[0] != 0:
                     indices = np.insert(indices, 0, indices[0] - 1)
                 if indices[-1] < len(x) - 1:
                     indices = np.append(indices, indices[-1] + 1)
 
                 y = y[indices]
```

### Comparing `fluprodia-3.0/PKG-INFO` & `fluprodia-3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluprodia
-Version: 3.0
+Version: 3.1
 Summary: Create beautiful fluid property diagrams using CoolProp and matplotlib
 Author-email: Francesco Witte <tespy@witte.sh>
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

