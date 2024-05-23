# Comparing `tmp/django_xlsx_serializer-0.3.0.tar.gz` & `tmp/django_xlsx_serializer-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_xlsx_serializer-0.3.0.tar", last modified: Tue May 21 21:07:21 2024, max compression
+gzip compressed data, was "django_xlsx_serializer-1.0.0.tar", last modified: Thu May 23 16:52:20 2024, max compression
```

## Comparing `django_xlsx_serializer-0.3.0.tar` & `django_xlsx_serializer-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:07:21.329388 django_xlsx_serializer-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-21 21:07:07.000000 django_xlsx_serializer-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14624 2024-05-21 21:07:21.329388 django_xlsx_serializer-0.3.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:07:21.325388 django_xlsx_serializer-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)    12555 2024-05-21 21:07:07.000000 django_xlsx_serializer-0.3.0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-21 21:07:07.000000 django_xlsx_serializer-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 21:07:21.329388 django_xlsx_serializer-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:07:21.325388 django_xlsx_serializer-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:07:21.329388 django_xlsx_serializer-0.3.0/src/django_xlsx_serializer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14624 2024-05-21 21:07:21.000000 django_xlsx_serializer-0.3.0/src/django_xlsx_serializer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-21 21:07:21.000000 django_xlsx_serializer-0.3.0/src/django_xlsx_serializer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 21:07:21.000000 django_xlsx_serializer-0.3.0/src/django_xlsx_serializer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-21 21:07:21.000000 django_xlsx_serializer-0.3.0/src/django_xlsx_serializer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-21 21:07:21.000000 django_xlsx_serializer-0.3.0/src/django_xlsx_serializer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:07:21.329388 django_xlsx_serializer-0.3.0/src/xlsx_serializer/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-21 21:07:07.000000 django_xlsx_serializer-0.3.0/src/xlsx_serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-21 21:07:07.000000 django_xlsx_serializer-0.3.0/src/xlsx_serializer/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    15106 2024-05-21 21:07:07.000000 django_xlsx_serializer-0.3.0/src/xlsx_serializer/core.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 21:07:07.000000 django_xlsx_serializer-0.3.0/src/xlsx_serializer/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:52:20.261709 django_xlsx_serializer-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-23 16:52:13.000000 django_xlsx_serializer-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13182 2024-05-23 16:52:20.257709 django_xlsx_serializer-1.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:52:20.257709 django_xlsx_serializer-1.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    11241 2024-05-23 16:52:13.000000 django_xlsx_serializer-1.0.0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-23 16:52:13.000000 django_xlsx_serializer-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 16:52:20.261709 django_xlsx_serializer-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:52:20.253709 django_xlsx_serializer-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:52:20.257709 django_xlsx_serializer-1.0.0/src/django_xlsx_serializer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13182 2024-05-23 16:52:20.000000 django_xlsx_serializer-1.0.0/src/django_xlsx_serializer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-23 16:52:20.000000 django_xlsx_serializer-1.0.0/src/django_xlsx_serializer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 16:52:20.000000 django_xlsx_serializer-1.0.0/src/django_xlsx_serializer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-23 16:52:20.000000 django_xlsx_serializer-1.0.0/src/django_xlsx_serializer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-23 16:52:20.000000 django_xlsx_serializer-1.0.0/src/django_xlsx_serializer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:52:20.257709 django_xlsx_serializer-1.0.0/src/xlsx_serializer/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-23 16:52:13.000000 django_xlsx_serializer-1.0.0/src/xlsx_serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-23 16:52:13.000000 django_xlsx_serializer-1.0.0/src/xlsx_serializer/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14906 2024-05-23 16:52:13.000000 django_xlsx_serializer-1.0.0/src/xlsx_serializer/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:52:13.000000 django_xlsx_serializer-1.0.0/src/xlsx_serializer/py.typed
```

### Comparing `django_xlsx_serializer-0.3.0/LICENSE` & `django_xlsx_serializer-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_xlsx_serializer-0.3.0/PKG-INFO` & `django_xlsx_serializer-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: django-xlsx-serializer
-Version: 0.3.0
+Version: 1.0.0
 Summary: Load/dump Django models from/to Excel 2007+ workbooks
 Author-email: Kamil Paduszyński <92403542+paduszyk@users.noreply.github.com>
 Project-URL: Repository, https://github.com/paduszyk/django-xlsx-serializer
-Project-URL: Documentation, https://github.com/paduszyk/django-xlsx-serializer#readme
-Project-URL: Issue tracker, https://github.com/paduszyk/django-xlsx-serializer/issues
 Keywords: django,django-application,excel,excel-export,excel-import
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
@@ -28,119 +26,82 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django<5.1,>=3.2
 Requires-Dist: openpyxl<4
 Requires-Dist: typing-extensions<5
 Provides-Extra: dev
+Requires-Dist: commitizen<4; extra == "dev"
 Requires-Dist: django-stubs[compatible-mypy]<6; extra == "dev"
 Requires-Dist: nox; extra == "dev"
 Requires-Dist: pre-commit<4; extra == "dev"
 Requires-Dist: pytest<9; extra == "dev"
 Requires-Dist: pytest-cov<6; extra == "dev"
 Requires-Dist: pytest-django<5; extra == "dev"
 Requires-Dist: pytest-custom-exit-code<1; extra == "dev"
 Requires-Dist: psycopg2-binary<3; extra == "dev"
 Requires-Dist: python-dotenv<2; extra == "dev"
 Requires-Dist: ruff<1; extra == "dev"
 Requires-Dist: types-openpyxl<4; extra == "dev"
 
 # django-xlsx-serializer
 
+[![PyPI: Version](https://img.shields.io/pypi/v/django-xlsx-serializer?style=flat-square&logo=pypi&logoColor=white)][pypi]
+[![PyPI: Python](https://img.shields.io/pypi/pyversions/django-xlsx-serializer?style=flat-square&logo=python&logoColor=white)][pypi]
+[![PyPI: Django](https://img.shields.io/pypi/djversions/django-xlsx-serializer?style=flat-square&color=0C4B33&label=django&logo=django)][pypi]
+[![PyPI: License](https://img.shields.io/pypi/l/django-xlsx-serializer?style=flat-square)][pypi]
+
 [![Pre-commit](https://img.shields.io/github/actions/workflow/status/paduszyk/django-xlsx-serializer/pre-commit-run.yml?style=flat-square&label=pre-commit&logo=pre-commit)][pre-commit]
 [![Python: CI](https://img.shields.io/github/actions/workflow/status/paduszyk/django-xlsx-serializer/python-ci.yml?style=flat-square&logo=github&label=CI)][python-ci]
 [![Codecov](https://img.shields.io/codecov/c/github/paduszyk/django-xlsx-serializer?style=flat-square&logo=codecov)][codecov]
 
 [![Nox](https://img.shields.io/badge/%F0%9F%A6%8A-Nox-D85E00.svg?style=flat-square)][nox]
 [![Ruff](https://img.shields.io/endpoint?style=flat-square&url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)][ruff]
 [![Mypy](https://img.shields.io/badge/type--checked-mypy-blue?style=flat-square&logo=python)][mypy]
 [![Prettier](https://img.shields.io/badge/code%20style-prettier-1E2B33?style=flat-square&logo=Prettier)][prettier]
 [![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-fa6673.svg?style=flat-square&logo=conventional-commits)][conventional-commits]
 
-## Table of Contents
-
-- [Overview](#overview)
-- [Features](#features)
-- [Requirements](#requirements)
-- [Prerequisites](#prerequisites)
-- [Installation](#installation)
-- [Django Configuration](#django-configuration)
-  - [Install as an App](#install-as-an-app)
-  - [Add to Serialization Modules](#add-to-serialization-modules)
-  - [Register from Another App](#register-from-another-app)
-- [Usage](#usage)
-  - [Excel Workbooks vs. Django Models](#excel-workbooks-vs-django-models)
-  - [Serialization](#serialization)
-  - [Deserialization](#deserialization)
-- [Contributing](#contributing)
-- [Authors](#authors)
-- [License](#license)
-
 ## Overview
 
 `django-xlsx-serializer` is a [Django][django] application designed to handle
 the data serialization and deserialization between Django models and Microsoft
 Excel 2007+ workbooks. Utilizing the [OpenPyXL][openpyxl] engine, this tool
-provides robust methods to export data from Django databases into XLSX files
-and import data from the files back into the databases. This functionality is
+provides robust methods to export data from Django databases into XLSX files and
+import data from the files back into the databases. This functionality is
 essential for applications that require data exchange between Django-based
 systems and Excel, facilitating such tasks as data migration, reporting, and
 backups.
 
 ## Features
 
-The app enables:
+The app allows you to:
 
-- Exporting Django models from a database to an Excel workbook via the
+- Export Django models from a database to an Excel workbook via the
   [`dumpdata`][django-dumpdata] command.
-- Populating databases from Excel fixtures using the [`loaddata`][django-loaddata]
+- Populate databases from Excel fixtures using the [`loaddata`][django-loaddata]
   command.
-- Interacting with Excel workbooks (either files or `openpyxl.Workbook` objects)
-  and the database using the [serialization][django-serialization] utilities
-  from `django.core.serializers`.
-
-Both serialization and deserialization were tested for all the available Django
-model fields except:
-
-- `BinaryField`
-- `GeneratedField`
-
-Pull requests introducing the support for those fields are welcome; see
-the [Contributing](#contributing) section for further details.
+- Interact with Excel workbooks (either files or `openpyxl.Workbook` objects)
+  and the database using the Django's core [serialization][django-serialization]
+  utilities.
 
 ## Requirements
 
 | Python | Django                  | Database engines    |
 | :----- | :---------------------- | :------------------ |
 | 3.9    | 3.2, 4.0, 4.1, 4.2      | SQLite3, PostgreSQL |
 | 3.10   | 3.2, 4.0, 4.1, 4.2, 5.0 | SQLite3, PostgreSQL |
 | 3.11   | 4.1, 4.2, 5.0           | SQLite3, PostgreSQL |
 | 3.12   | 4.2, 5.0                | SQLite3, PostgreSQL |
 
-For all Python/Django/database setups, the package additionally requires
-OpenPyXL < 4.
-
-## Prerequisites
-
-This documentation assumes you are familiar with the following Django concepts:
-
-- [Models and fields][django-model-fields]
-- [Management commands][django-commands]
-- [Serialization][django-serialization] and [fixtures][django-fixtures]
-
-If you are unsure about your knowledge of these concepts, it is strongly
-recommended that you review the Django documentation by following the links
-provided above. The official documentation offers detailed explanations and
-examples to help you better understand how this app works and how to use it
-properly.
+All setups require OpenPyXL < 4.
 
 ## Installation
 
-The fastest way to add the package to your Python environment is to download
-and install it directly from [PyPI][pypi]. Use `pip`:
+The fastest way to add the package to your Python environment is to download and
+install it directly from [PyPI][pypi]. Use `pip`:
 
 ```console
 pip install django-xlsx-serializer
 ```
 
 or any other dependency manager of your preference.
 
@@ -157,16 +118,15 @@
 ## Django Configuration
 
 The app utilities can be incorporated into your Django project by following one
 of the approaches listed below:
 
 1. Installing the package as an app.
 2. Adding the package to serialization modules.
-3. Registering the app's serializers module in the configuration class of
-   another app installed in the project.
+3. Registering the app's serializers module from another app.
 
 All of them associate the app's serializer with the `xlsx` format.
 
 ### Install as an App
 
 In your project settings module add `xlsx_serializers` to `INSTALLED_APPS`:
 
@@ -218,15 +178,15 @@
 > utilities (e.g., custom commands, template tags, etc.). The configuration
 > class of such an app is a good place to apply the code snippet above.
 
 ## Usage
 
 ### Excel Workbooks vs. Django Models
 
-The app adopts the following correspondence between Excel workbooks (i.e., the
+The app adopts quite intuitive correspondence between Excel workbooks (i.e., the
 collections of worksheets) and Django models:
 
 - A Django model is represented by a single worksheet.
 - In an Excel workbook, the models are identified by worksheet names.
 - Within an Excel worksheet, model instances are represented by rows, while the
   columns correspond to the model's fields.
 
@@ -245,16 +205,16 @@
 >>> from django.core import serializers
 >>> from polls.models import Question
 >>> serializers.serialize("xlsx", Question.objects.all(), output="dump.xlsx")
 # Prints: <openpyxl.workbook.workbook.Workbook object at ...>
 ```
 
 Both the command and expression shown above save `dump.xlsx` workbook file. The
-latter additionally returns an `openpyxl.Workbook` object, which can
-be used later if necessary (e.g., in development or maintenance scripts).
+latter additionally returns an `openpyxl.Workbook` object, which can be used
+later if necessary (e.g., in development or maintenance scripts).
 
 When serializing, the app creates worksheets named using fully qualified model
 labels. For example, the `Question` model defined in the `polls` app is
 serialized to the "polls.Question" worksheet. Excel does not accept worksheet
 names longer than 31 characters. If the model's label is longer, it's truncated.
 A useful feature allowing you to circumvent this issue is that the output
 worksheet names can be customized using the `model_sheet_names` option. So, the
@@ -267,16 +227,16 @@
         model_sheet_names={"polls.Question": "Questions"},
     )
 >>> workbook
 # Prints: <openpyxl.workbook.workbook.Workbook object at ...>
 ```
 
 results in the `polls.Question` model data serialized in the "Questions"
-worksheet. Note that this
-option is not available when using the app via the `dumpdata` command.
+worksheet. Note that this option is not available when using the app via the
+`dumpdata` command.
 
 > The app inspects each key and value of the `model_sheet_names` dictionary. For
 > the keys, it validates whether they represent valid model identifiers. The
 > values, in turn, are checked to see if they are unique, are not too long, and
 > do not contain invalid characters (`?`, `*`, `:`, `\`, `/`, `[`, `]`).
 
 Other key points:
@@ -318,43 +278,40 @@
   enabled in Django settings requires date/time values to be saved as ISO 8601
   strings (date/time type values in Excel don't store timezone information).
 - Deserializing `JSONfield` requires values in a format compatible with the JSON
   decoder of the respective field.
 - In the case of `ManyToManyField` provide string representations of Python
   lists containing the primary (or natural, see the next bullet) keys of the
   related objects.
-- The app supports deserialization from natural keys. Make sure to provide the
-  keys that are valid string representations of the corresponding values (i.e.,
-  tuples of primitive Python literals; in most cases, they are strings &nddash;
-  if so, use single quotes as text delimiters);
+- The app handles deserialization from natural keys by using `ast.literal_eval`.
+  Make sure to provide the keys that are valid string representations of the
+  corresponding values (i.e., tuples of primitive Python literals; in most
+  cases, they are strings &nddash; if so, use single quotes as text delimiters).
 
 ## Contributing
 
-- This is an open-source project that embraces contributions of all types.
-- We require all contributors to adhere to our [Code of Conduct][code-of-conduct].
-- For comprehensive instructions on how to contribute to the project, please
-  refer to our [Contributing Guide][contributing].
+This is an open-source project that embraces contributions of all types. We
+require all contributors to adhere to our [Code of Conduct][code-of-conduct].
+For comprehensive instructions on how to contribute to the project, please refer
+to our [Contributing Guide][contributing].
 
 ## Authors
 
 Created and maintained by Kamil Paduszyński ([@paduszyk][paduszyk]).
 
 ## License
 
 Released under the [MIT license][license].
 
 [code-of-conduct]: https://github.com/paduszyk/django-xlsx-serializer/blob/main/docs/CODE_OF_CONDUCT.md
 [codecov]: https://app.codecov.io/gh/paduszyk/django-xlsx-serializer
 [contributing]: https://github.com/paduszyk/django-xlsx-serializer/blob/main/docs/CONTRIBUTING.md
 [conventional-commits]: https://www.conventionalcommits.org/en/v1.0.0/
-[django-commands]: https://docs.djangoproject.com/en/5.0/ref/django-admin/
 [django-dumpdata]: https://docs.djangoproject.com/en/5.0/ref/django-admin/#dumpdata
-[django-fixtures]: https://docs.djangoproject.com/en/5.0/topics/db/fixtures/
 [django-loaddata]: https://docs.djangoproject.com/en/5.0/ref/django-admin/#loaddata
-[django-model-fields]: https://docs.djangoproject.com/en/5.0/ref/models/fields/
 [django-serialization]: https://docs.djangoproject.com/en/5.0/topics/serialization/
 [django]: https://www.djangoproject.com
 [license]: https://github.com/paduszyk/django-xlsx-serializer/blob/main/LICENSE
 [mypy]: https://mypy.readthedocs.io
 [nox]: https://github.com/wntrblm/nox
 [openpyxl]: https://openpyxl.readthedocs.io/en/stable/
 [paduszyk]: https://github.com/paduszyk
```

### Comparing `django_xlsx_serializer-0.3.0/docs/README.md` & `django_xlsx_serializer-1.0.0/docs/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,100 +1,62 @@
 # django-xlsx-serializer
 
+[![PyPI: Version](https://img.shields.io/pypi/v/django-xlsx-serializer?style=flat-square&logo=pypi&logoColor=white)][pypi]
+[![PyPI: Python](https://img.shields.io/pypi/pyversions/django-xlsx-serializer?style=flat-square&logo=python&logoColor=white)][pypi]
+[![PyPI: Django](https://img.shields.io/pypi/djversions/django-xlsx-serializer?style=flat-square&color=0C4B33&label=django&logo=django)][pypi]
+[![PyPI: License](https://img.shields.io/pypi/l/django-xlsx-serializer?style=flat-square)][pypi]
+
 [![Pre-commit](https://img.shields.io/github/actions/workflow/status/paduszyk/django-xlsx-serializer/pre-commit-run.yml?style=flat-square&label=pre-commit&logo=pre-commit)][pre-commit]
 [![Python: CI](https://img.shields.io/github/actions/workflow/status/paduszyk/django-xlsx-serializer/python-ci.yml?style=flat-square&logo=github&label=CI)][python-ci]
 [![Codecov](https://img.shields.io/codecov/c/github/paduszyk/django-xlsx-serializer?style=flat-square&logo=codecov)][codecov]
 
 [![Nox](https://img.shields.io/badge/%F0%9F%A6%8A-Nox-D85E00.svg?style=flat-square)][nox]
 [![Ruff](https://img.shields.io/endpoint?style=flat-square&url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)][ruff]
 [![Mypy](https://img.shields.io/badge/type--checked-mypy-blue?style=flat-square&logo=python)][mypy]
 [![Prettier](https://img.shields.io/badge/code%20style-prettier-1E2B33?style=flat-square&logo=Prettier)][prettier]
 [![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-fa6673.svg?style=flat-square&logo=conventional-commits)][conventional-commits]
 
-## Table of Contents
-
-- [Overview](#overview)
-- [Features](#features)
-- [Requirements](#requirements)
-- [Prerequisites](#prerequisites)
-- [Installation](#installation)
-- [Django Configuration](#django-configuration)
-  - [Install as an App](#install-as-an-app)
-  - [Add to Serialization Modules](#add-to-serialization-modules)
-  - [Register from Another App](#register-from-another-app)
-- [Usage](#usage)
-  - [Excel Workbooks vs. Django Models](#excel-workbooks-vs-django-models)
-  - [Serialization](#serialization)
-  - [Deserialization](#deserialization)
-- [Contributing](#contributing)
-- [Authors](#authors)
-- [License](#license)
-
 ## Overview
 
 `django-xlsx-serializer` is a [Django][django] application designed to handle
 the data serialization and deserialization between Django models and Microsoft
 Excel 2007+ workbooks. Utilizing the [OpenPyXL][openpyxl] engine, this tool
-provides robust methods to export data from Django databases into XLSX files
-and import data from the files back into the databases. This functionality is
+provides robust methods to export data from Django databases into XLSX files and
+import data from the files back into the databases. This functionality is
 essential for applications that require data exchange between Django-based
 systems and Excel, facilitating such tasks as data migration, reporting, and
 backups.
 
 ## Features
 
-The app enables:
+The app allows you to:
 
-- Exporting Django models from a database to an Excel workbook via the
+- Export Django models from a database to an Excel workbook via the
   [`dumpdata`][django-dumpdata] command.
-- Populating databases from Excel fixtures using the [`loaddata`][django-loaddata]
+- Populate databases from Excel fixtures using the [`loaddata`][django-loaddata]
   command.
-- Interacting with Excel workbooks (either files or `openpyxl.Workbook` objects)
-  and the database using the [serialization][django-serialization] utilities
-  from `django.core.serializers`.
-
-Both serialization and deserialization were tested for all the available Django
-model fields except:
-
-- `BinaryField`
-- `GeneratedField`
-
-Pull requests introducing the support for those fields are welcome; see
-the [Contributing](#contributing) section for further details.
+- Interact with Excel workbooks (either files or `openpyxl.Workbook` objects)
+  and the database using the Django's core [serialization][django-serialization]
+  utilities.
 
 ## Requirements
 
 | Python | Django                  | Database engines    |
 | :----- | :---------------------- | :------------------ |
 | 3.9    | 3.2, 4.0, 4.1, 4.2      | SQLite3, PostgreSQL |
 | 3.10   | 3.2, 4.0, 4.1, 4.2, 5.0 | SQLite3, PostgreSQL |
 | 3.11   | 4.1, 4.2, 5.0           | SQLite3, PostgreSQL |
 | 3.12   | 4.2, 5.0                | SQLite3, PostgreSQL |
 
-For all Python/Django/database setups, the package additionally requires
-OpenPyXL < 4.
-
-## Prerequisites
-
-This documentation assumes you are familiar with the following Django concepts:
-
-- [Models and fields][django-model-fields]
-- [Management commands][django-commands]
-- [Serialization][django-serialization] and [fixtures][django-fixtures]
-
-If you are unsure about your knowledge of these concepts, it is strongly
-recommended that you review the Django documentation by following the links
-provided above. The official documentation offers detailed explanations and
-examples to help you better understand how this app works and how to use it
-properly.
+All setups require OpenPyXL < 4.
 
 ## Installation
 
-The fastest way to add the package to your Python environment is to download
-and install it directly from [PyPI][pypi]. Use `pip`:
+The fastest way to add the package to your Python environment is to download and
+install it directly from [PyPI][pypi]. Use `pip`:
 
 ```console
 pip install django-xlsx-serializer
 ```
 
 or any other dependency manager of your preference.
 
@@ -111,16 +73,15 @@
 ## Django Configuration
 
 The app utilities can be incorporated into your Django project by following one
 of the approaches listed below:
 
 1. Installing the package as an app.
 2. Adding the package to serialization modules.
-3. Registering the app's serializers module in the configuration class of
-   another app installed in the project.
+3. Registering the app's serializers module from another app.
 
 All of them associate the app's serializer with the `xlsx` format.
 
 ### Install as an App
 
 In your project settings module add `xlsx_serializers` to `INSTALLED_APPS`:
 
@@ -172,15 +133,15 @@
 > utilities (e.g., custom commands, template tags, etc.). The configuration
 > class of such an app is a good place to apply the code snippet above.
 
 ## Usage
 
 ### Excel Workbooks vs. Django Models
 
-The app adopts the following correspondence between Excel workbooks (i.e., the
+The app adopts quite intuitive correspondence between Excel workbooks (i.e., the
 collections of worksheets) and Django models:
 
 - A Django model is represented by a single worksheet.
 - In an Excel workbook, the models are identified by worksheet names.
 - Within an Excel worksheet, model instances are represented by rows, while the
   columns correspond to the model's fields.
 
@@ -199,16 +160,16 @@
 >>> from django.core import serializers
 >>> from polls.models import Question
 >>> serializers.serialize("xlsx", Question.objects.all(), output="dump.xlsx")
 # Prints: <openpyxl.workbook.workbook.Workbook object at ...>
 ```
 
 Both the command and expression shown above save `dump.xlsx` workbook file. The
-latter additionally returns an `openpyxl.Workbook` object, which can
-be used later if necessary (e.g., in development or maintenance scripts).
+latter additionally returns an `openpyxl.Workbook` object, which can be used
+later if necessary (e.g., in development or maintenance scripts).
 
 When serializing, the app creates worksheets named using fully qualified model
 labels. For example, the `Question` model defined in the `polls` app is
 serialized to the "polls.Question" worksheet. Excel does not accept worksheet
 names longer than 31 characters. If the model's label is longer, it's truncated.
 A useful feature allowing you to circumvent this issue is that the output
 worksheet names can be customized using the `model_sheet_names` option. So, the
@@ -221,16 +182,16 @@
         model_sheet_names={"polls.Question": "Questions"},
     )
 >>> workbook
 # Prints: <openpyxl.workbook.workbook.Workbook object at ...>
 ```
 
 results in the `polls.Question` model data serialized in the "Questions"
-worksheet. Note that this
-option is not available when using the app via the `dumpdata` command.
+worksheet. Note that this option is not available when using the app via the
+`dumpdata` command.
 
 > The app inspects each key and value of the `model_sheet_names` dictionary. For
 > the keys, it validates whether they represent valid model identifiers. The
 > values, in turn, are checked to see if they are unique, are not too long, and
 > do not contain invalid characters (`?`, `*`, `:`, `\`, `/`, `[`, `]`).
 
 Other key points:
@@ -272,43 +233,40 @@
   enabled in Django settings requires date/time values to be saved as ISO 8601
   strings (date/time type values in Excel don't store timezone information).
 - Deserializing `JSONfield` requires values in a format compatible with the JSON
   decoder of the respective field.
 - In the case of `ManyToManyField` provide string representations of Python
   lists containing the primary (or natural, see the next bullet) keys of the
   related objects.
-- The app supports deserialization from natural keys. Make sure to provide the
-  keys that are valid string representations of the corresponding values (i.e.,
-  tuples of primitive Python literals; in most cases, they are strings &nddash;
-  if so, use single quotes as text delimiters);
+- The app handles deserialization from natural keys by using `ast.literal_eval`.
+  Make sure to provide the keys that are valid string representations of the
+  corresponding values (i.e., tuples of primitive Python literals; in most
+  cases, they are strings &nddash; if so, use single quotes as text delimiters).
 
 ## Contributing
 
-- This is an open-source project that embraces contributions of all types.
-- We require all contributors to adhere to our [Code of Conduct][code-of-conduct].
-- For comprehensive instructions on how to contribute to the project, please
-  refer to our [Contributing Guide][contributing].
+This is an open-source project that embraces contributions of all types. We
+require all contributors to adhere to our [Code of Conduct][code-of-conduct].
+For comprehensive instructions on how to contribute to the project, please refer
+to our [Contributing Guide][contributing].
 
 ## Authors
 
 Created and maintained by Kamil Paduszyński ([@paduszyk][paduszyk]).
 
 ## License
 
 Released under the [MIT license][license].
 
 [code-of-conduct]: https://github.com/paduszyk/django-xlsx-serializer/blob/main/docs/CODE_OF_CONDUCT.md
 [codecov]: https://app.codecov.io/gh/paduszyk/django-xlsx-serializer
 [contributing]: https://github.com/paduszyk/django-xlsx-serializer/blob/main/docs/CONTRIBUTING.md
 [conventional-commits]: https://www.conventionalcommits.org/en/v1.0.0/
-[django-commands]: https://docs.djangoproject.com/en/5.0/ref/django-admin/
 [django-dumpdata]: https://docs.djangoproject.com/en/5.0/ref/django-admin/#dumpdata
-[django-fixtures]: https://docs.djangoproject.com/en/5.0/topics/db/fixtures/
 [django-loaddata]: https://docs.djangoproject.com/en/5.0/ref/django-admin/#loaddata
-[django-model-fields]: https://docs.djangoproject.com/en/5.0/ref/models/fields/
 [django-serialization]: https://docs.djangoproject.com/en/5.0/topics/serialization/
 [django]: https://www.djangoproject.com
 [license]: https://github.com/paduszyk/django-xlsx-serializer/blob/main/LICENSE
 [mypy]: https://mypy.readthedocs.io
 [nox]: https://github.com/wntrblm/nox
 [openpyxl]: https://openpyxl.readthedocs.io/en/stable/
 [paduszyk]: https://github.com/paduszyk
```

### Comparing `django_xlsx_serializer-0.3.0/pyproject.toml` & `django_xlsx_serializer-1.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -45,19 +45,18 @@
   "Programming Language :: Python :: 3.12",
   "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Repository" = "https://github.com/paduszyk/django-xlsx-serializer"
-"Documentation" = "https://github.com/paduszyk/django-xlsx-serializer#readme"
-"Issue tracker" = "https://github.com/paduszyk/django-xlsx-serializer/issues"
 
 [project.optional-dependencies]
 dev = [
+  "commitizen < 4",
   "django-stubs[compatible-mypy] < 6",
   "nox",
   "pre-commit < 4",
   "pytest < 9",
   "pytest-cov < 6",
   "pytest-django < 5",
   "pytest-custom-exit-code < 1",
@@ -74,20 +73,18 @@
 version = { attr = "xlsx_serializer.__version__" }
 
 # Commitizen
 # https://commitizen-tools.github.io/commitizen/config/
 
 [tool.commitizen]
 name = "cz_conventional_commits"
+version = "1.0.0"
 version_files = [
   "src/xlsx_serializer/__init__.py:__version__",
 ]
-version_provider = "scm"
-tag_format = "v$version"
-bump_message = "chore(release): version $current_version → $new_version [skip ci]"
 
 # Ruff
 # https://docs.astral.sh/ruff/configuration/
 # https://docs.astral.sh/ruff/rules/
 # https://docs.astral.sh/ruff/settings/
 
 [tool.ruff]
@@ -189,12 +186,11 @@
 
 [tool.coverage.run]
 source = ["src/"]
 
 [tool.coverage.report]
 exclude_also = [
   "if TYPE_CHECKING:",
-  "raise NotImplementedError",
 ]
 
 [tool.coverage.xml]
 output = "coverage.xml"
```

### Comparing `django_xlsx_serializer-0.3.0/src/django_xlsx_serializer.egg-info/PKG-INFO` & `django_xlsx_serializer-1.0.0/src/django_xlsx_serializer.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: django-xlsx-serializer
-Version: 0.3.0
+Version: 1.0.0
 Summary: Load/dump Django models from/to Excel 2007+ workbooks
 Author-email: Kamil Paduszyński <92403542+paduszyk@users.noreply.github.com>
 Project-URL: Repository, https://github.com/paduszyk/django-xlsx-serializer
-Project-URL: Documentation, https://github.com/paduszyk/django-xlsx-serializer#readme
-Project-URL: Issue tracker, https://github.com/paduszyk/django-xlsx-serializer/issues
 Keywords: django,django-application,excel,excel-export,excel-import
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
@@ -28,119 +26,82 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django<5.1,>=3.2
 Requires-Dist: openpyxl<4
 Requires-Dist: typing-extensions<5
 Provides-Extra: dev
+Requires-Dist: commitizen<4; extra == "dev"
 Requires-Dist: django-stubs[compatible-mypy]<6; extra == "dev"
 Requires-Dist: nox; extra == "dev"
 Requires-Dist: pre-commit<4; extra == "dev"
 Requires-Dist: pytest<9; extra == "dev"
 Requires-Dist: pytest-cov<6; extra == "dev"
 Requires-Dist: pytest-django<5; extra == "dev"
 Requires-Dist: pytest-custom-exit-code<1; extra == "dev"
 Requires-Dist: psycopg2-binary<3; extra == "dev"
 Requires-Dist: python-dotenv<2; extra == "dev"
 Requires-Dist: ruff<1; extra == "dev"
 Requires-Dist: types-openpyxl<4; extra == "dev"
 
 # django-xlsx-serializer
 
+[![PyPI: Version](https://img.shields.io/pypi/v/django-xlsx-serializer?style=flat-square&logo=pypi&logoColor=white)][pypi]
+[![PyPI: Python](https://img.shields.io/pypi/pyversions/django-xlsx-serializer?style=flat-square&logo=python&logoColor=white)][pypi]
+[![PyPI: Django](https://img.shields.io/pypi/djversions/django-xlsx-serializer?style=flat-square&color=0C4B33&label=django&logo=django)][pypi]
+[![PyPI: License](https://img.shields.io/pypi/l/django-xlsx-serializer?style=flat-square)][pypi]
+
 [![Pre-commit](https://img.shields.io/github/actions/workflow/status/paduszyk/django-xlsx-serializer/pre-commit-run.yml?style=flat-square&label=pre-commit&logo=pre-commit)][pre-commit]
 [![Python: CI](https://img.shields.io/github/actions/workflow/status/paduszyk/django-xlsx-serializer/python-ci.yml?style=flat-square&logo=github&label=CI)][python-ci]
 [![Codecov](https://img.shields.io/codecov/c/github/paduszyk/django-xlsx-serializer?style=flat-square&logo=codecov)][codecov]
 
 [![Nox](https://img.shields.io/badge/%F0%9F%A6%8A-Nox-D85E00.svg?style=flat-square)][nox]
 [![Ruff](https://img.shields.io/endpoint?style=flat-square&url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)][ruff]
 [![Mypy](https://img.shields.io/badge/type--checked-mypy-blue?style=flat-square&logo=python)][mypy]
 [![Prettier](https://img.shields.io/badge/code%20style-prettier-1E2B33?style=flat-square&logo=Prettier)][prettier]
 [![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-fa6673.svg?style=flat-square&logo=conventional-commits)][conventional-commits]
 
-## Table of Contents
-
-- [Overview](#overview)
-- [Features](#features)
-- [Requirements](#requirements)
-- [Prerequisites](#prerequisites)
-- [Installation](#installation)
-- [Django Configuration](#django-configuration)
-  - [Install as an App](#install-as-an-app)
-  - [Add to Serialization Modules](#add-to-serialization-modules)
-  - [Register from Another App](#register-from-another-app)
-- [Usage](#usage)
-  - [Excel Workbooks vs. Django Models](#excel-workbooks-vs-django-models)
-  - [Serialization](#serialization)
-  - [Deserialization](#deserialization)
-- [Contributing](#contributing)
-- [Authors](#authors)
-- [License](#license)
-
 ## Overview
 
 `django-xlsx-serializer` is a [Django][django] application designed to handle
 the data serialization and deserialization between Django models and Microsoft
 Excel 2007+ workbooks. Utilizing the [OpenPyXL][openpyxl] engine, this tool
-provides robust methods to export data from Django databases into XLSX files
-and import data from the files back into the databases. This functionality is
+provides robust methods to export data from Django databases into XLSX files and
+import data from the files back into the databases. This functionality is
 essential for applications that require data exchange between Django-based
 systems and Excel, facilitating such tasks as data migration, reporting, and
 backups.
 
 ## Features
 
-The app enables:
+The app allows you to:
 
-- Exporting Django models from a database to an Excel workbook via the
+- Export Django models from a database to an Excel workbook via the
   [`dumpdata`][django-dumpdata] command.
-- Populating databases from Excel fixtures using the [`loaddata`][django-loaddata]
+- Populate databases from Excel fixtures using the [`loaddata`][django-loaddata]
   command.
-- Interacting with Excel workbooks (either files or `openpyxl.Workbook` objects)
-  and the database using the [serialization][django-serialization] utilities
-  from `django.core.serializers`.
-
-Both serialization and deserialization were tested for all the available Django
-model fields except:
-
-- `BinaryField`
-- `GeneratedField`
-
-Pull requests introducing the support for those fields are welcome; see
-the [Contributing](#contributing) section for further details.
+- Interact with Excel workbooks (either files or `openpyxl.Workbook` objects)
+  and the database using the Django's core [serialization][django-serialization]
+  utilities.
 
 ## Requirements
 
 | Python | Django                  | Database engines    |
 | :----- | :---------------------- | :------------------ |
 | 3.9    | 3.2, 4.0, 4.1, 4.2      | SQLite3, PostgreSQL |
 | 3.10   | 3.2, 4.0, 4.1, 4.2, 5.0 | SQLite3, PostgreSQL |
 | 3.11   | 4.1, 4.2, 5.0           | SQLite3, PostgreSQL |
 | 3.12   | 4.2, 5.0                | SQLite3, PostgreSQL |
 
-For all Python/Django/database setups, the package additionally requires
-OpenPyXL < 4.
-
-## Prerequisites
-
-This documentation assumes you are familiar with the following Django concepts:
-
-- [Models and fields][django-model-fields]
-- [Management commands][django-commands]
-- [Serialization][django-serialization] and [fixtures][django-fixtures]
-
-If you are unsure about your knowledge of these concepts, it is strongly
-recommended that you review the Django documentation by following the links
-provided above. The official documentation offers detailed explanations and
-examples to help you better understand how this app works and how to use it
-properly.
+All setups require OpenPyXL < 4.
 
 ## Installation
 
-The fastest way to add the package to your Python environment is to download
-and install it directly from [PyPI][pypi]. Use `pip`:
+The fastest way to add the package to your Python environment is to download and
+install it directly from [PyPI][pypi]. Use `pip`:
 
 ```console
 pip install django-xlsx-serializer
 ```
 
 or any other dependency manager of your preference.
 
@@ -157,16 +118,15 @@
 ## Django Configuration
 
 The app utilities can be incorporated into your Django project by following one
 of the approaches listed below:
 
 1. Installing the package as an app.
 2. Adding the package to serialization modules.
-3. Registering the app's serializers module in the configuration class of
-   another app installed in the project.
+3. Registering the app's serializers module from another app.
 
 All of them associate the app's serializer with the `xlsx` format.
 
 ### Install as an App
 
 In your project settings module add `xlsx_serializers` to `INSTALLED_APPS`:
 
@@ -218,15 +178,15 @@
 > utilities (e.g., custom commands, template tags, etc.). The configuration
 > class of such an app is a good place to apply the code snippet above.
 
 ## Usage
 
 ### Excel Workbooks vs. Django Models
 
-The app adopts the following correspondence between Excel workbooks (i.e., the
+The app adopts quite intuitive correspondence between Excel workbooks (i.e., the
 collections of worksheets) and Django models:
 
 - A Django model is represented by a single worksheet.
 - In an Excel workbook, the models are identified by worksheet names.
 - Within an Excel worksheet, model instances are represented by rows, while the
   columns correspond to the model's fields.
 
@@ -245,16 +205,16 @@
 >>> from django.core import serializers
 >>> from polls.models import Question
 >>> serializers.serialize("xlsx", Question.objects.all(), output="dump.xlsx")
 # Prints: <openpyxl.workbook.workbook.Workbook object at ...>
 ```
 
 Both the command and expression shown above save `dump.xlsx` workbook file. The
-latter additionally returns an `openpyxl.Workbook` object, which can
-be used later if necessary (e.g., in development or maintenance scripts).
+latter additionally returns an `openpyxl.Workbook` object, which can be used
+later if necessary (e.g., in development or maintenance scripts).
 
 When serializing, the app creates worksheets named using fully qualified model
 labels. For example, the `Question` model defined in the `polls` app is
 serialized to the "polls.Question" worksheet. Excel does not accept worksheet
 names longer than 31 characters. If the model's label is longer, it's truncated.
 A useful feature allowing you to circumvent this issue is that the output
 worksheet names can be customized using the `model_sheet_names` option. So, the
@@ -267,16 +227,16 @@
         model_sheet_names={"polls.Question": "Questions"},
     )
 >>> workbook
 # Prints: <openpyxl.workbook.workbook.Workbook object at ...>
 ```
 
 results in the `polls.Question` model data serialized in the "Questions"
-worksheet. Note that this
-option is not available when using the app via the `dumpdata` command.
+worksheet. Note that this option is not available when using the app via the
+`dumpdata` command.
 
 > The app inspects each key and value of the `model_sheet_names` dictionary. For
 > the keys, it validates whether they represent valid model identifiers. The
 > values, in turn, are checked to see if they are unique, are not too long, and
 > do not contain invalid characters (`?`, `*`, `:`, `\`, `/`, `[`, `]`).
 
 Other key points:
@@ -318,43 +278,40 @@
   enabled in Django settings requires date/time values to be saved as ISO 8601
   strings (date/time type values in Excel don't store timezone information).
 - Deserializing `JSONfield` requires values in a format compatible with the JSON
   decoder of the respective field.
 - In the case of `ManyToManyField` provide string representations of Python
   lists containing the primary (or natural, see the next bullet) keys of the
   related objects.
-- The app supports deserialization from natural keys. Make sure to provide the
-  keys that are valid string representations of the corresponding values (i.e.,
-  tuples of primitive Python literals; in most cases, they are strings &nddash;
-  if so, use single quotes as text delimiters);
+- The app handles deserialization from natural keys by using `ast.literal_eval`.
+  Make sure to provide the keys that are valid string representations of the
+  corresponding values (i.e., tuples of primitive Python literals; in most
+  cases, they are strings &nddash; if so, use single quotes as text delimiters).
 
 ## Contributing
 
-- This is an open-source project that embraces contributions of all types.
-- We require all contributors to adhere to our [Code of Conduct][code-of-conduct].
-- For comprehensive instructions on how to contribute to the project, please
-  refer to our [Contributing Guide][contributing].
+This is an open-source project that embraces contributions of all types. We
+require all contributors to adhere to our [Code of Conduct][code-of-conduct].
+For comprehensive instructions on how to contribute to the project, please refer
+to our [Contributing Guide][contributing].
 
 ## Authors
 
 Created and maintained by Kamil Paduszyński ([@paduszyk][paduszyk]).
 
 ## License
 
 Released under the [MIT license][license].
 
 [code-of-conduct]: https://github.com/paduszyk/django-xlsx-serializer/blob/main/docs/CODE_OF_CONDUCT.md
 [codecov]: https://app.codecov.io/gh/paduszyk/django-xlsx-serializer
 [contributing]: https://github.com/paduszyk/django-xlsx-serializer/blob/main/docs/CONTRIBUTING.md
 [conventional-commits]: https://www.conventionalcommits.org/en/v1.0.0/
-[django-commands]: https://docs.djangoproject.com/en/5.0/ref/django-admin/
 [django-dumpdata]: https://docs.djangoproject.com/en/5.0/ref/django-admin/#dumpdata
-[django-fixtures]: https://docs.djangoproject.com/en/5.0/topics/db/fixtures/
 [django-loaddata]: https://docs.djangoproject.com/en/5.0/ref/django-admin/#loaddata
-[django-model-fields]: https://docs.djangoproject.com/en/5.0/ref/models/fields/
 [django-serialization]: https://docs.djangoproject.com/en/5.0/topics/serialization/
 [django]: https://www.djangoproject.com
 [license]: https://github.com/paduszyk/django-xlsx-serializer/blob/main/LICENSE
 [mypy]: https://mypy.readthedocs.io
 [nox]: https://github.com/wntrblm/nox
 [openpyxl]: https://openpyxl.readthedocs.io/en/stable/
 [paduszyk]: https://github.com/paduszyk
```

### Comparing `django_xlsx_serializer-0.3.0/src/xlsx_serializer/core.py` & `django_xlsx_serializer-1.0.0/src/xlsx_serializer/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,16 @@
 from contextlib import suppress
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Final
 
 import openpyxl
 
 from django.apps import apps
+from django.core.serializers import python
 from django.core.serializers.base import DeserializedObject, SerializationError
-from django.core.serializers.python import Deserializer as PythonDeserializer
-from django.core.serializers.python import Serializer as PythonSerializer
 from django.db import models
 
 if TYPE_CHECKING:
     from collections.abc import Iterator
 
     from django.db.models import Model
 
@@ -33,15 +32,47 @@
     from typing_extensions import override
 
 SHEET_NAME_MAX_LENGTH: Final[int] = 31
 
 SHEET_NAME_INVALID_CHARACTERS: Final[str] = "\\?*:/[]"
 
 
-class Serializer(PythonSerializer):
+def _get_model(model_identifier: str) -> type[Model]:
+    # Determine the model's name and app label.
+    if "." in (model_label := model_identifier.lower()):
+        app_label, model_name = model_label.split(".")
+    else:
+        app_label, model_name = None, model_label
+
+    # Determine the candidates for the model to be returned.
+    models_candidates = [
+        model
+        for model in apps.get_models()
+        if model._meta.model_name == model_name
+        and (True if app_label is None else model._meta.app_label == app_label)
+    ]
+
+    # An identifier is valid if it represents a unique model.
+    if (num_model_candidates := len(models_candidates)) != 1:
+        if num_model_candidates == 0:
+            msg = f"model {model_identifier!r} isn't installed"
+        else:
+            app_labels = ", ".join(
+                [f"{model._meta.app_label!r}" for model in models_candidates],
+            )
+            msg = (
+                f"model {model_identifier!r} found in multiple apps ({app_labels}); "
+                f"use a fully qualified label to properly refer to the requested model"
+            )
+        raise LookupError(msg)
+
+    return models_candidates[0]
+
+
+class Serializer(python.Serializer):
     # Make the serializer discoverable with the `dumpdata` command.
     internal_use_only = False
 
     # If the stream is not specified in the options, force it to be set to `None`
     # (the base serializer class uses `io.StringIO` by default).
     stream_class = type(None)
 
@@ -327,19 +358,17 @@
 
                 # Handle valid data types representing an empty cell.
                 if value in ("", None):
                     if field.null:
                         fields[name] = None
                     elif field.blank:
                         fields[name] = ""
+                    # Continuing at this point may lead to integrity errors (tested).
                     continue
 
-                    # Based on our tests, continuing at this point can lead to integrity
-                    # errors. However, this app's main goal is not to validate fixtures.
-
                 # Handle natural foreign keys and many-to-many relations.
                 if isinstance(
                     field,
                     (
                         models.ForeignKey,
                         models.ManyToManyField,
                         models.OneToOneField,
@@ -347,40 +376,8 @@
                 ) and isinstance(value, str):
                     fields[name] = ast.literal_eval(value)
 
                 # Handle JSON values.
                 if isinstance(field, models.JSONField):
                     fields[name] = json.loads(value, cls=field.decoder)
 
-        return PythonDeserializer(python_objects, **self._options)
-
-
-def _get_model(model_identifier: str) -> type[Model]:
-    # Determine the model's name and app label.
-    if "." in (model_label := model_identifier.lower()):
-        app_label, model_name = model_label.split(".")
-    else:
-        app_label, model_name = None, model_label
-
-    # Determine the candidates for the model to be returned.
-    models_candidates = [
-        model
-        for model in apps.get_models()
-        if model._meta.model_name == model_name
-        and (True if app_label is None else model._meta.app_label == app_label)
-    ]
-
-    # An identifier is valid if it represents a unique model.
-    if (num_model_candidates := len(models_candidates)) != 1:
-        if num_model_candidates == 0:
-            msg = f"model {model_identifier!r} isn't installed"
-        else:
-            app_labels = ", ".join(
-                [f"{model._meta.app_label!r}" for model in models_candidates],
-            )
-            msg = (
-                f"model {model_identifier!r} found in multiple apps ({app_labels}); "
-                f"use a fully qualified label to properly refer to the requested model"
-            )
-        raise LookupError(msg)
-
-    return models_candidates[0]
+        return python.Deserializer(python_objects, **self._options)
```

