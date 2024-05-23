# Comparing `tmp/pylint_pytest-1.1.8.tar.gz` & `tmp/pylint-pytest-2.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylint_pytest-1.1.8.tar", last modified: Thu May 23 08:26:31 2024, max compression
+gzip compressed data, was "pylint-pytest-2.0.0a0.tar", last modified: Fri Feb  2 16:54:31 2024, max compression
```

## Comparing `pylint_pytest-1.1.8.tar` & `pylint-pytest-2.0.0a0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:26:31.644855 pylint_pytest-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-23 08:26:14.000000 pylint_pytest-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-23 08:26:14.000000 pylint_pytest-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-05-23 08:26:31.644855 pylint_pytest-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-23 08:26:14.000000 pylint_pytest-1.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:26:31.640855 pylint_pytest-1.1.8/pylint_pytest/
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-23 08:26:14.000000 pylint_pytest-1.1.8/pylint_pytest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:26:31.640855 pylint_pytest-1.1.8/pylint_pytest/checkers/
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-23 08:26:14.000000 pylint_pytest-1.1.8/pylint_pytest/checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-23 08:26:14.000000 pylint_pytest-1.1.8/pylint_pytest/checkers/class_attr_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-05-23 08:26:14.000000 pylint_pytest-1.1.8/pylint_pytest/checkers/fixture.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-23 08:26:14.000000 pylint_pytest-1.1.8/pylint_pytest/checkers/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-05-23 08:26:14.000000 pylint_pytest-1.1.8/pylint_pytest/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:26:31.640855 pylint_pytest-1.1.8/pylint_pytest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-05-23 08:26:31.000000 pylint_pytest-1.1.8/pylint_pytest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-23 08:26:31.000000 pylint_pytest-1.1.8/pylint_pytest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 08:26:31.000000 pylint_pytest-1.1.8/pylint_pytest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-23 08:26:31.000000 pylint_pytest-1.1.8/pylint_pytest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-23 08:26:31.000000 pylint_pytest-1.1.8/pylint_pytest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-05-23 08:26:14.000000 pylint_pytest-1.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-23 08:26:31.644855 pylint_pytest-1.1.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2058 2024-05-23 08:26:14.000000 pylint_pytest-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 16:54:31.496373 pylint-pytest-2.0.0a0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-02-02 16:54:19.000000 pylint-pytest-2.0.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-02 16:54:19.000000 pylint-pytest-2.0.0a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-02-02 16:54:31.496373 pylint-pytest-2.0.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-02-02 16:54:19.000000 pylint-pytest-2.0.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 16:54:31.496373 pylint-pytest-2.0.0a0/pylint_pytest/
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-02-02 16:54:19.000000 pylint-pytest-2.0.0a0/pylint_pytest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 16:54:31.496373 pylint-pytest-2.0.0a0/pylint_pytest/checkers/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-02-02 16:54:19.000000 pylint-pytest-2.0.0a0/pylint_pytest/checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-02-02 16:54:19.000000 pylint-pytest-2.0.0a0/pylint_pytest/checkers/class_attr_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8685 2024-02-02 16:54:19.000000 pylint-pytest-2.0.0a0/pylint_pytest/checkers/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-02-02 16:54:19.000000 pylint-pytest-2.0.0a0/pylint_pytest/checkers/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-02-02 16:54:19.000000 pylint-pytest-2.0.0a0/pylint_pytest/checkers/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-02-02 16:54:19.000000 pylint-pytest-2.0.0a0/pylint_pytest/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 16:54:31.496373 pylint-pytest-2.0.0a0/pylint_pytest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-02-02 16:54:31.000000 pylint-pytest-2.0.0a0/pylint_pytest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-02-02 16:54:31.000000 pylint-pytest-2.0.0a0/pylint_pytest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 16:54:31.000000 pylint-pytest-2.0.0a0/pylint_pytest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-02 16:54:31.000000 pylint-pytest-2.0.0a0/pylint_pytest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-02 16:54:31.000000 pylint-pytest-2.0.0a0/pylint_pytest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-02-02 16:54:19.000000 pylint-pytest-2.0.0a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-02 16:54:31.496373 pylint-pytest-2.0.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-02 16:54:19.000000 pylint-pytest-2.0.0a0/setup.py
```

### Comparing `pylint_pytest-1.1.8/LICENSE` & `pylint-pytest-2.0.0a0/LICENSE`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 The MIT License (MIT)
 
 Copyright (c) 2020 Reverb Chu
+Copyright (c) 2023-2024 Stavros Ntentos
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pylint_pytest-1.1.8/PKG-INFO` & `pylint-pytest-2.0.0a0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,62 @@
 Metadata-Version: 2.1
 Name: pylint-pytest
-Version: 1.1.8
+Version: 2.0.0a0
 Summary: A Pylint plugin to suppress pytest-related false positives.
-Home-page: https://github.com/pylint-dev/pylint-pytest
-Author: Stavros Ntentos
-Author-email: 133706+stdedos@users.noreply.github.com
-License: MIT
+Author: Reverb Chu
+Maintainer-email: Stavros Ntentos <133706+stdedos@users.noreply.github.com>, Pierre Sassoulas <pierre.sassoulas@gmail.com>
+License: The MIT License (MIT)
+        
+        Copyright (c) 2020 Reverb Chu
+        Copyright (c) 2023-2024 Stavros Ntentos
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in
+        all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+        THE SOFTWARE.
+        
 Project-URL: Changelog, https://github.com/pylint-dev/pylint-pytest/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/pylint-dev/pylint-pytest#readme
-Project-URL: Say Thanks!, https://saythanks.io/to/stdedos
+Project-URL: Homepage, https://github.com/pylint-dev/pylint-pytest
 Project-URL: Source, https://github.com/pylint-dev/pylint-pytest
 Project-URL: Tracker, https://github.com/pylint-dev/pylint-pytest/issues
+Project-URL: Say Thanks!, https://saythanks.io/to/stdedos
 Keywords: pylint,pytest,plugin
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pylint>=2
-Requires-Dist: pytest<=8.2.0,>=4.6
+Requires-Dist: pylint<4,>=2
+Requires-Dist: pytest>=4.6
 
 # pylint-pytest
 
 ![PyPI - Version](https://img.shields.io/pypi/v/pylint-pytest)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pylint-pytest)
 ![PyPI - Downloads](https://img.shields.io/pypi/dd/pylint-pytest)
 ![PyPI - License](https://img.shields.io/pypi/l/pylint-pytest)
```

### Comparing `pylint_pytest-1.1.8/README.md` & `pylint-pytest-2.0.0a0/README.md`

 * *Files identical despite different names*

### Comparing `pylint_pytest-1.1.8/pylint_pytest/checkers/__init__.py` & `pylint-pytest-2.0.0a0/pylint_pytest/checkers/__init__.py`

 * *Files identical despite different names*

### Comparing `pylint_pytest-1.1.8/pylint_pytest/checkers/class_attr_loader.py` & `pylint-pytest-2.0.0a0/pylint_pytest/checkers/class_attr_loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from typing import Optional, Set
+from __future__ import annotations
 
 from astroid import Assign, Attribute, ClassDef, Name
 
 from ..utils import _can_use_fixture, _is_class_autouse_fixture
 from . import BasePytestChecker
 
 
 class ClassAttrLoader(BasePytestChecker):
     msgs = {"E6400": ("", "pytest-class-attr-loader", "")}
 
     in_setup = False
-    request_cls: Set[str] = set()
-    class_node: Optional[ClassDef] = None
+    request_cls: set[str] = set()
+    class_node: ClassDef | None = None
 
     def visit_functiondef(self, node):
         """determine if a method is a class setup method"""
         self.in_setup = False
         self.request_cls = set()
         self.class_node = None
```

### Comparing `pylint_pytest-1.1.8/pylint_pytest/utils.py` & `pylint-pytest-2.0.0a0/pylint_pytest/utils.py`

 * *Files identical despite different names*

### Comparing `pylint_pytest-1.1.8/pylint_pytest.egg-info/PKG-INFO` & `pylint-pytest-2.0.0a0/pylint_pytest.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,62 @@
 Metadata-Version: 2.1
 Name: pylint-pytest
-Version: 1.1.8
+Version: 2.0.0a0
 Summary: A Pylint plugin to suppress pytest-related false positives.
-Home-page: https://github.com/pylint-dev/pylint-pytest
-Author: Stavros Ntentos
-Author-email: 133706+stdedos@users.noreply.github.com
-License: MIT
+Author: Reverb Chu
+Maintainer-email: Stavros Ntentos <133706+stdedos@users.noreply.github.com>, Pierre Sassoulas <pierre.sassoulas@gmail.com>
+License: The MIT License (MIT)
+        
+        Copyright (c) 2020 Reverb Chu
+        Copyright (c) 2023-2024 Stavros Ntentos
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in
+        all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+        THE SOFTWARE.
+        
 Project-URL: Changelog, https://github.com/pylint-dev/pylint-pytest/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/pylint-dev/pylint-pytest#readme
-Project-URL: Say Thanks!, https://saythanks.io/to/stdedos
+Project-URL: Homepage, https://github.com/pylint-dev/pylint-pytest
 Project-URL: Source, https://github.com/pylint-dev/pylint-pytest
 Project-URL: Tracker, https://github.com/pylint-dev/pylint-pytest/issues
+Project-URL: Say Thanks!, https://saythanks.io/to/stdedos
 Keywords: pylint,pytest,plugin
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pylint>=2
-Requires-Dist: pytest<=8.2.0,>=4.6
+Requires-Dist: pylint<4,>=2
+Requires-Dist: pytest>=4.6
 
 # pylint-pytest
 
 ![PyPI - Version](https://img.shields.io/pypi/v/pylint-pytest)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pylint-pytest)
 ![PyPI - Downloads](https://img.shields.io/pypi/dd/pylint-pytest)
 ![PyPI - License](https://img.shields.io/pypi/l/pylint-pytest)
```

### Comparing `pylint_pytest-1.1.8/pyproject.toml` & `pylint-pytest-2.0.0a0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,75 @@
-# Only a configuration storage, for now
+[build-system]
+requires = ["setuptools>=66.1"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "pylint-pytest"
+version = "2.0.0a0"
+license = {file = "LICENSE"}
+description = "A Pylint plugin to suppress pytest-related false positives."
+
+authors = [
+    {name = "Reverb Chu"},
+]
+maintainers = [
+    {name = "Stavros Ntentos", email = "133706+stdedos@users.noreply.github.com"},
+    {name = "Pierre Sassoulas", email = "pierre.sassoulas@gmail.com"},
+]
+
+readme = "README.md"
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Developers",
+    "Topic :: Software Development :: Testing",
+    "Topic :: Software Development :: Quality Assurance",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: Implementation :: CPython",
+    "Operating System :: OS Independent",
+    "License :: OSI Approved :: MIT License",
+]
+keywords = [
+    "pylint",
+    "pytest",
+    "plugin",
+]
+
+requires-python = ">=3.8"
+dependencies = [
+    "pylint>=2,<4",
+    "pytest>=4.6",
+]
+
+# [project.optional-dependencies] moved to requirements/dev.in
+
+[project.urls]
+Changelog = "https://github.com/pylint-dev/pylint-pytest/blob/master/CHANGELOG.md"
+Documentation = "https://github.com/pylint-dev/pylint-pytest#readme"
+Homepage = "https://github.com/pylint-dev/pylint-pytest"
+Source = "https://github.com/pylint-dev/pylint-pytest"
+Tracker = "https://github.com/pylint-dev/pylint-pytest/issues"
+"Say Thanks!" = "https://saythanks.io/to/stdedos"
+
+[tool.setuptools]
+license-files = ["LICENSE"]
+
+[tool.setuptools.packages.find]
+exclude = [
+    "tests*",
+    "sandbox",
+]
+
+[tool.aliases]
+test = "pytest"
 
 [tool.black]
 line-length = 100
 
 [tool.coverage]
 run.branch = true
 run.data_file = "test_artifacts/.coverage"
@@ -32,15 +99,15 @@
     'raise UnreachableCodeException',
 ]
 paths.source = [
     "pylint_pytest/",
 ]
 
 [tool.mypy]
-python_version = "3.7"
+python_version = "3.8"
 check_untyped_defs = true
 explicit_package_bases = true
 namespace_packages = true
 show_error_codes = true
 strict_optional = true
 warn_redundant_casts = true
 warn_unreachable = true
@@ -85,16 +152,15 @@
     "UP", # pyupgrade
 ]
 
 ignore = [
     "RUF012", # Mutable class attributes should be annotated with `typing.ClassVar`
 ]
 
-# py36, but ruff does not support it :/
-target-version = "py37"
+target-version = "py38"
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.ruff.extend-per-file-ignores]
 "tests/**/test_*.py" = [
     "S101", # pytest works with `assert`s
@@ -109,15 +175,15 @@
     # The below are debateable
     "S311", # Standard pseudo-random generators are not suitable for cryptographic purposes
     "PLR2004", # Magic value used in comparison
 ]
 
 [tool.pylint]
 
-py-version = "3.6"
+py-version = "3.8"
 
 ignore-paths="tests/input" # Ignore test inputs
 
 load-plugins= [
     "pylint_pytest",
     "pylint.extensions.bad_builtin",
     "pylint.extensions.broad_try_clause",
```

