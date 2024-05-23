# Comparing `tmp/ddcutils-1.0.7.tar.gz` & `tmp/ddcutils-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddcutils-1.0.7.tar", max compression
+gzip compressed data, was "ddcutils-1.0.9.tar", max compression
```

## Comparing `ddcutils-1.0.7.tar` & `ddcutils-1.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1062 2024-01-23 01:52:51.914466 ddcutils-1.0.7/LICENSE
--rw-r--r--   0        0        0     6705 2024-01-23 01:52:51.914466 ddcutils-1.0.7/README.md
--rw-r--r--   0        0        0     1162 2024-01-23 01:52:51.914466 ddcutils-1.0.7/ddcUtils/__init__.py
--rw-r--r--   0        0        0      249 2024-01-23 01:52:51.914466 ddcutils-1.0.7/ddcUtils/constants.py
--rw-r--r--   0        0        0       43 2024-01-23 01:52:51.914466 ddcutils-1.0.7/ddcUtils/databases/__init__.py
--rw-r--r--   0        0        0     2534 2024-01-23 01:52:51.914466 ddcutils-1.0.7/ddcUtils/databases/database.py
--rw-r--r--   0        0        0     1861 2024-01-23 01:52:51.914466 ddcutils-1.0.7/ddcUtils/databases/db_utils.py
--rw-r--r--   0        0        0      815 2024-01-23 01:52:51.914466 ddcutils-1.0.7/ddcUtils/exceptions.py
--rw-r--r--   0        0        0    11818 2024-01-23 01:52:51.914466 ddcutils-1.0.7/ddcUtils/file_utils.py
--rw-r--r--   0        0        0     5018 2024-01-23 01:52:51.914466 ddcutils-1.0.7/ddcUtils/log.py
--rw-r--r--   0        0        0     3051 2024-01-23 01:52:51.914466 ddcutils-1.0.7/ddcUtils/misc_utils.py
--rw-r--r--   0        0        0     1873 2024-01-23 01:52:51.914466 ddcutils-1.0.7/ddcUtils/os_utils.py
--rw-r--r--   0        0        0      815 2024-01-23 01:52:51.914466 ddcutils-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     7291 1970-01-01 00:00:00.000000 ddcutils-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-01-23 17:40:57.132768 ddcutils-1.0.9/LICENSE
+-rw-r--r--   0        0        0     6701 2024-01-23 17:40:57.132768 ddcutils-1.0.9/README.md
+-rw-r--r--   0        0        0     1568 2024-01-23 17:40:57.132768 ddcutils-1.0.9/ddcUtils/__init__.py
+-rw-r--r--   0        0        0      249 2024-01-23 17:40:57.132768 ddcutils-1.0.9/ddcUtils/constants.py
+-rw-r--r--   0        0        0       43 2024-01-23 17:40:57.132768 ddcutils-1.0.9/ddcUtils/databases/__init__.py
+-rw-r--r--   0        0        0     2534 2024-01-23 17:40:57.132768 ddcutils-1.0.9/ddcUtils/databases/database.py
+-rw-r--r--   0        0        0     1861 2024-01-23 17:40:57.132768 ddcutils-1.0.9/ddcUtils/databases/db_utils.py
+-rw-r--r--   0        0        0      815 2024-01-23 17:40:57.132768 ddcutils-1.0.9/ddcUtils/exceptions.py
+-rw-r--r--   0        0        0    11818 2024-01-23 17:40:57.132768 ddcutils-1.0.9/ddcUtils/file_utils.py
+-rw-r--r--   0        0        0     5018 2024-01-23 17:40:57.132768 ddcutils-1.0.9/ddcUtils/log.py
+-rw-r--r--   0        0        0     3051 2024-01-23 17:40:57.132768 ddcutils-1.0.9/ddcUtils/misc_utils.py
+-rw-r--r--   0        0        0     1873 2024-01-23 17:40:57.132768 ddcutils-1.0.9/ddcUtils/os_utils.py
+-rw-r--r--   0        0        0      834 2024-01-23 17:40:57.132768 ddcutils-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     7330 1970-01-01 00:00:00.000000 ddcutils-1.0.9/PKG-INFO
```

### Comparing `ddcutils-1.0.7/LICENSE` & `ddcutils-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ddcutils-1.0.7/README.md` & `ddcutils-1.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Few Utility Functions
 
-[<img src="https://img.shields.io/github/license/ddc/ddcUtils.svg?style=plastic">](https://github.com/ddc/ddcUtils/blob/master/LICENSE)
-[<img src="https://img.shields.io/badge/Python-3.11+-blue.svg?style=plastic">](https://www.python.org)
-[<img src="https://img.shields.io/pypi/v/ddcUtils.svg?style=plastic">](https://pypi.python.org/pypi/ddcUtils)
+[![License](https://img.shields.io/github/license/ddc/ddcUtils.svg?style=plastic)](https://github.com/ddc/ddcUtils/blob/master/LICENSE)
+[![Python](https://img.shields.io/badge/Python-3.11+-blue.svg?style=plastic)](https://www.python.org)
+[![pypi](https://img.shields.io/pypi/v/ddcUtils.svg?style=plastic)](https://pypi.python.org/pypi/ddcUtils)
 [![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fddc%2FddcUtils%2Fbadge%3Fref%3Dmain&style=plastic&label=build&logo=none)](https://actions-badge.atrox.dev/ddc/ddcUtils/goto?ref=main)
 
 
 # Install
 ```shell
 pip install ddcUtils
 pip install git+https://github.com/ddc/ddcUtils
```

### Comparing `ddcutils-1.0.7/ddcUtils/__init__.py` & `ddcutils-1.0.9/ddcUtils/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,58 @@
 from importlib.metadata import version
 import logging
+import os
+from pathlib import Path
 from typing import NamedTuple, Literal
-from logging import NullHandler
-from .misc_utils import Object, MiscUtils
-from .file_utils import FileUtils
-from .os_utils import OsUtils
 from .databases.db_utils import DBUtils
 from .exceptions import get_exception
+from .file_utils import FileUtils
 from .log import Log
-
-
-class VersionInfo(NamedTuple):
-    major: int
-    minor: int
-    micro: int
-    releaselevel: Literal["alpha", "beta", "candidate", "final"]
-    serial: int
+from .misc_utils import Object, MiscUtils
+from .os_utils import OsUtils
 
 
 __title__ = "ddcUtils"
 __author__ = "Daniel Costa"
 __email__ = "danieldcsta@gmail.com>"
 __license__ = "MIT"
 __copyright__ = "Copyright 2023-present ddc"
-__req_python_version__ = (3, 11, 0)
+_req_python_version = (3, 11, 0)
 
 
 try:
-    __version__ = tuple(int(x) for x in version(__title__).split("."))
-    _release_level = "final"
+    _version = tuple(int(x) for x in version(__title__).split("."))
 except ModuleNotFoundError:
-    __version__ = (0, 0, 0)
-    _release_level = "test"
+    # this will be called on local tests, since theres no package installed
+    import toml
+    pyproject = toml.load(os.path.join(Path(__file__).parent.parent, "pyproject.toml"))
+    _version = pyproject["tool"]["poetry"]["version"]
+    del pyproject
+
+
+class VersionInfo(NamedTuple):
+    major: int
+    minor: int
+    micro: int
+    releaselevel: Literal["alpha", "beta", "candidate", "final"]
+    serial: int
 
+
+__version__ = _version
 __version_info__: VersionInfo = VersionInfo(
     major=__version__[0],
     minor=__version__[1],
     micro=__version__[2],
-    releaselevel=_release_level,
+    releaselevel="final",
+    serial=0
+)
+__req_python_version__: VersionInfo = VersionInfo(
+    major=_req_python_version[0],
+    minor=_req_python_version[1],
+    micro=_req_python_version[2],
+    releaselevel="final",
     serial=0
 )
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
-del logging, NamedTuple, Literal, VersionInfo, version
+del logging, NamedTuple, Literal, VersionInfo, version, _version, _req_python_version
```

### Comparing `ddcutils-1.0.7/ddcUtils/databases/database.py` & `ddcutils-1.0.9/ddcUtils/databases/database.py`

 * *Files identical despite different names*

### Comparing `ddcutils-1.0.7/ddcUtils/databases/db_utils.py` & `ddcutils-1.0.9/ddcUtils/databases/db_utils.py`

 * *Files identical despite different names*

### Comparing `ddcutils-1.0.7/ddcUtils/exceptions.py` & `ddcutils-1.0.9/ddcUtils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ddcutils-1.0.7/ddcUtils/file_utils.py` & `ddcutils-1.0.9/ddcUtils/file_utils.py`

 * *Files identical despite different names*

### Comparing `ddcutils-1.0.7/ddcUtils/log.py` & `ddcutils-1.0.9/ddcUtils/log.py`

 * *Files identical despite different names*

### Comparing `ddcutils-1.0.7/ddcUtils/misc_utils.py` & `ddcutils-1.0.9/ddcUtils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `ddcutils-1.0.7/ddcUtils/os_utils.py` & `ddcutils-1.0.9/ddcUtils/os_utils.py`

 * *Files identical despite different names*

### Comparing `ddcutils-1.0.7/pyproject.toml` & `ddcutils-1.0.9/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [build-system]
 requires = ["poetry-core>=1.8.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ddcUtils"
-version = "1.0.7"
+version = "1.0.9"
 description = "Few Utilities"
 readme = "README.md"
 license = "MIT"
 authors = ["Daniel Costa <danieldcsta@gmail.com>"]
 homepage = "https://github.com/ddc/ddcUtils"
 packages = [{include = "ddcUtils"}]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.11.0"
 SQLAlchemy = "^2.0.25"
 urllib3 = "^2.1.0"
 requests = "^2.31.0"
+toml = "^0.10.2"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.4"
 coverage = "^7.4.0"
 poethepoet = "^0.24.4"
 
 [tool.poe.tasks]
```

### Comparing `ddcutils-1.0.7/PKG-INFO` & `ddcutils-1.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: ddcUtils
-Version: 1.0.7
+Version: 1.0.9
 Summary: Few Utilities
 Home-page: https://github.com/ddc/ddcUtils
 License: MIT
 Author: Daniel Costa
 Author-email: danieldcsta@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.11.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: SQLAlchemy (>=2.0.25,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: urllib3 (>=2.1.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Few Utility Functions
 
-[<img src="https://img.shields.io/github/license/ddc/ddcUtils.svg?style=plastic">](https://github.com/ddc/ddcUtils/blob/master/LICENSE)
-[<img src="https://img.shields.io/badge/Python-3.11+-blue.svg?style=plastic">](https://www.python.org)
-[<img src="https://img.shields.io/pypi/v/ddcUtils.svg?style=plastic">](https://pypi.python.org/pypi/ddcUtils)
+[![License](https://img.shields.io/github/license/ddc/ddcUtils.svg?style=plastic)](https://github.com/ddc/ddcUtils/blob/master/LICENSE)
+[![Python](https://img.shields.io/badge/Python-3.11+-blue.svg?style=plastic)](https://www.python.org)
+[![pypi](https://img.shields.io/pypi/v/ddcUtils.svg?style=plastic)](https://pypi.python.org/pypi/ddcUtils)
 [![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fddc%2FddcUtils%2Fbadge%3Fref%3Dmain&style=plastic&label=build&logo=none)](https://actions-badge.atrox.dev/ddc/ddcUtils/goto?ref=main)
 
 
 # Install
 ```shell
 pip install ddcUtils
 pip install git+https://github.com/ddc/ddcUtils
```

