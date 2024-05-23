# Comparing `tmp/django_mapengine-1.7.0.tar.gz` & `tmp/django_mapengine-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_mapengine-1.7.0.tar", max compression
+gzip compressed data, was "django_mapengine-1.8.0.tar", max compression
```

## Comparing `django_mapengine-1.7.0.tar` & `django_mapengine-1.8.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1069 2024-03-12 15:15:44.559160 django_mapengine-1.7.0/LICENSE
--rw-r--r--   0        0        0     3721 2024-05-13 08:57:55.365433 django_mapengine-1.7.0/README.md
--rw-r--r--   0        0        0       60 2024-05-13 08:57:55.365433 django_mapengine-1.7.0/django_mapengine/__init__.py
--rw-r--r--   0        0        0     3895 2024-04-25 07:43:15.134289 django_mapengine-1.7.0/django_mapengine/apps.py
--rw-r--r--   0        0        0     6738 2024-03-12 15:15:44.559160 django_mapengine-1.7.0/django_mapengine/choropleth.py
--rw-r--r--   0        0        0    43608 2024-03-12 15:15:44.559160 django_mapengine-1.7.0/django_mapengine/colorbrewer.py
--rw-r--r--   0        0        0     2230 2024-03-26 11:51:33.500776 django_mapengine-1.7.0/django_mapengine/distill.py
--rw-r--r--   0        0        0    10173 2024-04-24 10:17:38.710736 django_mapengine-1.7.0/django_mapengine/layers.py
--rw-r--r--   0        0        0      928 2024-03-14 11:59:59.035708 django_mapengine-1.7.0/django_mapengine/legend.py
--rw-r--r--   0        0        0      655 2024-05-13 08:57:55.369433 django_mapengine-1.7.0/django_mapengine/middleware.py
--rw-r--r--   0        0        0     2516 2024-03-14 11:59:59.039708 django_mapengine-1.7.0/django_mapengine/mvt.py
--rw-r--r--   0        0        0     2161 2023-06-14 12:49:56.418190 django_mapengine-1.7.0/django_mapengine/popups.py
--rw-r--r--   0        0        0     4014 2024-04-24 10:17:38.710736 django_mapengine-1.7.0/django_mapengine/setup.py
--rw-r--r--   0        0        0     5664 2024-04-24 10:17:38.710736 django_mapengine-1.7.0/django_mapengine/sources.py
--rw-r--r--   0        0        0    12661 2024-04-25 07:43:15.134289 django_mapengine-1.7.0/django_mapengine/static/django_mapengine/images/layer_ctrl_dark.svg
--rw-r--r--   0        0        0    14131 2024-04-24 10:17:38.710736 django_mapengine-1.7.0/django_mapengine/static/django_mapengine/images/layer_ctrl_default.svg
--rw-r--r--   0        0        0    12284 2024-04-25 07:43:15.134289 django_mapengine-1.7.0/django_mapengine/static/django_mapengine/images/layer_ctrl_light.svg
--rw-r--r--   0        0        0    10121 2024-04-24 10:17:38.710736 django_mapengine-1.7.0/django_mapengine/static/django_mapengine/images/layer_ctrl_satellite.svg
--rw-r--r--   0        0        0     1262 2024-04-24 10:17:38.710736 django_mapengine-1.7.0/django_mapengine/static/django_mapengine/js/basemaps.js
--rw-r--r--   0        0        0     3220 2024-02-02 13:11:04.816042 django_mapengine-1.7.0/django_mapengine/static/django_mapengine/js/choropleth.js
--rw-r--r--   0        0        0      455 2024-03-12 15:15:44.559160 django_mapengine-1.7.0/django_mapengine/static/django_mapengine/js/events.js
--rw-r--r--   0        0        0      605 2023-06-14 12:49:56.422190 django_mapengine-1.7.0/django_mapengine/static/django_mapengine/js/helper.js
--rw-r--r--   0        0        0     1128 2023-08-23 11:10:37.048313 django_mapengine-1.7.0/django_mapengine/static/django_mapengine/js/init.js
--rw-r--r--   0        0        0     3577 2024-04-24 10:17:38.710736 django_mapengine-1.7.0/django_mapengine/static/django_mapengine/js/layer.js
--rw-r--r--   0        0        0     3069 2023-07-13 09:07:49.785869 django_mapengine-1.7.0/django_mapengine/static/django_mapengine/js/legend.js
--rw-r--r--   0        0        0     1782 2024-04-24 10:17:38.710736 django_mapengine-1.7.0/django_mapengine/static/django_mapengine/js/map.js
--rw-r--r--   0        0        0     2804 2024-03-12 15:15:49.899159 django_mapengine-1.7.0/django_mapengine/static/django_mapengine/js/popup.js
--rw-r--r--   0        0        0     2558 2023-06-14 12:49:56.422190 django_mapengine-1.7.0/django_mapengine/static/django_mapengine/js/regions.js
--rw-r--r--   0        0        0      513 2023-06-14 12:49:56.422190 django_mapengine-1.7.0/django_mapengine/static/django_mapengine/js/store.js
--rw-r--r--   0        0        0      318 2024-04-24 10:17:38.710736 django_mapengine-1.7.0/django_mapengine/templates/django_mapengine/map.html
--rw-r--r--   0        0        0     1227 2024-04-24 10:17:38.710736 django_mapengine-1.7.0/django_mapengine/templates/django_mapengine/map_basemaps.html
--rw-r--r--   0        0        0      937 2024-03-07 12:05:14.131045 django_mapengine-1.7.0/django_mapengine/templates/django_mapengine/map_js.html
--rw-r--r--   0        0        0      489 2024-04-24 10:17:38.710736 django_mapengine-1.7.0/django_mapengine/templates/django_mapengine/map_json.html
--rw-r--r--   0        0        0     1968 2024-03-14 11:59:59.039708 django_mapengine-1.7.0/django_mapengine/urls.py
--rw-r--r--   0        0        0     1264 2023-06-14 12:49:56.422190 django_mapengine-1.7.0/django_mapengine/utils.py
--rw-r--r--   0        0        0     2955 2024-05-13 08:26:48.533344 django_mapengine-1.7.0/django_mapengine/views.py
--rw-r--r--   0        0        0     1767 2024-05-13 08:57:55.369433 django_mapengine-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     4602 1970-01-01 00:00:00.000000 django_mapengine-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-03-12 15:15:44.559160 django_mapengine-1.8.0/LICENSE
+-rw-r--r--   0        0        0     3821 2024-05-23 12:36:56.660901 django_mapengine-1.8.0/README.md
+-rw-r--r--   0        0        0       60 2024-05-23 12:36:56.660901 django_mapengine-1.8.0/django_mapengine/__init__.py
+-rw-r--r--   0        0        0     3895 2024-04-25 07:43:15.134289 django_mapengine-1.8.0/django_mapengine/apps.py
+-rw-r--r--   0        0        0     7049 2024-05-23 12:36:56.660901 django_mapengine-1.8.0/django_mapengine/choropleth.py
+-rw-r--r--   0        0        0    43608 2024-03-12 15:15:44.559160 django_mapengine-1.8.0/django_mapengine/colorbrewer.py
+-rw-r--r--   0        0        0     2230 2024-03-26 11:51:33.500776 django_mapengine-1.8.0/django_mapengine/distill.py
+-rw-r--r--   0        0        0    10173 2024-04-24 10:17:38.710736 django_mapengine-1.8.0/django_mapengine/layers.py
+-rw-r--r--   0        0        0      928 2024-03-14 11:59:59.035708 django_mapengine-1.8.0/django_mapengine/legend.py
+-rw-r--r--   0        0        0      655 2024-05-13 08:57:55.369433 django_mapengine-1.8.0/django_mapengine/middleware.py
+-rw-r--r--   0        0        0     2516 2024-03-14 11:59:59.039708 django_mapengine-1.8.0/django_mapengine/mvt.py
+-rw-r--r--   0        0        0     2161 2023-06-14 12:49:56.418190 django_mapengine-1.8.0/django_mapengine/popups.py
+-rw-r--r--   0        0        0     4014 2024-04-24 10:17:38.710736 django_mapengine-1.8.0/django_mapengine/setup.py
+-rw-r--r--   0        0        0     5664 2024-04-24 10:17:38.710736 django_mapengine-1.8.0/django_mapengine/sources.py
+-rw-r--r--   0        0        0    12661 2024-04-25 07:43:15.134289 django_mapengine-1.8.0/django_mapengine/static/django_mapengine/images/layer_ctrl_dark.svg
+-rw-r--r--   0        0        0    14131 2024-04-24 10:17:38.710736 django_mapengine-1.8.0/django_mapengine/static/django_mapengine/images/layer_ctrl_default.svg
+-rw-r--r--   0        0        0    12284 2024-04-25 07:43:15.134289 django_mapengine-1.8.0/django_mapengine/static/django_mapengine/images/layer_ctrl_light.svg
+-rw-r--r--   0        0        0    10121 2024-04-24 10:17:38.710736 django_mapengine-1.8.0/django_mapengine/static/django_mapengine/images/layer_ctrl_satellite.svg
+-rw-r--r--   0        0        0     1262 2024-04-24 10:17:38.710736 django_mapengine-1.8.0/django_mapengine/static/django_mapengine/js/basemaps.js
+-rw-r--r--   0        0        0     3220 2024-02-02 13:11:04.816042 django_mapengine-1.8.0/django_mapengine/static/django_mapengine/js/choropleth.js
+-rw-r--r--   0        0        0      455 2024-03-12 15:15:44.559160 django_mapengine-1.8.0/django_mapengine/static/django_mapengine/js/events.js
+-rw-r--r--   0        0        0      605 2023-06-14 12:49:56.422190 django_mapengine-1.8.0/django_mapengine/static/django_mapengine/js/helper.js
+-rw-r--r--   0        0        0     1128 2023-08-23 11:10:37.048313 django_mapengine-1.8.0/django_mapengine/static/django_mapengine/js/init.js
+-rw-r--r--   0        0        0     3577 2024-04-24 10:17:38.710736 django_mapengine-1.8.0/django_mapengine/static/django_mapengine/js/layer.js
+-rw-r--r--   0        0        0     3047 2024-05-23 12:36:56.660901 django_mapengine-1.8.0/django_mapengine/static/django_mapengine/js/legend.js
+-rw-r--r--   0        0        0     1782 2024-04-24 10:17:38.710736 django_mapengine-1.8.0/django_mapengine/static/django_mapengine/js/map.js
+-rw-r--r--   0        0        0     2804 2024-03-12 15:15:49.899159 django_mapengine-1.8.0/django_mapengine/static/django_mapengine/js/popup.js
+-rw-r--r--   0        0        0     2558 2023-06-14 12:49:56.422190 django_mapengine-1.8.0/django_mapengine/static/django_mapengine/js/regions.js
+-rw-r--r--   0        0        0      513 2023-06-14 12:49:56.422190 django_mapengine-1.8.0/django_mapengine/static/django_mapengine/js/store.js
+-rw-r--r--   0        0        0      318 2024-04-24 10:17:38.710736 django_mapengine-1.8.0/django_mapengine/templates/django_mapengine/map.html
+-rw-r--r--   0        0        0     1227 2024-04-24 10:17:38.710736 django_mapengine-1.8.0/django_mapengine/templates/django_mapengine/map_basemaps.html
+-rw-r--r--   0        0        0      937 2024-03-07 12:05:14.131045 django_mapengine-1.8.0/django_mapengine/templates/django_mapengine/map_js.html
+-rw-r--r--   0        0        0      489 2024-04-24 10:17:38.710736 django_mapengine-1.8.0/django_mapengine/templates/django_mapengine/map_json.html
+-rw-r--r--   0        0        0     1968 2024-03-14 11:59:59.039708 django_mapengine-1.8.0/django_mapengine/urls.py
+-rw-r--r--   0        0        0     1264 2023-06-14 12:49:56.422190 django_mapengine-1.8.0/django_mapengine/utils.py
+-rw-r--r--   0        0        0     2955 2024-05-13 08:26:48.533344 django_mapengine-1.8.0/django_mapengine/views.py
+-rw-r--r--   0        0        0     1785 2024-05-23 12:36:56.660901 django_mapengine-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     4702 1970-01-01 00:00:00.000000 django_mapengine-1.8.0/PKG-INFO
```

### Comparing `django_mapengine-1.7.0/LICENSE` & `django_mapengine-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.7.0/README.md` & `django_mapengine-1.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -112,8 +112,10 @@
    ```html
    <script src="{% static 'django_mapengine/js/basemaps.js' %}" type="text/javascript"></script>
    {% include 'django_mapengine/map_basemaps.html'}
    ```
 
 # User Guides
 
-- [Layers](docs/LAYERS.md)
+- [How to define layers](docs/LAYERS.md)
+- [How to enable popups](docs/POPUPS.md)
+- [How to set up clusters](docs/CLUSTERS.md)
```

#### html2text {}

```diff
@@ -34,9 +34,10 @@
 javascript %} {{ block.super }} {% compress js %}
 {% endcompress %} {% endblock javascript %} {% block inline_javascript %} {%
 include 'django_mapengine/map_json.html' %} {% compress js %} {% include
 'django_mapengine/map_js.html' %} {% endcompress %} {% endblock %} {% block css
 %} {% compress css %}
 {% endcompress %} {% endblock css %} ``` 7. If you want to integrate basemaps
 to your map add the following to the corresponding places: ```html
-{% include 'django_mapengine/map_basemaps.html'} ``` # User Guides - [Layers]
-(docs/LAYERS.md)
+{% include 'django_mapengine/map_basemaps.html'} ``` # User Guides - [How to
+define layers](docs/LAYERS.md) - [How to enable popups](docs/POPUPS.md) - [How
+to set up clusters](docs/CLUSTERS.md)
```

### Comparing `django_mapengine-1.7.0/django_mapengine/apps.py` & `django_mapengine-1.8.0/django_mapengine/apps.py`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.7.0/django_mapengine/choropleth.py` & `django_mapengine-1.8.0/django_mapengine/choropleth.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pathlib
 from typing import Optional, Union
 
 from . import colorbrewer
 
 MAX_COLORBREWER_STEPS = 9
 
-DEFAULT_CHOROPLETH_CONFIG = {"color_palette": "YlGnBu", "num_colors": 6}
+DEFAULT_CHOROPLETH_CONFIG = {"color_palette": "YlGnBu", "num_colors": 5}
 
 
 class ChoroplethError(Exception):
     """Raised if something is wrong with choropleth values or parameters."""
 
 
 class Choropleth:
@@ -97,16 +97,16 @@
                 raise ChoroplethError(error_msg)
             min_value = self.__calculate_lower_limit(min(values))
             max_value = self.__calculate_upper_limit(max(values))
             if choropleth_config["num_colors"]:
                 num = choropleth_config["num_colors"]
             else:
                 num = 6
-            step = (max_value - min_value) / (num - 1)
-            return [min_value + i * step for i in range(num - 1)] + [max_value]
+            step_size = self.__calculate_step_size(min_value, max_value, num)
+            return [min_value + i * step_size for i in range(num)] + [max_value]
 
         if "values" not in choropleth_config:
             error_msg = "Values have to be set in style file in order to composite choropleth colors."
             raise ChoroplethError(error_msg)
         return choropleth_config["values"]
 
     def get_fill_color(self, name: str, values: Optional[list] = None) -> list:
@@ -135,53 +135,62 @@
         steps = self.__calculate_steps(choropleth_config, values)
         if choropleth_config["color_palette"] not in colorbrewer.sequential["multihue"]:
             error_msg = f"Invalid color palette for choropleth {name=}."
             raise ChoroplethError(error_msg)
         if len(steps) > MAX_COLORBREWER_STEPS:
             error_msg = f"Too many choropleth values given for {name=}."
             raise IndexError(error_msg)
-        colors = colorbrewer.sequential["multihue"][choropleth_config["color_palette"]][len(steps)]
+        colors = colorbrewer.sequential["multihue"][choropleth_config["color_palette"]][len(steps) - 1]
         fill_color = [
             "interpolate",
             ["linear"],
             ["feature-state", name],
         ]
         for value, color in zip(steps, colors):
             fill_color.append(value)
             rgb_color = f"rgb({color[0]}, {color[1]}, {color[2]})"
             fill_color.append(rgb_color)
         return fill_color
 
     @staticmethod
+    def __calculate_step_size(min_value: float, max_value: float, num: int) -> float:
+        """
+        Calculate step size
+
+        Algorithm tries to find nice step sizes instead of simply dividing range by number of steps.
+        """
+        return (max_value - min_value) / num
+
+    @staticmethod
     def __calculate_lower_limit(number: float) -> int:
         """
         Calculate a significant number as lower limit for choropleth coloring
 
         Parameters
         ----------
         number: float
             find lower limit for this number
 
         Returns
         -------
         int
-            rounded down value by meaningful amount, depending on the size of mini
+            rounded down value by meaningful amount
 
         Raises
         ------
         ValueError
             if lower limit cannot be found
         """
         if number == 0:
-            return number
+            return int(number)
         if number < 1:
             return int((number * 10) / 10)
-        if number > 1:
-            digits = int(math.log10(number))
-            return int(number / pow(10, digits)) * 10**digits
+        if number >= 1:
+            digits = int(math.log10(number)) + 1
+            return int(number / 10**digits) * 10**digits
         raise ValueError(f"Cannot find lower limit for {number=}")
 
     @staticmethod
     def __calculate_upper_limit(number: float) -> int:
         """Calculate a significant number as upper limit for choropleth coloring.
 
         Parameters
@@ -195,13 +204,13 @@
             rounded up value by meaningful amount, depending on the size of number
 
         Raises
         ------
         ValueError
             if upper limit cannot be found
         """
-        if number < 1:
+        if number <= 1:
             return math.ceil((number * 10) / 10)
         if number > 1:
-            digits = int(math.log10(number))
+            digits = int(math.log10(number)) + 1
             return math.ceil(number / 10**digits) * 10**digits
         raise ValueError(f"Cannot find upper limit for {number=}")
```

### Comparing `django_mapengine-1.7.0/django_mapengine/colorbrewer.py` & `django_mapengine-1.8.0/django_mapengine/colorbrewer.py`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.7.0/django_mapengine/distill.py` & `django_mapengine-1.8.0/django_mapengine/distill.py`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.7.0/django_mapengine/layers.py` & `django_mapengine-1.8.0/django_mapengine/layers.py`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.7.0/django_mapengine/legend.py` & `django_mapengine-1.8.0/django_mapengine/legend.py`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.7.0/django_mapengine/middleware.py` & `django_mapengine-1.8.0/django_mapengine/middleware.py`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.7.0/django_mapengine/mvt.py` & `django_mapengine-1.8.0/django_mapengine/mvt.py`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.7.0/django_mapengine/popups.py` & `django_mapengine-1.8.0/django_mapengine/popups.py`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.7.0/django_mapengine/setup.py` & `django_mapengine-1.8.0/django_mapengine/setup.py`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.7.0/django_mapengine/sources.py` & `django_mapengine-1.8.0/django_mapengine/sources.py`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.7.0/django_mapengine/static/django_mapengine/images/layer_ctrl_dark.svg` & `django_mapengine-1.8.0/django_mapengine/static/django_mapengine/images/layer_ctrl_dark.svg`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.7.0/django_mapengine/static/django_mapengine/images/layer_ctrl_default.svg` & `django_mapengine-1.8.0/django_mapengine/static/django_mapengine/images/layer_ctrl_default.svg`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.7.0/django_mapengine/static/django_mapengine/images/layer_ctrl_light.svg` & `django_mapengine-1.8.0/django_mapengine/static/django_mapengine/images/layer_ctrl_light.svg`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.7.0/django_mapengine/static/django_mapengine/images/layer_ctrl_satellite.svg` & `django_mapengine-1.8.0/django_mapengine/static/django_mapengine/images/layer_ctrl_satellite.svg`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.7.0/django_mapengine/static/django_mapengine/js/basemaps.js` & `django_mapengine-1.8.0/django_mapengine/static/django_mapengine/js/basemaps.js`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.7.0/django_mapengine/static/django_mapengine/js/choropleth.js` & `django_mapengine-1.8.0/django_mapengine/static/django_mapengine/js/choropleth.js`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.7.0/django_mapengine/static/django_mapengine/js/helper.js` & `django_mapengine-1.8.0/django_mapengine/static/django_mapengine/js/helper.js`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.7.0/django_mapengine/static/django_mapengine/js/init.js` & `django_mapengine-1.8.0/django_mapengine/static/django_mapengine/js/init.js`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.7.0/django_mapengine/static/django_mapengine/js/layer.js` & `django_mapengine-1.8.0/django_mapengine/static/django_mapengine/js/layer.js`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.7.0/django_mapengine/static/django_mapengine/js/legend.js` & `django_mapengine-1.8.0/django_mapengine/static/django_mapengine/js/legend.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -20,61 +20,52 @@
     <div class="legend__heading">
       <span class="legend__title">Legend -&nbsp;</span>
       <span class="legend__detail">${title}</span>
       <div class="legend__unit">${unit ? `(${unit})` : ""}</div>
     </div>
     <div class="legend__wrap">
       <div class="legend__column">
-        ${valueRanges.filter((value, idx) => idx < nextColumnStartIndex).map((value, idx) => `<div class="legend__item" id="legend__item__color-${idx}">${value}</div>`).join(' ')}
+        ${valueRanges.filter((value, idx) => idx <= nextColumnStartIndex).map((value, idx) => `<div class="legend__item" id="legend__item__color-${idx}">${value}</div>`).join(' ')}
       </div>
       <div class="legend__column">
-        ${valueRanges.filter((value, idx) => idx >= nextColumnStartIndex).map((value, idx) => `<div class="legend__item" id="legend__item__color-${idx + nextColumnStartIndex}">${value}</div>`).join(' ')}
+        ${valueRanges.filter((value, idx) => idx > nextColumnStartIndex).map((value, idx) => `<div class="legend__item" id="legend__item__color-${idx + nextColumnStartIndex}">${value}</div>`).join(' ')}
       </div>
     </div>
     <style>
     ${colors.map((colorValue, idx) => ` #legend__item__color-${idx}:before { background-color: ${colorValue}; }`).join(' ')}
     </style>
   `;
 };
 
 
 function loadLegend(msg, choroplethName) {
-    const title = map_store.cold.choropleths[choroplethName]["title"];
-    const unit = map_store.cold.choropleths[choroplethName]["unit"];
+    const title = map_store.cold.choropleths[choroplethName].title;
+    const unit = map_store.cold.choropleths[choroplethName].unit;
     const paintPropertiesPerLayer = map_store.cold.storedChoroplethPaintProperties[choroplethName];
 
     /* Find active layer */
     let paintProperties = null;
     for (const layerID in paintPropertiesPerLayer) {
         const layer = map.getLayer(layerID);
-        if (map.getZoom() > layer.minzoom && map.getZoom() < layer.maxzoom) {
+        if (layer.visibility === "visible") {
             paintProperties = paintPropertiesPerLayer[layerID];
-            break
+            break;
         }
     }
+    if (paintProperties === null) {
+        return logMessage(msg);
+    }
 
-    let colors = [];
-    let values = [];
-
-    for (const element in paintProperties["fill-color"]) {
-        let current = paintProperties["fill-color"][element];
-
-        if (typeof(current) == "number") {
-            if (Number.isInteger(current) === false) {
-                current = current.toFixed(2);
-            }
-
-            if (values.length === 0) {
-                values.push("0 - " + String(current));
-            } else {
-                values.push(values[values.length - 1].split(" ").slice(-1)[0] + " - " + String(current));
-            }
-        }
+    const colors = paintProperties["fill-color"].slice(3).filter((_, index) => index % 2 !== 0);
+    const values = paintProperties["fill-color"].slice(3).filter((_, index) => (index + 1) % 2 !== 0).map(value => value < 100 ? value.toFixed(2) : Math.round(value));
 
-        if (typeof(current) == "string" && current.slice(0, 3) === "rgb") {
-            colors.push(current);
-        }
+    let valueRanges = [];
+    const step_size = parseFloat(values[1]) - parseFloat(values[0]);
+    for (let i = 0; i < values.length; i++) {
+        const nextValue = i === values.length - 1 ? parseFloat(values[i]) + step_size : values[i + 1];
+        valueRanges.push(`${values[i]} - ${nextValue}`);
     }
+
     const entriesPerColumn = Math.floor(values.length / 2);
-    legendElement.innerHTML = createLegend(title, unit, colors, values, entriesPerColumn);
+    legendElement.innerHTML = createLegend(title, unit, colors, valueRanges, entriesPerColumn);
     return logMessage(msg);
 }
```

### Comparing `django_mapengine-1.7.0/django_mapengine/static/django_mapengine/js/map.js` & `django_mapengine-1.8.0/django_mapengine/static/django_mapengine/js/map.js`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.7.0/django_mapengine/static/django_mapengine/js/popup.js` & `django_mapengine-1.8.0/django_mapengine/static/django_mapengine/js/popup.js`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.7.0/django_mapengine/static/django_mapengine/js/regions.js` & `django_mapengine-1.8.0/django_mapengine/static/django_mapengine/js/regions.js`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.7.0/django_mapengine/static/django_mapengine/js/store.js` & `django_mapengine-1.8.0/django_mapengine/static/django_mapengine/js/store.js`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.7.0/django_mapengine/templates/django_mapengine/map_basemaps.html` & `django_mapengine-1.8.0/django_mapengine/templates/django_mapengine/map_basemaps.html`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.7.0/django_mapengine/templates/django_mapengine/map_js.html` & `django_mapengine-1.8.0/django_mapengine/templates/django_mapengine/map_js.html`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.7.0/django_mapengine/urls.py` & `django_mapengine-1.8.0/django_mapengine/urls.py`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.7.0/django_mapengine/utils.py` & `django_mapengine-1.8.0/django_mapengine/utils.py`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.7.0/django_mapengine/views.py` & `django_mapengine-1.8.0/django_mapengine/views.py`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.7.0/pyproject.toml` & `django_mapengine-1.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-mapengine"
-version = "1.7.0"
+version = "1.8.0"
 description = "Map engine for maplibre in django"
 authors = ["Hendrik Huyskens <hendrik.huyskens@rl-institut.de>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -25,14 +25,15 @@
 [tool.poetry.group.dev.dependencies]
 django = "^3.2.3"
 black = "^23.1.0"
 isort = "^5.12.0"
 flake8 = "^7.0.0"
 pylint = "^3.0.3"
 pylint-django = "^2.5.5"
+pytest = "^8.2.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [project.urls]
 Homepage = "https://github.com/rl-institut/django-mapengine"
```

### Comparing `django_mapengine-1.7.0/PKG-INFO` & `django_mapengine-1.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mapengine
-Version: 1.7.0
+Version: 1.8.0
 Summary: Map engine for maplibre in django
 Author: Hendrik Huyskens
 Author-email: hendrik.huyskens@rl-institut.de
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -134,9 +134,11 @@
    ```html
    <script src="{% static 'django_mapengine/js/basemaps.js' %}" type="text/javascript"></script>
    {% include 'django_mapengine/map_basemaps.html'}
    ```
 
 # User Guides
 
-- [Layers](docs/LAYERS.md)
+- [How to define layers](docs/LAYERS.md)
+- [How to enable popups](docs/POPUPS.md)
+- [How to set up clusters](docs/CLUSTERS.md)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-mapengine Version: 1.7.0 Summary: Map engine
+Metadata-Version: 2.1 Name: django-mapengine Version: 1.8.0 Summary: Map engine
 for maplibre in django Author: Hendrik Huyskens Author-email:
 hendrik.huyskens@rl-institut.de Requires-Python: >=3.9,<3.12 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
 Dist: django-appconf (>=1.0.5,<2.0.0) Requires-Dist: django-distill
@@ -47,9 +47,10 @@
 javascript %} {{ block.super }} {% compress js %}
 {% endcompress %} {% endblock javascript %} {% block inline_javascript %} {%
 include 'django_mapengine/map_json.html' %} {% compress js %} {% include
 'django_mapengine/map_js.html' %} {% endcompress %} {% endblock %} {% block css
 %} {% compress css %}
 {% endcompress %} {% endblock css %} ``` 7. If you want to integrate basemaps
 to your map add the following to the corresponding places: ```html
-{% include 'django_mapengine/map_basemaps.html'} ``` # User Guides - [Layers]
-(docs/LAYERS.md)
+{% include 'django_mapengine/map_basemaps.html'} ``` # User Guides - [How to
+define layers](docs/LAYERS.md) - [How to enable popups](docs/POPUPS.md) - [How
+to set up clusters](docs/CLUSTERS.md)
```

