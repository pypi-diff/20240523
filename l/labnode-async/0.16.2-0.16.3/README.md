# Comparing `tmp/labnode_async-0.16.2.tar.gz` & `tmp/labnode_async-0.16.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labnode_async-0.16.2.tar", last modified: Thu Sep 14 13:40:34 2023, max compression
+gzip compressed data, was "labnode_async-0.16.3.tar", last modified: Thu May 23 13:33:37 2024, max compression
```

## Comparing `labnode_async-0.16.2.tar` & `labnode_async-0.16.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 13:40:34.246642 labnode_async-0.16.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2023-09-14 13:40:06.000000 labnode_async-0.16.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2023-09-14 13:40:34.246642 labnode_async-0.16.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2023-09-14 13:40:06.000000 labnode_async-0.16.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 13:40:34.242642 labnode_async-0.16.2/labnode_async/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2023-09-14 13:40:06.000000 labnode_async-0.16.2/labnode_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-09-14 13:40:06.000000 labnode_async-0.16.2/labnode_async/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    14136 2023-09-14 13:40:06.000000 labnode_async-0.16.2/labnode_async/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2023-09-14 13:40:06.000000 labnode_async-0.16.2/labnode_async/device_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2023-09-14 13:40:06.000000 labnode_async-0.16.2/labnode_async/devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2023-09-14 13:40:06.000000 labnode_async-0.16.2/labnode_async/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2023-09-14 13:40:06.000000 labnode_async-0.16.2/labnode_async/ip_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2023-09-14 13:40:06.000000 labnode_async-0.16.2/labnode_async/labnode.py
--rw-r--r--   0 runner    (1001) docker     (127)    33462 2023-09-14 13:40:06.000000 labnode_async-0.16.2/labnode_async/pid_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     4105 2023-09-14 13:40:06.000000 labnode_async-0.16.2/labnode_async/serial_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 13:40:34.246642 labnode_async-0.16.2/labnode_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2023-09-14 13:40:34.000000 labnode_async-0.16.2/labnode_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      509 2023-09-14 13:40:34.000000 labnode_async-0.16.2/labnode_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-14 13:40:34.000000 labnode_async-0.16.2/labnode_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      188 2023-09-14 13:40:34.000000 labnode_async-0.16.2/labnode_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-09-14 13:40:34.000000 labnode_async-0.16.2/labnode_async.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2023-09-14 13:40:06.000000 labnode_async-0.16.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-14 13:40:34.246642 labnode_async-0.16.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-09-14 13:40:06.000000 labnode_async-0.16.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:33:37.854377 labnode_async-0.16.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-23 13:33:14.000000 labnode_async-0.16.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-05-23 13:33:37.854377 labnode_async-0.16.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-23 13:33:14.000000 labnode_async-0.16.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:33:37.854377 labnode_async-0.16.3/labnode_async/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-23 13:33:14.000000 labnode_async-0.16.3/labnode_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-23 13:33:14.000000 labnode_async-0.16.3/labnode_async/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14136 2024-05-23 13:33:14.000000 labnode_async-0.16.3/labnode_async/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-23 13:33:14.000000 labnode_async-0.16.3/labnode_async/device_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-05-23 13:33:14.000000 labnode_async-0.16.3/labnode_async/devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-23 13:33:14.000000 labnode_async-0.16.3/labnode_async/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-05-23 13:33:14.000000 labnode_async-0.16.3/labnode_async/ip_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-05-23 13:33:14.000000 labnode_async-0.16.3/labnode_async/labnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33462 2024-05-23 13:33:14.000000 labnode_async-0.16.3/labnode_async/pid_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-05-23 13:33:14.000000 labnode_async-0.16.3/labnode_async/serial_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:33:37.854377 labnode_async-0.16.3/labnode_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-05-23 13:33:37.000000 labnode_async-0.16.3/labnode_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-23 13:33:37.000000 labnode_async-0.16.3/labnode_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 13:33:37.000000 labnode_async-0.16.3/labnode_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-23 13:33:37.000000 labnode_async-0.16.3/labnode_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-23 13:33:37.000000 labnode_async-0.16.3/labnode_async.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-23 13:33:14.000000 labnode_async-0.16.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 13:33:37.854377 labnode_async-0.16.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-23 13:33:14.000000 labnode_async-0.16.3/setup.py
```

### Comparing `labnode_async-0.16.2/LICENSE` & `labnode_async-0.16.3/LICENSE`

 * *Files identical despite different names*

### Comparing `labnode_async-0.16.2/PKG-INFO` & `labnode_async-0.16.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labnode_async
-Version: 0.16.2
+Version: 0.16.3
 Summary: Python3 AsyncIO Labnode driver
 Author-email: Patrick Baus <patrick.baus@physik.tu-darmstadt.de>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/PatrickBaus/labnode_async
 Project-URL: Bug Tracker, https://github.com/PatrickBaus/labnode_async/issues
 Project-URL: Download, https://github.com/PatrickBaus/labnode_async/releases
 Project-URL: Documentation, https://patrickbaus.github.io/labnode_async/
@@ -43,21 +43,22 @@
 Requires-Dist: myst-parser; extra == "doc"
 Requires-Dist: sphinx; extra == "doc"
 Provides-Extra: test
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: pytest; extra == "test"
 
-[![pylint](https://github.com/PatrickBaus/labnode_async/actions/workflows/pylint.yml/badge.svg)](https://github.com/PatrickBaus/labnode_async/actions/workflows/pylint.yml)
+[![pylint](../../actions/workflows/pylint.yml/badge.svg)](../../actions/workflows/pylint.yml)
 [![PyPI](https://img.shields.io/pypi/v/labnode_async)](https://pypi.org/project/labnode_async/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/labnode_async)
 ![PyPI - Status](https://img.shields.io/pypi/status/labnode_async)
+[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](LICENSE)
 [![code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 # LabNode
-This is the Python3 AsyncIO API library for the [Labnode](https://github.com/TU-Darmstadt-APQ/Labnode_PID) system.
+This is the Python3 asyncio API library for the [Labnode](https://github.com/TU-Darmstadt-APQ/Labnode_PID) system.
 
 The library is fully type-hinted.
 
 ## Documentation
 The full documentation can be found on GitHub Pages:
 [https://patrickbaus.github.io/labnode_async/](https://patrickbaus.github.io/labnode_async/). I use the
 [Numpydoc](https://numpydoc.readthedocs.io/en/latest/format.html) style for documentation and
@@ -82,19 +83,19 @@
 
 # Create a device and start coding
 async with IPConnection("192.1680.0.2") as device:
     # Add your code here
     ...
 ```
 
-See [examples/](https://github.com/PatrickBaus/labnode_async/blob/master/examples/) for more working examples.
+See [examples/](/examples/) for more working examples.
 
 ## Versioning
 I use [SemVer](http://semver.org/) for versioning. For the versions available, see the
-[tags of this repository](https://github.com/PatrickBaus/labnode_async/tags).
+[tags of this repository](../../tags).
 
 ## Authors
 * **Patrick Baus** - *Initial work* - [PatrickBaus](https://github.com/PatrickBaus)
 
 ## License
 This project is licensed under the GPL v3 license - see the
-[LICENSE](https://github.com/PatrickBaus/labnode_async/blob/master/LICENSE) file for details.
+[LICENSE](LICENSE) file for details.
```

### Comparing `labnode_async-0.16.2/README.md` & `labnode_async-0.16.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-[![pylint](https://github.com/PatrickBaus/labnode_async/actions/workflows/pylint.yml/badge.svg)](https://github.com/PatrickBaus/labnode_async/actions/workflows/pylint.yml)
+[![pylint](../../actions/workflows/pylint.yml/badge.svg)](../../actions/workflows/pylint.yml)
 [![PyPI](https://img.shields.io/pypi/v/labnode_async)](https://pypi.org/project/labnode_async/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/labnode_async)
 ![PyPI - Status](https://img.shields.io/pypi/status/labnode_async)
+[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](LICENSE)
 [![code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 # LabNode
-This is the Python3 AsyncIO API library for the [Labnode](https://github.com/TU-Darmstadt-APQ/Labnode_PID) system.
+This is the Python3 asyncio API library for the [Labnode](https://github.com/TU-Darmstadt-APQ/Labnode_PID) system.
 
 The library is fully type-hinted.
 
 ## Documentation
 The full documentation can be found on GitHub Pages:
 [https://patrickbaus.github.io/labnode_async/](https://patrickbaus.github.io/labnode_async/). I use the
 [Numpydoc](https://numpydoc.readthedocs.io/en/latest/format.html) style for documentation and
@@ -33,19 +34,19 @@
 
 # Create a device and start coding
 async with IPConnection("192.1680.0.2") as device:
     # Add your code here
     ...
 ```
 
-See [examples/](https://github.com/PatrickBaus/labnode_async/blob/master/examples/) for more working examples.
+See [examples/](/examples/) for more working examples.
 
 ## Versioning
 I use [SemVer](http://semver.org/) for versioning. For the versions available, see the
-[tags of this repository](https://github.com/PatrickBaus/labnode_async/tags).
+[tags of this repository](../../tags).
 
 ## Authors
 * **Patrick Baus** - *Initial work* - [PatrickBaus](https://github.com/PatrickBaus)
 
 ## License
 This project is licensed under the GPL v3 license - see the
-[LICENSE](https://github.com/PatrickBaus/labnode_async/blob/master/LICENSE) file for details.
+[LICENSE](LICENSE) file for details.
```

### Comparing `labnode_async-0.16.2/labnode_async/connection.py` & `labnode_async-0.16.3/labnode_async/connection.py`

 * *Files identical despite different names*

### Comparing `labnode_async-0.16.2/labnode_async/device_factory.py` & `labnode_async-0.16.3/labnode_async/device_factory.py`

 * *Files identical despite different names*

### Comparing `labnode_async-0.16.2/labnode_async/devices.py` & `labnode_async-0.16.3/labnode_async/devices.py`

 * *Files identical despite different names*

### Comparing `labnode_async-0.16.2/labnode_async/errors.py` & `labnode_async-0.16.3/labnode_async/errors.py`

 * *Files identical despite different names*

### Comparing `labnode_async-0.16.2/labnode_async/ip_connection.py` & `labnode_async-0.16.3/labnode_async/ip_connection.py`

 * *Files identical despite different names*

### Comparing `labnode_async-0.16.2/labnode_async/labnode.py` & `labnode_async-0.16.3/labnode_async/labnode.py`

 * *Files identical despite different names*

### Comparing `labnode_async-0.16.2/labnode_async/pid_controller.py` & `labnode_async-0.16.3/labnode_async/pid_controller.py`

 * *Files identical despite different names*

### Comparing `labnode_async-0.16.2/labnode_async/serial_connection.py` & `labnode_async-0.16.3/labnode_async/serial_connection.py`

 * *Files identical despite different names*

### Comparing `labnode_async-0.16.2/labnode_async.egg-info/PKG-INFO` & `labnode_async-0.16.3/labnode_async.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: labnode-async
-Version: 0.16.2
+Name: labnode_async
+Version: 0.16.3
 Summary: Python3 AsyncIO Labnode driver
 Author-email: Patrick Baus <patrick.baus@physik.tu-darmstadt.de>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/PatrickBaus/labnode_async
 Project-URL: Bug Tracker, https://github.com/PatrickBaus/labnode_async/issues
 Project-URL: Download, https://github.com/PatrickBaus/labnode_async/releases
 Project-URL: Documentation, https://patrickbaus.github.io/labnode_async/
@@ -43,21 +43,22 @@
 Requires-Dist: myst-parser; extra == "doc"
 Requires-Dist: sphinx; extra == "doc"
 Provides-Extra: test
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: pytest; extra == "test"
 
-[![pylint](https://github.com/PatrickBaus/labnode_async/actions/workflows/pylint.yml/badge.svg)](https://github.com/PatrickBaus/labnode_async/actions/workflows/pylint.yml)
+[![pylint](../../actions/workflows/pylint.yml/badge.svg)](../../actions/workflows/pylint.yml)
 [![PyPI](https://img.shields.io/pypi/v/labnode_async)](https://pypi.org/project/labnode_async/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/labnode_async)
 ![PyPI - Status](https://img.shields.io/pypi/status/labnode_async)
+[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](LICENSE)
 [![code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 # LabNode
-This is the Python3 AsyncIO API library for the [Labnode](https://github.com/TU-Darmstadt-APQ/Labnode_PID) system.
+This is the Python3 asyncio API library for the [Labnode](https://github.com/TU-Darmstadt-APQ/Labnode_PID) system.
 
 The library is fully type-hinted.
 
 ## Documentation
 The full documentation can be found on GitHub Pages:
 [https://patrickbaus.github.io/labnode_async/](https://patrickbaus.github.io/labnode_async/). I use the
 [Numpydoc](https://numpydoc.readthedocs.io/en/latest/format.html) style for documentation and
@@ -82,19 +83,19 @@
 
 # Create a device and start coding
 async with IPConnection("192.1680.0.2") as device:
     # Add your code here
     ...
 ```
 
-See [examples/](https://github.com/PatrickBaus/labnode_async/blob/master/examples/) for more working examples.
+See [examples/](/examples/) for more working examples.
 
 ## Versioning
 I use [SemVer](http://semver.org/) for versioning. For the versions available, see the
-[tags of this repository](https://github.com/PatrickBaus/labnode_async/tags).
+[tags of this repository](../../tags).
 
 ## Authors
 * **Patrick Baus** - *Initial work* - [PatrickBaus](https://github.com/PatrickBaus)
 
 ## License
 This project is licensed under the GPL v3 license - see the
-[LICENSE](https://github.com/PatrickBaus/labnode_async/blob/master/LICENSE) file for details.
+[LICENSE](LICENSE) file for details.
```

### Comparing `labnode_async-0.16.2/pyproject.toml` & `labnode_async-0.16.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     "slow",
 ]
 
 [build-system]
 requires = [
     "setuptools>=61.0",
     "typing-extensions; python_version <'3.11'",
-    "cbor2",
+    "cbor2>=5.6.2",
     "cobs",
     "pyserial-asyncio",
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.dynamic]
 version = {attr = "labnode_async.__version__"}
```

