# Comparing `tmp/liboxide-0.1.0.tar.gz` & `tmp/liboxide-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liboxide-0.1.0.tar", last modified: Tue Dec 26 09:17:43 2023, max compression
+gzip compressed data, was "liboxide-0.1.1.tar", last modified: Thu May 23 19:17:21 2024, max compression
```

## Comparing `liboxide-0.1.0.tar` & `liboxide-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 09:17:43.029081 liboxide-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2023-12-26 09:17:23.000000 liboxide-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2023-12-26 09:17:43.025081 liboxide-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      342 2023-12-26 09:17:23.000000 liboxide-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 09:17:43.025081 liboxide-0.1.0/liboxide/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2023-12-26 09:17:23.000000 liboxide-0.1.0/liboxide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2023-12-26 09:17:23.000000 liboxide-0.1.0/liboxide/_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2023-12-26 09:17:23.000000 liboxide-0.1.0/liboxide/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2023-12-26 09:17:23.000000 liboxide-0.1.0/liboxide/_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2023-12-26 09:17:23.000000 liboxide-0.1.0/liboxide/_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2023-12-26 09:17:23.000000 liboxide-0.1.0/liboxide/_power.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2023-12-26 09:17:23.000000 liboxide-0.1.0/liboxide/_screen.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2023-12-26 09:17:23.000000 liboxide-0.1.0/liboxide/_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2023-12-26 09:17:23.000000 liboxide-0.1.0/liboxide/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2023-12-26 09:17:23.000000 liboxide-0.1.0/liboxide/_wifi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2023-12-26 09:17:23.000000 liboxide-0.1.0/liboxide/_xdgsettings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 09:17:43.025081 liboxide-0.1.0/liboxide.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2023-12-26 09:17:43.000000 liboxide-0.1.0/liboxide.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      383 2023-12-26 09:17:43.000000 liboxide-0.1.0/liboxide.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-26 09:17:43.000000 liboxide-0.1.0/liboxide.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-26 09:17:43.000000 liboxide-0.1.0/liboxide.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      953 2023-12-26 09:17:23.000000 liboxide-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-26 09:17:43.029081 liboxide-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:21.187852 liboxide-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-23 19:17:17.000000 liboxide-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-23 19:17:21.187852 liboxide-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-23 19:17:17.000000 liboxide-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:21.187852 liboxide-0.1.1/liboxide/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-23 19:17:17.000000 liboxide-0.1.1/liboxide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-23 19:17:17.000000 liboxide-0.1.1/liboxide/_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-23 19:17:17.000000 liboxide-0.1.1/liboxide/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-23 19:17:17.000000 liboxide-0.1.1/liboxide/_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-23 19:17:17.000000 liboxide-0.1.1/liboxide/_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-23 19:17:17.000000 liboxide-0.1.1/liboxide/_power.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-23 19:17:17.000000 liboxide-0.1.1/liboxide/_screen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-23 19:17:17.000000 liboxide-0.1.1/liboxide/_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-23 19:17:17.000000 liboxide-0.1.1/liboxide/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-23 19:17:17.000000 liboxide-0.1.1/liboxide/_wifi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-23 19:17:17.000000 liboxide-0.1.1/liboxide/_xdgsettings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:21.187852 liboxide-0.1.1/liboxide.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-23 19:17:21.000000 liboxide-0.1.1/liboxide.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-23 19:17:21.000000 liboxide-0.1.1/liboxide.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 19:17:21.000000 liboxide-0.1.1/liboxide.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-23 19:17:21.000000 liboxide-0.1.1/liboxide.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-23 19:17:17.000000 liboxide-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 19:17:21.187852 liboxide-0.1.1/setup.cfg
```

### Comparing `liboxide-0.1.0/LICENSE` & `liboxide-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `liboxide-0.1.0/PKG-INFO` & `liboxide-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liboxide
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python wrapper around the oxide command line tools.
 Author-email: Nathaniel van Diepen <eeems@eeems.email>
 Maintainer-email: Nathaniel van Diepen <eeems@eeems.email>
 Project-URL: Homepage, https://github.com/Eeems-Org/python-liboxide
 Project-URL: Repository, https://github.com/Eeems-Org/python-liboxide.git
 Project-URL: Issues, https://github.com/Eeems-Org/python-liboxide/issues
 Classifier: Intended Audience :: Developers
@@ -14,14 +14,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![liboxide on PyPI](https://img.shields.io/pypi/v/liboxide)](https://pypi.org/project/liboxide)
+
 Python wrapper around the oxide command line tools
 ==================================================
 
 Installation
 ============
 
 ```bash
@@ -35,8 +37,16 @@
 import liboxide
 
 liboxide.wifi.enable()
 
 print("Applications:")
 for name, app in liboxide.apps.applications.items():
     print(f"  {name}: {app.bin}")
+
+autoLock = liboxide.settings.get("autoLock")
+print("Automatically locking after {autoLock} minutes")
+
+print(f"Battery level: {liboxide.power.batteryLevel}")
+while True:
+    batteryLevel = liboxide.power.on.batteryLevelChanged()
+    print(f"Battery level: {batteryLevel}")
 ```
```

### Comparing `liboxide-0.1.0/liboxide/__init__.py` & `liboxide-0.1.1/liboxide/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from ._apps import Application
 from ._apps import AppsAPI as apps
 from ._errors import TooFewArguments
 from ._errors import TooManyArguments
+from ._errors import ObjectNotFound
+from ._errors import RotException
 from ._notification import Notification
 from ._notification import NotificationAPI as notification
 from ._power import PowerAPI as power
 from ._screen import ScreenAPI as screen
 from ._screen import Screenshot
 from ._system import SystemAPI as system
 from ._wifi import BSS
```

### Comparing `liboxide-0.1.0/liboxide/_apps.py` & `liboxide-0.1.1/liboxide/_apps.py`

 * *Files identical despite different names*

### Comparing `liboxide-0.1.0/liboxide/_base.py` & `liboxide-0.1.1/liboxide/_base.py`

 * *Files identical despite different names*

### Comparing `liboxide-0.1.0/liboxide/_notification.py` & `liboxide-0.1.1/liboxide/_notification.py`

 * *Files identical despite different names*

### Comparing `liboxide-0.1.0/liboxide/_screen.py` & `liboxide-0.1.1/liboxide/_screen.py`

 * *Files identical despite different names*

### Comparing `liboxide-0.1.0/liboxide/_system.py` & `liboxide-0.1.1/liboxide/_system.py`

 * *Files identical despite different names*

### Comparing `liboxide-0.1.0/liboxide/_util.py` & `liboxide-0.1.1/liboxide/_util.py`

 * *Files identical despite different names*

### Comparing `liboxide-0.1.0/liboxide/_wifi.py` & `liboxide-0.1.1/liboxide/_wifi.py`

 * *Files identical despite different names*

### Comparing `liboxide-0.1.0/liboxide/_xdgsettings.py` & `liboxide-0.1.1/liboxide/_xdgsettings.py`

 * *Files identical despite different names*

### Comparing `liboxide-0.1.0/liboxide.egg-info/PKG-INFO` & `liboxide-0.1.1/liboxide.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liboxide
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python wrapper around the oxide command line tools.
 Author-email: Nathaniel van Diepen <eeems@eeems.email>
 Maintainer-email: Nathaniel van Diepen <eeems@eeems.email>
 Project-URL: Homepage, https://github.com/Eeems-Org/python-liboxide
 Project-URL: Repository, https://github.com/Eeems-Org/python-liboxide.git
 Project-URL: Issues, https://github.com/Eeems-Org/python-liboxide/issues
 Classifier: Intended Audience :: Developers
@@ -14,14 +14,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![liboxide on PyPI](https://img.shields.io/pypi/v/liboxide)](https://pypi.org/project/liboxide)
+
 Python wrapper around the oxide command line tools
 ==================================================
 
 Installation
 ============
 
 ```bash
@@ -35,8 +37,16 @@
 import liboxide
 
 liboxide.wifi.enable()
 
 print("Applications:")
 for name, app in liboxide.apps.applications.items():
     print(f"  {name}: {app.bin}")
+
+autoLock = liboxide.settings.get("autoLock")
+print("Automatically locking after {autoLock} minutes")
+
+print(f"Battery level: {liboxide.power.batteryLevel}")
+while True:
+    batteryLevel = liboxide.power.on.batteryLevelChanged()
+    print(f"Battery level: {batteryLevel}")
 ```
```

### Comparing `liboxide-0.1.0/pyproject.toml` & `liboxide-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "liboxide"
 description = "Python wrapper around the oxide command line tools."
 readme = "README.md"
-version = "0.1.0"
+version = "0.1.1"
 requires-python = ">= 3.9"
 authors = [
     {name = "Nathaniel van Diepen", email = "eeems@eeems.email"},
 ]
 maintainers = [
     {name = "Nathaniel van Diepen", email = "eeems@eeems.email"},
 ]
```

