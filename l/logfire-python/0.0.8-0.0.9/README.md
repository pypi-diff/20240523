# Comparing `tmp/logfire-python-0.0.8.tar.gz` & `tmp/logfire_python-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logfire-python-0.0.8.tar", last modified: Fri Jul 28 07:24:23 2023, max compression
+gzip compressed data, was "logfire_python-0.0.9.tar", last modified: Thu May 23 04:50:12 2024, max compression
```

## Comparing `logfire-python-0.0.8.tar` & `logfire_python-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-28 07:24:23.797150 logfire-python-0.0.8/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      735 2023-06-22 13:06:58.000000 logfire-python-0.0.8/LICENSE.md
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      106 2023-06-22 13:06:58.000000 logfire-python-0.0.8/MANIFEST.in
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3754 2023-07-28 07:24:23.797150 logfire-python-0.0.8/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2664 2023-07-28 07:22:25.000000 logfire-python-0.0.8/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-28 07:24:23.797150 logfire-python-0.0.8/logfire/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      251 2023-06-22 13:06:58.000000 logfire-python-0.0.8/logfire/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      141 2023-06-22 13:06:58.000000 logfire-python-0.0.8/logfire/compat.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2998 2023-06-22 13:06:58.000000 logfire-python-0.0.8/logfire/flusher.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      968 2023-06-22 13:06:58.000000 logfire-python-0.0.8/logfire/formatter.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2759 2023-06-22 13:08:01.000000 logfire-python-0.0.8/logfire/frame.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2612 2023-07-28 07:09:44.000000 logfire-python-0.0.8/logfire/handler.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1156 2023-06-22 13:06:58.000000 logfire-python-0.0.8/logfire/helpers.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      588 2023-06-22 13:06:58.000000 logfire-python-0.0.8/logfire/uploader.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-28 07:24:23.797150 logfire-python-0.0.8/logfire_python.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3754 2023-07-28 07:24:23.000000 logfire-python-0.0.8/logfire_python.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-07-28 07:24:23.000000 logfire-python-0.0.8/logfire_python.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-28 07:24:23.000000 logfire-python-0.0.8/logfire_python.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       98 2023-07-28 07:24:23.000000 logfire-python-0.0.8/logfire_python.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        8 2023-07-28 07:24:23.000000 logfire-python-0.0.8/logfire_python.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1318 2023-07-28 07:22:26.000000 logfire-python-0.0.8/pyproject.toml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      222 2023-06-22 13:06:58.000000 logfire-python-0.0.8/requirements.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-28 07:24:23.797150 logfire-python-0.0.8/setup.cfg
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       54 2023-06-22 13:06:58.000000 logfire-python-0.0.8/setup.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-28 07:24:23.797150 logfire-python-0.0.8/tests/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 13:06:58.000000 logfire-python-0.0.8/tests/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5062 2023-07-28 07:22:24.000000 logfire-python-0.0.8/tests/test_flusher.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5264 2023-06-22 13:06:58.000000 logfire-python-0.0.8/tests/test_formatter.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1955 2023-06-22 13:06:58.000000 logfire-python-0.0.8/tests/test_frame.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4337 2023-06-22 13:06:58.000000 logfire-python-0.0.8/tests/test_handler.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1846 2023-06-22 13:06:58.000000 logfire-python-0.0.8/tests/test_helpers.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1059 2023-06-22 13:06:58.000000 logfire-python-0.0.8/tests/test_uploader.py
+drwxrwxrwx   0        0        0        0 2024-05-23 04:50:12.593154 logfire_python-0.0.9/
+-rw-rw-rw-   0        0        0      741 2024-05-23 01:37:49.000000 logfire_python-0.0.9/LICENSE.md
+-rw-rw-rw-   0        0        0      112 2024-05-23 01:37:49.000000 logfire_python-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4144 2024-05-23 04:50:12.591151 logfire_python-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2745 2024-05-23 01:37:49.000000 logfire_python-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 04:50:12.516158 logfire_python-0.0.9/logfire/
+-rw-rw-rw-   0        0        0      260 2024-05-23 01:37:49.000000 logfire_python-0.0.9/logfire/__init__.py
+-rw-rw-rw-   0        0        0      148 2024-05-23 01:37:49.000000 logfire_python-0.0.9/logfire/compat.py
+-rw-rw-rw-   0        0        0     3079 2024-05-23 01:37:49.000000 logfire_python-0.0.9/logfire/flusher.py
+-rw-rw-rw-   0        0        0      993 2024-05-23 01:37:49.000000 logfire_python-0.0.9/logfire/formatter.py
+-rw-rw-rw-   0        0        0     2848 2024-05-23 01:37:49.000000 logfire_python-0.0.9/logfire/frame.py
+-rw-rw-rw-   0        0        0     2663 2024-05-23 01:40:30.000000 logfire_python-0.0.9/logfire/handler.py
+-rw-rw-rw-   0        0        0     1201 2024-05-23 01:37:49.000000 logfire_python-0.0.9/logfire/helpers.py
+-rw-rw-rw-   0        0        0      607 2024-05-23 01:37:49.000000 logfire_python-0.0.9/logfire/uploader.py
+drwxrwxrwx   0        0        0        0 2024-05-23 04:50:12.587148 logfire_python-0.0.9/logfire_python.egg-info/
+-rw-rw-rw-   0        0        0     4144 2024-05-23 04:50:12.000000 logfire_python-0.0.9/logfire_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2024-05-23 04:50:12.000000 logfire_python-0.0.9/logfire_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 04:50:12.000000 logfire_python-0.0.9/logfire_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2024-05-23 04:50:12.000000 logfire_python-0.0.9/logfire_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-23 04:50:12.000000 logfire_python-0.0.9/logfire_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1372 2024-05-23 04:49:31.000000 logfire_python-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      222 2024-05-23 01:37:49.000000 logfire_python-0.0.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 04:50:12.593154 logfire_python-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0       58 2024-05-23 01:37:49.000000 logfire_python-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 04:50:12.584152 logfire_python-0.0.9/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-23 01:37:49.000000 logfire_python-0.0.9/tests/__init__.py
+-rw-rw-rw-   0        0        0     5206 2024-05-23 01:37:49.000000 logfire_python-0.0.9/tests/test_flusher.py
+-rw-rw-rw-   0        0        0     5399 2024-05-23 01:37:49.000000 logfire_python-0.0.9/tests/test_formatter.py
+-rw-rw-rw-   0        0        0     1997 2024-05-23 01:37:49.000000 logfire_python-0.0.9/tests/test_frame.py
+-rw-rw-rw-   0        0        0     4466 2024-05-23 01:37:49.000000 logfire_python-0.0.9/tests/test_handler.py
+-rw-rw-rw-   0        0        0     1904 2024-05-23 01:37:49.000000 logfire_python-0.0.9/tests/test_helpers.py
+-rw-rw-rw-   0        0        0     1090 2024-05-23 01:37:49.000000 logfire_python-0.0.9/tests/test_uploader.py
```

### Comparing `logfire-python-0.0.8/LICENSE.md` & `logfire_python-0.0.9/LICENSE.md`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-# License
-
-Copyright 2023 Logfire
-
-Permission to use, copy, modify, and/or distribute this software for any purpose with or without fee is hereby granted, provided that the above copyright notice and this permission notice appear in all copies.
-
+# License
+
+Copyright 2023 Logfire
+
+Permission to use, copy, modify, and/or distribute this software for any purpose with or without fee is hereby granted, provided that the above copyright notice and this permission notice appear in all copies.
+
 THE SOFTWARE IS PROVIDED “AS IS” AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
```

### Comparing `logfire-python-0.0.8/PKG-INFO` & `logfire_python-0.0.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,99 +1,106 @@
-Metadata-Version: 2.1
-Name: logfire-python
-Version: 0.0.8
-Summary: Logfire.ai client library
-Author-email: Logfire <support@logfire.ai>
-Project-URL: Homepage, https://github.com/logfire-sh/logfire-python
-Keywords: api,logfire,logging,client
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: ISC License (ISCL)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE.md
-
-# Logfire - Python Logging Made Easy
-
-
-[![ISC License](https://img.shields.io/badge/license-ISC-ff69b4.svg)](LICENSE.md)
-[![PyPI version](https://badge.fury.io/py/logfire-python.svg)](https://badge.fury.io/py/logfire-python)
-
-
-Collect logs directly from any Python code, including Django.
-
-[Logfire](https://logfire.ai) is a hosted service that centralizes all of your logs into one place. Allowing for analysis, correlation and filtering with SQL. Actionable dashboards and collaboration come built-in. Logfire works with [any language or platform and any data source](https://docs.logfire.ai/). 
-
-### Features
-- Simple integration. Integrates with the Python `logging` library.
-- Support for structured logging and events.
-- Automatically captures useful context.
-- Performant, light weight, with a thoughtful design.
-
-### Supported language versions
-- Python 3.6.5 or newer
-- `pip` 20.0.2 or newer
-
-# Installation
-Install the Logfire Python client library using the `pip` command:
-
-```bash
-pip install logfire-python
-```
-
-*Make sure you install the `logfire-python` package and not a different package with the `logfire` keyword in the package name from a different author.*
-
----
-
-# Example project
-
-To help you get started with using Logfire in your Python projects, we have prepared a simple Python program that showcases the usage of Logfire logger.
-
-## Download and install the example project
-
-You can download the [example project](https://github.com/logfire-sh/logfire-python/tree/master/example-project) from GitHub directly or you can clone it to a select directory. Then install the `logfire-python` client library as shown before:
-
-```bash
-pip install logfire-python
-```
-
- ## Run the example project
- 
- To run the example application, simply run the following command:
-
-```bash
-python main.py <source-token>
-```
-
-*Don't forget to replace `<source-token>` with your actual source token which you can find by going to logfire.com -> sources -> edit.*
-
-
-If you have trouble running the command above, check your Python installation and try running it with the `python3` command instead. It should give you the following output:
-
-```
-Output:
-All done! You can check your logs now.
-```
-
-This example project will create a total of 6 logs. Each corresponding to its respective method.
-
-## Explore how example project works
- 
-Learn how to setup Python logging by exploring the workings of the [example project](https://github.com/logfire-sh/logfire-python/tree/master/example-project) in detail. 
- 
----
- 
-## Get in touch
-
-Have any questions? Please explore the Logfire [documentation](https://docs.ai/) or contact our [support](https://support@logfire.ai).
+Metadata-Version: 2.1
+Name: logfire-python
+Version: 0.0.9
+Summary: Logfire.ai client library
+Author-email: Logfire <support@logfire.ai>
+Project-URL: Homepage, https://github.com/logfire-sh/logfire-python
+Keywords: api,logfire,logging,client
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: ISC License (ISCL)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: requests
+Requires-Dist: msgpack
+Provides-Extra: dev
+Requires-Dist: coverage>=3.7.1; extra == "dev"
+Requires-Dist: httpretty>=0.9.4; extra == "dev"
+Requires-Dist: nose>=1.3.7; extra == "dev"
+Requires-Dist: unittest2>=0.8.0; extra == "dev"
+Requires-Dist: mock>=1.0.1; extra == "dev"
+
+# Logfire - Python Logging Made Easy
+
+
+[![ISC License](https://img.shields.io/badge/license-ISC-ff69b4.svg)](LICENSE.md)
+[![PyPI version](https://badge.fury.io/py/logfire-python.svg)](https://badge.fury.io/py/logfire-python)
+
+
+Collect logs directly from any Python code, including Django.
+
+[Logfire](https://logfire.sh) is a hosted service that centralizes all of your logs into one place. Allowing for analysis, correlation and filtering with SQL. Actionable dashboards and collaboration come built-in. Logfire works with [any language or platform and any data source](https://docs.logfire.sh/). 
+
+### Features
+- Simple integration. Integrates with the Python `logging` library.
+- Support for structured logging and events.
+- Automatically captures useful context.
+- Performant, light weight, with a thoughtful design.
+
+### Supported language versions
+- Python 3.6.5 or newer
+- `pip` 20.0.2 or newer
+
+# Installation
+Install the Logfire Python client library using the `pip` command:
+
+```bash
+pip install logfire-python
+```
+
+*Make sure you install the `logfire-python` package and not a different package with the `logfire` keyword in the package name from a different author.*
+
+---
+
+# Example project
+
+To help you get started with using Logfire in your Python projects, we have prepared a simple Python program that showcases the usage of Logfire logger.
+
+## Download and install the example project
+
+You can download the [example project](https://github.com/logfire-sh/logfire-python/tree/master/example-project) from GitHub directly or you can clone it to a select directory. Then install the `logfire-python` client library as shown before:
+
+```bash
+pip install logfire-python
+```
+
+ ## Run the example project
+ 
+ To run the example application, simply run the following command:
+
+```bash
+python main.py <source-token>
+```
+
+*Don't forget to replace `<source-token>` with your actual source token which you can find by going to logfire.com -> sources -> edit.*
+
+
+If you have trouble running the command above, check your Python installation and try running it with the `python3` command instead. It should give you the following output:
+
+```
+Output:
+All done! You can check your logs now.
+```
+
+This example project will create a total of 6 logs. Each corresponding to its respective method.
+
+## Explore how example project works
+ 
+Learn how to setup Python logging by exploring the workings of the [example project](https://github.com/logfire-sh/logfire-python/tree/master/example-project) in detail. 
+ 
+---
+ 
+## Get in touch
+
+Have any questions? Please explore the Logfire [documentation](https://docs.logfire.sh/) or contact our [support](https://support@logfire.sh).
```

### Comparing `logfire-python-0.0.8/README.md` & `logfire_python-0.0.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-# Logfire - Python Logging Made Easy
-
-
-[![ISC License](https://img.shields.io/badge/license-ISC-ff69b4.svg)](LICENSE.md)
-[![PyPI version](https://badge.fury.io/py/logfire-python.svg)](https://badge.fury.io/py/logfire-python)
-
-
-Collect logs directly from any Python code, including Django.
-
-[Logfire](https://logfire.ai) is a hosted service that centralizes all of your logs into one place. Allowing for analysis, correlation and filtering with SQL. Actionable dashboards and collaboration come built-in. Logfire works with [any language or platform and any data source](https://docs.logfire.ai/). 
-
-### Features
-- Simple integration. Integrates with the Python `logging` library.
-- Support for structured logging and events.
-- Automatically captures useful context.
-- Performant, light weight, with a thoughtful design.
-
-### Supported language versions
-- Python 3.6.5 or newer
-- `pip` 20.0.2 or newer
-
-# Installation
-Install the Logfire Python client library using the `pip` command:
-
-```bash
-pip install logfire-python
-```
-
-*Make sure you install the `logfire-python` package and not a different package with the `logfire` keyword in the package name from a different author.*
-
----
-
-# Example project
-
-To help you get started with using Logfire in your Python projects, we have prepared a simple Python program that showcases the usage of Logfire logger.
-
-## Download and install the example project
-
-You can download the [example project](https://github.com/logfire-sh/logfire-python/tree/master/example-project) from GitHub directly or you can clone it to a select directory. Then install the `logfire-python` client library as shown before:
-
-```bash
-pip install logfire-python
-```
-
- ## Run the example project
- 
- To run the example application, simply run the following command:
-
-```bash
-python main.py <source-token>
-```
-
-*Don't forget to replace `<source-token>` with your actual source token which you can find by going to logfire.com -> sources -> edit.*
-
-
-If you have trouble running the command above, check your Python installation and try running it with the `python3` command instead. It should give you the following output:
-
-```
-Output:
-All done! You can check your logs now.
-```
-
-This example project will create a total of 6 logs. Each corresponding to its respective method.
-
-## Explore how example project works
- 
-Learn how to setup Python logging by exploring the workings of the [example project](https://github.com/logfire-sh/logfire-python/tree/master/example-project) in detail. 
- 
----
- 
-## Get in touch
-
-Have any questions? Please explore the Logfire [documentation](https://docs.ai/) or contact our [support](https://support@logfire.ai).
+# Logfire - Python Logging Made Easy
+
+
+[![ISC License](https://img.shields.io/badge/license-ISC-ff69b4.svg)](LICENSE.md)
+[![PyPI version](https://badge.fury.io/py/logfire-python.svg)](https://badge.fury.io/py/logfire-python)
+
+
+Collect logs directly from any Python code, including Django.
+
+[Logfire](https://logfire.sh) is a hosted service that centralizes all of your logs into one place. Allowing for analysis, correlation and filtering with SQL. Actionable dashboards and collaboration come built-in. Logfire works with [any language or platform and any data source](https://docs.logfire.sh/). 
+
+### Features
+- Simple integration. Integrates with the Python `logging` library.
+- Support for structured logging and events.
+- Automatically captures useful context.
+- Performant, light weight, with a thoughtful design.
+
+### Supported language versions
+- Python 3.6.5 or newer
+- `pip` 20.0.2 or newer
+
+# Installation
+Install the Logfire Python client library using the `pip` command:
+
+```bash
+pip install logfire-python
+```
+
+*Make sure you install the `logfire-python` package and not a different package with the `logfire` keyword in the package name from a different author.*
+
+---
+
+# Example project
+
+To help you get started with using Logfire in your Python projects, we have prepared a simple Python program that showcases the usage of Logfire logger.
+
+## Download and install the example project
+
+You can download the [example project](https://github.com/logfire-sh/logfire-python/tree/master/example-project) from GitHub directly or you can clone it to a select directory. Then install the `logfire-python` client library as shown before:
+
+```bash
+pip install logfire-python
+```
+
+ ## Run the example project
+ 
+ To run the example application, simply run the following command:
+
+```bash
+python main.py <source-token>
+```
+
+*Don't forget to replace `<source-token>` with your actual source token which you can find by going to logfire.com -> sources -> edit.*
+
+
+If you have trouble running the command above, check your Python installation and try running it with the `python3` command instead. It should give you the following output:
+
+```
+Output:
+All done! You can check your logs now.
+```
+
+This example project will create a total of 6 logs. Each corresponding to its respective method.
+
+## Explore how example project works
+ 
+Learn how to setup Python logging by exploring the workings of the [example project](https://github.com/logfire-sh/logfire-python/tree/master/example-project) in detail. 
+ 
+---
+ 
+## Get in touch
+
+Have any questions? Please explore the Logfire [documentation](https://docs.logfire.sh/) or contact our [support](https://support@logfire.sh).
```

### Comparing `logfire-python-0.0.8/logfire/formatter.py` & `logfire_python-0.0.9/logfire/formatter.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# coding: utf-8
-from __future__ import print_function, unicode_literals
-import logging
-import json
-
-from .helpers import DEFAULT_CONTEXT
-from .frame import create_frame
-
-
-class LogfireFormatter(logging.Formatter):
-    def __init__(self,
-                 context=DEFAULT_CONTEXT,
-                 json_default=None,
-                 json_encoder=None):
-        self.context = context
-        self.json_default = json_default
-        self.json_encoder = json_encoder
-
-    def format(self, record):
-        # Because the formatter does not have an underlying format string for
-        # which `extra` may be used to substitute arguments (see
-        # https://docs.python.org/2/library/logging.html#logging.debug ), we
-        # augment the log frame with all of the entries in extra.
-        frame = create_frame(record, record.getMessage(), self.context, include_extra_attributes=True)
-        return json.dumps(frame, default=self.json_default, cls=self.json_encoder)
+# coding: utf-8
+from __future__ import print_function, unicode_literals
+import logging
+import json
+
+from .helpers import DEFAULT_CONTEXT
+from .frame import create_frame
+
+
+class LogfireFormatter(logging.Formatter):
+    def __init__(self,
+                 context=DEFAULT_CONTEXT,
+                 json_default=None,
+                 json_encoder=None):
+        self.context = context
+        self.json_default = json_default
+        self.json_encoder = json_encoder
+
+    def format(self, record):
+        # Because the formatter does not have an underlying format string for
+        # which `extra` may be used to substitute arguments (see
+        # https://docs.python.org/2/library/logging.html#logging.debug ), we
+        # augment the log frame with all of the entries in extra.
+        frame = create_frame(record, record.getMessage(), self.context, include_extra_attributes=True)
+        return json.dumps(frame, default=self.json_default, cls=self.json_encoder)
```

### Comparing `logfire-python-0.0.8/logfire/frame.py` & `logfire_python-0.0.9/logfire/frame.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-# coding: utf-8
-from __future__ import print_function, unicode_literals
-from datetime import datetime
-import json
-
-from os import path
-import __main__
-
-def create_frame(record, message, context, include_extra_attributes=False):
-    r = record.__dict__
-    frame = {}
-    # Python 3 only solution if we ever drop Python 2.7.
-    # frame['dt'] = datetime.utcfromtimestamp(r['created']).replace(tzinfo=timezone.utc).isoformat()
-    frame['dt'] = "{}+00:00".format(datetime.utcfromtimestamp(r['created']).isoformat())
-    frame['level'] = level = _levelname(r['levelname'])
-    frame['severity'] = int(r['levelno'] / 10)
-    frame['message'] = message
-    frame['context'] = ctx = {}
-
-    # Runtime context
-    ctx['runtime'] = runtime = {}
-    runtime['function'] = r['funcName']
-    runtime['file'] = _relative_to_main_module_if_possible(r['pathname'])
-    runtime['line'] = r['lineno']
-    runtime['thread_id'] = r['thread']
-    runtime['thread_name'] = r['threadName']
-    runtime['logger_name'] = r['name']
-
-    # Runtime context
-    ctx['system'] = system = {}
-    system['pid'] = r['process']
-    system['process_name'] = r['processName']
-
-    # Custom context
-    if context.exists():
-        ctx.update(context.collapse())
-
-    events = _parse_custom_events(record, include_extra_attributes)
-    if events:
-        frame.update(events)
-
-    return frame
-
-
-def _parse_custom_events(record, include_extra_attributes):
-    default_keys = {
-        'args', 'asctime', 'created', 'exc_info', 'exc_text', 'pathname',
-        'funcName', 'levelname', 'levelno', 'lineno', 'module', 'msecs',
-        'message', 'msg', 'name', 'pathname', 'process', 'processName',
-        'relativeCreated', 'thread', 'threadName'
-    }
-    extra_keys = {
-        'filename', 'stack_info'
-    }
-    events = {}
-    extra = {}
-    for key, val in record.__dict__.items():
-        if key in default_keys:
-            continue
-        if not include_extra_attributes and not isinstance(val, dict):
-            continue
-        if key not in extra_keys:
-            if isinstance(val, str):
-                extra[key] = val
-            else:
-                extra[key] = json.dumps(val)
-        else:
-            events[key] = val
-    if extra :
-        events["extra"] = extra
-    return events
-
-
-def _levelname(level):
-    return {
-        'debug': 'debug',
-        'info': 'info',
-        'warning': 'warn',
-        'error': 'error',
-        'critical': 'critical',
-    }[level.lower()]
-
-
-def _relative_to_main_module_if_possible(pathname):
-    has_main_module = hasattr(__main__, '__file__')
-    return _relative_to_main_module(pathname) if has_main_module else pathname
-
-def _relative_to_main_module(pathname):
-    return path.relpath(pathname, path.dirname(__main__.__file__))
+# coding: utf-8
+from __future__ import print_function, unicode_literals
+from datetime import datetime
+import json
+
+from os import path
+import __main__
+
+def create_frame(record, message, context, include_extra_attributes=False):
+    r = record.__dict__
+    frame = {}
+    # Python 3 only solution if we ever drop Python 2.7.
+    # frame['dt'] = datetime.utcfromtimestamp(r['created']).replace(tzinfo=timezone.utc).isoformat()
+    frame['dt'] = "{}+00:00".format(datetime.utcfromtimestamp(r['created']).isoformat())
+    frame['level'] = level = _levelname(r['levelname'])
+    frame['severity'] = int(r['levelno'] / 10)
+    frame['message'] = message
+    frame['context'] = ctx = {}
+
+    # Runtime context
+    ctx['runtime'] = runtime = {}
+    runtime['function'] = r['funcName']
+    runtime['file'] = _relative_to_main_module_if_possible(r['pathname'])
+    runtime['line'] = r['lineno']
+    runtime['thread_id'] = r['thread']
+    runtime['thread_name'] = r['threadName']
+    runtime['logger_name'] = r['name']
+
+    # Runtime context
+    ctx['system'] = system = {}
+    system['pid'] = r['process']
+    system['process_name'] = r['processName']
+
+    # Custom context
+    if context.exists():
+        ctx.update(context.collapse())
+
+    events = _parse_custom_events(record, include_extra_attributes)
+    if events:
+        frame.update(events)
+
+    return frame
+
+
+def _parse_custom_events(record, include_extra_attributes):
+    default_keys = {
+        'args', 'asctime', 'created', 'exc_info', 'exc_text', 'pathname',
+        'funcName', 'levelname', 'levelno', 'lineno', 'module', 'msecs',
+        'message', 'msg', 'name', 'pathname', 'process', 'processName',
+        'relativeCreated', 'thread', 'threadName'
+    }
+    extra_keys = {
+        'filename', 'stack_info'
+    }
+    events = {}
+    extra = {}
+    for key, val in record.__dict__.items():
+        if key in default_keys:
+            continue
+        if not include_extra_attributes and not isinstance(val, dict):
+            continue
+        if key not in extra_keys:
+            if isinstance(val, str):
+                extra[key] = val
+            else:
+                extra[key] = json.dumps(val)
+        else:
+            events[key] = val
+    if extra :
+        events["extra"] = extra
+    return events
+
+
+def _levelname(level):
+    return {
+        'debug': 'debug',
+        'info': 'info',
+        'warning': 'warn',
+        'error': 'error',
+        'critical': 'critical',
+    }[level.lower()]
+
+
+def _relative_to_main_module_if_possible(pathname):
+    has_main_module = hasattr(__main__, '__file__')
+    return _relative_to_main_module(pathname) if has_main_module else pathname
+
+def _relative_to_main_module(pathname):
+    return path.relpath(pathname, path.dirname(__main__.__file__))
```

### Comparing `logfire-python-0.0.8/logfire/handler.py` & `logfire_python-0.0.9/logfire/handler.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,69 +1,73 @@
-from __future__ import print_function, unicode_literals
-import logging
-import multiprocessing
-
-from .compat import queue
-from .helpers import DEFAULT_CONTEXT
-from .flusher import FlushWorker
-from .uploader import Uploader
-from .frame import create_frame
-
-DEFAULT_HOST = 'https://in.logfire.ai'
-DEFAULT_BUFFER_CAPACITY = 1000
-DEFAULT_FLUSH_INTERVAL = 1
-DEFAULT_RAISE_EXCEPTIONS = False
-DEFAULT_DROP_EXTRA_EVENTS = True
-DEFAULT_INCLUDE_EXTRA_ATTRIBUTES = True
-
-
-class LogfireHandler(logging.Handler):
-    def __init__(self,
-                 source_token,
-                 host=DEFAULT_HOST,
-                 buffer_capacity=DEFAULT_BUFFER_CAPACITY,
-                 flush_interval=DEFAULT_FLUSH_INTERVAL,
-                 raise_exceptions=DEFAULT_RAISE_EXCEPTIONS,
-                 drop_extra_events=DEFAULT_DROP_EXTRA_EVENTS,
-                 include_extra_attributes=DEFAULT_INCLUDE_EXTRA_ATTRIBUTES,
-                 context=DEFAULT_CONTEXT,
-                 level=logging.NOTSET):
-        super(LogfireHandler, self).__init__(level=level)
-        self.source_token = source_token
-        self.host = host
-        self.context = context
-        self.pipe = multiprocessing.JoinableQueue(maxsize=buffer_capacity)
-        self.uploader = Uploader(self.source_token, self.host)
-        self.drop_extra_events = drop_extra_events
-        self.include_extra_attributes = include_extra_attributes
-        self.buffer_capacity = buffer_capacity
-        self.flush_interval = flush_interval
-        self.raise_exceptions = raise_exceptions
-        self.dropcount = 0
-        self.flush_thread = FlushWorker(
-            self.uploader,
-            self.pipe,
-            self.buffer_capacity,
-            self.flush_interval
-        )
-        if self._is_main_process():
-            self.flush_thread.start()
-
-    def _is_main_process(self):
-        return multiprocessing.current_process()._parent_pid == None
-
-    def emit(self, record):
-        try:
-            if self._is_main_process() and not self.flush_thread.is_alive():
-                self.flush_thread.start()
-            message = self.format(record)
-            frame = create_frame(record, message, self.context, include_extra_attributes=self.include_extra_attributes)
-            try:
-                self.pipe.put(frame, block=(not self.drop_extra_events))
-            except queue.Full:
-                # Only raised when not blocking, which means that extra events
-                # should be dropped.
-                self.dropcount += 1
-                pass
-        except Exception as e:
-            if self.raise_exceptions:
-                raise e
+from __future__ import print_function, unicode_literals
+import logging
+import multiprocessing
+
+from .compat import queue
+from .helpers import DEFAULT_CONTEXT
+from .flusher import FlushWorker
+from .uploader import Uploader
+from .frame import create_frame
+
+DEFAULT_HOST = "https://in.logfire.ai"
+DEFAULT_BUFFER_CAPACITY = 1000
+DEFAULT_FLUSH_INTERVAL = 1
+DEFAULT_RAISE_EXCEPTIONS = False
+DEFAULT_DROP_EXTRA_EVENTS = True
+DEFAULT_INCLUDE_EXTRA_ATTRIBUTES = True
+
+
+class LogfireHandler(logging.Handler):
+    def __init__(
+        self,
+        source_token,
+        host=DEFAULT_HOST,
+        buffer_capacity=DEFAULT_BUFFER_CAPACITY,
+        flush_interval=DEFAULT_FLUSH_INTERVAL,
+        raise_exceptions=DEFAULT_RAISE_EXCEPTIONS,
+        drop_extra_events=DEFAULT_DROP_EXTRA_EVENTS,
+        include_extra_attributes=DEFAULT_INCLUDE_EXTRA_ATTRIBUTES,
+        context=DEFAULT_CONTEXT,
+        level=logging.NOTSET,
+    ):
+        super(LogfireHandler, self).__init__(level=level)
+        self.source_token = source_token
+        self.host = host
+        self.context = context
+        self.pipe = multiprocessing.JoinableQueue(maxsize=buffer_capacity)
+        self.uploader = Uploader(self.source_token, self.host)
+        self.drop_extra_events = drop_extra_events
+        self.include_extra_attributes = include_extra_attributes
+        self.buffer_capacity = buffer_capacity
+        self.flush_interval = flush_interval
+        self.raise_exceptions = raise_exceptions
+        self.dropcount = 0
+        self.flush_thread = FlushWorker(
+            self.uploader, self.pipe, self.buffer_capacity, self.flush_interval
+        )
+        if self._is_main_process():
+            self.flush_thread.start()
+
+    def _is_main_process(self):
+        return multiprocessing.current_process()._parent_pid == None
+
+    def emit(self, record):
+        try:
+            if self._is_main_process() and not self.flush_thread.is_alive():
+                self.flush_thread.start()
+            message = self.format(record)
+            frame = create_frame(
+                record,
+                message,
+                self.context,
+                include_extra_attributes=self.include_extra_attributes,
+            )
+            try:
+                self.pipe.put(frame, block=(not self.drop_extra_events))
+            except queue.Full:
+                # Only raised when not blocking, which means that extra events
+                # should be dropped.
+                self.dropcount += 1
+                pass
+        except Exception as e:
+            if self.raise_exceptions:
+                raise e
```

### Comparing `logfire-python-0.0.8/logfire/helpers.py` & `logfire_python-0.0.9/logfire/helpers.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-# coding: utf-8
-from __future__ import print_function, unicode_literals
-
-
-class LogfireContext(object):
-    def __init__(self):
-        self.extras = []
-
-    def context(self, *args, **kwargs):
-        if args:
-            raise ValueError(
-                'All contexts must be passed by name as keyword arguments'
-            )
-        for key, val in kwargs.items():
-            if not isinstance(val, dict):
-                raise ValueError(
-                    'All contexts must be dictionaries: %s' % key
-                )
-        self.extras.append(kwargs)
-        return self
-
-    def __call__(self, *args, **kwargs):
-        return self.context(*args, **kwargs)
-
-    def __enter__(self):
-        return self
-
-    def __exit__(self, type_, value, traceback):
-        if type_ is not None:
-            return False
-        self.extras.pop()
-        return self
-
-    def exists(self):
-        return bool(self.extras)
-
-    def collapse(self):
-        x = {}
-        for contexts in self.extras:
-            for name, data in contexts.items():
-                x.setdefault(name, {}).update(data)
-        return x
-
-
-DEFAULT_CONTEXT = LogfireContext()
+# coding: utf-8
+from __future__ import print_function, unicode_literals
+
+
+class LogfireContext(object):
+    def __init__(self):
+        self.extras = []
+
+    def context(self, *args, **kwargs):
+        if args:
+            raise ValueError(
+                'All contexts must be passed by name as keyword arguments'
+            )
+        for key, val in kwargs.items():
+            if not isinstance(val, dict):
+                raise ValueError(
+                    'All contexts must be dictionaries: %s' % key
+                )
+        self.extras.append(kwargs)
+        return self
+
+    def __call__(self, *args, **kwargs):
+        return self.context(*args, **kwargs)
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, type_, value, traceback):
+        if type_ is not None:
+            return False
+        self.extras.pop()
+        return self
+
+    def exists(self):
+        return bool(self.extras)
+
+    def collapse(self):
+        x = {}
+        for contexts in self.extras:
+            for name, data in contexts.items():
+                x.setdefault(name, {}).update(data)
+        return x
+
+
+DEFAULT_CONTEXT = LogfireContext()
```

### Comparing `logfire-python-0.0.8/logfire_python.egg-info/PKG-INFO` & `logfire_python-0.0.9/logfire_python.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,99 +1,106 @@
-Metadata-Version: 2.1
-Name: logfire-python
-Version: 0.0.8
-Summary: Logfire.ai client library
-Author-email: Logfire <support@logfire.ai>
-Project-URL: Homepage, https://github.com/logfire-sh/logfire-python
-Keywords: api,logfire,logging,client
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: ISC License (ISCL)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE.md
-
-# Logfire - Python Logging Made Easy
-
-
-[![ISC License](https://img.shields.io/badge/license-ISC-ff69b4.svg)](LICENSE.md)
-[![PyPI version](https://badge.fury.io/py/logfire-python.svg)](https://badge.fury.io/py/logfire-python)
-
-
-Collect logs directly from any Python code, including Django.
-
-[Logfire](https://logfire.ai) is a hosted service that centralizes all of your logs into one place. Allowing for analysis, correlation and filtering with SQL. Actionable dashboards and collaboration come built-in. Logfire works with [any language or platform and any data source](https://docs.logfire.ai/). 
-
-### Features
-- Simple integration. Integrates with the Python `logging` library.
-- Support for structured logging and events.
-- Automatically captures useful context.
-- Performant, light weight, with a thoughtful design.
-
-### Supported language versions
-- Python 3.6.5 or newer
-- `pip` 20.0.2 or newer
-
-# Installation
-Install the Logfire Python client library using the `pip` command:
-
-```bash
-pip install logfire-python
-```
-
-*Make sure you install the `logfire-python` package and not a different package with the `logfire` keyword in the package name from a different author.*
-
----
-
-# Example project
-
-To help you get started with using Logfire in your Python projects, we have prepared a simple Python program that showcases the usage of Logfire logger.
-
-## Download and install the example project
-
-You can download the [example project](https://github.com/logfire-sh/logfire-python/tree/master/example-project) from GitHub directly or you can clone it to a select directory. Then install the `logfire-python` client library as shown before:
-
-```bash
-pip install logfire-python
-```
-
- ## Run the example project
- 
- To run the example application, simply run the following command:
-
-```bash
-python main.py <source-token>
-```
-
-*Don't forget to replace `<source-token>` with your actual source token which you can find by going to logfire.com -> sources -> edit.*
-
-
-If you have trouble running the command above, check your Python installation and try running it with the `python3` command instead. It should give you the following output:
-
-```
-Output:
-All done! You can check your logs now.
-```
-
-This example project will create a total of 6 logs. Each corresponding to its respective method.
-
-## Explore how example project works
- 
-Learn how to setup Python logging by exploring the workings of the [example project](https://github.com/logfire-sh/logfire-python/tree/master/example-project) in detail. 
- 
----
- 
-## Get in touch
-
-Have any questions? Please explore the Logfire [documentation](https://docs.ai/) or contact our [support](https://support@logfire.ai).
+Metadata-Version: 2.1
+Name: logfire-python
+Version: 0.0.9
+Summary: Logfire.ai client library
+Author-email: Logfire <support@logfire.ai>
+Project-URL: Homepage, https://github.com/logfire-sh/logfire-python
+Keywords: api,logfire,logging,client
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: ISC License (ISCL)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: requests
+Requires-Dist: msgpack
+Provides-Extra: dev
+Requires-Dist: coverage>=3.7.1; extra == "dev"
+Requires-Dist: httpretty>=0.9.4; extra == "dev"
+Requires-Dist: nose>=1.3.7; extra == "dev"
+Requires-Dist: unittest2>=0.8.0; extra == "dev"
+Requires-Dist: mock>=1.0.1; extra == "dev"
+
+# Logfire - Python Logging Made Easy
+
+
+[![ISC License](https://img.shields.io/badge/license-ISC-ff69b4.svg)](LICENSE.md)
+[![PyPI version](https://badge.fury.io/py/logfire-python.svg)](https://badge.fury.io/py/logfire-python)
+
+
+Collect logs directly from any Python code, including Django.
+
+[Logfire](https://logfire.sh) is a hosted service that centralizes all of your logs into one place. Allowing for analysis, correlation and filtering with SQL. Actionable dashboards and collaboration come built-in. Logfire works with [any language or platform and any data source](https://docs.logfire.sh/). 
+
+### Features
+- Simple integration. Integrates with the Python `logging` library.
+- Support for structured logging and events.
+- Automatically captures useful context.
+- Performant, light weight, with a thoughtful design.
+
+### Supported language versions
+- Python 3.6.5 or newer
+- `pip` 20.0.2 or newer
+
+# Installation
+Install the Logfire Python client library using the `pip` command:
+
+```bash
+pip install logfire-python
+```
+
+*Make sure you install the `logfire-python` package and not a different package with the `logfire` keyword in the package name from a different author.*
+
+---
+
+# Example project
+
+To help you get started with using Logfire in your Python projects, we have prepared a simple Python program that showcases the usage of Logfire logger.
+
+## Download and install the example project
+
+You can download the [example project](https://github.com/logfire-sh/logfire-python/tree/master/example-project) from GitHub directly or you can clone it to a select directory. Then install the `logfire-python` client library as shown before:
+
+```bash
+pip install logfire-python
+```
+
+ ## Run the example project
+ 
+ To run the example application, simply run the following command:
+
+```bash
+python main.py <source-token>
+```
+
+*Don't forget to replace `<source-token>` with your actual source token which you can find by going to logfire.com -> sources -> edit.*
+
+
+If you have trouble running the command above, check your Python installation and try running it with the `python3` command instead. It should give you the following output:
+
+```
+Output:
+All done! You can check your logs now.
+```
+
+This example project will create a total of 6 logs. Each corresponding to its respective method.
+
+## Explore how example project works
+ 
+Learn how to setup Python logging by exploring the workings of the [example project](https://github.com/logfire-sh/logfire-python/tree/master/example-project) in detail. 
+ 
+---
+ 
+## Get in touch
+
+Have any questions? Please explore the Logfire [documentation](https://docs.logfire.sh/) or contact our [support](https://support@logfire.sh).
```

### Comparing `logfire-python-0.0.8/logfire_python.egg-info/SOURCES.txt` & `logfire_python-0.0.9/logfire_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logfire-python-0.0.8/pyproject.toml` & `logfire_python-0.0.9/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,42 @@
-[build-system]
-requires = ["setuptools>=61.0.0", "wheel"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "logfire-python"
-version = "0.0.8"
-description = "Logfire.ai client library"
-readme = "README.md"
-authors = [{ name = "Logfire", email = "support@logfire.ai" }]
-license = { file = "LICENSE" }
-classifiers = [
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: ISC License (ISCL)",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 2",
-    "Programming Language :: Python :: 2.7",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.5",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-]
-keywords = ["api", "logfire", "logging", "client"]
-dependencies = [
-    "requests",
-    "msgpack",
-]
-
-[project.optional-dependencies]
-dev = ["coverage>=3.7.1", "httpretty>=0.9.4", "nose>=1.3.7", "unittest2>=0.8.0", "mock>=1.0.1"]
-
-[project.urls]
-Homepage = "https://github.com/logfire-sh/logfire-python"
+[build-system]
+requires = ["setuptools>=61.0.0", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "logfire-python"
+version = "0.0.9"
+description = "Logfire.ai client library"
+readme = "README.md"
+authors = [{ name = "Logfire", email = "support@logfire.ai" }]
+license = { file = "LICENSE" }
+classifiers = [
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: ISC License (ISCL)",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 2",
+    "Programming Language :: Python :: 2.7",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.5",
+    "Programming Language :: Python :: 3.6",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+]
+keywords = ["api", "logfire", "logging", "client"]
+dependencies = ["requests", "msgpack"]
+
+[project.optional-dependencies]
+dev = [
+    "coverage>=3.7.1",
+    "httpretty>=0.9.4",
+    "nose>=1.3.7",
+    "unittest2>=0.8.0",
+    "mock>=1.0.1",
+]
+
+[project.urls]
+Homepage = "https://github.com/logfire-sh/logfire-python"
```

### Comparing `logfire-python-0.0.8/tests/test_flusher.py` & `logfire_python-0.0.9/tests/test_flusher.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,144 +1,144 @@
-# coding: utf-8
-from __future__ import print_function, unicode_literals
-import mock
-import time
-import threading
-import unittest2
-
-from logfire.compat import queue
-from logfire.flusher import RETRY_SCHEDULE
-from logfire.flusher import FlushWorker
-from logfire.uploader import Uploader
-
-
-class TestFlushWorker(unittest2.TestCase):
-    host = 'https://in.logfire.ai'
-    source_token = 'dummy_source_token'
-    buffer_capacity = 5
-    flush_interval = 2
-
-    def _setup_worker(self, uploader=None):
-        pipe = queue.Queue(maxsize=self.buffer_capacity)
-        uploader = uploader or Uploader(self.source_token, self.host)
-        fw = FlushWorker(uploader, pipe, self.buffer_capacity, self.flush_interval)
-        return pipe, uploader, fw
-
-    def test_is_thread(self):
-        pipe, uploader, fw = self._setup_worker()
-        self.assertIsInstance(fw, threading.Thread)
-
-    def test_flushes_when_queue_is_full(self):
-        first_frame = list(range(self.buffer_capacity))
-        second_frame = list(range(self.buffer_capacity, self.buffer_capacity * 2))
-        self.calls = 0
-        self.flush_interval = 1000
-
-        def uploader(frame):
-            self.calls += 1
-            self.assertEqual(frame, first_frame)
-            return mock.MagicMock(status_code=202)
-
-        pipe, _, fw = self._setup_worker(uploader)
-
-        for log in first_frame:
-            pipe.put(log, block=False)
-
-        t1 = time.time()
-        fw.step()
-        t2 = time.time()
-        self.assertLess(t2 - t1, self.flush_interval)
-
-        self.assertEqual(self.calls, 1)
-
-    @mock.patch('logfire.flusher._calculate_time_remaining')
-    def test_flushes_after_interval(self, calculate_time_remaining):
-        self.buffer_capacity = 10
-        num_items = 2
-        first_frame = list(range(self.buffer_capacity))
-        self.assertLess(num_items, self.buffer_capacity)
-
-        self.upload_calls = 0
-        def uploader(frame):
-            self.upload_calls += 1
-            self.assertEqual(frame, first_frame[:num_items])
-            return mock.MagicMock(status_code=202)
-
-        self.timeout_calls = 0
-        def timeout(last_flush, interval):
-            self.timeout_calls += 1
-            # Until the last item has been retrieved from the pipe, the timeout
-            # length doesn't matter. After the last item has been retrieved,
-            # return a very small number so that the blocking get times out
-            if self.timeout_calls < num_items:
-                return 1000000
-            return 0
-        calculate_time_remaining.side_effect = timeout
-
-        pipe, _, fw = self._setup_worker(uploader)
-        for i in range(num_items):
-            pipe.put(first_frame[i], block=False)
-
-        fw.step()
-        self.assertEqual(self.upload_calls, 1)
-        self.assertEqual(self.timeout_calls, 2)
-
-    @mock.patch('logfire.flusher._calculate_time_remaining')
-    @mock.patch('logfire.flusher._initial_time_remaining')
-    def test_does_nothing_without_any_items(self, initial_time_remaining, calculate_time_remaining):
-        calculate_time_remaining.side_effect = lambda a,b: 0.0
-        initial_time_remaining.side_effect = lambda a: 0.0001
-
-        uploader = mock.MagicMock(side_effect=mock.MagicMock(status_code=202))
-        pipe, _, fw = self._setup_worker(uploader)
-
-        self.assertEqual(pipe.qsize(), 0)
-        fw.step()
-        self.assertFalse(uploader.called)
-
-    @mock.patch('logfire.flusher.time.sleep')
-    def test_retries_according_to_schedule(self, mock_sleep):
-        first_frame = list(range(self.buffer_capacity))
-
-        self.uploader_calls = 0
-        def uploader(frame):
-            self.uploader_calls += 1
-            self.assertEqual(frame, first_frame)
-            return mock.MagicMock(status_code=500)
-
-        self.sleep_calls = 0
-        def sleep(time):
-            self.assertEqual(time, RETRY_SCHEDULE[self.sleep_calls])
-            self.sleep_calls += 1
-        mock_sleep.side_effect = sleep
-
-        pipe, _, fw = self._setup_worker(uploader)
-
-        for log in first_frame:
-            pipe.put(log, block=False)
-
-        fw.step()
-        self.assertEqual(self.uploader_calls, len(RETRY_SCHEDULE) + 1)
-        self.assertEqual(self.sleep_calls, len(RETRY_SCHEDULE))
-
-    @mock.patch('logfire.flusher.sys.exit')
-    def test_shutdown_condition_empties_queue_and_calls_exit(self, mock_exit):
-        self.buffer_capacity = 10
-        num_items = 5
-        first_frame = list(range(self.buffer_capacity))
-        self.assertLess(num_items, self.buffer_capacity)
-
-        self.upload_calls = 0
-        def uploader(frame):
-            self.upload_calls += 1
-            self.assertEqual(frame, first_frame[:num_items])
-            return mock.MagicMock(status_code=202)
-
-        pipe, _, fw = self._setup_worker(uploader)
-        fw.parent_thread = mock.MagicMock(is_alive=lambda: False)
-
-        for i in range(num_items):
-            pipe.put(first_frame[i], block=False)
-
-        fw.step()
-        self.assertEqual(self.upload_calls, 1)
-        self.assertEqual(mock_exit.call_count, 1)
+# coding: utf-8
+from __future__ import print_function, unicode_literals
+import mock
+import time
+import threading
+import unittest2
+
+from logfire.compat import queue
+from logfire.flusher import RETRY_SCHEDULE
+from logfire.flusher import FlushWorker
+from logfire.uploader import Uploader
+
+
+class TestFlushWorker(unittest2.TestCase):
+    host = 'https://in.logfire.sh'
+    source_token = 'dummy_source_token'
+    buffer_capacity = 5
+    flush_interval = 2
+
+    def _setup_worker(self, uploader=None):
+        pipe = queue.Queue(maxsize=self.buffer_capacity)
+        uploader = uploader or Uploader(self.source_token, self.host)
+        fw = FlushWorker(uploader, pipe, self.buffer_capacity, self.flush_interval)
+        return pipe, uploader, fw
+
+    def test_is_thread(self):
+        pipe, uploader, fw = self._setup_worker()
+        self.assertIsInstance(fw, threading.Thread)
+
+    def test_flushes_when_queue_is_full(self):
+        first_frame = list(range(self.buffer_capacity))
+        second_frame = list(range(self.buffer_capacity, self.buffer_capacity * 2))
+        self.calls = 0
+        self.flush_interval = 1000
+
+        def uploader(frame):
+            self.calls += 1
+            self.assertEqual(frame, first_frame)
+            return mock.MagicMock(status_code=202)
+
+        pipe, _, fw = self._setup_worker(uploader)
+
+        for log in first_frame:
+            pipe.put(log, block=False)
+
+        t1 = time.time()
+        fw.step()
+        t2 = time.time()
+        self.assertLess(t2 - t1, self.flush_interval)
+
+        self.assertEqual(self.calls, 1)
+
+    @mock.patch('logfire.flusher._calculate_time_remaining')
+    def test_flushes_after_interval(self, calculate_time_remaining):
+        self.buffer_capacity = 10
+        num_items = 2
+        first_frame = list(range(self.buffer_capacity))
+        self.assertLess(num_items, self.buffer_capacity)
+
+        self.upload_calls = 0
+        def uploader(frame):
+            self.upload_calls += 1
+            self.assertEqual(frame, first_frame[:num_items])
+            return mock.MagicMock(status_code=202)
+
+        self.timeout_calls = 0
+        def timeout(last_flush, interval):
+            self.timeout_calls += 1
+            # Until the last item has been retrieved from the pipe, the timeout
+            # length doesn't matter. After the last item has been retrieved,
+            # return a very small number so that the blocking get times out
+            if self.timeout_calls < num_items:
+                return 1000000
+            return 0
+        calculate_time_remaining.side_effect = timeout
+
+        pipe, _, fw = self._setup_worker(uploader)
+        for i in range(num_items):
+            pipe.put(first_frame[i], block=False)
+
+        fw.step()
+        self.assertEqual(self.upload_calls, 1)
+        self.assertEqual(self.timeout_calls, 2)
+
+    @mock.patch('logfire.flusher._calculate_time_remaining')
+    @mock.patch('logfire.flusher._initial_time_remaining')
+    def test_does_nothing_without_any_items(self, initial_time_remaining, calculate_time_remaining):
+        calculate_time_remaining.side_effect = lambda a,b: 0.0
+        initial_time_remaining.side_effect = lambda a: 0.0001
+
+        uploader = mock.MagicMock(side_effect=mock.MagicMock(status_code=202))
+        pipe, _, fw = self._setup_worker(uploader)
+
+        self.assertEqual(pipe.qsize(), 0)
+        fw.step()
+        self.assertFalse(uploader.called)
+
+    @mock.patch('logfire.flusher.time.sleep')
+    def test_retries_according_to_schedule(self, mock_sleep):
+        first_frame = list(range(self.buffer_capacity))
+
+        self.uploader_calls = 0
+        def uploader(frame):
+            self.uploader_calls += 1
+            self.assertEqual(frame, first_frame)
+            return mock.MagicMock(status_code=500)
+
+        self.sleep_calls = 0
+        def sleep(time):
+            self.assertEqual(time, RETRY_SCHEDULE[self.sleep_calls])
+            self.sleep_calls += 1
+        mock_sleep.side_effect = sleep
+
+        pipe, _, fw = self._setup_worker(uploader)
+
+        for log in first_frame:
+            pipe.put(log, block=False)
+
+        fw.step()
+        self.assertEqual(self.uploader_calls, len(RETRY_SCHEDULE) + 1)
+        self.assertEqual(self.sleep_calls, len(RETRY_SCHEDULE))
+
+    @mock.patch('logfire.flusher.sys.exit')
+    def test_shutdown_condition_empties_queue_and_calls_exit(self, mock_exit):
+        self.buffer_capacity = 10
+        num_items = 5
+        first_frame = list(range(self.buffer_capacity))
+        self.assertLess(num_items, self.buffer_capacity)
+
+        self.upload_calls = 0
+        def uploader(frame):
+            self.upload_calls += 1
+            self.assertEqual(frame, first_frame[:num_items])
+            return mock.MagicMock(status_code=202)
+
+        pipe, _, fw = self._setup_worker(uploader)
+        fw.parent_thread = mock.MagicMock(is_alive=lambda: False)
+
+        for i in range(num_items):
+            pipe.put(first_frame[i], block=False)
+
+        fw.step()
+        self.assertEqual(self.upload_calls, 1)
+        self.assertEqual(mock_exit.call_count, 1)
```

### Comparing `logfire-python-0.0.8/tests/test_formatter.py` & `logfire_python-0.0.9/tests/test_formatter.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,135 +1,135 @@
-# coding: utf-8
-import mock
-import time
-import threading
-import json
-import unittest2
-import pdb
-import logging
-
-import logfire
-from logfire.formatter import LogfireFormatter
-from logfire.helpers import LogfireContext
-
-
-class TestLogfireFormatter(unittest2.TestCase):
-    def setUp(self):
-        self.context = LogfireContext()
-        self.customer = {'id': '1'}
-        self.order = {'id': '1234', 'amount': 200, 'item': '#19849'}
-
-    def _check_and_get_line(self, loglines):
-        self.assertEqual(len(loglines), 1)
-        return loglines[0]
-
-    def test_format_emits_single_line(self):
-        formatter = logfire.LogfireFormatter(context=self.context)
-        logger, loglines = logger_and_lines(formatter)
-        self.assertFalse(loglines)
-
-        logger.info('Hello\n\n\n\n\n\nWorld')
-        line = self._check_and_get_line(loglines)
-        self.assertEqual(len(line.split('\n')), 1)
-
-    def test_format_creates_json_serialized_frame_with_context(self):
-        formatter = logfire.LogfireFormatter(context=self.context)
-        logger, loglines = logger_and_lines(formatter)
-        self.assertFalse(loglines)
-
-        with self.context(customer=self.customer):
-            logger.info('Received order id=%s', self.order['id'], extra={'order': self.order})
-
-        line = self._check_and_get_line(loglines)
-        frame = json.loads(line)
-        self.assertEqual(frame['message'], 'Received order id=%s' % self.order['id'])
-        self.assertEqual(frame['order'], self.order)
-        self.assertEqual(frame['context']['customer'], self.customer)
-
-    def test_format_collapses_context(self):
-        formatter = logfire.LogfireFormatter(context=self.context)
-        logger, loglines = logger_and_lines(formatter)
-        self.assertFalse(loglines)
-
-        with self.context(customer=self.customer):
-            with self.context(customer={'trusted': True}):
-                logger.info('Received an order', extra={'order': self.order})
-
-        line = self._check_and_get_line(loglines)
-        frame = json.loads(line)
-        self.assertEqual(frame['message'], 'Received an order')
-        self.assertEqual(frame['order'], self.order)
-        self.assertEqual(frame['context']['customer'], {'id': self.customer['id'], 'trusted': True})
-
-    def test_format_with_custom_default_json_serializer(self):
-        def suppress_encoding_errors(obj):
-            return 'Could not encode type=%s' % type(obj).__name__
-
-        default_formatter = logfire.LogfireFormatter(context=self.context)
-        default_logger, _ = logger_and_lines(default_formatter, 'default')
-
-        suppress_formatter = logfire.LogfireFormatter(context=self.context, json_default=suppress_encoding_errors)
-        suppress_logger, loglines = logger_and_lines(suppress_formatter, 'suppress')
-
-        self.assertIsNot(default_logger, suppress_logger)
-
-        with self.context(data={'not_encodable': Dummy()}):
-            with self.assertRaises(TypeError):
-                default_logger.info('hello')
-            suppress_logger.info('goodbye')
-
-        line = self._check_and_get_line(loglines)
-        frame = json.loads(line)
-        self.assertEqual(frame['message'], 'goodbye')
-        self.assertEqual(frame['context']['data'], {'not_encodable': 'Could not encode type=Dummy'})
-
-    def test_format_with_custom_default_json_encoder(self):
-        default_formatter = logfire.LogfireFormatter(context=self.context)
-        default_logger, _ = logger_and_lines(default_formatter, 'default')
-
-        dummy_capable_formatter = logfire.LogfireFormatter(context=self.context, json_encoder=DummyCapableEncoder)
-        dummy_capable_logger, loglines = logger_and_lines(dummy_capable_formatter, 'dummy_capable')
-
-        self.assertIsNot(default_logger, dummy_capable_logger)
-
-        with self.context(data={'not_encodable': Dummy()}):
-            with self.assertRaises(TypeError):
-                default_logger.info('hello')
-            dummy_capable_logger.info('goodbye')
-
-        line = self._check_and_get_line(loglines)
-        frame = json.loads(line)
-        self.assertEqual(frame['message'], 'goodbye')
-        self.assertEqual(frame['context']['data'], {'not_encodable': '<Dummy instance>'})
-
-
-class Dummy(object):
-    """ Because this is a custom class, it cannot be encoded by the default JSONEncoder. """
-
-
-class DummyCapableEncoder(json.JSONEncoder):
-    """ A JSONEncoder that can encode instances of the Dummy class. """
-    def default(self, obj):
-        if isinstance(obj, Dummy):
-            return '<Dummy instance>'
-        return super(CustomEncoder, self).default(obj)
-
-
-class ListHandler(logging.Handler):
-    """ Accumulates all log lines in a list for testing purposes. """
-    def __init__(self, *args, **kwargs):
-        super(ListHandler, self).__init__(*args, **kwargs)
-        self.lines = []
-
-    def emit(self, record):
-        logline = self.format(record)
-        self.lines.append(logline)
-
-def logger_and_lines(formatter, name=__name__):
-    """ Helper for more easily writing formatter tests. """
-    logger = logging.getLogger(name)
-    logger.setLevel(logging.DEBUG)
-    logger.handlers = []
-    handler = ListHandler()
-    handler.setFormatter(formatter)
-    logger.addHandler(handler)
-    return logger, handler.lines
+# coding: utf-8
+import mock
+import time
+import threading
+import json
+import unittest2
+import pdb
+import logging
+
+import logfire
+from logfire.formatter import LogfireFormatter
+from logfire.helpers import LogfireContext
+
+
+class TestLogfireFormatter(unittest2.TestCase):
+    def setUp(self):
+        self.context = LogfireContext()
+        self.customer = {'id': '1'}
+        self.order = {'id': '1234', 'amount': 200, 'item': '#19849'}
+
+    def _check_and_get_line(self, loglines):
+        self.assertEqual(len(loglines), 1)
+        return loglines[0]
+
+    def test_format_emits_single_line(self):
+        formatter = logfire.LogfireFormatter(context=self.context)
+        logger, loglines = logger_and_lines(formatter)
+        self.assertFalse(loglines)
+
+        logger.info('Hello\n\n\n\n\n\nWorld')
+        line = self._check_and_get_line(loglines)
+        self.assertEqual(len(line.split('\n')), 1)
+
+    def test_format_creates_json_serialized_frame_with_context(self):
+        formatter = logfire.LogfireFormatter(context=self.context)
+        logger, loglines = logger_and_lines(formatter)
+        self.assertFalse(loglines)
+
+        with self.context(customer=self.customer):
+            logger.info('Received order id=%s', self.order['id'], extra={'order': self.order})
+
+        line = self._check_and_get_line(loglines)
+        frame = json.loads(line)
+        self.assertEqual(frame['message'], 'Received order id=%s' % self.order['id'])
+        self.assertEqual(frame['order'], self.order)
+        self.assertEqual(frame['context']['customer'], self.customer)
+
+    def test_format_collapses_context(self):
+        formatter = logfire.LogfireFormatter(context=self.context)
+        logger, loglines = logger_and_lines(formatter)
+        self.assertFalse(loglines)
+
+        with self.context(customer=self.customer):
+            with self.context(customer={'trusted': True}):
+                logger.info('Received an order', extra={'order': self.order})
+
+        line = self._check_and_get_line(loglines)
+        frame = json.loads(line)
+        self.assertEqual(frame['message'], 'Received an order')
+        self.assertEqual(frame['order'], self.order)
+        self.assertEqual(frame['context']['customer'], {'id': self.customer['id'], 'trusted': True})
+
+    def test_format_with_custom_default_json_serializer(self):
+        def suppress_encoding_errors(obj):
+            return 'Could not encode type=%s' % type(obj).__name__
+
+        default_formatter = logfire.LogfireFormatter(context=self.context)
+        default_logger, _ = logger_and_lines(default_formatter, 'default')
+
+        suppress_formatter = logfire.LogfireFormatter(context=self.context, json_default=suppress_encoding_errors)
+        suppress_logger, loglines = logger_and_lines(suppress_formatter, 'suppress')
+
+        self.assertIsNot(default_logger, suppress_logger)
+
+        with self.context(data={'not_encodable': Dummy()}):
+            with self.assertRaises(TypeError):
+                default_logger.info('hello')
+            suppress_logger.info('goodbye')
+
+        line = self._check_and_get_line(loglines)
+        frame = json.loads(line)
+        self.assertEqual(frame['message'], 'goodbye')
+        self.assertEqual(frame['context']['data'], {'not_encodable': 'Could not encode type=Dummy'})
+
+    def test_format_with_custom_default_json_encoder(self):
+        default_formatter = logfire.LogfireFormatter(context=self.context)
+        default_logger, _ = logger_and_lines(default_formatter, 'default')
+
+        dummy_capable_formatter = logfire.LogfireFormatter(context=self.context, json_encoder=DummyCapableEncoder)
+        dummy_capable_logger, loglines = logger_and_lines(dummy_capable_formatter, 'dummy_capable')
+
+        self.assertIsNot(default_logger, dummy_capable_logger)
+
+        with self.context(data={'not_encodable': Dummy()}):
+            with self.assertRaises(TypeError):
+                default_logger.info('hello')
+            dummy_capable_logger.info('goodbye')
+
+        line = self._check_and_get_line(loglines)
+        frame = json.loads(line)
+        self.assertEqual(frame['message'], 'goodbye')
+        self.assertEqual(frame['context']['data'], {'not_encodable': '<Dummy instance>'})
+
+
+class Dummy(object):
+    """ Because this is a custom class, it cannot be encoded by the default JSONEncoder. """
+
+
+class DummyCapableEncoder(json.JSONEncoder):
+    """ A JSONEncoder that can encode instances of the Dummy class. """
+    def default(self, obj):
+        if isinstance(obj, Dummy):
+            return '<Dummy instance>'
+        return super(CustomEncoder, self).default(obj)
+
+
+class ListHandler(logging.Handler):
+    """ Accumulates all log lines in a list for testing purposes. """
+    def __init__(self, *args, **kwargs):
+        super(ListHandler, self).__init__(*args, **kwargs)
+        self.lines = []
+
+    def emit(self, record):
+        logline = self.format(record)
+        self.lines.append(logline)
+
+def logger_and_lines(formatter, name=__name__):
+    """ Helper for more easily writing formatter tests. """
+    logger = logging.getLogger(name)
+    logger.setLevel(logging.DEBUG)
+    logger.handlers = []
+    handler = ListHandler()
+    handler.setFormatter(formatter)
+    logger.addHandler(handler)
+    return logger, handler.lines
```

### Comparing `logfire-python-0.0.8/tests/test_handler.py` & `logfire_python-0.0.9/tests/test_handler.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-# coding: utf-8
-from __future__ import print_function, unicode_literals
-import mock
-import time
-import threading
-import unittest2
-import logging
-
-from logfire.handler import LogfireHandler
-
-
-class TestLogfireHandler(unittest2.TestCase):
-    source_token = 'dummy_source_token'
-    host = 'dummy_host'
-
-    @mock.patch('logfire.handler.FlushWorker')
-    def test_handler_creates_uploader_from_args(self, MockWorker):
-        handler = LogfireHandler(source_token=self.source_token, host=self.host)
-        self.assertEqual(handler.uploader.source_token, self.source_token)
-        self.assertEqual(handler.uploader.host, self.host)
-
-    @mock.patch('logfire.handler.FlushWorker')
-    def test_handler_creates_pipe_from_args(self, MockWorker):
-        buffer_capacity = 9
-        flush_interval = 1
-        handler = LogfireHandler(
-            source_token=self.source_token,
-            buffer_capacity=buffer_capacity,
-            flush_interval=flush_interval
-        )
-        self.assertEqual(handler.pipe._maxsize, buffer_capacity)
-
-    @mock.patch('logfire.handler.FlushWorker')
-    def test_handler_creates_and_starts_worker_from_args(self, MockWorker):
-        buffer_capacity = 9
-        flush_interval = 9
-        handler = LogfireHandler(source_token=self.source_token, buffer_capacity=buffer_capacity, flush_interval=flush_interval)
-        MockWorker.assert_called_with(
-            handler.uploader,
-            handler.pipe,
-            buffer_capacity,
-            flush_interval
-        )
-        self.assertTrue(handler.flush_thread.start.called)
-
-    @mock.patch('logfire.handler.FlushWorker')
-    def test_emit_starts_thread_if_not_alive(self, MockWorker):
-        handler = LogfireHandler(source_token=self.source_token)
-        self.assertTrue(handler.flush_thread.start.call_count, 1)
-        handler.flush_thread.is_alive = mock.Mock(return_value=False)
-
-        logger = logging.getLogger(__name__)
-        logger.handlers = []
-        logger.addHandler(handler)
-        logger.critical('hello')
-
-        self.assertEqual(handler.flush_thread.start.call_count, 2)
-
-    @mock.patch('logfire.handler.FlushWorker')
-    def test_emit_drops_records_if_configured(self, MockWorker):
-        buffer_capacity = 1
-        handler = LogfireHandler(
-            source_token=self.source_token,
-            buffer_capacity=buffer_capacity,
-            drop_extra_events=True
-        )
-
-        logger = logging.getLogger(__name__)
-        logger.handlers = []
-        logger.addHandler(handler)
-        logger.critical('hello')
-        logger.critical('goodbye')
-
-        log_entry = handler.pipe.get()
-        self.assertEqual(log_entry['message'], 'hello')
-        self.assertTrue(handler.pipe.empty())
-        self.assertEqual(handler.dropcount, 1)
-
-    @mock.patch('logfire.handler.FlushWorker')
-    def test_emit_does_not_drop_records_if_configured(self, MockWorker):
-        buffer_capacity = 1
-        handler = LogfireHandler(
-            source_token=self.source_token,
-            buffer_capacity=buffer_capacity,
-            drop_extra_events=False
-        )
-
-        def consumer(q):
-            while True:
-                if q.full():
-                    while not q.empty():
-                        _ = q.get(block=True)
-                time.sleep(.2)
-
-        t = threading.Thread(target=consumer, args=(handler.pipe,))
-        t.daemon = True
-
-        logger = logging.getLogger(__name__)
-        logger.handlers = []
-        logger.addHandler(handler)
-        logger.critical('hello')
-
-        self.assertTrue(handler.pipe.full())
-        t.start()
-        logger.critical('goodbye')
-        logger.critical('goodbye2')
-
-        self.assertEqual(handler.dropcount, 0)
-
-    @mock.patch('logfire.handler.FlushWorker')
-    def test_error_suppression(self, MockWorker):
-        buffer_capacity = 1
-        handler = LogfireHandler(
-            source_token=self.source_token,
-            buffer_capacity=buffer_capacity,
-            raise_exceptions=True
-        )
-
-        handler.pipe = mock.MagicMock(put=mock.Mock(side_effect=ValueError))
-
-        logger = logging.getLogger(__name__)
-        logger.handlers = []
-        logger.addHandler(handler)
-
-        with self.assertRaises(ValueError):
-            logger.critical('hello')
-
-        handler.raise_exceptions = False
-        logger.critical('hello')
+# coding: utf-8
+from __future__ import print_function, unicode_literals
+import mock
+import time
+import threading
+import unittest2
+import logging
+
+from logfire.handler import LogfireHandler
+
+
+class TestLogfireHandler(unittest2.TestCase):
+    source_token = 'dummy_source_token'
+    host = 'dummy_host'
+
+    @mock.patch('logfire.handler.FlushWorker')
+    def test_handler_creates_uploader_from_args(self, MockWorker):
+        handler = LogfireHandler(source_token=self.source_token, host=self.host)
+        self.assertEqual(handler.uploader.source_token, self.source_token)
+        self.assertEqual(handler.uploader.host, self.host)
+
+    @mock.patch('logfire.handler.FlushWorker')
+    def test_handler_creates_pipe_from_args(self, MockWorker):
+        buffer_capacity = 9
+        flush_interval = 1
+        handler = LogfireHandler(
+            source_token=self.source_token,
+            buffer_capacity=buffer_capacity,
+            flush_interval=flush_interval
+        )
+        self.assertEqual(handler.pipe._maxsize, buffer_capacity)
+
+    @mock.patch('logfire.handler.FlushWorker')
+    def test_handler_creates_and_starts_worker_from_args(self, MockWorker):
+        buffer_capacity = 9
+        flush_interval = 9
+        handler = LogfireHandler(source_token=self.source_token, buffer_capacity=buffer_capacity, flush_interval=flush_interval)
+        MockWorker.assert_called_with(
+            handler.uploader,
+            handler.pipe,
+            buffer_capacity,
+            flush_interval
+        )
+        self.assertTrue(handler.flush_thread.start.called)
+
+    @mock.patch('logfire.handler.FlushWorker')
+    def test_emit_starts_thread_if_not_alive(self, MockWorker):
+        handler = LogfireHandler(source_token=self.source_token)
+        self.assertTrue(handler.flush_thread.start.call_count, 1)
+        handler.flush_thread.is_alive = mock.Mock(return_value=False)
+
+        logger = logging.getLogger(__name__)
+        logger.handlers = []
+        logger.addHandler(handler)
+        logger.critical('hello')
+
+        self.assertEqual(handler.flush_thread.start.call_count, 2)
+
+    @mock.patch('logfire.handler.FlushWorker')
+    def test_emit_drops_records_if_configured(self, MockWorker):
+        buffer_capacity = 1
+        handler = LogfireHandler(
+            source_token=self.source_token,
+            buffer_capacity=buffer_capacity,
+            drop_extra_events=True
+        )
+
+        logger = logging.getLogger(__name__)
+        logger.handlers = []
+        logger.addHandler(handler)
+        logger.critical('hello')
+        logger.critical('goodbye')
+
+        log_entry = handler.pipe.get()
+        self.assertEqual(log_entry['message'], 'hello')
+        self.assertTrue(handler.pipe.empty())
+        self.assertEqual(handler.dropcount, 1)
+
+    @mock.patch('logfire.handler.FlushWorker')
+    def test_emit_does_not_drop_records_if_configured(self, MockWorker):
+        buffer_capacity = 1
+        handler = LogfireHandler(
+            source_token=self.source_token,
+            buffer_capacity=buffer_capacity,
+            drop_extra_events=False
+        )
+
+        def consumer(q):
+            while True:
+                if q.full():
+                    while not q.empty():
+                        _ = q.get(block=True)
+                time.sleep(.2)
+
+        t = threading.Thread(target=consumer, args=(handler.pipe,))
+        t.daemon = True
+
+        logger = logging.getLogger(__name__)
+        logger.handlers = []
+        logger.addHandler(handler)
+        logger.critical('hello')
+
+        self.assertTrue(handler.pipe.full())
+        t.start()
+        logger.critical('goodbye')
+        logger.critical('goodbye2')
+
+        self.assertEqual(handler.dropcount, 0)
+
+    @mock.patch('logfire.handler.FlushWorker')
+    def test_error_suppression(self, MockWorker):
+        buffer_capacity = 1
+        handler = LogfireHandler(
+            source_token=self.source_token,
+            buffer_capacity=buffer_capacity,
+            raise_exceptions=True
+        )
+
+        handler.pipe = mock.MagicMock(put=mock.Mock(side_effect=ValueError))
+
+        logger = logging.getLogger(__name__)
+        logger.handlers = []
+        logger.addHandler(handler)
+
+        with self.assertRaises(ValueError):
+            logger.critical('hello')
+
+        handler.raise_exceptions = False
+        logger.critical('hello')
```

### Comparing `logfire-python-0.0.8/tests/test_helpers.py` & `logfire_python-0.0.9/tests/test_helpers.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-# coding: utf-8
-from __future__ import print_function, unicode_literals
-import unittest2
-
-from logfire import LogfireContext
-
-
-class TestLogfireContext(unittest2.TestCase):
-
-    def test_exists(self):
-        c = LogfireContext()
-        self.assertFalse(c.exists())
-        with c(user={'name': 'a'}):
-            self.assertTrue(c.exists())
-        self.assertFalse(c.exists())
-
-    def test_only_accepts_keyword_argument_dicts(self):
-        c = LogfireContext()
-        # Named context passes
-        c(user={'name': 'a'})
-        # Non-named contexts fail, even if they're dicts
-        for garbage in ['x', 1, [{'name': 'a'}], {'name': 'a'}]:
-            with self.assertRaises(ValueError):
-                c(garbage)
-        # Named contexts fail if they are not dicts
-        for garbage in [{'user': 1}, {'user': []}, {'user': tuple()}]:
-            with self.assertRaises(ValueError):
-                c(**garbage)
-
-    def test_does_not_suppress_exceptions(self):
-        c = LogfireContext()
-        with self.assertRaises(ValueError):
-            with c(user={'name': 'a'}):
-                raise ValueError('should be thrown')
-
-    def test_nested_collapse(self):
-        c = LogfireContext()
-        self.assertEqual(c.collapse(), {})
-
-        with c(user={'name': 'a', 'count': 1}):
-            self.assertEqual(
-                c.collapse(),
-                {'user': {'name': 'a', 'count': 1}}
-            )
-
-            with c(user={'name': 'b'}, other={'foo': 'bar'}):
-                self.assertEqual(
-                    c.collapse(),
-                    {'user': {'name': 'b', 'count': 1},
-                     'other': {'foo': 'bar'}}
-                )
-
-            self.assertEqual(
-                c.collapse(),
-                {'user': {'name': 'a', 'count': 1}}
-            )
-
-        self.assertEqual(c.collapse(), {})
+# coding: utf-8
+from __future__ import print_function, unicode_literals
+import unittest2
+
+from logfire import LogfireContext
+
+
+class TestLogfireContext(unittest2.TestCase):
+
+    def test_exists(self):
+        c = LogfireContext()
+        self.assertFalse(c.exists())
+        with c(user={'name': 'a'}):
+            self.assertTrue(c.exists())
+        self.assertFalse(c.exists())
+
+    def test_only_accepts_keyword_argument_dicts(self):
+        c = LogfireContext()
+        # Named context passes
+        c(user={'name': 'a'})
+        # Non-named contexts fail, even if they're dicts
+        for garbage in ['x', 1, [{'name': 'a'}], {'name': 'a'}]:
+            with self.assertRaises(ValueError):
+                c(garbage)
+        # Named contexts fail if they are not dicts
+        for garbage in [{'user': 1}, {'user': []}, {'user': tuple()}]:
+            with self.assertRaises(ValueError):
+                c(**garbage)
+
+    def test_does_not_suppress_exceptions(self):
+        c = LogfireContext()
+        with self.assertRaises(ValueError):
+            with c(user={'name': 'a'}):
+                raise ValueError('should be thrown')
+
+    def test_nested_collapse(self):
+        c = LogfireContext()
+        self.assertEqual(c.collapse(), {})
+
+        with c(user={'name': 'a', 'count': 1}):
+            self.assertEqual(
+                c.collapse(),
+                {'user': {'name': 'a', 'count': 1}}
+            )
+
+            with c(user={'name': 'b'}, other={'foo': 'bar'}):
+                self.assertEqual(
+                    c.collapse(),
+                    {'user': {'name': 'b', 'count': 1},
+                     'other': {'foo': 'bar'}}
+                )
+
+            self.assertEqual(
+                c.collapse(),
+                {'user': {'name': 'a', 'count': 1}}
+            )
+
+        self.assertEqual(c.collapse(), {})
```

### Comparing `logfire-python-0.0.8/tests/test_uploader.py` & `logfire_python-0.0.9/tests/test_uploader.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# coding: utf-8
-from __future__ import print_function, unicode_literals
-import msgpack
-import mock
-import unittest2
-
-from logfire.uploader import Uploader
-
-
-class TestUploader(unittest2.TestCase):
-    host = 'https://in.logfire.com'
-    source_token = 'dummy_source_token'
-    frame = [1, 2, 3]
-
-    @mock.patch('logfire.uploader.requests.Session.post')
-    def test_call(self, post):
-        def mock_post(endpoint, data=None, headers=None):
-            # Check that the data is sent to ther correct endpoint
-            self.assertEqual(endpoint, self.host)
-            # Check the content-type
-            self.assertIsInstance(headers, dict)
-            self.assertIn('Authorization', headers)
-            self.assertEqual('application/msgpack', headers.get('Content-Type'))
-            # Check the content was msgpacked correctly
-            self.assertEqual(msgpack.unpackb(data, raw=False), self.frame)
-
-        post.side_effect = mock_post
-        u = Uploader(self.source_token, self.host)
-        u(self.frame)
-
-        self.assertTrue(post.called)
+# coding: utf-8
+from __future__ import print_function, unicode_literals
+import msgpack
+import mock
+import unittest2
+
+from logfire.uploader import Uploader
+
+
+class TestUploader(unittest2.TestCase):
+    host = 'https://in.logfire.com'
+    source_token = 'dummy_source_token'
+    frame = [1, 2, 3]
+
+    @mock.patch('logfire.uploader.requests.Session.post')
+    def test_call(self, post):
+        def mock_post(endpoint, data=None, headers=None):
+            # Check that the data is sent to ther correct endpoint
+            self.assertEqual(endpoint, self.host)
+            # Check the content-type
+            self.assertIsInstance(headers, dict)
+            self.assertIn('Authorization', headers)
+            self.assertEqual('application/msgpack', headers.get('Content-Type'))
+            # Check the content was msgpacked correctly
+            self.assertEqual(msgpack.unpackb(data, raw=False), self.frame)
+
+        post.side_effect = mock_post
+        u = Uploader(self.source_token, self.host)
+        u(self.frame)
+
+        self.assertTrue(post.called)
```

