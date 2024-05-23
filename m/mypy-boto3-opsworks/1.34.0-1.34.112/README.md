# Comparing `tmp/mypy-boto3-opsworks-1.34.0.tar.gz` & `tmp/mypy_boto3_opsworks-1.34.112.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-opsworks-1.34.0.tar", last modified: Wed Dec 13 21:23:25 2023, max compression
+gzip compressed data, was "mypy_boto3_opsworks-1.34.112.tar", last modified: Thu May 23 19:32:39 2024, max compression
```

## Comparing `mypy-boto3-opsworks-1.34.0.tar` & `mypy_boto3_opsworks-1.34.112.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:25.191308 mypy-boto3-opsworks-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:14:58.000000 mypy-boto3-opsworks-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15835 2023-12-13 21:23:25.191308 mypy-boto3-opsworks-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14298 2023-12-13 21:14:58.000000 mypy-boto3-opsworks-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:25.187308 mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks/
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2023-12-13 21:14:58.000000 mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2023-12-13 21:14:58.000000 mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      909 2023-12-13 21:14:58.000000 mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51773 2023-12-13 21:14:58.000000 mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    51769 2023-12-13 21:14:58.000000 mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12988 2023-12-13 21:14:58.000000 mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    12986 2023-12-13 21:14:58.000000 mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2023-12-13 21:14:58.000000 mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2023-12-13 21:14:58.000000 mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:14:58.000000 mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    19476 2023-12-13 21:14:58.000000 mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    19465 2023-12-13 21:14:58.000000 mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    60119 2023-12-13 21:15:01.000000 mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    60118 2023-12-13 21:15:01.000000 mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:14:58.000000 mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6634 2023-12-13 21:14:58.000000 mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6628 2023-12-13 21:14:58.000000 mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:23:25.191308 mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15835 2023-12-13 21:23:25.000000 mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      841 2023-12-13 21:23:25.000000 mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:25.000000 mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:23:25.000000 mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:23:25.000000 mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-12-13 21:23:25.000000 mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:23:25.191308 mypy-boto3-opsworks-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2023-12-13 21:14:57.000000 mypy-boto3-opsworks-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:32:39.268768 mypy_boto3_opsworks-1.34.112/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-23 19:32:26.000000 mypy_boto3_opsworks-1.34.112/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15861 2024-05-23 19:32:39.268768 mypy_boto3_opsworks-1.34.112/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14300 2024-05-23 19:32:26.000000 mypy_boto3_opsworks-1.34.112/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:32:39.268768 mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-23 19:32:26.000000 mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-23 19:32:26.000000 mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-23 19:32:26.000000 mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51819 2024-05-23 19:32:26.000000 mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51816 2024-05-23 19:32:26.000000 mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13187 2024-05-23 19:32:27.000000 mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13187 2024-05-23 19:32:27.000000 mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-23 19:32:27.000000 mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-23 19:32:27.000000 mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:32:26.000000 mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    19588 2024-05-23 19:32:27.000000 mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19578 2024-05-23 19:32:27.000000 mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    62747 2024-05-23 19:32:28.000000 mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62747 2024-05-23 19:32:28.000000 mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-23 19:32:26.000000 mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-05-23 19:32:27.000000 mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-05-23 19:32:27.000000 mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:32:39.268768 mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15861 2024-05-23 19:32:39.000000 mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-23 19:32:39.000000 mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 19:32:39.000000 mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 19:32:39.000000 mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-23 19:32:39.000000 mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-23 19:32:39.000000 mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 19:32:39.268768 mypy_boto3_opsworks-1.34.112/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-23 19:32:26.000000 mypy_boto3_opsworks-1.34.112/setup.py
```

### Comparing `mypy-boto3-opsworks-1.34.0/LICENSE` & `mypy_boto3_opsworks-1.34.112/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2024 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-opsworks-1.34.0/PKG-INFO` & `mypy_boto3_opsworks-1.34.112/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opsworks
-Version: 1.34.0
-Summary: Type annotations for boto3.OpsWorks 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.112
+Summary: Type annotations for boto3.OpsWorks 1.34.112 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-opsworks"></a>
 
 # mypy-boto3-opsworks
 
 [![PyPI - mypy-boto3-opsworks](https://img.shields.io/pypi/v/mypy-boto3-opsworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opsworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opsworks)](https://pepy.tech/project/mypy-boto3-opsworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpsWorks 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
+[boto3.OpsWorks 1.34.112](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-opsworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-opsworks-1.34.0/README.md` & `mypy_boto3_opsworks-1.34.112/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opsworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opsworks)](https://pepy.tech/project/mypy-boto3-opsworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpsWorks 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
+[boto3.OpsWorks 1.34.112](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-opsworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks/__init__.py` & `mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,18 +45,16 @@
     InstanceRegisteredWaiter,
     InstanceStoppedWaiter,
     InstanceTerminatedWaiter,
 )
 
 Client = OpsWorksClient
 
-
 ServiceResource = OpsWorksServiceResource
 
-
 __all__ = (
     "AppExistsWaiter",
     "Client",
     "DeploymentSuccessfulWaiter",
     "DescribeEcsClustersPaginator",
     "InstanceOnlineWaiter",
     "InstanceRegisteredWaiter",
```

### Comparing `mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks/__init__.pyi` & `mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks/__main__.py` & `mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.OpsWorks 1.34.0\nVersion:         1.34.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.OpsWorks 1.34.112\n"
+        "Version:         1.34.112\n"
+        "Builder version: 7.24.0\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.0")
+    print("1.34.112")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks/client.py` & `mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,27 +26,27 @@
     AutoScalingTypeType,
     LayerAttributesKeysType,
     LayerTypeType,
     RootDeviceTypeType,
 )
 from .paginator import DescribeEcsClustersPaginator
 from .type_defs import (
-    AutoScalingThresholdsTypeDef,
+    AutoScalingThresholdsUnionTypeDef,
     BlockDeviceMappingTypeDef,
     ChefConfigurationTypeDef,
     CloneStackResultTypeDef,
-    CloudWatchLogsConfigurationTypeDef,
+    CloudWatchLogsConfigurationUnionTypeDef,
     CreateAppResultTypeDef,
     CreateDeploymentResultTypeDef,
     CreateInstanceResultTypeDef,
     CreateLayerResultTypeDef,
     CreateStackResultTypeDef,
     CreateUserProfileResultTypeDef,
     DataSourceTypeDef,
-    DeploymentCommandTypeDef,
+    DeploymentCommandUnionTypeDef,
     DescribeAgentVersionsResultTypeDef,
     DescribeAppsResultTypeDef,
     DescribeCommandsResultTypeDef,
     DescribeDeploymentsResultTypeDef,
     DescribeEcsClustersResultTypeDef,
     DescribeElasticIpsResultTypeDef,
     DescribeElasticLoadBalancersResultTypeDef,
@@ -68,24 +68,24 @@
     EmptyResponseMetadataTypeDef,
     EnvironmentVariableTypeDef,
     GetHostnameSuggestionResultTypeDef,
     GrantAccessResultTypeDef,
     InstanceIdentityTypeDef,
     LifecycleEventConfigurationTypeDef,
     ListTagsResultTypeDef,
-    RecipesTypeDef,
+    RecipesUnionTypeDef,
     RegisterEcsClusterResultTypeDef,
     RegisterElasticIpResultTypeDef,
     RegisterInstanceResultTypeDef,
     RegisterVolumeResultTypeDef,
     SourceTypeDef,
     SslConfigurationTypeDef,
     StackConfigurationManagerTypeDef,
     VolumeConfigurationTypeDef,
-    WeeklyAutoScalingScheduleTypeDef,
+    WeeklyAutoScalingScheduleUnionTypeDef,
 )
 from .waiter import (
     AppExistsWaiter,
     DeploymentSuccessfulWaiter,
     InstanceOnlineWaiter,
     InstanceRegisteredWaiter,
     InstanceStoppedWaiter,
@@ -93,15 +93,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("OpsWorksClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -202,15 +201,15 @@
         UseCustomCookbooks: bool = ...,
         UseOpsworksSecurityGroups: bool = ...,
         CustomCookbooksSource: SourceTypeDef = ...,
         DefaultSshKeyName: str = ...,
         ClonePermissions: bool = ...,
         CloneAppIds: Sequence[str] = ...,
         DefaultRootDeviceType: RootDeviceTypeType = ...,
-        AgentVersion: str = ...
+        AgentVersion: str = ...,
     ) -> CloneStackResultTypeDef:
         """
         Creates a clone of a specified stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.clone_stack)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#clone_stack)
         """
@@ -233,33 +232,33 @@
         Description: str = ...,
         DataSources: Sequence[DataSourceTypeDef] = ...,
         AppSource: SourceTypeDef = ...,
         Domains: Sequence[str] = ...,
         EnableSsl: bool = ...,
         SslConfiguration: SslConfigurationTypeDef = ...,
         Attributes: Mapping[AppAttributesKeysType, str] = ...,
-        Environment: Sequence[EnvironmentVariableTypeDef] = ...
+        Environment: Sequence[EnvironmentVariableTypeDef] = ...,
     ) -> CreateAppResultTypeDef:
         """
         Creates an app for a specified stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.create_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#create_app)
         """
 
     def create_deployment(
         self,
         *,
         StackId: str,
-        Command: DeploymentCommandTypeDef,
+        Command: DeploymentCommandUnionTypeDef,
         AppId: str = ...,
         InstanceIds: Sequence[str] = ...,
         LayerIds: Sequence[str] = ...,
         Comment: str = ...,
-        CustomJson: str = ...
+        CustomJson: str = ...,
     ) -> CreateDeploymentResultTypeDef:
         """
         Runs deployment or stack commands.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.create_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#create_deployment)
         """
@@ -280,15 +279,15 @@
         SubnetId: str = ...,
         Architecture: ArchitectureType = ...,
         RootDeviceType: RootDeviceTypeType = ...,
         BlockDeviceMappings: Sequence[BlockDeviceMappingTypeDef] = ...,
         InstallUpdatesOnBoot: bool = ...,
         EbsOptimized: bool = ...,
         AgentVersion: str = ...,
-        Tenancy: str = ...
+        Tenancy: str = ...,
     ) -> CreateInstanceResultTypeDef:
         """
         Creates an instance in a specified stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.create_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#create_instance)
         """
@@ -297,27 +296,27 @@
         self,
         *,
         StackId: str,
         Type: LayerTypeType,
         Name: str,
         Shortname: str,
         Attributes: Mapping[LayerAttributesKeysType, str] = ...,
-        CloudWatchLogsConfiguration: CloudWatchLogsConfigurationTypeDef = ...,
+        CloudWatchLogsConfiguration: CloudWatchLogsConfigurationUnionTypeDef = ...,
         CustomInstanceProfileArn: str = ...,
         CustomJson: str = ...,
         CustomSecurityGroupIds: Sequence[str] = ...,
         Packages: Sequence[str] = ...,
         VolumeConfigurations: Sequence[VolumeConfigurationTypeDef] = ...,
         EnableAutoHealing: bool = ...,
         AutoAssignElasticIps: bool = ...,
         AutoAssignPublicIps: bool = ...,
-        CustomRecipes: RecipesTypeDef = ...,
+        CustomRecipes: RecipesUnionTypeDef = ...,
         InstallUpdatesOnBoot: bool = ...,
         UseEbsOptimizedInstances: bool = ...,
-        LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...
+        LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...,
     ) -> CreateLayerResultTypeDef:
         """
         Creates a layer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.create_layer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#create_layer)
         """
@@ -339,30 +338,30 @@
         ConfigurationManager: StackConfigurationManagerTypeDef = ...,
         ChefConfiguration: ChefConfigurationTypeDef = ...,
         UseCustomCookbooks: bool = ...,
         UseOpsworksSecurityGroups: bool = ...,
         CustomCookbooksSource: SourceTypeDef = ...,
         DefaultSshKeyName: str = ...,
         DefaultRootDeviceType: RootDeviceTypeType = ...,
-        AgentVersion: str = ...
+        AgentVersion: str = ...,
     ) -> CreateStackResultTypeDef:
         """
         Creates a new stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.create_stack)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#create_stack)
         """
 
     def create_user_profile(
         self,
         *,
         IamUserArn: str,
         SshUsername: str = ...,
         SshPublicKey: str = ...,
-        AllowSelfManagement: bool = ...
+        AllowSelfManagement: bool = ...,
     ) -> CreateUserProfileResultTypeDef:
         """
         Creates a new user profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.create_user_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#create_user_profile)
         """
@@ -424,15 +423,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.deregister_elastic_ip)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#deregister_elastic_ip)
         """
 
     def deregister_instance(self, *, InstanceId: str) -> EmptyResponseMetadataTypeDef:
         """
-        Deregister a registered Amazon EC2 or on-premises instance.
+        Deregister an instance from OpsWorks Stacks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.deregister_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#deregister_instance)
         """
 
     def deregister_rds_db_instance(self, *, RdsDbInstanceArn: str) -> EmptyResponseMetadataTypeDef:
         """
@@ -450,15 +449,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#deregister_volume)
         """
 
     def describe_agent_versions(
         self, *, StackId: str = ..., ConfigurationManager: StackConfigurationManagerTypeDef = ...
     ) -> DescribeAgentVersionsResultTypeDef:
         """
-        Describes the available AWS OpsWorks Stacks agent versions.
+        Describes the available OpsWorks Stacks agent versions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.describe_agent_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#describe_agent_versions)
         """
 
     def describe_apps(
         self, *, StackId: str = ..., AppIds: Sequence[str] = ...
@@ -492,15 +491,15 @@
 
     def describe_ecs_clusters(
         self,
         *,
         EcsClusterArns: Sequence[str] = ...,
         StackId: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeEcsClustersResultTypeDef:
         """
         Describes Amazon ECS clusters that are registered with a stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.describe_ecs_clusters)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#describe_ecs_clusters)
         """
@@ -562,15 +561,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.describe_my_user_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#describe_my_user_profile)
         """
 
     def describe_operating_systems(self) -> DescribeOperatingSystemsResponseTypeDef:
         """
-        Describes the operating systems that are supported by AWS OpsWorks Stacks.
+        Describes the operating systems that are supported by OpsWorks Stacks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.describe_operating_systems)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#describe_operating_systems)
         """
 
     def describe_permissions(
         self, *, IamUserArn: str = ..., StackId: str = ...
@@ -602,15 +601,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#describe_rds_db_instances)
         """
 
     def describe_service_errors(
         self, *, StackId: str = ..., InstanceId: str = ..., ServiceErrorIds: Sequence[str] = ...
     ) -> DescribeServiceErrorsResultTypeDef:
         """
-        Describes AWS OpsWorks Stacks service errors.
+        Describes OpsWorks Stacks service errors.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.describe_service_errors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#describe_service_errors)
         """
 
     def describe_stack_provisioning_parameters(
         self, *, StackId: str
@@ -662,15 +661,15 @@
 
     def describe_volumes(
         self,
         *,
         InstanceId: str = ...,
         StackId: str = ...,
         RaidArrayId: str = ...,
-        VolumeIds: Sequence[str] = ...
+        VolumeIds: Sequence[str] = ...,
     ) -> DescribeVolumesResultTypeDef:
         """
         Describes an instance's Amazon EBS volumes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.describe_volumes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#describe_volumes)
         """
@@ -770,18 +769,18 @@
         *,
         StackId: str,
         Hostname: str = ...,
         PublicIp: str = ...,
         PrivateIp: str = ...,
         RsaPublicKey: str = ...,
         RsaPublicKeyFingerprint: str = ...,
-        InstanceIdentity: InstanceIdentityTypeDef = ...
+        InstanceIdentity: InstanceIdentityTypeDef = ...,
     ) -> RegisterInstanceResultTypeDef:
         """
-        Registers instances that were created outside of AWS OpsWorks Stacks with a
+        Registers instances that were created outside of OpsWorks Stacks with a
         specified
         stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.register_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#register_instance)
         """
 
@@ -806,16 +805,16 @@
         """
 
     def set_load_based_auto_scaling(
         self,
         *,
         LayerId: str,
         Enable: bool = ...,
-        UpScaling: AutoScalingThresholdsTypeDef = ...,
-        DownScaling: AutoScalingThresholdsTypeDef = ...
+        UpScaling: AutoScalingThresholdsUnionTypeDef = ...,
+        DownScaling: AutoScalingThresholdsUnionTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Specify the load-based auto scaling configuration for a specified layer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.set_load_based_auto_scaling)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#set_load_based_auto_scaling)
         """
@@ -823,25 +822,25 @@
     def set_permission(
         self,
         *,
         StackId: str,
         IamUserArn: str,
         AllowSsh: bool = ...,
         AllowSudo: bool = ...,
-        Level: str = ...
+        Level: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Specifies a user's permissions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.set_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#set_permission)
         """
 
     def set_time_based_auto_scaling(
-        self, *, InstanceId: str, AutoScalingSchedule: WeeklyAutoScalingScheduleTypeDef = ...
+        self, *, InstanceId: str, AutoScalingSchedule: WeeklyAutoScalingScheduleUnionTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Specify the time-based auto scaling configuration for a specified instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.set_time_based_auto_scaling)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#set_time_based_auto_scaling)
         """
@@ -878,15 +877,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#stop_stack)
         """
 
     def tag_resource(
         self, *, ResourceArn: str, Tags: Mapping[str, str]
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Apply cost-allocation tags to a specified stack or layer in AWS OpsWorks Stacks.
+        Apply cost-allocation tags to a specified stack or layer in OpsWorks Stacks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#tag_resource)
         """
 
     def unassign_instance(self, *, InstanceId: str) -> EmptyResponseMetadataTypeDef:
         """
@@ -923,15 +922,15 @@
         DataSources: Sequence[DataSourceTypeDef] = ...,
         Type: AppTypeType = ...,
         AppSource: SourceTypeDef = ...,
         Domains: Sequence[str] = ...,
         EnableSsl: bool = ...,
         SslConfiguration: SslConfigurationTypeDef = ...,
         Attributes: Mapping[AppAttributesKeysType, str] = ...,
-        Environment: Sequence[EnvironmentVariableTypeDef] = ...
+        Environment: Sequence[EnvironmentVariableTypeDef] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a specified app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.update_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#update_app)
         """
@@ -954,15 +953,15 @@
         Hostname: str = ...,
         Os: str = ...,
         AmiId: str = ...,
         SshKeyName: str = ...,
         Architecture: ArchitectureType = ...,
         InstallUpdatesOnBoot: bool = ...,
         EbsOptimized: bool = ...,
-        AgentVersion: str = ...
+        AgentVersion: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a specified instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.update_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#update_instance)
         """
@@ -970,27 +969,27 @@
     def update_layer(
         self,
         *,
         LayerId: str,
         Name: str = ...,
         Shortname: str = ...,
         Attributes: Mapping[LayerAttributesKeysType, str] = ...,
-        CloudWatchLogsConfiguration: CloudWatchLogsConfigurationTypeDef = ...,
+        CloudWatchLogsConfiguration: CloudWatchLogsConfigurationUnionTypeDef = ...,
         CustomInstanceProfileArn: str = ...,
         CustomJson: str = ...,
         CustomSecurityGroupIds: Sequence[str] = ...,
         Packages: Sequence[str] = ...,
         VolumeConfigurations: Sequence[VolumeConfigurationTypeDef] = ...,
         EnableAutoHealing: bool = ...,
         AutoAssignElasticIps: bool = ...,
         AutoAssignPublicIps: bool = ...,
-        CustomRecipes: RecipesTypeDef = ...,
+        CustomRecipes: RecipesUnionTypeDef = ...,
         InstallUpdatesOnBoot: bool = ...,
         UseEbsOptimizedInstances: bool = ...,
-        LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...
+        LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a specified layer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.update_layer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#update_layer)
         """
@@ -1029,30 +1028,30 @@
         ConfigurationManager: StackConfigurationManagerTypeDef = ...,
         ChefConfiguration: ChefConfigurationTypeDef = ...,
         UseCustomCookbooks: bool = ...,
         CustomCookbooksSource: SourceTypeDef = ...,
         DefaultSshKeyName: str = ...,
         DefaultRootDeviceType: RootDeviceTypeType = ...,
         UseOpsworksSecurityGroups: bool = ...,
-        AgentVersion: str = ...
+        AgentVersion: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a specified stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.update_stack)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#update_stack)
         """
 
     def update_user_profile(
         self,
         *,
         IamUserArn: str,
         SshUsername: str = ...,
         SshPublicKey: str = ...,
-        AllowSelfManagement: bool = ...
+        AllowSelfManagement: bool = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a specified user profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.update_user_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#update_user_profile)
         """
```

### Comparing `mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks/client.pyi` & `mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -26,27 +26,27 @@
     AutoScalingTypeType,
     LayerAttributesKeysType,
     LayerTypeType,
     RootDeviceTypeType,
 )
 from .paginator import DescribeEcsClustersPaginator
 from .type_defs import (
-    AutoScalingThresholdsTypeDef,
+    AutoScalingThresholdsUnionTypeDef,
     BlockDeviceMappingTypeDef,
     ChefConfigurationTypeDef,
     CloneStackResultTypeDef,
-    CloudWatchLogsConfigurationTypeDef,
+    CloudWatchLogsConfigurationUnionTypeDef,
     CreateAppResultTypeDef,
     CreateDeploymentResultTypeDef,
     CreateInstanceResultTypeDef,
     CreateLayerResultTypeDef,
     CreateStackResultTypeDef,
     CreateUserProfileResultTypeDef,
     DataSourceTypeDef,
-    DeploymentCommandTypeDef,
+    DeploymentCommandUnionTypeDef,
     DescribeAgentVersionsResultTypeDef,
     DescribeAppsResultTypeDef,
     DescribeCommandsResultTypeDef,
     DescribeDeploymentsResultTypeDef,
     DescribeEcsClustersResultTypeDef,
     DescribeElasticIpsResultTypeDef,
     DescribeElasticLoadBalancersResultTypeDef,
@@ -68,24 +68,24 @@
     EmptyResponseMetadataTypeDef,
     EnvironmentVariableTypeDef,
     GetHostnameSuggestionResultTypeDef,
     GrantAccessResultTypeDef,
     InstanceIdentityTypeDef,
     LifecycleEventConfigurationTypeDef,
     ListTagsResultTypeDef,
-    RecipesTypeDef,
+    RecipesUnionTypeDef,
     RegisterEcsClusterResultTypeDef,
     RegisterElasticIpResultTypeDef,
     RegisterInstanceResultTypeDef,
     RegisterVolumeResultTypeDef,
     SourceTypeDef,
     SslConfigurationTypeDef,
     StackConfigurationManagerTypeDef,
     VolumeConfigurationTypeDef,
-    WeeklyAutoScalingScheduleTypeDef,
+    WeeklyAutoScalingScheduleUnionTypeDef,
 )
 from .waiter import (
     AppExistsWaiter,
     DeploymentSuccessfulWaiter,
     InstanceOnlineWaiter,
     InstanceRegisteredWaiter,
     InstanceStoppedWaiter,
@@ -198,15 +198,15 @@
         UseCustomCookbooks: bool = ...,
         UseOpsworksSecurityGroups: bool = ...,
         CustomCookbooksSource: SourceTypeDef = ...,
         DefaultSshKeyName: str = ...,
         ClonePermissions: bool = ...,
         CloneAppIds: Sequence[str] = ...,
         DefaultRootDeviceType: RootDeviceTypeType = ...,
-        AgentVersion: str = ...
+        AgentVersion: str = ...,
     ) -> CloneStackResultTypeDef:
         """
         Creates a clone of a specified stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.clone_stack)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#clone_stack)
         """
@@ -229,33 +229,33 @@
         Description: str = ...,
         DataSources: Sequence[DataSourceTypeDef] = ...,
         AppSource: SourceTypeDef = ...,
         Domains: Sequence[str] = ...,
         EnableSsl: bool = ...,
         SslConfiguration: SslConfigurationTypeDef = ...,
         Attributes: Mapping[AppAttributesKeysType, str] = ...,
-        Environment: Sequence[EnvironmentVariableTypeDef] = ...
+        Environment: Sequence[EnvironmentVariableTypeDef] = ...,
     ) -> CreateAppResultTypeDef:
         """
         Creates an app for a specified stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.create_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#create_app)
         """
 
     def create_deployment(
         self,
         *,
         StackId: str,
-        Command: DeploymentCommandTypeDef,
+        Command: DeploymentCommandUnionTypeDef,
         AppId: str = ...,
         InstanceIds: Sequence[str] = ...,
         LayerIds: Sequence[str] = ...,
         Comment: str = ...,
-        CustomJson: str = ...
+        CustomJson: str = ...,
     ) -> CreateDeploymentResultTypeDef:
         """
         Runs deployment or stack commands.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.create_deployment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#create_deployment)
         """
@@ -276,15 +276,15 @@
         SubnetId: str = ...,
         Architecture: ArchitectureType = ...,
         RootDeviceType: RootDeviceTypeType = ...,
         BlockDeviceMappings: Sequence[BlockDeviceMappingTypeDef] = ...,
         InstallUpdatesOnBoot: bool = ...,
         EbsOptimized: bool = ...,
         AgentVersion: str = ...,
-        Tenancy: str = ...
+        Tenancy: str = ...,
     ) -> CreateInstanceResultTypeDef:
         """
         Creates an instance in a specified stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.create_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#create_instance)
         """
@@ -293,27 +293,27 @@
         self,
         *,
         StackId: str,
         Type: LayerTypeType,
         Name: str,
         Shortname: str,
         Attributes: Mapping[LayerAttributesKeysType, str] = ...,
-        CloudWatchLogsConfiguration: CloudWatchLogsConfigurationTypeDef = ...,
+        CloudWatchLogsConfiguration: CloudWatchLogsConfigurationUnionTypeDef = ...,
         CustomInstanceProfileArn: str = ...,
         CustomJson: str = ...,
         CustomSecurityGroupIds: Sequence[str] = ...,
         Packages: Sequence[str] = ...,
         VolumeConfigurations: Sequence[VolumeConfigurationTypeDef] = ...,
         EnableAutoHealing: bool = ...,
         AutoAssignElasticIps: bool = ...,
         AutoAssignPublicIps: bool = ...,
-        CustomRecipes: RecipesTypeDef = ...,
+        CustomRecipes: RecipesUnionTypeDef = ...,
         InstallUpdatesOnBoot: bool = ...,
         UseEbsOptimizedInstances: bool = ...,
-        LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...
+        LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...,
     ) -> CreateLayerResultTypeDef:
         """
         Creates a layer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.create_layer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#create_layer)
         """
@@ -335,30 +335,30 @@
         ConfigurationManager: StackConfigurationManagerTypeDef = ...,
         ChefConfiguration: ChefConfigurationTypeDef = ...,
         UseCustomCookbooks: bool = ...,
         UseOpsworksSecurityGroups: bool = ...,
         CustomCookbooksSource: SourceTypeDef = ...,
         DefaultSshKeyName: str = ...,
         DefaultRootDeviceType: RootDeviceTypeType = ...,
-        AgentVersion: str = ...
+        AgentVersion: str = ...,
     ) -> CreateStackResultTypeDef:
         """
         Creates a new stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.create_stack)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#create_stack)
         """
 
     def create_user_profile(
         self,
         *,
         IamUserArn: str,
         SshUsername: str = ...,
         SshPublicKey: str = ...,
-        AllowSelfManagement: bool = ...
+        AllowSelfManagement: bool = ...,
     ) -> CreateUserProfileResultTypeDef:
         """
         Creates a new user profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.create_user_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#create_user_profile)
         """
@@ -420,15 +420,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.deregister_elastic_ip)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#deregister_elastic_ip)
         """
 
     def deregister_instance(self, *, InstanceId: str) -> EmptyResponseMetadataTypeDef:
         """
-        Deregister a registered Amazon EC2 or on-premises instance.
+        Deregister an instance from OpsWorks Stacks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.deregister_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#deregister_instance)
         """
 
     def deregister_rds_db_instance(self, *, RdsDbInstanceArn: str) -> EmptyResponseMetadataTypeDef:
         """
@@ -446,15 +446,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#deregister_volume)
         """
 
     def describe_agent_versions(
         self, *, StackId: str = ..., ConfigurationManager: StackConfigurationManagerTypeDef = ...
     ) -> DescribeAgentVersionsResultTypeDef:
         """
-        Describes the available AWS OpsWorks Stacks agent versions.
+        Describes the available OpsWorks Stacks agent versions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.describe_agent_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#describe_agent_versions)
         """
 
     def describe_apps(
         self, *, StackId: str = ..., AppIds: Sequence[str] = ...
@@ -488,15 +488,15 @@
 
     def describe_ecs_clusters(
         self,
         *,
         EcsClusterArns: Sequence[str] = ...,
         StackId: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeEcsClustersResultTypeDef:
         """
         Describes Amazon ECS clusters that are registered with a stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.describe_ecs_clusters)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#describe_ecs_clusters)
         """
@@ -558,15 +558,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.describe_my_user_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#describe_my_user_profile)
         """
 
     def describe_operating_systems(self) -> DescribeOperatingSystemsResponseTypeDef:
         """
-        Describes the operating systems that are supported by AWS OpsWorks Stacks.
+        Describes the operating systems that are supported by OpsWorks Stacks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.describe_operating_systems)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#describe_operating_systems)
         """
 
     def describe_permissions(
         self, *, IamUserArn: str = ..., StackId: str = ...
@@ -598,15 +598,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#describe_rds_db_instances)
         """
 
     def describe_service_errors(
         self, *, StackId: str = ..., InstanceId: str = ..., ServiceErrorIds: Sequence[str] = ...
     ) -> DescribeServiceErrorsResultTypeDef:
         """
-        Describes AWS OpsWorks Stacks service errors.
+        Describes OpsWorks Stacks service errors.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.describe_service_errors)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#describe_service_errors)
         """
 
     def describe_stack_provisioning_parameters(
         self, *, StackId: str
@@ -658,15 +658,15 @@
 
     def describe_volumes(
         self,
         *,
         InstanceId: str = ...,
         StackId: str = ...,
         RaidArrayId: str = ...,
-        VolumeIds: Sequence[str] = ...
+        VolumeIds: Sequence[str] = ...,
     ) -> DescribeVolumesResultTypeDef:
         """
         Describes an instance's Amazon EBS volumes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.describe_volumes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#describe_volumes)
         """
@@ -766,18 +766,18 @@
         *,
         StackId: str,
         Hostname: str = ...,
         PublicIp: str = ...,
         PrivateIp: str = ...,
         RsaPublicKey: str = ...,
         RsaPublicKeyFingerprint: str = ...,
-        InstanceIdentity: InstanceIdentityTypeDef = ...
+        InstanceIdentity: InstanceIdentityTypeDef = ...,
     ) -> RegisterInstanceResultTypeDef:
         """
-        Registers instances that were created outside of AWS OpsWorks Stacks with a
+        Registers instances that were created outside of OpsWorks Stacks with a
         specified
         stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.register_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#register_instance)
         """
 
@@ -802,16 +802,16 @@
         """
 
     def set_load_based_auto_scaling(
         self,
         *,
         LayerId: str,
         Enable: bool = ...,
-        UpScaling: AutoScalingThresholdsTypeDef = ...,
-        DownScaling: AutoScalingThresholdsTypeDef = ...
+        UpScaling: AutoScalingThresholdsUnionTypeDef = ...,
+        DownScaling: AutoScalingThresholdsUnionTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Specify the load-based auto scaling configuration for a specified layer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.set_load_based_auto_scaling)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#set_load_based_auto_scaling)
         """
@@ -819,25 +819,25 @@
     def set_permission(
         self,
         *,
         StackId: str,
         IamUserArn: str,
         AllowSsh: bool = ...,
         AllowSudo: bool = ...,
-        Level: str = ...
+        Level: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Specifies a user's permissions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.set_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#set_permission)
         """
 
     def set_time_based_auto_scaling(
-        self, *, InstanceId: str, AutoScalingSchedule: WeeklyAutoScalingScheduleTypeDef = ...
+        self, *, InstanceId: str, AutoScalingSchedule: WeeklyAutoScalingScheduleUnionTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Specify the time-based auto scaling configuration for a specified instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.set_time_based_auto_scaling)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#set_time_based_auto_scaling)
         """
@@ -874,15 +874,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#stop_stack)
         """
 
     def tag_resource(
         self, *, ResourceArn: str, Tags: Mapping[str, str]
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Apply cost-allocation tags to a specified stack or layer in AWS OpsWorks Stacks.
+        Apply cost-allocation tags to a specified stack or layer in OpsWorks Stacks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#tag_resource)
         """
 
     def unassign_instance(self, *, InstanceId: str) -> EmptyResponseMetadataTypeDef:
         """
@@ -919,15 +919,15 @@
         DataSources: Sequence[DataSourceTypeDef] = ...,
         Type: AppTypeType = ...,
         AppSource: SourceTypeDef = ...,
         Domains: Sequence[str] = ...,
         EnableSsl: bool = ...,
         SslConfiguration: SslConfigurationTypeDef = ...,
         Attributes: Mapping[AppAttributesKeysType, str] = ...,
-        Environment: Sequence[EnvironmentVariableTypeDef] = ...
+        Environment: Sequence[EnvironmentVariableTypeDef] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a specified app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.update_app)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#update_app)
         """
@@ -950,15 +950,15 @@
         Hostname: str = ...,
         Os: str = ...,
         AmiId: str = ...,
         SshKeyName: str = ...,
         Architecture: ArchitectureType = ...,
         InstallUpdatesOnBoot: bool = ...,
         EbsOptimized: bool = ...,
-        AgentVersion: str = ...
+        AgentVersion: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a specified instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.update_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#update_instance)
         """
@@ -966,27 +966,27 @@
     def update_layer(
         self,
         *,
         LayerId: str,
         Name: str = ...,
         Shortname: str = ...,
         Attributes: Mapping[LayerAttributesKeysType, str] = ...,
-        CloudWatchLogsConfiguration: CloudWatchLogsConfigurationTypeDef = ...,
+        CloudWatchLogsConfiguration: CloudWatchLogsConfigurationUnionTypeDef = ...,
         CustomInstanceProfileArn: str = ...,
         CustomJson: str = ...,
         CustomSecurityGroupIds: Sequence[str] = ...,
         Packages: Sequence[str] = ...,
         VolumeConfigurations: Sequence[VolumeConfigurationTypeDef] = ...,
         EnableAutoHealing: bool = ...,
         AutoAssignElasticIps: bool = ...,
         AutoAssignPublicIps: bool = ...,
-        CustomRecipes: RecipesTypeDef = ...,
+        CustomRecipes: RecipesUnionTypeDef = ...,
         InstallUpdatesOnBoot: bool = ...,
         UseEbsOptimizedInstances: bool = ...,
-        LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...
+        LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a specified layer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.update_layer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#update_layer)
         """
@@ -1025,30 +1025,30 @@
         ConfigurationManager: StackConfigurationManagerTypeDef = ...,
         ChefConfiguration: ChefConfigurationTypeDef = ...,
         UseCustomCookbooks: bool = ...,
         CustomCookbooksSource: SourceTypeDef = ...,
         DefaultSshKeyName: str = ...,
         DefaultRootDeviceType: RootDeviceTypeType = ...,
         UseOpsworksSecurityGroups: bool = ...,
-        AgentVersion: str = ...
+        AgentVersion: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a specified stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.update_stack)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#update_stack)
         """
 
     def update_user_profile(
         self,
         *,
         IamUserArn: str,
         SshUsername: str = ...,
         SshPublicKey: str = ...,
-        AllowSelfManagement: bool = ...
+        AllowSelfManagement: bool = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a specified user profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.update_user_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/client/#update_user_profile)
         """
```

### Comparing `mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks/literals.py` & `mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AppAttributesKeysType",
     "AppExistsWaiterName",
     "AppTypeType",
     "ArchitectureType",
     "AutoScalingTypeType",
     "CloudWatchLogsEncodingType",
@@ -47,15 +46,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AppAttributesKeysType = Literal[
     "AutoBundleOnDeploy", "AwsFlowRubySettings", "DocumentRoot", "RailsEnv"
 ]
 AppExistsWaiterName = Literal["app_exists"]
 AppTypeType = Literal["aws-flow-ruby", "java", "nodejs", "other", "php", "rails", "static"]
 ArchitectureType = Literal["i386", "x86_64"]
 AutoScalingTypeType = Literal["load", "timer"]
@@ -244,14 +242,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -262,14 +261,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -287,14 +287,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -307,24 +308,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -385,15 +388,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -435,14 +437,15 @@
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie2",
+    "mailmanager",
     "managedblockchain",
     "managedblockchain-query",
     "marketplace-agreement",
     "marketplace-catalog",
     "marketplace-deployment",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
@@ -465,17 +468,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -520,14 +525,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -565,19 +571,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks/literals.pyi` & `mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -242,14 +242,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -260,14 +261,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -285,14 +287,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -305,24 +308,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -383,15 +388,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -433,14 +437,15 @@
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie2",
+    "mailmanager",
     "managedblockchain",
     "managedblockchain-query",
     "marketplace-agreement",
     "marketplace-catalog",
     "marketplace-deployment",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
@@ -463,17 +468,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -518,14 +525,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -563,19 +571,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks/paginator.py` & `mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import DescribeEcsClustersResultTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("DescribeEcsClustersPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -46,13 +45,13 @@
     """
 
     def paginate(
         self,
         *,
         EcsClusterArns: Sequence[str] = ...,
         StackId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeEcsClustersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Paginator.DescribeEcsClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/paginators/#describeecsclusterspaginator)
         """
```

### Comparing `mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks/paginator.pyi` & `mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -43,13 +43,13 @@
     """
 
     def paginate(
         self,
         *,
         EcsClusterArns: Sequence[str] = ...,
         StackId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeEcsClustersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Paginator.DescribeEcsClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/paginators/#describeecsclusterspaginator)
         """
```

### Comparing `mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks/service_resource.py` & `mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks/service_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "OpsWorksServiceResource",
     "Layer",
     "Stack",
     "StackSummary",
     "ServiceResourceStacksCollection",
     "StackLayersCollection",
@@ -179,14 +178,15 @@
     custom_recipes: RecipesResponseTypeDef
     created_at: str
     install_updates_on_boot: bool
     use_ebs_optimized_instances: bool
     lifecycle_event_configuration: LifecycleEventConfigurationResponseTypeDef
     id: str
     stack: "Stack"
+    meta: "OpsWorksResourceMeta"
 
     def delete(self) -> None:
         """
         Deletes a specified layer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Layer.delete)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/service_resource/#layerdelete-method)
@@ -232,14 +232,15 @@
 
     name: str
     arn: str
     layers_count: int
     apps_count: int
     instances_count: InstancesCountResponseTypeDef
     stack_id: str
+    meta: "OpsWorksResourceMeta"
 
     def Stack(self) -> "_Stack":
         """
         Creates a Stack resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.StackSummary.Stack)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/service_resource/#stacksummarystack-method)
@@ -303,16 +304,17 @@
     custom_cookbooks_source: SourceResponseTypeDef
     default_ssh_key_name: str
     created_at: str
     default_root_device_type: RootDeviceTypeType
     agent_version: str
     id: str
     layers: StackLayersCollection
+    meta: "OpsWorksResourceMeta"
 
-    def Summary(self) -> _StackSummary:
+    def Summary(self) -> "_StackSummary":
         """
         Creates a StackSummary resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Stack.Summary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/service_resource/#stacksummary-method)
         """
 
@@ -331,16 +333,16 @@
         VolumeConfigurations: Sequence[VolumeConfigurationTypeDef] = ...,
         EnableAutoHealing: bool = ...,
         AutoAssignElasticIps: bool = ...,
         AutoAssignPublicIps: bool = ...,
         CustomRecipes: RecipesTypeDef = ...,
         InstallUpdatesOnBoot: bool = ...,
         UseEbsOptimizedInstances: bool = ...,
-        LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...
-    ) -> _Layer:
+        LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...,
+    ) -> "_Layer":
         """
         Creates a layer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Stack.create_layer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/service_resource/#stackcreate_layer-method)
         """
 
@@ -393,31 +395,31 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.ServiceResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/service_resource/)
     """
 
     meta: "OpsWorksResourceMeta"
     stacks: ServiceResourceStacksCollection
 
-    def Layer(self, id: str) -> _Layer:
+    def Layer(self, id: str) -> "_Layer":
         """
         Creates a Layer resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.ServiceResource.Layer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/service_resource/#opsworksserviceresourcelayer-method)
         """
 
-    def Stack(self, id: str) -> _Stack:
+    def Stack(self, id: str) -> "_Stack":
         """
         Creates a Stack resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.ServiceResource.Stack)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/service_resource/#opsworksserviceresourcestack-method)
         """
 
-    def StackSummary(self, stack_id: str) -> _StackSummary:
+    def StackSummary(self, stack_id: str) -> "_StackSummary":
         """
         Creates a StackSummary resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.ServiceResource.StackSummary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/service_resource/#opsworksserviceresourcestacksummary-method)
         """
 
@@ -438,16 +440,16 @@
         ConfigurationManager: StackConfigurationManagerTypeDef = ...,
         ChefConfiguration: ChefConfigurationTypeDef = ...,
         UseCustomCookbooks: bool = ...,
         UseOpsworksSecurityGroups: bool = ...,
         CustomCookbooksSource: SourceTypeDef = ...,
         DefaultSshKeyName: str = ...,
         DefaultRootDeviceType: RootDeviceTypeType = ...,
-        AgentVersion: str = ...
-    ) -> _Stack:
+        AgentVersion: str = ...,
+    ) -> "_Stack":
         """
         Creates a new stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.ServiceResource.create_stack)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/service_resource/#opsworksserviceresourcecreate_stack-method)
         """
```

### Comparing `mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks/service_resource.pyi` & `mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks/service_resource.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -175,14 +175,15 @@
     custom_recipes: RecipesResponseTypeDef
     created_at: str
     install_updates_on_boot: bool
     use_ebs_optimized_instances: bool
     lifecycle_event_configuration: LifecycleEventConfigurationResponseTypeDef
     id: str
     stack: "Stack"
+    meta: "OpsWorksResourceMeta"
 
     def delete(self) -> None:
         """
         Deletes a specified layer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Layer.delete)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/service_resource/#layerdelete-method)
@@ -226,14 +227,15 @@
 
     name: str
     arn: str
     layers_count: int
     apps_count: int
     instances_count: InstancesCountResponseTypeDef
     stack_id: str
+    meta: "OpsWorksResourceMeta"
 
     def Stack(self) -> "_Stack":
         """
         Creates a Stack resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.StackSummary.Stack)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/service_resource/#stacksummarystack-method)
@@ -295,16 +297,17 @@
     custom_cookbooks_source: SourceResponseTypeDef
     default_ssh_key_name: str
     created_at: str
     default_root_device_type: RootDeviceTypeType
     agent_version: str
     id: str
     layers: StackLayersCollection
+    meta: "OpsWorksResourceMeta"
 
-    def Summary(self) -> _StackSummary:
+    def Summary(self) -> "_StackSummary":
         """
         Creates a StackSummary resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Stack.Summary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/service_resource/#stacksummary-method)
         """
 
@@ -323,16 +326,16 @@
         VolumeConfigurations: Sequence[VolumeConfigurationTypeDef] = ...,
         EnableAutoHealing: bool = ...,
         AutoAssignElasticIps: bool = ...,
         AutoAssignPublicIps: bool = ...,
         CustomRecipes: RecipesTypeDef = ...,
         InstallUpdatesOnBoot: bool = ...,
         UseEbsOptimizedInstances: bool = ...,
-        LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...
-    ) -> _Layer:
+        LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...,
+    ) -> "_Layer":
         """
         Creates a layer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Stack.create_layer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/service_resource/#stackcreate_layer-method)
         """
 
@@ -382,31 +385,31 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.ServiceResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/service_resource/)
     """
 
     meta: "OpsWorksResourceMeta"
     stacks: ServiceResourceStacksCollection
 
-    def Layer(self, id: str) -> _Layer:
+    def Layer(self, id: str) -> "_Layer":
         """
         Creates a Layer resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.ServiceResource.Layer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/service_resource/#opsworksserviceresourcelayer-method)
         """
 
-    def Stack(self, id: str) -> _Stack:
+    def Stack(self, id: str) -> "_Stack":
         """
         Creates a Stack resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.ServiceResource.Stack)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/service_resource/#opsworksserviceresourcestack-method)
         """
 
-    def StackSummary(self, stack_id: str) -> _StackSummary:
+    def StackSummary(self, stack_id: str) -> "_StackSummary":
         """
         Creates a StackSummary resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.ServiceResource.StackSummary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/service_resource/#opsworksserviceresourcestacksummary-method)
         """
 
@@ -427,16 +430,16 @@
         ConfigurationManager: StackConfigurationManagerTypeDef = ...,
         ChefConfiguration: ChefConfigurationTypeDef = ...,
         UseCustomCookbooks: bool = ...,
         UseOpsworksSecurityGroups: bool = ...,
         CustomCookbooksSource: SourceTypeDef = ...,
         DefaultSshKeyName: str = ...,
         DefaultRootDeviceType: RootDeviceTypeType = ...,
-        AgentVersion: str = ...
-    ) -> _Stack:
+        AgentVersion: str = ...,
+    ) -> "_Stack":
         """
         Creates a new stack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.ServiceResource.create_stack)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/service_resource/#opsworksserviceresourcecreate_stack-method)
         """
```

### Comparing `mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks/type_defs.py` & `mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_opsworks.type_defs import StackConfigurationManagerTypeDef
 
     data: StackConfigurationManagerTypeDef = ...
     ```
 """
 
 import sys
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AppAttributesKeysType,
     AppTypeType,
     ArchitectureType,
     AutoScalingTypeType,
     CloudWatchLogsEncodingType,
@@ -41,25 +41,25 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "StackConfigurationManagerTypeDef",
     "DataSourceTypeDef",
     "EnvironmentVariableTypeDef",
     "SourceTypeDef",
     "SslConfigurationTypeDef",
     "AssignInstanceRequestRequestTypeDef",
     "AssignVolumeRequestRequestTypeDef",
     "AssociateElasticIpRequestRequestTypeDef",
     "AttachElasticLoadBalancerRequestRequestTypeDef",
+    "AutoScalingThresholdsOutputTypeDef",
     "AutoScalingThresholdsTypeDef",
     "EbsBlockDeviceTypeDef",
     "ResponseMetadataTypeDef",
     "ChefConfigurationTypeDef",
     "CloudWatchLogsLogStreamTypeDef",
     "CommandTypeDef",
     "DeploymentCommandTypeDef",
@@ -67,14 +67,15 @@
     "VolumeConfigurationTypeDef",
     "CreateUserProfileRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteInstanceRequestRequestTypeDef",
     "DeleteLayerRequestRequestTypeDef",
     "DeleteStackRequestRequestTypeDef",
     "DeleteUserProfileRequestRequestTypeDef",
+    "DeploymentCommandOutputTypeDef",
     "DeregisterEcsClusterRequestRequestTypeDef",
     "DeregisterElasticIpRequestRequestTypeDef",
     "DeregisterInstanceRequestRequestTypeDef",
     "DeregisterRdsDbInstanceRequestRequestTypeDef",
     "DeregisterVolumeRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeAppsRequestRequestTypeDef",
@@ -111,14 +112,15 @@
     "DisassociateElasticIpRequestRequestTypeDef",
     "GetHostnameSuggestionRequestRequestTypeDef",
     "GrantAccessRequestRequestTypeDef",
     "TemporaryCredentialTypeDef",
     "InstanceIdentityTypeDef",
     "ReportedOsTypeDef",
     "InstancesCountTypeDef",
+    "RecipesOutputTypeDef",
     "ShutdownEventConfigurationTypeDef",
     "ListTagsRequestRequestTypeDef",
     "OperatingSystemConfigurationManagerTypeDef",
     "RebootInstanceRequestRequestTypeDef",
     "RegisterEcsClusterRequestRequestTypeDef",
     "RegisterElasticIpRequestRequestTypeDef",
     "RegisterRdsDbInstanceRequestRequestTypeDef",
@@ -126,14 +128,15 @@
     "SetPermissionRequestRequestTypeDef",
     "WeeklyAutoScalingScheduleTypeDef",
     "StartInstanceRequestRequestTypeDef",
     "StartStackRequestRequestTypeDef",
     "StopInstanceRequestRequestTypeDef",
     "StopStackRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "WeeklyAutoScalingScheduleOutputTypeDef",
     "UnassignInstanceRequestRequestTypeDef",
     "UnassignVolumeRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateElasticIpRequestRequestTypeDef",
     "UpdateInstanceRequestRequestTypeDef",
     "UpdateMyUserProfileRequestRequestTypeDef",
     "UpdateRdsDbInstanceRequestRequestTypeDef",
@@ -141,14 +144,15 @@
     "UpdateVolumeRequestRequestTypeDef",
     "AgentVersionTypeDef",
     "DescribeAgentVersionsRequestRequestTypeDef",
     "AppTypeDef",
     "CreateAppRequestRequestTypeDef",
     "UpdateAppRequestRequestTypeDef",
     "LoadBasedAutoScalingConfigurationTypeDef",
+    "AutoScalingThresholdsUnionTypeDef",
     "SetLoadBasedAutoScalingRequestRequestTypeDef",
     "BlockDeviceMappingTypeDef",
     "ChefConfigurationResponseTypeDef",
     "CloneStackResultTypeDef",
     "CreateAppResultTypeDef",
     "CreateDeploymentResultTypeDef",
     "CreateInstanceResultTypeDef",
@@ -168,18 +172,20 @@
     "SourceResponseTypeDef",
     "StackConfigurationManagerResponseTypeDef",
     "CloneStackRequestRequestTypeDef",
     "CreateStackRequestRequestTypeDef",
     "CreateStackRequestServiceResourceCreateStackTypeDef",
     "StackTypeDef",
     "UpdateStackRequestRequestTypeDef",
+    "CloudWatchLogsConfigurationOutputTypeDef",
     "CloudWatchLogsConfigurationResponseTypeDef",
     "CloudWatchLogsConfigurationTypeDef",
     "DescribeCommandsResultTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
+    "DeploymentCommandUnionTypeDef",
     "DeploymentTypeDef",
     "DescribeAppsRequestAppExistsWaitTypeDef",
     "DescribeDeploymentsRequestDeploymentSuccessfulWaitTypeDef",
     "DescribeInstancesRequestInstanceOnlineWaitTypeDef",
     "DescribeInstancesRequestInstanceRegisteredWaitTypeDef",
     "DescribeInstancesRequestInstanceStoppedWaitTypeDef",
     "DescribeInstancesRequestInstanceTerminatedWaitTypeDef",
@@ -193,25 +199,28 @@
     "DescribeRdsDbInstancesResultTypeDef",
     "DescribeServiceErrorsResultTypeDef",
     "DescribeUserProfilesResultTypeDef",
     "DescribeVolumesResultTypeDef",
     "GrantAccessResultTypeDef",
     "RegisterInstanceRequestRequestTypeDef",
     "StackSummaryTypeDef",
+    "RecipesUnionTypeDef",
     "LifecycleEventConfigurationResponseTypeDef",
     "LifecycleEventConfigurationTypeDef",
     "OperatingSystemTypeDef",
     "SetTimeBasedAutoScalingRequestRequestTypeDef",
     "TimeBasedAutoScalingConfigurationTypeDef",
+    "WeeklyAutoScalingScheduleUnionTypeDef",
     "DescribeAgentVersionsResultTypeDef",
     "DescribeAppsResultTypeDef",
     "DescribeLoadBasedAutoScalingResultTypeDef",
     "CreateInstanceRequestRequestTypeDef",
     "InstanceTypeDef",
     "DescribeStacksResultTypeDef",
+    "CloudWatchLogsConfigurationUnionTypeDef",
     "DescribeDeploymentsResultTypeDef",
     "DescribeStackSummaryResultTypeDef",
     "CreateLayerRequestRequestTypeDef",
     "CreateLayerRequestStackCreateLayerTypeDef",
     "LayerTypeDef",
     "UpdateLayerRequestRequestTypeDef",
     "DescribeOperatingSystemsResponseTypeDef",
@@ -286,24 +295,36 @@
 AttachElasticLoadBalancerRequestRequestTypeDef = TypedDict(
     "AttachElasticLoadBalancerRequestRequestTypeDef",
     {
         "ElasticLoadBalancerName": str,
         "LayerId": str,
     },
 )
+AutoScalingThresholdsOutputTypeDef = TypedDict(
+    "AutoScalingThresholdsOutputTypeDef",
+    {
+        "InstanceCount": NotRequired[int],
+        "ThresholdsWaitTime": NotRequired[int],
+        "IgnoreMetricsTime": NotRequired[int],
+        "CpuThreshold": NotRequired[float],
+        "MemoryThreshold": NotRequired[float],
+        "LoadThreshold": NotRequired[float],
+        "Alarms": NotRequired[List[str]],
+    },
+)
 AutoScalingThresholdsTypeDef = TypedDict(
     "AutoScalingThresholdsTypeDef",
     {
         "InstanceCount": NotRequired[int],
         "ThresholdsWaitTime": NotRequired[int],
         "IgnoreMetricsTime": NotRequired[int],
         "CpuThreshold": NotRequired[float],
         "MemoryThreshold": NotRequired[float],
         "LoadThreshold": NotRequired[float],
-        "Alarms": NotRequired[List[str]],
+        "Alarms": NotRequired[Sequence[str]],
     },
 )
 EbsBlockDeviceTypeDef = TypedDict(
     "EbsBlockDeviceTypeDef",
     {
         "SnapshotId": NotRequired[str],
         "Iops": NotRequired[int],
@@ -312,18 +333,18 @@
         "DeleteOnTermination": NotRequired[bool],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 ChefConfigurationTypeDef = TypedDict(
     "ChefConfigurationTypeDef",
     {
         "ManageBerkshelf": NotRequired[bool],
         "BerkshelfVersion": NotRequired[str],
@@ -426,14 +447,21 @@
 )
 DeleteUserProfileRequestRequestTypeDef = TypedDict(
     "DeleteUserProfileRequestRequestTypeDef",
     {
         "IamUserArn": str,
     },
 )
+DeploymentCommandOutputTypeDef = TypedDict(
+    "DeploymentCommandOutputTypeDef",
+    {
+        "Name": DeploymentCommandNameType,
+        "Args": NotRequired[Dict[str, List[str]]],
+    },
+)
 DeregisterEcsClusterRequestRequestTypeDef = TypedDict(
     "DeregisterEcsClusterRequestRequestTypeDef",
     {
         "EcsClusterArn": str,
     },
 )
 DeregisterElasticIpRequestRequestTypeDef = TypedDict(
@@ -807,14 +835,24 @@
         "Stopped": NotRequired[int],
         "Stopping": NotRequired[int],
         "Terminated": NotRequired[int],
         "Terminating": NotRequired[int],
         "Unassigning": NotRequired[int],
     },
 )
+RecipesOutputTypeDef = TypedDict(
+    "RecipesOutputTypeDef",
+    {
+        "Setup": NotRequired[List[str]],
+        "Configure": NotRequired[List[str]],
+        "Deploy": NotRequired[List[str]],
+        "Undeploy": NotRequired[List[str]],
+        "Shutdown": NotRequired[List[str]],
+    },
+)
 ShutdownEventConfigurationTypeDef = TypedDict(
     "ShutdownEventConfigurationTypeDef",
     {
         "ExecutionTimeout": NotRequired[int],
         "DelayUntilElbConnectionsDrained": NotRequired[bool],
     },
 )
@@ -878,21 +916,21 @@
         "AllowSudo": NotRequired[bool],
         "Level": NotRequired[str],
     },
 )
 WeeklyAutoScalingScheduleTypeDef = TypedDict(
     "WeeklyAutoScalingScheduleTypeDef",
     {
-        "Monday": NotRequired[Dict[str, str]],
-        "Tuesday": NotRequired[Dict[str, str]],
-        "Wednesday": NotRequired[Dict[str, str]],
-        "Thursday": NotRequired[Dict[str, str]],
-        "Friday": NotRequired[Dict[str, str]],
-        "Saturday": NotRequired[Dict[str, str]],
-        "Sunday": NotRequired[Dict[str, str]],
+        "Monday": NotRequired[Mapping[str, str]],
+        "Tuesday": NotRequired[Mapping[str, str]],
+        "Wednesday": NotRequired[Mapping[str, str]],
+        "Thursday": NotRequired[Mapping[str, str]],
+        "Friday": NotRequired[Mapping[str, str]],
+        "Saturday": NotRequired[Mapping[str, str]],
+        "Sunday": NotRequired[Mapping[str, str]],
     },
 )
 StartInstanceRequestRequestTypeDef = TypedDict(
     "StartInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
@@ -919,14 +957,26 @@
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
+WeeklyAutoScalingScheduleOutputTypeDef = TypedDict(
+    "WeeklyAutoScalingScheduleOutputTypeDef",
+    {
+        "Monday": NotRequired[Dict[str, str]],
+        "Tuesday": NotRequired[Dict[str, str]],
+        "Wednesday": NotRequired[Dict[str, str]],
+        "Thursday": NotRequired[Dict[str, str]],
+        "Friday": NotRequired[Dict[str, str]],
+        "Saturday": NotRequired[Dict[str, str]],
+        "Sunday": NotRequired[Dict[str, str]],
+    },
+)
 UnassignInstanceRequestRequestTypeDef = TypedDict(
     "UnassignInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 UnassignVolumeRequestRequestTypeDef = TypedDict(
@@ -1064,18 +1114,21 @@
     },
 )
 LoadBasedAutoScalingConfigurationTypeDef = TypedDict(
     "LoadBasedAutoScalingConfigurationTypeDef",
     {
         "LayerId": NotRequired[str],
         "Enable": NotRequired[bool],
-        "UpScaling": NotRequired[AutoScalingThresholdsTypeDef],
-        "DownScaling": NotRequired[AutoScalingThresholdsTypeDef],
+        "UpScaling": NotRequired[AutoScalingThresholdsOutputTypeDef],
+        "DownScaling": NotRequired[AutoScalingThresholdsOutputTypeDef],
     },
 )
+AutoScalingThresholdsUnionTypeDef = Union[
+    AutoScalingThresholdsTypeDef, AutoScalingThresholdsOutputTypeDef
+]
 SetLoadBasedAutoScalingRequestRequestTypeDef = TypedDict(
     "SetLoadBasedAutoScalingRequestRequestTypeDef",
     {
         "LayerId": str,
         "Enable": NotRequired[bool],
         "UpScaling": NotRequired[AutoScalingThresholdsTypeDef],
         "DownScaling": NotRequired[AutoScalingThresholdsTypeDef],
@@ -1195,16 +1248,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListTagsResultTypeDef = TypedDict(
     "ListTagsResultTypeDef",
     {
         "Tags": Dict[str, str],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 RecipesResponseTypeDef = TypedDict(
     "RecipesResponseTypeDef",
     {
         "Setup": List[str],
         "Configure": List[str],
@@ -1383,14 +1436,21 @@
         "CustomCookbooksSource": NotRequired[SourceTypeDef],
         "DefaultSshKeyName": NotRequired[str],
         "DefaultRootDeviceType": NotRequired[RootDeviceTypeType],
         "UseOpsworksSecurityGroups": NotRequired[bool],
         "AgentVersion": NotRequired[str],
     },
 )
+CloudWatchLogsConfigurationOutputTypeDef = TypedDict(
+    "CloudWatchLogsConfigurationOutputTypeDef",
+    {
+        "Enabled": NotRequired[bool],
+        "LogStreams": NotRequired[List[CloudWatchLogsLogStreamTypeDef]],
+    },
+)
 CloudWatchLogsConfigurationResponseTypeDef = TypedDict(
     "CloudWatchLogsConfigurationResponseTypeDef",
     {
         "Enabled": bool,
         "LogStreams": List[CloudWatchLogsLogStreamTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1417,26 +1477,27 @@
         "AppId": NotRequired[str],
         "InstanceIds": NotRequired[Sequence[str]],
         "LayerIds": NotRequired[Sequence[str]],
         "Comment": NotRequired[str],
         "CustomJson": NotRequired[str],
     },
 )
+DeploymentCommandUnionTypeDef = Union[DeploymentCommandTypeDef, DeploymentCommandOutputTypeDef]
 DeploymentTypeDef = TypedDict(
     "DeploymentTypeDef",
     {
         "DeploymentId": NotRequired[str],
         "StackId": NotRequired[str],
         "AppId": NotRequired[str],
         "CreatedAt": NotRequired[str],
         "CompletedAt": NotRequired[str],
         "Duration": NotRequired[int],
         "IamUserArn": NotRequired[str],
         "Comment": NotRequired[str],
-        "Command": NotRequired[DeploymentCommandTypeDef],
+        "Command": NotRequired[DeploymentCommandOutputTypeDef],
         "Status": NotRequired[str],
         "CustomJson": NotRequired[str],
         "InstanceIds": NotRequired[List[str]],
     },
 )
 DescribeAppsRequestAppExistsWaitTypeDef = TypedDict(
     "DescribeAppsRequestAppExistsWaitTypeDef",
@@ -1499,16 +1560,16 @@
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 DescribeEcsClustersResultTypeDef = TypedDict(
     "DescribeEcsClustersResultTypeDef",
     {
         "EcsClusters": List[EcsClusterTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeElasticIpsResultTypeDef = TypedDict(
     "DescribeElasticIpsResultTypeDef",
     {
         "ElasticIps": List[ElasticIpTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1596,14 +1657,15 @@
         "Name": NotRequired[str],
         "Arn": NotRequired[str],
         "LayersCount": NotRequired[int],
         "AppsCount": NotRequired[int],
         "InstancesCount": NotRequired[InstancesCountTypeDef],
     },
 )
+RecipesUnionTypeDef = Union[RecipesTypeDef, RecipesOutputTypeDef]
 LifecycleEventConfigurationResponseTypeDef = TypedDict(
     "LifecycleEventConfigurationResponseTypeDef",
     {
         "Shutdown": ShutdownEventConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1632,17 +1694,20 @@
         "AutoScalingSchedule": NotRequired[WeeklyAutoScalingScheduleTypeDef],
     },
 )
 TimeBasedAutoScalingConfigurationTypeDef = TypedDict(
     "TimeBasedAutoScalingConfigurationTypeDef",
     {
         "InstanceId": NotRequired[str],
-        "AutoScalingSchedule": NotRequired[WeeklyAutoScalingScheduleTypeDef],
+        "AutoScalingSchedule": NotRequired[WeeklyAutoScalingScheduleOutputTypeDef],
     },
 )
+WeeklyAutoScalingScheduleUnionTypeDef = Union[
+    WeeklyAutoScalingScheduleTypeDef, WeeklyAutoScalingScheduleOutputTypeDef
+]
 DescribeAgentVersionsResultTypeDef = TypedDict(
     "DescribeAgentVersionsResultTypeDef",
     {
         "AgentVersions": List[AgentVersionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1732,14 +1797,17 @@
 DescribeStacksResultTypeDef = TypedDict(
     "DescribeStacksResultTypeDef",
     {
         "Stacks": List[StackTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CloudWatchLogsConfigurationUnionTypeDef = Union[
+    CloudWatchLogsConfigurationTypeDef, CloudWatchLogsConfigurationOutputTypeDef
+]
 DescribeDeploymentsResultTypeDef = TypedDict(
     "DescribeDeploymentsResultTypeDef",
     {
         "Deployments": List[DeploymentTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1801,26 +1869,26 @@
         "Arn": NotRequired[str],
         "StackId": NotRequired[str],
         "LayerId": NotRequired[str],
         "Type": NotRequired[LayerTypeType],
         "Name": NotRequired[str],
         "Shortname": NotRequired[str],
         "Attributes": NotRequired[Dict[LayerAttributesKeysType, str]],
-        "CloudWatchLogsConfiguration": NotRequired[CloudWatchLogsConfigurationTypeDef],
+        "CloudWatchLogsConfiguration": NotRequired[CloudWatchLogsConfigurationOutputTypeDef],
         "CustomInstanceProfileArn": NotRequired[str],
         "CustomJson": NotRequired[str],
         "CustomSecurityGroupIds": NotRequired[List[str]],
         "DefaultSecurityGroupNames": NotRequired[List[str]],
         "Packages": NotRequired[List[str]],
         "VolumeConfigurations": NotRequired[List[VolumeConfigurationTypeDef]],
         "EnableAutoHealing": NotRequired[bool],
         "AutoAssignElasticIps": NotRequired[bool],
         "AutoAssignPublicIps": NotRequired[bool],
-        "DefaultRecipes": NotRequired[RecipesTypeDef],
-        "CustomRecipes": NotRequired[RecipesTypeDef],
+        "DefaultRecipes": NotRequired[RecipesOutputTypeDef],
+        "CustomRecipes": NotRequired[RecipesOutputTypeDef],
         "CreatedAt": NotRequired[str],
         "InstallUpdatesOnBoot": NotRequired[bool],
         "UseEbsOptimizedInstances": NotRequired[bool],
         "LifecycleEventConfiguration": NotRequired[LifecycleEventConfigurationTypeDef],
     },
 )
 UpdateLayerRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks/type_defs.pyi` & `mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_opsworks.type_defs import StackConfigurationManagerTypeDef
 
     data: StackConfigurationManagerTypeDef = ...
     ```
 """
 
 import sys
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AppAttributesKeysType,
     AppTypeType,
     ArchitectureType,
     AutoScalingTypeType,
     CloudWatchLogsEncodingType,
@@ -51,14 +51,15 @@
     "EnvironmentVariableTypeDef",
     "SourceTypeDef",
     "SslConfigurationTypeDef",
     "AssignInstanceRequestRequestTypeDef",
     "AssignVolumeRequestRequestTypeDef",
     "AssociateElasticIpRequestRequestTypeDef",
     "AttachElasticLoadBalancerRequestRequestTypeDef",
+    "AutoScalingThresholdsOutputTypeDef",
     "AutoScalingThresholdsTypeDef",
     "EbsBlockDeviceTypeDef",
     "ResponseMetadataTypeDef",
     "ChefConfigurationTypeDef",
     "CloudWatchLogsLogStreamTypeDef",
     "CommandTypeDef",
     "DeploymentCommandTypeDef",
@@ -66,14 +67,15 @@
     "VolumeConfigurationTypeDef",
     "CreateUserProfileRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteInstanceRequestRequestTypeDef",
     "DeleteLayerRequestRequestTypeDef",
     "DeleteStackRequestRequestTypeDef",
     "DeleteUserProfileRequestRequestTypeDef",
+    "DeploymentCommandOutputTypeDef",
     "DeregisterEcsClusterRequestRequestTypeDef",
     "DeregisterElasticIpRequestRequestTypeDef",
     "DeregisterInstanceRequestRequestTypeDef",
     "DeregisterRdsDbInstanceRequestRequestTypeDef",
     "DeregisterVolumeRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeAppsRequestRequestTypeDef",
@@ -110,14 +112,15 @@
     "DisassociateElasticIpRequestRequestTypeDef",
     "GetHostnameSuggestionRequestRequestTypeDef",
     "GrantAccessRequestRequestTypeDef",
     "TemporaryCredentialTypeDef",
     "InstanceIdentityTypeDef",
     "ReportedOsTypeDef",
     "InstancesCountTypeDef",
+    "RecipesOutputTypeDef",
     "ShutdownEventConfigurationTypeDef",
     "ListTagsRequestRequestTypeDef",
     "OperatingSystemConfigurationManagerTypeDef",
     "RebootInstanceRequestRequestTypeDef",
     "RegisterEcsClusterRequestRequestTypeDef",
     "RegisterElasticIpRequestRequestTypeDef",
     "RegisterRdsDbInstanceRequestRequestTypeDef",
@@ -125,14 +128,15 @@
     "SetPermissionRequestRequestTypeDef",
     "WeeklyAutoScalingScheduleTypeDef",
     "StartInstanceRequestRequestTypeDef",
     "StartStackRequestRequestTypeDef",
     "StopInstanceRequestRequestTypeDef",
     "StopStackRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "WeeklyAutoScalingScheduleOutputTypeDef",
     "UnassignInstanceRequestRequestTypeDef",
     "UnassignVolumeRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateElasticIpRequestRequestTypeDef",
     "UpdateInstanceRequestRequestTypeDef",
     "UpdateMyUserProfileRequestRequestTypeDef",
     "UpdateRdsDbInstanceRequestRequestTypeDef",
@@ -140,14 +144,15 @@
     "UpdateVolumeRequestRequestTypeDef",
     "AgentVersionTypeDef",
     "DescribeAgentVersionsRequestRequestTypeDef",
     "AppTypeDef",
     "CreateAppRequestRequestTypeDef",
     "UpdateAppRequestRequestTypeDef",
     "LoadBasedAutoScalingConfigurationTypeDef",
+    "AutoScalingThresholdsUnionTypeDef",
     "SetLoadBasedAutoScalingRequestRequestTypeDef",
     "BlockDeviceMappingTypeDef",
     "ChefConfigurationResponseTypeDef",
     "CloneStackResultTypeDef",
     "CreateAppResultTypeDef",
     "CreateDeploymentResultTypeDef",
     "CreateInstanceResultTypeDef",
@@ -167,18 +172,20 @@
     "SourceResponseTypeDef",
     "StackConfigurationManagerResponseTypeDef",
     "CloneStackRequestRequestTypeDef",
     "CreateStackRequestRequestTypeDef",
     "CreateStackRequestServiceResourceCreateStackTypeDef",
     "StackTypeDef",
     "UpdateStackRequestRequestTypeDef",
+    "CloudWatchLogsConfigurationOutputTypeDef",
     "CloudWatchLogsConfigurationResponseTypeDef",
     "CloudWatchLogsConfigurationTypeDef",
     "DescribeCommandsResultTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
+    "DeploymentCommandUnionTypeDef",
     "DeploymentTypeDef",
     "DescribeAppsRequestAppExistsWaitTypeDef",
     "DescribeDeploymentsRequestDeploymentSuccessfulWaitTypeDef",
     "DescribeInstancesRequestInstanceOnlineWaitTypeDef",
     "DescribeInstancesRequestInstanceRegisteredWaitTypeDef",
     "DescribeInstancesRequestInstanceStoppedWaitTypeDef",
     "DescribeInstancesRequestInstanceTerminatedWaitTypeDef",
@@ -192,25 +199,28 @@
     "DescribeRdsDbInstancesResultTypeDef",
     "DescribeServiceErrorsResultTypeDef",
     "DescribeUserProfilesResultTypeDef",
     "DescribeVolumesResultTypeDef",
     "GrantAccessResultTypeDef",
     "RegisterInstanceRequestRequestTypeDef",
     "StackSummaryTypeDef",
+    "RecipesUnionTypeDef",
     "LifecycleEventConfigurationResponseTypeDef",
     "LifecycleEventConfigurationTypeDef",
     "OperatingSystemTypeDef",
     "SetTimeBasedAutoScalingRequestRequestTypeDef",
     "TimeBasedAutoScalingConfigurationTypeDef",
+    "WeeklyAutoScalingScheduleUnionTypeDef",
     "DescribeAgentVersionsResultTypeDef",
     "DescribeAppsResultTypeDef",
     "DescribeLoadBasedAutoScalingResultTypeDef",
     "CreateInstanceRequestRequestTypeDef",
     "InstanceTypeDef",
     "DescribeStacksResultTypeDef",
+    "CloudWatchLogsConfigurationUnionTypeDef",
     "DescribeDeploymentsResultTypeDef",
     "DescribeStackSummaryResultTypeDef",
     "CreateLayerRequestRequestTypeDef",
     "CreateLayerRequestStackCreateLayerTypeDef",
     "LayerTypeDef",
     "UpdateLayerRequestRequestTypeDef",
     "DescribeOperatingSystemsResponseTypeDef",
@@ -285,24 +295,36 @@
 AttachElasticLoadBalancerRequestRequestTypeDef = TypedDict(
     "AttachElasticLoadBalancerRequestRequestTypeDef",
     {
         "ElasticLoadBalancerName": str,
         "LayerId": str,
     },
 )
+AutoScalingThresholdsOutputTypeDef = TypedDict(
+    "AutoScalingThresholdsOutputTypeDef",
+    {
+        "InstanceCount": NotRequired[int],
+        "ThresholdsWaitTime": NotRequired[int],
+        "IgnoreMetricsTime": NotRequired[int],
+        "CpuThreshold": NotRequired[float],
+        "MemoryThreshold": NotRequired[float],
+        "LoadThreshold": NotRequired[float],
+        "Alarms": NotRequired[List[str]],
+    },
+)
 AutoScalingThresholdsTypeDef = TypedDict(
     "AutoScalingThresholdsTypeDef",
     {
         "InstanceCount": NotRequired[int],
         "ThresholdsWaitTime": NotRequired[int],
         "IgnoreMetricsTime": NotRequired[int],
         "CpuThreshold": NotRequired[float],
         "MemoryThreshold": NotRequired[float],
         "LoadThreshold": NotRequired[float],
-        "Alarms": NotRequired[List[str]],
+        "Alarms": NotRequired[Sequence[str]],
     },
 )
 EbsBlockDeviceTypeDef = TypedDict(
     "EbsBlockDeviceTypeDef",
     {
         "SnapshotId": NotRequired[str],
         "Iops": NotRequired[int],
@@ -311,18 +333,18 @@
         "DeleteOnTermination": NotRequired[bool],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 ChefConfigurationTypeDef = TypedDict(
     "ChefConfigurationTypeDef",
     {
         "ManageBerkshelf": NotRequired[bool],
         "BerkshelfVersion": NotRequired[str],
@@ -425,14 +447,21 @@
 )
 DeleteUserProfileRequestRequestTypeDef = TypedDict(
     "DeleteUserProfileRequestRequestTypeDef",
     {
         "IamUserArn": str,
     },
 )
+DeploymentCommandOutputTypeDef = TypedDict(
+    "DeploymentCommandOutputTypeDef",
+    {
+        "Name": DeploymentCommandNameType,
+        "Args": NotRequired[Dict[str, List[str]]],
+    },
+)
 DeregisterEcsClusterRequestRequestTypeDef = TypedDict(
     "DeregisterEcsClusterRequestRequestTypeDef",
     {
         "EcsClusterArn": str,
     },
 )
 DeregisterElasticIpRequestRequestTypeDef = TypedDict(
@@ -806,14 +835,24 @@
         "Stopped": NotRequired[int],
         "Stopping": NotRequired[int],
         "Terminated": NotRequired[int],
         "Terminating": NotRequired[int],
         "Unassigning": NotRequired[int],
     },
 )
+RecipesOutputTypeDef = TypedDict(
+    "RecipesOutputTypeDef",
+    {
+        "Setup": NotRequired[List[str]],
+        "Configure": NotRequired[List[str]],
+        "Deploy": NotRequired[List[str]],
+        "Undeploy": NotRequired[List[str]],
+        "Shutdown": NotRequired[List[str]],
+    },
+)
 ShutdownEventConfigurationTypeDef = TypedDict(
     "ShutdownEventConfigurationTypeDef",
     {
         "ExecutionTimeout": NotRequired[int],
         "DelayUntilElbConnectionsDrained": NotRequired[bool],
     },
 )
@@ -877,21 +916,21 @@
         "AllowSudo": NotRequired[bool],
         "Level": NotRequired[str],
     },
 )
 WeeklyAutoScalingScheduleTypeDef = TypedDict(
     "WeeklyAutoScalingScheduleTypeDef",
     {
-        "Monday": NotRequired[Dict[str, str]],
-        "Tuesday": NotRequired[Dict[str, str]],
-        "Wednesday": NotRequired[Dict[str, str]],
-        "Thursday": NotRequired[Dict[str, str]],
-        "Friday": NotRequired[Dict[str, str]],
-        "Saturday": NotRequired[Dict[str, str]],
-        "Sunday": NotRequired[Dict[str, str]],
+        "Monday": NotRequired[Mapping[str, str]],
+        "Tuesday": NotRequired[Mapping[str, str]],
+        "Wednesday": NotRequired[Mapping[str, str]],
+        "Thursday": NotRequired[Mapping[str, str]],
+        "Friday": NotRequired[Mapping[str, str]],
+        "Saturday": NotRequired[Mapping[str, str]],
+        "Sunday": NotRequired[Mapping[str, str]],
     },
 )
 StartInstanceRequestRequestTypeDef = TypedDict(
     "StartInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
@@ -918,14 +957,26 @@
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
+WeeklyAutoScalingScheduleOutputTypeDef = TypedDict(
+    "WeeklyAutoScalingScheduleOutputTypeDef",
+    {
+        "Monday": NotRequired[Dict[str, str]],
+        "Tuesday": NotRequired[Dict[str, str]],
+        "Wednesday": NotRequired[Dict[str, str]],
+        "Thursday": NotRequired[Dict[str, str]],
+        "Friday": NotRequired[Dict[str, str]],
+        "Saturday": NotRequired[Dict[str, str]],
+        "Sunday": NotRequired[Dict[str, str]],
+    },
+)
 UnassignInstanceRequestRequestTypeDef = TypedDict(
     "UnassignInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 UnassignVolumeRequestRequestTypeDef = TypedDict(
@@ -1063,18 +1114,21 @@
     },
 )
 LoadBasedAutoScalingConfigurationTypeDef = TypedDict(
     "LoadBasedAutoScalingConfigurationTypeDef",
     {
         "LayerId": NotRequired[str],
         "Enable": NotRequired[bool],
-        "UpScaling": NotRequired[AutoScalingThresholdsTypeDef],
-        "DownScaling": NotRequired[AutoScalingThresholdsTypeDef],
+        "UpScaling": NotRequired[AutoScalingThresholdsOutputTypeDef],
+        "DownScaling": NotRequired[AutoScalingThresholdsOutputTypeDef],
     },
 )
+AutoScalingThresholdsUnionTypeDef = Union[
+    AutoScalingThresholdsTypeDef, AutoScalingThresholdsOutputTypeDef
+]
 SetLoadBasedAutoScalingRequestRequestTypeDef = TypedDict(
     "SetLoadBasedAutoScalingRequestRequestTypeDef",
     {
         "LayerId": str,
         "Enable": NotRequired[bool],
         "UpScaling": NotRequired[AutoScalingThresholdsTypeDef],
         "DownScaling": NotRequired[AutoScalingThresholdsTypeDef],
@@ -1194,16 +1248,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListTagsResultTypeDef = TypedDict(
     "ListTagsResultTypeDef",
     {
         "Tags": Dict[str, str],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 RecipesResponseTypeDef = TypedDict(
     "RecipesResponseTypeDef",
     {
         "Setup": List[str],
         "Configure": List[str],
@@ -1382,14 +1436,21 @@
         "CustomCookbooksSource": NotRequired[SourceTypeDef],
         "DefaultSshKeyName": NotRequired[str],
         "DefaultRootDeviceType": NotRequired[RootDeviceTypeType],
         "UseOpsworksSecurityGroups": NotRequired[bool],
         "AgentVersion": NotRequired[str],
     },
 )
+CloudWatchLogsConfigurationOutputTypeDef = TypedDict(
+    "CloudWatchLogsConfigurationOutputTypeDef",
+    {
+        "Enabled": NotRequired[bool],
+        "LogStreams": NotRequired[List[CloudWatchLogsLogStreamTypeDef]],
+    },
+)
 CloudWatchLogsConfigurationResponseTypeDef = TypedDict(
     "CloudWatchLogsConfigurationResponseTypeDef",
     {
         "Enabled": bool,
         "LogStreams": List[CloudWatchLogsLogStreamTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1416,26 +1477,27 @@
         "AppId": NotRequired[str],
         "InstanceIds": NotRequired[Sequence[str]],
         "LayerIds": NotRequired[Sequence[str]],
         "Comment": NotRequired[str],
         "CustomJson": NotRequired[str],
     },
 )
+DeploymentCommandUnionTypeDef = Union[DeploymentCommandTypeDef, DeploymentCommandOutputTypeDef]
 DeploymentTypeDef = TypedDict(
     "DeploymentTypeDef",
     {
         "DeploymentId": NotRequired[str],
         "StackId": NotRequired[str],
         "AppId": NotRequired[str],
         "CreatedAt": NotRequired[str],
         "CompletedAt": NotRequired[str],
         "Duration": NotRequired[int],
         "IamUserArn": NotRequired[str],
         "Comment": NotRequired[str],
-        "Command": NotRequired[DeploymentCommandTypeDef],
+        "Command": NotRequired[DeploymentCommandOutputTypeDef],
         "Status": NotRequired[str],
         "CustomJson": NotRequired[str],
         "InstanceIds": NotRequired[List[str]],
     },
 )
 DescribeAppsRequestAppExistsWaitTypeDef = TypedDict(
     "DescribeAppsRequestAppExistsWaitTypeDef",
@@ -1498,16 +1560,16 @@
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 DescribeEcsClustersResultTypeDef = TypedDict(
     "DescribeEcsClustersResultTypeDef",
     {
         "EcsClusters": List[EcsClusterTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeElasticIpsResultTypeDef = TypedDict(
     "DescribeElasticIpsResultTypeDef",
     {
         "ElasticIps": List[ElasticIpTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1595,14 +1657,15 @@
         "Name": NotRequired[str],
         "Arn": NotRequired[str],
         "LayersCount": NotRequired[int],
         "AppsCount": NotRequired[int],
         "InstancesCount": NotRequired[InstancesCountTypeDef],
     },
 )
+RecipesUnionTypeDef = Union[RecipesTypeDef, RecipesOutputTypeDef]
 LifecycleEventConfigurationResponseTypeDef = TypedDict(
     "LifecycleEventConfigurationResponseTypeDef",
     {
         "Shutdown": ShutdownEventConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1631,17 +1694,20 @@
         "AutoScalingSchedule": NotRequired[WeeklyAutoScalingScheduleTypeDef],
     },
 )
 TimeBasedAutoScalingConfigurationTypeDef = TypedDict(
     "TimeBasedAutoScalingConfigurationTypeDef",
     {
         "InstanceId": NotRequired[str],
-        "AutoScalingSchedule": NotRequired[WeeklyAutoScalingScheduleTypeDef],
+        "AutoScalingSchedule": NotRequired[WeeklyAutoScalingScheduleOutputTypeDef],
     },
 )
+WeeklyAutoScalingScheduleUnionTypeDef = Union[
+    WeeklyAutoScalingScheduleTypeDef, WeeklyAutoScalingScheduleOutputTypeDef
+]
 DescribeAgentVersionsResultTypeDef = TypedDict(
     "DescribeAgentVersionsResultTypeDef",
     {
         "AgentVersions": List[AgentVersionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1731,14 +1797,17 @@
 DescribeStacksResultTypeDef = TypedDict(
     "DescribeStacksResultTypeDef",
     {
         "Stacks": List[StackTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CloudWatchLogsConfigurationUnionTypeDef = Union[
+    CloudWatchLogsConfigurationTypeDef, CloudWatchLogsConfigurationOutputTypeDef
+]
 DescribeDeploymentsResultTypeDef = TypedDict(
     "DescribeDeploymentsResultTypeDef",
     {
         "Deployments": List[DeploymentTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1800,26 +1869,26 @@
         "Arn": NotRequired[str],
         "StackId": NotRequired[str],
         "LayerId": NotRequired[str],
         "Type": NotRequired[LayerTypeType],
         "Name": NotRequired[str],
         "Shortname": NotRequired[str],
         "Attributes": NotRequired[Dict[LayerAttributesKeysType, str]],
-        "CloudWatchLogsConfiguration": NotRequired[CloudWatchLogsConfigurationTypeDef],
+        "CloudWatchLogsConfiguration": NotRequired[CloudWatchLogsConfigurationOutputTypeDef],
         "CustomInstanceProfileArn": NotRequired[str],
         "CustomJson": NotRequired[str],
         "CustomSecurityGroupIds": NotRequired[List[str]],
         "DefaultSecurityGroupNames": NotRequired[List[str]],
         "Packages": NotRequired[List[str]],
         "VolumeConfigurations": NotRequired[List[VolumeConfigurationTypeDef]],
         "EnableAutoHealing": NotRequired[bool],
         "AutoAssignElasticIps": NotRequired[bool],
         "AutoAssignPublicIps": NotRequired[bool],
-        "DefaultRecipes": NotRequired[RecipesTypeDef],
-        "CustomRecipes": NotRequired[RecipesTypeDef],
+        "DefaultRecipes": NotRequired[RecipesOutputTypeDef],
+        "CustomRecipes": NotRequired[RecipesOutputTypeDef],
         "CreatedAt": NotRequired[str],
         "InstallUpdatesOnBoot": NotRequired[bool],
         "UseEbsOptimizedInstances": NotRequired[bool],
         "LifecycleEventConfiguration": NotRequired[LifecycleEventConfigurationTypeDef],
     },
 )
 UpdateLayerRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks/waiter.py` & `mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks/waiter.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     """
 
     def wait(
         self,
         *,
         StackId: str = ...,
         AppIds: Sequence[str] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Waiter.AppExists.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/waiters/#appexistswaiter)
         """
 
 
@@ -73,15 +73,15 @@
 
     def wait(
         self,
         *,
         StackId: str = ...,
         AppId: str = ...,
         DeploymentIds: Sequence[str] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Waiter.DeploymentSuccessful.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/waiters/#deploymentsuccessfulwaiter)
         """
 
 
@@ -93,15 +93,15 @@
 
     def wait(
         self,
         *,
         StackId: str = ...,
         LayerId: str = ...,
         InstanceIds: Sequence[str] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Waiter.InstanceOnline.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/waiters/#instanceonlinewaiter)
         """
 
 
@@ -113,15 +113,15 @@
 
     def wait(
         self,
         *,
         StackId: str = ...,
         LayerId: str = ...,
         InstanceIds: Sequence[str] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Waiter.InstanceRegistered.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/waiters/#instanceregisteredwaiter)
         """
 
 
@@ -133,15 +133,15 @@
 
     def wait(
         self,
         *,
         StackId: str = ...,
         LayerId: str = ...,
         InstanceIds: Sequence[str] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Waiter.InstanceStopped.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/waiters/#instancestoppedwaiter)
         """
 
 
@@ -153,13 +153,13 @@
 
     def wait(
         self,
         *,
         StackId: str = ...,
         LayerId: str = ...,
         InstanceIds: Sequence[str] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Waiter.InstanceTerminated.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/waiters/#instanceterminatedwaiter)
         """
```

### Comparing `mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks/waiter.pyi` & `mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks/waiter.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     """
 
     def wait(
         self,
         *,
         StackId: str = ...,
         AppIds: Sequence[str] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Waiter.AppExists.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/waiters/#appexistswaiter)
         """
 
 class DeploymentSuccessfulWaiter(Waiter):
@@ -71,15 +71,15 @@
 
     def wait(
         self,
         *,
         StackId: str = ...,
         AppId: str = ...,
         DeploymentIds: Sequence[str] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Waiter.DeploymentSuccessful.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/waiters/#deploymentsuccessfulwaiter)
         """
 
 class InstanceOnlineWaiter(Waiter):
@@ -90,15 +90,15 @@
 
     def wait(
         self,
         *,
         StackId: str = ...,
         LayerId: str = ...,
         InstanceIds: Sequence[str] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Waiter.InstanceOnline.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/waiters/#instanceonlinewaiter)
         """
 
 class InstanceRegisteredWaiter(Waiter):
@@ -109,15 +109,15 @@
 
     def wait(
         self,
         *,
         StackId: str = ...,
         LayerId: str = ...,
         InstanceIds: Sequence[str] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Waiter.InstanceRegistered.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/waiters/#instanceregisteredwaiter)
         """
 
 class InstanceStoppedWaiter(Waiter):
@@ -128,15 +128,15 @@
 
     def wait(
         self,
         *,
         StackId: str = ...,
         LayerId: str = ...,
         InstanceIds: Sequence[str] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Waiter.InstanceStopped.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/waiters/#instancestoppedwaiter)
         """
 
 class InstanceTerminatedWaiter(Waiter):
@@ -147,13 +147,13 @@
 
     def wait(
         self,
         *,
         StackId: str = ...,
         LayerId: str = ...,
         InstanceIds: Sequence[str] = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Waiter.InstanceTerminated.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/waiters/#instanceterminatedwaiter)
         """
```

### Comparing `mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks.egg-info/PKG-INFO` & `mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opsworks
-Version: 1.34.0
-Summary: Type annotations for boto3.OpsWorks 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.112
+Summary: Type annotations for boto3.OpsWorks 1.34.112 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-opsworks"></a>
 
 # mypy-boto3-opsworks
 
 [![PyPI - mypy-boto3-opsworks](https://img.shields.io/pypi/v/mypy-boto3-opsworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opsworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opsworks)](https://pepy.tech/project/mypy-boto3-opsworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpsWorks 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
+[boto3.OpsWorks 1.34.112](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-opsworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-opsworks-1.34.0/mypy_boto3_opsworks.egg-info/SOURCES.txt` & `mypy_boto3_opsworks-1.34.112/mypy_boto3_opsworks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworks-1.34.0/setup.py` & `mypy_boto3_opsworks-1.34.112/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,48 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-opsworks",
-    version="1.34.0",
+    version="1.34.112",
     packages=["mypy_boto3_opsworks"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.OpsWorks 1.34.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
-    ),
+    description="Type annotations for boto3.OpsWorks 1.34.112 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
-        "Typing :: Typed",
+        "Typing :: Stubs Only",
     ],
     keywords="boto3 opsworks type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_opsworks": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworks/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

