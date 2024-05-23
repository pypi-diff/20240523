# Comparing `tmp/sharklog-0.0.3.tar.gz` & `tmp/sharklog-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharklog-0.0.3.tar", last modified: Tue May 21 09:20:37 2024, max compression
+gzip compressed data, was "sharklog-0.0.4.tar", last modified: Thu May 23 06:38:30 2024, max compression
```

## Comparing `sharklog-0.0.3.tar` & `sharklog-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 jinqi     (1000) jinqi     (1000)        0 2024-05-21 09:20:37.271542 sharklog-0.0.3/
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)     1069 2024-05-21 04:05:28.000000 sharklog-0.0.3/LICENSE
--rw-r--r--   0 jinqi     (1000) jinqi     (1000)     3249 2024-05-21 09:20:37.271542 sharklog-0.0.3/PKG-INFO
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)     1610 2024-05-21 08:40:36.000000 sharklog-0.0.3/README.md
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)      502 2024-05-21 09:20:16.000000 sharklog-0.0.3/pyproject.toml
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)       38 2024-05-21 09:20:37.271542 sharklog-0.0.3/setup.cfg
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)       38 2024-05-21 04:05:28.000000 sharklog-0.0.3/setup.py
-drwxrwxr-x   0 jinqi     (1000) jinqi     (1000)        0 2024-05-21 09:20:37.271542 sharklog-0.0.3/src/
-drwxrwxr-x   0 jinqi     (1000) jinqi     (1000)        0 2024-05-21 09:20:37.271542 sharklog-0.0.3/src/sharklog/
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)        0 2024-05-21 04:05:28.000000 sharklog-0.0.3/src/sharklog/__init__.py
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)     1961 2024-05-21 08:33:18.000000 sharklog-0.0.3/src/sharklog/logging.py
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)      132 2024-05-21 08:58:30.000000 sharklog-0.0.3/src/sharklog/settings.py
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)     1780 2024-05-21 08:58:19.000000 sharklog-0.0.3/src/sharklog/utils.py
-drwxrwxr-x   0 jinqi     (1000) jinqi     (1000)        0 2024-05-21 09:20:37.271542 sharklog-0.0.3/src/sharklog.egg-info/
--rw-r--r--   0 jinqi     (1000) jinqi     (1000)     3249 2024-05-21 09:20:37.000000 sharklog-0.0.3/src/sharklog.egg-info/PKG-INFO
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)      281 2024-05-21 09:20:37.000000 sharklog-0.0.3/src/sharklog.egg-info/SOURCES.txt
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)        1 2024-05-21 09:20:37.000000 sharklog-0.0.3/src/sharklog.egg-info/dependency_links.txt
--rw-rw-r--   0 jinqi     (1000) jinqi     (1000)        9 2024-05-21 09:20:37.000000 sharklog-0.0.3/src/sharklog.egg-info/top_level.txt
+drwxrwxr-x   0 jinqi     (1000) jinqi     (1000)        0 2024-05-23 06:38:30.729612 sharklog-0.0.4/
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)     1069 2024-05-21 04:05:28.000000 sharklog-0.0.4/LICENSE
+-rw-r--r--   0 jinqi     (1000) jinqi     (1000)     5044 2024-05-23 06:38:30.729612 sharklog-0.0.4/PKG-INFO
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)     3405 2024-05-23 06:37:48.000000 sharklog-0.0.4/README.md
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)      502 2024-05-23 06:38:12.000000 sharklog-0.0.4/pyproject.toml
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)       38 2024-05-23 06:38:30.729612 sharklog-0.0.4/setup.cfg
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)       38 2024-05-21 04:05:28.000000 sharklog-0.0.4/setup.py
+drwxrwxr-x   0 jinqi     (1000) jinqi     (1000)        0 2024-05-23 06:38:30.729612 sharklog-0.0.4/src/
+drwxrwxr-x   0 jinqi     (1000) jinqi     (1000)        0 2024-05-23 06:38:30.729612 sharklog-0.0.4/src/sharklog/
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)        0 2024-05-21 04:05:28.000000 sharklog-0.0.4/src/sharklog/__init__.py
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)     1949 2024-05-23 06:20:01.000000 sharklog-0.0.4/src/sharklog/logging.py
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)      132 2024-05-21 10:10:46.000000 sharklog-0.0.4/src/sharklog/settings.py
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)     1780 2024-05-23 06:19:43.000000 sharklog-0.0.4/src/sharklog/utils.py
+drwxrwxr-x   0 jinqi     (1000) jinqi     (1000)        0 2024-05-23 06:38:30.729612 sharklog-0.0.4/src/sharklog.egg-info/
+-rw-r--r--   0 jinqi     (1000) jinqi     (1000)     5044 2024-05-23 06:38:30.000000 sharklog-0.0.4/src/sharklog.egg-info/PKG-INFO
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)      281 2024-05-23 06:38:30.000000 sharklog-0.0.4/src/sharklog.egg-info/SOURCES.txt
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)        1 2024-05-23 06:38:30.000000 sharklog-0.0.4/src/sharklog.egg-info/dependency_links.txt
+-rw-rw-r--   0 jinqi     (1000) jinqi     (1000)        9 2024-05-23 06:38:30.000000 sharklog-0.0.4/src/sharklog.egg-info/top_level.txt
```

### Comparing `sharklog-0.0.3/LICENSE` & `sharklog-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sharklog-0.0.3/PKG-INFO` & `sharklog-0.0.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharklog
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python logging helper
 Author-email: Shi Changshan <changshanshi@outlook.com>
 License: MIT License
         
         Copyright (c) 2024 ShiChangshan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,15 +34,14 @@
 
 # sharklog
 
 Python logging helper.
 
 [![PyPI License](https://img.shields.io/pypi/l/sharklog.svg)](https://pypi.org/project/sharklog)
 [![PyPI Version](https://img.shields.io/pypi/v/sharklog.svg)](https://pypi.org/project/sharklog)
-[![PyPI Downloads](https://img.shields.io/pypi/dm/sharklog.svg)](https://pypistats.org/packages/sharklog)
 
 ## Quick Start
 
 - Install sharklog:
 
 ```bash
 python -m pip install sharklog
@@ -50,51 +49,111 @@
 
 - Use in standalone script:
 
 ```python
 # standalone.py
 from sharklog import logging
 
-logging.init(debug=True)
+logging.init(debug=True)    # init all loggers with level=logging.DEBUG
+# or logging.init(level=logging.DEBUG)
 logging.debug("debug message")
 logging.info("info message")
 logging.warning("warning message")
 logging.error("error message")
 ```
 
-- Use in module:
+If you want to change logging level for a module, you can set it in the module by:
 
 ```python
-# submodule.py which is placed under package `parent`
+from sharklog import logging
+logging.getLogger().setLevel(logging.DEBUG)
+```
+
+or set it outside the module by specifying the logger name:
+
+```python
+from sharklog import logging
+logging.getLogger("module_name").setLevel(logging.DEBUG)
+```
+
+The default format of log messages is:
+
+```python
+"[%(levelname)s]: %(message)s [%(asctime)s](%(filename)s:%(lineno)d)"
+```
+
+## Usage in Package Development
+
+Now I assume your file structure is like this:
+
+```bash
+--- parent_package
+    |--- __init__.py
+    |--- parent_module.py
+    |--- logger.py
+    |--- sub_package
+        |--- __init__.py
+        |--- sub_module.py
+```
+
+- First, you can add `NullHandler` to the root logger in `parent_package/__init__.py`, which logger named `parent_package`:
+
+```python
+# parent/__init__.py
+from sharklog import logging
+
+logging.getLogger().addHandler(logging.NullHandler())
+```
+
+This is mentioned in the [Python Logging HOWTO](https://docs.python.org/3/howto/logging.html#configuring-logging-for-a-library) to identify the logger's default behavior.
+
+- Then, use `logging` in your package, they will be prefixed with the logger name `parent_package.`:
+
+```python
+# parent_module.py which is placed under package `parent_package`
 from sharklog import logging
 
-logger = logging.getLogger()    # the logger name will be `parent.submodule`
+logger = logging.getLogger()    # the logger name will be `parent_package.parent_module`
 
 logger.debug("debug message")
 logger.info("info message")
 logger.warning("warning message")
 logger.error("error message")
 ```
 
 If you already using builtin logging module, you can use sharklog as a drop-in replacement.
 
 Just change ~~`import logging`~~ into `from sharklog import logging`. Then you can use `logging` as usual:
 
 ```python
-# module_name.py
+# sub_module.py
 from sharklog import logging
 
 # these log messages will be prefixed with the logger name `xxxpackage.xxmodule.module_name`
+# here, as an example, the logger name will be `parent_package.sub_package.sub_module`
 logging.debug("debug message")
 logging.info("info message")
 logging.warning("warning message")
 logging.error("error message")
 ```
 
-## Usage in Package Development
+- Finally, you can set the logging level for the package in the main script which using the package:
 
 ```python
-# parent/__init__.py
+# main.py
 from sharklog import logging
 
-logging.getLogger().addHandler(logging.NullHandler())
+from parent_package import parent_module
+from parent_package.sub_package import sub_module
+
+if __name__ == "__main__":
+    logging.init(debug=True)    # init all loggers with level=logging.DEBUG
+    # or logging.init(level=logging.DEBUG)
+    # logging inside the package will use the level set here
+```
+
+Or if you want to change the logging level for a specific module, you can set it in the module by:
+
+```python
+from sharklog import logging
+logging.getLogger().setLevel(logging.WARNING)
 ```
```

### Comparing `sharklog-0.0.3/src/sharklog/logging.py` & `sharklog-0.0.4/src/sharklog/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-import sys
 import inspect
 import logging
-from logging import *
+import sys
+from logging import *  # noqa
 
-from sharklog import utils
-from sharklog import settings
+from sharklog import settings, utils
 
 
 def init(*, debug=False, level=None, **kwargs):
     if debug:
         settings.DEFAULT_LEVEL = logging.DEBUG
     elif level is not None:
         try:
```

### Comparing `sharklog-0.0.3/src/sharklog/utils.py` & `sharklog-0.0.4/src/sharklog/utils.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+import dataclasses
 import inspect
 import logging
-from typing import Dict, Tuple
-import dataclasses
 from pprint import pformat
+from typing import Dict, Tuple
 
 
 def create_logger_record(
     level, message, *args, name: str = "", exc_info=None, **kwargs
 ) -> bool:
     frame = inspect.currentframe().f_back.f_back.f_back  # type: ignore
     assert frame
```

### Comparing `sharklog-0.0.3/src/sharklog.egg-info/PKG-INFO` & `sharklog-0.0.4/src/sharklog.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharklog
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python logging helper
 Author-email: Shi Changshan <changshanshi@outlook.com>
 License: MIT License
         
         Copyright (c) 2024 ShiChangshan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,15 +34,14 @@
 
 # sharklog
 
 Python logging helper.
 
 [![PyPI License](https://img.shields.io/pypi/l/sharklog.svg)](https://pypi.org/project/sharklog)
 [![PyPI Version](https://img.shields.io/pypi/v/sharklog.svg)](https://pypi.org/project/sharklog)
-[![PyPI Downloads](https://img.shields.io/pypi/dm/sharklog.svg)](https://pypistats.org/packages/sharklog)
 
 ## Quick Start
 
 - Install sharklog:
 
 ```bash
 python -m pip install sharklog
@@ -50,51 +49,111 @@
 
 - Use in standalone script:
 
 ```python
 # standalone.py
 from sharklog import logging
 
-logging.init(debug=True)
+logging.init(debug=True)    # init all loggers with level=logging.DEBUG
+# or logging.init(level=logging.DEBUG)
 logging.debug("debug message")
 logging.info("info message")
 logging.warning("warning message")
 logging.error("error message")
 ```
 
-- Use in module:
+If you want to change logging level for a module, you can set it in the module by:
 
 ```python
-# submodule.py which is placed under package `parent`
+from sharklog import logging
+logging.getLogger().setLevel(logging.DEBUG)
+```
+
+or set it outside the module by specifying the logger name:
+
+```python
+from sharklog import logging
+logging.getLogger("module_name").setLevel(logging.DEBUG)
+```
+
+The default format of log messages is:
+
+```python
+"[%(levelname)s]: %(message)s [%(asctime)s](%(filename)s:%(lineno)d)"
+```
+
+## Usage in Package Development
+
+Now I assume your file structure is like this:
+
+```bash
+--- parent_package
+    |--- __init__.py
+    |--- parent_module.py
+    |--- logger.py
+    |--- sub_package
+        |--- __init__.py
+        |--- sub_module.py
+```
+
+- First, you can add `NullHandler` to the root logger in `parent_package/__init__.py`, which logger named `parent_package`:
+
+```python
+# parent/__init__.py
+from sharklog import logging
+
+logging.getLogger().addHandler(logging.NullHandler())
+```
+
+This is mentioned in the [Python Logging HOWTO](https://docs.python.org/3/howto/logging.html#configuring-logging-for-a-library) to identify the logger's default behavior.
+
+- Then, use `logging` in your package, they will be prefixed with the logger name `parent_package.`:
+
+```python
+# parent_module.py which is placed under package `parent_package`
 from sharklog import logging
 
-logger = logging.getLogger()    # the logger name will be `parent.submodule`
+logger = logging.getLogger()    # the logger name will be `parent_package.parent_module`
 
 logger.debug("debug message")
 logger.info("info message")
 logger.warning("warning message")
 logger.error("error message")
 ```
 
 If you already using builtin logging module, you can use sharklog as a drop-in replacement.
 
 Just change ~~`import logging`~~ into `from sharklog import logging`. Then you can use `logging` as usual:
 
 ```python
-# module_name.py
+# sub_module.py
 from sharklog import logging
 
 # these log messages will be prefixed with the logger name `xxxpackage.xxmodule.module_name`
+# here, as an example, the logger name will be `parent_package.sub_package.sub_module`
 logging.debug("debug message")
 logging.info("info message")
 logging.warning("warning message")
 logging.error("error message")
 ```
 
-## Usage in Package Development
+- Finally, you can set the logging level for the package in the main script which using the package:
 
 ```python
-# parent/__init__.py
+# main.py
 from sharklog import logging
 
-logging.getLogger().addHandler(logging.NullHandler())
+from parent_package import parent_module
+from parent_package.sub_package import sub_module
+
+if __name__ == "__main__":
+    logging.init(debug=True)    # init all loggers with level=logging.DEBUG
+    # or logging.init(level=logging.DEBUG)
+    # logging inside the package will use the level set here
+```
+
+Or if you want to change the logging level for a specific module, you can set it in the module by:
+
+```python
+from sharklog import logging
+logging.getLogger().setLevel(logging.WARNING)
 ```
```

