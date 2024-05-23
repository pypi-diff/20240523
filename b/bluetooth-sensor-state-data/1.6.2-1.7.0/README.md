# Comparing `tmp/bluetooth_sensor_state_data-1.6.2.tar.gz` & `tmp/bluetooth_sensor_state_data-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluetooth_sensor_state_data-1.6.2.tar", max compression
+gzip compressed data, was "bluetooth_sensor_state_data-1.7.0.tar", max compression
```

## Comparing `bluetooth_sensor_state_data-1.6.2.tar` & `bluetooth_sensor_state_data-1.7.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11345 2023-07-07 17:34:25.427437 bluetooth_sensor_state_data-1.6.2/LICENSE
--rw-r--r--   0        0        0     3740 2023-07-07 17:34:25.427437 bluetooth_sensor_state_data-1.6.2/README.md
--rw-r--r--   0        0        0     2532 2023-07-07 17:34:26.435433 bluetooth_sensor_state_data-1.6.2/pyproject.toml
--rw-r--r--   0        0        0     3128 2023-07-07 17:34:26.399433 bluetooth_sensor_state_data-1.6.2/src/bluetooth_sensor_state_data/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 17:34:25.427437 bluetooth_sensor_state_data-1.6.2/src/bluetooth_sensor_state_data/py.typed
--rw-r--r--   0        0        0     5268 1970-01-01 00:00:00.000000 bluetooth_sensor_state_data-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0    11345 2024-05-23 00:50:58.647638 bluetooth_sensor_state_data-1.7.0/LICENSE
+-rw-r--r--   0        0        0     3740 2024-05-23 00:50:58.647638 bluetooth_sensor_state_data-1.7.0/README.md
+-rw-r--r--   0        0        0     2532 2024-05-23 00:50:59.499643 bluetooth_sensor_state_data-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2992 2024-05-23 00:50:59.475643 bluetooth_sensor_state_data-1.7.0/src/bluetooth_sensor_state_data/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 00:50:58.651638 bluetooth_sensor_state_data-1.7.0/src/bluetooth_sensor_state_data/py.typed
+-rw-r--r--   0        0        0     5319 1970-01-01 00:00:00.000000 bluetooth_sensor_state_data-1.7.0/PKG-INFO
```

### Comparing `bluetooth_sensor_state_data-1.6.2/LICENSE` & `bluetooth_sensor_state_data-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bluetooth_sensor_state_data-1.6.2/README.md` & `bluetooth_sensor_state_data-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `bluetooth_sensor_state_data-1.6.2/pyproject.toml` & `bluetooth_sensor_state_data-1.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bluetooth-sensor-state-data"
-version = "1.6.2"
+version = "1.7.0"
 description = "Models for storing and converting Bluetooth Sensor State Data"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/bluetooth-devices/bluetooth-sensor-state-data"
 documentation = "https://bluetooth-sensor-state-data.readthedocs.io"
 classifiers = [
```

### Comparing `bluetooth_sensor_state_data-1.6.2/src/bluetooth_sensor_state_data/__init__.py` & `bluetooth_sensor_state_data-1.7.0/src/bluetooth_sensor_state_data/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-__version__ = "1.6.2"
+__version__ = "1.7.0"
 
 from abc import abstractmethod
 
 from home_assistant_bluetooth import BluetoothServiceInfo
 from sensor_state_data import DeviceClass, SensorData, SensorUpdate, Units
 
 SIGNAL_STRENGTH_KEY = DeviceClass.SIGNAL_STRENGTH.value
@@ -14,52 +14,47 @@
 
 class BluetoothData(SensorData):
     """Update bluetooth data."""
 
     def __init__(self) -> None:
         """Initialize the class."""
         super().__init__()
-        self._last_manufacturer_data_set_by_source: dict[
-            str, set[tuple[int, bytes]]
-        ] = {}
+        self._last_manufacturer_data_by_source: dict[str, dict[int, bytes]] = {}
 
     def changed_manufacturer_data(
         self, data: BluetoothServiceInfo, exclude_ids: set[int] | None = None
     ) -> dict[int, bytes]:
         """Find changed manufacturer data.
 
         This function is not re-entrant. It must only
         be called once per update.
         """
         manufacturer_data = data.manufacturer_data
         source = data.source
+        last_manufacturer_data = self._last_manufacturer_data_by_source.get(source)
 
-        last_manufacturer_data_set = (
-            self._last_manufacturer_data_set_by_source.setdefault(source, set())
-        )
         if exclude_ids:
             # If there are specific manufacturer data IDs to exclude,
             # then remove them from the set of manufacturer data.
-            manufacturer_data_set = {
-                key_val
-                for key_val in manufacturer_data.items()
-                if key_val[0] not in exclude_ids
+            new_manufacturer_data = {
+                k: v for k, v in manufacturer_data.items() if k not in exclude_ids
             }
         else:
-            manufacturer_data_set = set(manufacturer_data.items())
-        self._last_manufacturer_data_set_by_source[source] = manufacturer_data_set
+            new_manufacturer_data = manufacturer_data
 
-        if not last_manufacturer_data_set:
+        self._last_manufacturer_data_by_source[source] = manufacturer_data
+
+        if not last_manufacturer_data:
             # If there is no previous data and there is only one value
             # return it
             return (
-                dict(manufacturer_data_set) if len(manufacturer_data_set) == 1 else {}
+                new_manufacturer_data.copy() if len(new_manufacturer_data) == 1 else {}
             )
 
-        return dict(manufacturer_data_set - last_manufacturer_data_set)
+        return dict(new_manufacturer_data.items() - last_manufacturer_data.items())
 
     @abstractmethod
     def _start_update(self, data: BluetoothServiceInfo) -> None:
         """Update the data."""
 
     def supported(self, data: BluetoothServiceInfo) -> bool:
         """Return True if the device is supported."""
```

### Comparing `bluetooth_sensor_state_data-1.6.2/PKG-INFO` & `bluetooth_sensor_state_data-1.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluetooth-sensor-state-data
-Version: 1.6.2
+Version: 1.7.0
 Summary: Models for storing and converting Bluetooth Sensor State Data
 Home-page: https://github.com/bluetooth-devices/bluetooth-sensor-state-data
 License: Apache Software License 2.0
 Author: J. Nick Koston
 Author-email: nick@koston.org
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -12,14 +12,15 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: docs
 Requires-Dist: Sphinx (>=5.0,<6.0) ; extra == "docs"
 Requires-Dist: home-assistant-bluetooth (>=1.3.0)
 Requires-Dist: myst-parser (>=0.18,<0.19) ; extra == "docs"
 Requires-Dist: sensor-state-data (>=2.0)
 Requires-Dist: sphinx-rtd-theme (>=1.0,<2.0) ; extra == "docs"
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1 Name: bluetooth-sensor-state-data Version: 1.6.2 Summary:
+Metadata-Version: 2.1 Name: bluetooth-sensor-state-data Version: 1.7.0 Summary:
 Models for storing and converting Bluetooth Sensor State Data Home-page: https:
 //github.com/bluetooth-devices/bluetooth-sensor-state-data License: Apache
 Software License 2.0 Author: J. Nick Koston Author-email: nick@koston.org
 Requires-Python: >=3.9,<4.0 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: Other/
 Proprietary License Classifier: Natural Language :: English Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries Provides-Extra: docs
-Requires-Dist: Sphinx (>=5.0,<6.0) ; extra == "docs" Requires-Dist: home-
-assistant-bluetooth (>=1.3.0) Requires-Dist: myst-parser (>=0.18,<0.19) ; extra
-== "docs" Requires-Dist: sensor-state-data (>=2.0) Requires-Dist: sphinx-rtd-
-theme (>=1.0,<2.0) ; extra == "docs" Project-URL: Bug Tracker, https://
-github.com/bluetooth-devices/bluetooth-sensor-state-data/issues Project-URL:
-Changelog, https://github.com/bluetooth-devices/bluetooth-sensor-state-data/
-blob/main/CHANGELOG.md Project-URL: Documentation, https://bluetooth-sensor-
-state-data.readthedocs.io Project-URL: Repository, https://github.com/
-bluetooth-devices/bluetooth-sensor-state-data Description-Content-Type: text/
-markdown # bluetooth-sensor-state-data
+Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
+Software Development :: Libraries Provides-Extra: docs Requires-Dist: Sphinx
+(>=5.0,<6.0) ; extra == "docs" Requires-Dist: home-assistant-bluetooth
+(>=1.3.0) Requires-Dist: myst-parser (>=0.18,<0.19) ; extra == "docs" Requires-
+Dist: sensor-state-data (>=2.0) Requires-Dist: sphinx-rtd-theme (>=1.0,<2.0) ;
+extra == "docs" Project-URL: Bug Tracker, https://github.com/bluetooth-devices/
+bluetooth-sensor-state-data/issues Project-URL: Changelog, https://github.com/
+bluetooth-devices/bluetooth-sensor-state-data/blob/main/CHANGELOG.md Project-
+URL: Documentation, https://bluetooth-sensor-state-data.readthedocs.io Project-
+URL: Repository, https://github.com/bluetooth-devices/bluetooth-sensor-state-
+data Description-Content-Type: text/markdown # bluetooth-sensor-state-data
           _[_C_I_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_T_e_s_t_ _c_o_v_e_r_a_g_e_ _p_e_r_c_e_n_t_a_g_e_]
                           _[_P_o_e_t_r_y_]_[_b_l_a_c_k_]_[_p_r_e_-_c_o_m_m_i_t_]
               _[_P_y_P_I_ _V_e_r_s_i_o_n_][Supported Python versions][License]
 Models for storing and converting Bluetooth Sensor State Data ## Installation
 Install this via pip (or your favourite package manager): `pip install
 bluetooth-sensor-state-data` ## Contributors â¨ Thanks goes to these wonderful
 people ([emoji key](https://allcontributors.org/docs/en/emoji-key)): This
```

