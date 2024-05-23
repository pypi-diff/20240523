# Comparing `tmp/browser_hz-4.0.1.tar.gz` & `tmp/browser_hz-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browser_hz-4.0.1.tar", max compression
+gzip compressed data, was "browser_hz-4.1.0.tar", max compression
```

## Comparing `browser_hz-4.0.1.tar` & `browser_hz-4.1.0.tar`

### file list

```diff
@@ -1,9 +1,12 @@
--rw-r--r--   0        0        0     1181 2023-09-03 11:52:14.867365 browser_hz-4.0.1/README.md
--rw-r--r--   0        0        0      634 2023-09-03 11:52:14.867365 browser_hz-4.0.1/browser_hz/__init__.py
--rw-r--r--   0        0        0     3089 2023-09-03 11:52:14.867365 browser_hz-4.0.1/browser_hz/browser.py
--rw-r--r--   0        0        0      845 2023-09-03 11:52:14.867365 browser_hz-4.0.1/browser_hz/browser_factory.py
--rw-r--r--   0        0        0      435 2023-09-03 11:52:14.867365 browser_hz-4.0.1/browser_hz/browser_type.py
--rw-r--r--   0        0        0        0 2023-09-03 11:52:14.867365 browser_hz-4.0.1/browser_hz/utils/__init__.py
--rw-r--r--   0        0        0      259 2023-09-03 11:52:14.867365 browser_hz-4.0.1/browser_hz/utils/request.py
--rw-r--r--   0        0        0      959 2023-09-03 11:52:14.867365 browser_hz-4.0.1/pyproject.toml
--rw-r--r--   0        0        0     1751 1970-01-01 00:00:00.000000 browser_hz-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1379 2024-05-23 10:01:26.566679 browser_hz-4.1.0/README.md
+-rw-r--r--   0        0        0      624 2024-05-23 10:01:26.566679 browser_hz-4.1.0/browser_hz/__init__.py
+-rw-r--r--   0        0        0     1863 2024-05-23 10:01:26.566679 browser_hz-4.1.0/browser_hz/browser.py
+-rw-r--r--   0        0        0      638 2024-05-23 10:01:26.566679 browser_hz-4.1.0/browser_hz/browser_factory.py
+-rw-r--r--   0        0        0     1000 2024-05-23 10:01:26.566679 browser_hz-4.1.0/browser_hz/browser_options.py
+-rw-r--r--   0        0        0      387 2024-05-23 10:01:26.566679 browser_hz-4.1.0/browser_hz/browsers.py
+-rw-r--r--   0        0        0        0 2024-05-23 10:01:26.566679 browser_hz-4.1.0/browser_hz/helpers/__init__.py
+-rw-r--r--   0        0        0      767 2024-05-23 10:01:26.566679 browser_hz-4.1.0/browser_hz/helpers/element_helper.py
+-rw-r--r--   0        0        0     1533 2024-05-23 10:01:26.566679 browser_hz-4.1.0/browser_hz/helpers/network_helper.py
+-rw-r--r--   0        0        0      520 2024-05-23 10:01:26.566679 browser_hz-4.1.0/browser_hz/helpers/wait_helper.py
+-rw-r--r--   0        0        0      989 2024-05-23 10:01:26.570679 browser_hz-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2000 1970-01-01 00:00:00.000000 browser_hz-4.1.0/PKG-INFO
```

### Comparing `browser_hz-4.0.1/README.md` & `browser_hz-4.1.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,15 @@
-# Browser
+# Advertisements Browser
 
+[<img src="https://img.shields.io/badge/development-advertisements_test-purple">](https://github.com/hubzaj/advertisements-test)
 [![version](https://img.shields.io/pypi/v/browser-hz)](https://pypi.org/project/browser-hz/)
 
 ## Background
 
-This project was initiated with the aim of comprehending the fundamental workings of Python packages, their
-distribution, and the process of releasing them using the project and dependency management tool, Poetry.
-The package was developed for internal utilization across various Python projects such
-as [browser-network-interception](https://github.com/hubzaj/browser-network-interception).
-Its primary objective is to facilitate an in-depth understanding of package management while serving as a valuable asset
-for diverse Python projects.
+The initiation of this project had the goal of gaining a comprehensive understanding of the fundamental mechanisms behind Python packages, their distribution, and the process of releasing them. Poetry, a project and dependency management tool, was employed to achieve this objective. The resulting package was designed for internal use across different Python projects, including [advertisements-test](https://github.com/hubzaj/advertisements-test). Its main purpose is to provide insight into package management intricacies while serving as a valuable resource for a variety of Python projects.
 
 ### How to build project
 
 Requirements:
 
 -     Python ^3.11
 -     Poetry ^1.5.1
```

### Comparing `browser_hz-4.0.1/browser_hz/__init__.py` & `browser_hz-4.1.0/browser_hz/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from contextlib import contextmanager
 from logging import Logger, getLogger
 from typing import Generator
 
 from browser_hz.browser import Browser
 from browser_hz.browser_factory import create_browser
-from browser_hz.browser_type import BrowserType
+from browser_hz.browsers import Browsers
 
 LOGGER: Logger = getLogger(__name__)
 
 
 @contextmanager
-def open_browser(browser_type_: BrowserType) -> Generator[Browser, None, None]:
+def open_browser(browser_type_: Browsers) -> Generator[Browser, None, None]:
     browser_: Browser | None = None
     try:
         LOGGER.info(f'Open web browser [{browser_type_}]')
         browser_ = create_browser(browser_type_)
         yield browser_
     finally:
         browser_.close_tab()
```

### Comparing `browser_hz-4.0.1/pyproject.toml` & `browser_hz-4.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 [tool.poetry]
 name = "browser-hz"
-version = "4.0.1"
+version = "4.1.0"
 description = "Tailored Selenium Wire extension for in-house project development."
 authors = ["Hubert Zajac <hubertzajac6@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "browser_hz" }]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pylint = "^2.17.5"
 mypy = "^1.5.1"
-webdriver-manager = "^4.0.0"
+webdriver-manager = "^4.0.1"
 pytest = "^7.3.1"
 selenium-wire = "^5.1.0"
 
 [tool.flake8]
 exclude = [".git", ".venv", "__pycache__"]
 max_line_length = 120
 max-complexity = 8
 
 [tool.pylint.messages_control]
 max-line-length = 120
 max-attributes = 10
 disable = [
     "missing-docstring",
-    "logging-fstring-interpolation"
+    "logging-fstring-interpolation",
+    "too-few-public-methods"
 ]
 good-names = "x, y"
 
 [tool.mypy]
 namespace_packages = true
 packages = ["browser_hz", "tests"]
 ignore_missing_imports = true
```

### Comparing `browser_hz-4.0.1/PKG-INFO` & `browser_hz-4.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 Metadata-Version: 2.1
 Name: browser-hz
-Version: 4.0.1
+Version: 4.1.0
 Summary: Tailored Selenium Wire extension for in-house project development.
 Author: Hubert Zajac
 Author-email: hubertzajac6@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: mypy (>=1.5.1,<2.0.0)
 Requires-Dist: pylint (>=2.17.5,<3.0.0)
 Requires-Dist: pytest (>=7.3.1,<8.0.0)
 Requires-Dist: selenium-wire (>=5.1.0,<6.0.0)
-Requires-Dist: webdriver-manager (>=4.0.0,<5.0.0)
+Requires-Dist: webdriver-manager (>=4.0.1,<5.0.0)
 Description-Content-Type: text/markdown
 
-# Browser
+# Advertisements Browser
 
+[<img src="https://img.shields.io/badge/development-advertisements_test-purple">](https://github.com/hubzaj/advertisements-test)
 [![version](https://img.shields.io/pypi/v/browser-hz)](https://pypi.org/project/browser-hz/)
 
 ## Background
 
-This project was initiated with the aim of comprehending the fundamental workings of Python packages, their
-distribution, and the process of releasing them using the project and dependency management tool, Poetry.
-The package was developed for internal utilization across various Python projects such
-as [browser-network-interception](https://github.com/hubzaj/browser-network-interception).
-Its primary objective is to facilitate an in-depth understanding of package management while serving as a valuable asset
-for diverse Python projects.
+The initiation of this project had the goal of gaining a comprehensive understanding of the fundamental mechanisms behind Python packages, their distribution, and the process of releasing them. Poetry, a project and dependency management tool, was employed to achieve this objective. The resulting package was designed for internal use across different Python projects, including [advertisements-test](https://github.com/hubzaj/advertisements-test). Its main purpose is to provide insight into package management intricacies while serving as a valuable resource for a variety of Python projects.
 
 ### How to build project
 
 Requirements:
 
 -     Python ^3.11
 -     Poetry ^1.5.1
```

