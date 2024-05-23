# Comparing `tmp/besser-1.1.1.tar.gz` & `tmp/besser-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "besser-1.1.1.tar", last modified: Sun May  5 18:41:06 2024, max compression
+gzip compressed data, was "besser-1.1.2.tar", last modified: Thu May 23 12:11:29 2024, max compression
```

## Comparing `besser-1.1.1.tar` & `besser-1.1.2.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.841696 besser-1.1.1/
--rw-rw-rw-   0        0        0     3777 2024-05-05 18:41:06.840693 besser-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2804 2024-04-29 14:01:22.000000 besser-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.722524 besser-1.1.1/besser/
-drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.733037 besser-1.1.1/besser/BUML/
--rw-rw-rw-   0        0        0        0 2023-11-29 15:43:44.000000 besser-1.1.1/besser/BUML/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.735037 besser-1.1.1/besser/BUML/metamodel/
--rw-rw-rw-   0        0        0        0 2023-10-23 15:26:16.000000 besser-1.1.1/besser/BUML/metamodel/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.737200 besser-1.1.1/besser/BUML/metamodel/gui/
--rw-rw-rw-   0        0        0       29 2024-03-07 10:53:16.000000 besser-1.1.1/besser/BUML/metamodel/gui/__init__.py
--rw-rw-rw-   0        0        0    25750 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/metamodel/gui/graphical_ui.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.740326 besser-1.1.1/besser/BUML/metamodel/object/
--rw-rw-rw-   0        0        0       21 2024-03-07 08:52:50.000000 besser-1.1.1/besser/BUML/metamodel/object/__init__.py
--rw-rw-rw-   0        0        0    10058 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/metamodel/object/object.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.743325 besser-1.1.1/besser/BUML/metamodel/ocl/
--rw-rw-rw-   0        0        0       20 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/metamodel/ocl/__init__.py
--rw-rw-rw-   0        0        0    18910 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/metamodel/ocl/rules.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.747325 besser-1.1.1/besser/BUML/metamodel/structural/
--rw-rw-rw-   0        0        0       25 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/metamodel/structural/__init__.py
--rw-rw-rw-   0        0        0    42620 2024-05-03 13:04:47.000000 besser-1.1.1/besser/BUML/metamodel/structural/structural.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.749157 besser-1.1.1/besser/BUML/notations/
--rw-rw-rw-   0        0        0        0 2023-10-23 15:26:16.000000 besser-1.1.1/besser/BUML/notations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.755179 besser-1.1.1/besser/BUML/notations/objectPlantUML/
--rw-rw-rw-   0        0        0     5938 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/notations/objectPlantUML/ODLexer.py
--rw-rw-rw-   0        0        0     4976 2024-05-03 13:06:20.000000 besser-1.1.1/besser/BUML/notations/objectPlantUML/ODListener.py
--rw-rw-rw-   0        0        0    25828 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/notations/objectPlantUML/ODParser.py
--rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/notations/objectPlantUML/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.766948 besser-1.1.1/besser/BUML/notations/ocl/
--rw-rw-rw-   0        0        0    23268 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/notations/ocl/BOCLLexer.py
--rw-rw-rw-   0        0        0    41633 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/notations/ocl/BOCLListener.py
--rw-rw-rw-   0        0        0   212929 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/notations/ocl/BOCLParser.py
--rw-rw-rw-   0        0        0     4732 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/notations/ocl/FactoryInstance.py
--rw-rw-rw-   0        0        0     1080 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/notations/ocl/OCLWrapper.py
--rw-rw-rw-   0        0        0    12723 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/notations/ocl/RootHandler.py
--rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/notations/ocl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.777205 besser-1.1.1/besser/BUML/notations/structuralPlantUML/
--rw-rw-rw-   0        0        0    10331 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/notations/structuralPlantUML/PlantUMLLexer.py
--rw-rw-rw-   0        0        0     6394 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/notations/structuralPlantUML/PlantUMLListener.py
--rw-rw-rw-   0        0        0    51575 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/notations/structuralPlantUML/PlantUMLParser.py
--rw-rw-rw-   0        0        0      203 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/notations/structuralPlantUML/__init__.py
--rw-rw-rw-   0        0        0     9094 2024-05-03 13:06:20.000000 besser-1.1.1/besser/BUML/notations/structuralPlantUML/plantUML_buml_listener.py
--rw-rw-rw-   0        0        0     1432 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/notations/structuralPlantUML/plantuml_to_buml.py
--rw-rw-rw-   0        0        0        0 2024-01-15 16:06:49.000000 besser-1.1.1/besser/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.780209 besser-1.1.1/besser/generators/
--rw-rw-rw-   0        0        0       34 2023-10-23 15:26:16.000000 besser-1.1.1/besser/generators/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.783205 besser-1.1.1/besser/generators/backend/
--rw-rw-rw-   0        0        0       32 2024-05-01 21:18:56.000000 besser-1.1.1/besser/generators/backend/__init__.py
--rw-rw-rw-   0        0        0     3276 2024-05-01 21:18:56.000000 besser-1.1.1/besser/generators/backend/backend_generator.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.785205 besser-1.1.1/besser/generators/django/
--rw-rw-rw-   0        0        0       31 2023-11-24 11:35:33.000000 besser-1.1.1/besser/generators/django/__init__.py
--rw-rw-rw-   0        0        0     1756 2024-01-15 16:11:55.000000 besser-1.1.1/besser/generators/django/django_generator.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.788900 besser-1.1.1/besser/generators/django/templates/
--rw-rw-rw-   0        0        0        0 2024-01-05 16:17:26.000000 besser-1.1.1/besser/generators/django/templates/__init__.py
--rw-rw-rw-   0        0        0      608 2023-11-24 11:35:33.000000 besser-1.1.1/besser/generators/django/templates/django_fields.py.j2
--rw-rw-rw-   0        0        0     3580 2024-05-01 21:18:56.000000 besser-1.1.1/besser/generators/django/templates/django_template.py.j2
--rw-rw-rw-   0        0        0     1166 2024-04-29 14:01:22.000000 besser-1.1.1/besser/generators/generator_interface.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.793002 besser-1.1.1/besser/generators/pydantic_classes/
--rw-rw-rw-   0        0        0       41 2024-05-01 21:18:56.000000 besser-1.1.1/besser/generators/pydantic_classes/__init__.py
--rw-rw-rw-   0        0        0     2593 2024-05-01 21:18:56.000000 besser-1.1.1/besser/generators/pydantic_classes/pydantic_classes_generator.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.795900 besser-1.1.1/besser/generators/pydantic_classes/templates/
--rw-rw-rw-   0        0        0        0 2024-05-01 21:18:56.000000 besser-1.1.1/besser/generators/pydantic_classes/templates/__init__.py
--rw-rw-rw-   0        0        0     3409 2024-05-01 21:18:56.000000 besser-1.1.1/besser/generators/pydantic_classes/templates/pydantic_classes_template.py.j2
-drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.798001 besser-1.1.1/besser/generators/python_classes/
--rw-rw-rw-   0        0        0       39 2023-11-03 14:54:15.000000 besser-1.1.1/besser/generators/python_classes/__init__.py
--rw-rw-rw-   0        0        0     1722 2024-05-01 21:18:56.000000 besser-1.1.1/besser/generators/python_classes/python_classes_generator.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.801949 besser-1.1.1/besser/generators/python_classes/templates/
--rw-rw-rw-   0        0        0        0 2024-01-05 16:17:26.000000 besser-1.1.1/besser/generators/python_classes/templates/__init__.py
--rw-rw-rw-   0        0        0     1461 2024-01-05 14:02:17.000000 besser-1.1.1/besser/generators/python_classes/templates/class_parameters.py.j2
--rw-rw-rw-   0        0        0     1496 2024-01-04 17:15:56.000000 besser-1.1.1/besser/generators/python_classes/templates/python_classes_template.py.j2
-drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.804900 besser-1.1.1/besser/generators/rest_api/
--rw-rw-rw-   0        0        0       33 2024-03-07 08:29:25.000000 besser-1.1.1/besser/generators/rest_api/__init__.py
--rw-rw-rw-   0        0        0     4716 2024-05-01 21:18:56.000000 besser-1.1.1/besser/generators/rest_api/rest_api_generator.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.808899 besser-1.1.1/besser/generators/rest_api/templates/
--rw-rw-rw-   0        0        0        0 2024-03-07 08:29:25.000000 besser-1.1.1/besser/generators/rest_api/templates/__init__.py
--rw-rw-rw-   0        0        0    11014 2024-05-01 21:18:56.000000 besser-1.1.1/besser/generators/rest_api/templates/backend_fast_api_template.py.j2
--rw-rw-rw-   0        0        0     4987 2024-05-01 21:18:56.000000 besser-1.1.1/besser/generators/rest_api/templates/fast_api_template.py.j2
-drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.811900 besser-1.1.1/besser/generators/sql/
--rw-rw-rw-   0        0        0       28 2023-11-03 14:54:15.000000 besser-1.1.1/besser/generators/sql/__init__.py
--rw-rw-rw-   0        0        0     2191 2024-01-15 16:14:26.000000 besser-1.1.1/besser/generators/sql/sql_generator.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.815900 besser-1.1.1/besser/generators/sql/templates/
--rw-rw-rw-   0        0        0        0 2024-01-05 16:17:26.000000 besser-1.1.1/besser/generators/sql/templates/__init__.py
--rw-rw-rw-   0        0        0     4633 2023-11-24 11:35:33.000000 besser-1.1.1/besser/generators/sql/templates/sql_dialects.sql.j2
--rw-rw-rw-   0        0        0     3608 2023-11-24 11:35:33.000000 besser-1.1.1/besser/generators/sql/templates/sql_template.sql.j2
-drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.817998 besser-1.1.1/besser/generators/sql_alchemy/
--rw-rw-rw-   0        0        0       36 2023-11-23 14:47:36.000000 besser-1.1.1/besser/generators/sql_alchemy/__init__.py
--rw-rw-rw-   0        0        0     1994 2024-01-15 16:14:45.000000 besser-1.1.1/besser/generators/sql_alchemy/sql_alchemy_generator.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.819900 besser-1.1.1/besser/generators/sql_alchemy/templates/
--rw-rw-rw-   0        0        0        0 2024-01-05 16:17:26.000000 besser-1.1.1/besser/generators/sql_alchemy/templates/__init__.py
--rw-rw-rw-   0        0        0     3695 2024-05-01 21:18:56.000000 besser-1.1.1/besser/generators/sql_alchemy/templates/sql_alchemy_template.py.j2
-drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.823901 besser-1.1.1/besser/utilities/
--rw-rw-rw-   0        0        0       50 2024-01-04 13:03:26.000000 besser-1.1.1/besser/utilities/__init__.py
--rw-rw-rw-   0        0        0     2897 2024-05-01 21:18:56.000000 besser-1.1.1/besser/utilities/image_to_buml.py
--rw-rw-rw-   0        0        0     2106 2024-01-15 16:16:07.000000 besser-1.1.1/besser/utilities/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.838686 besser-1.1.1/besser.egg-info/
--rw-rw-rw-   0        0        0     3777 2024-05-05 18:41:06.000000 besser-1.1.1/besser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3529 2024-05-05 18:41:06.000000 besser-1.1.1/besser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 18:41:06.000000 besser-1.1.1/besser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      263 2024-05-05 18:41:06.000000 besser-1.1.1/besser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-05 18:41:06.000000 besser-1.1.1/besser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       97 2023-10-23 15:26:16.000000 besser-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      277 2024-05-01 21:18:56.000000 besser-1.1.1/requirements.txt
--rw-rw-rw-   0        0        0      659 2024-05-05 18:41:06.842695 besser-1.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.824900 besser-1.1.1/tests/
--rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.1/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.828901 besser-1.1.1/tests/gui/
--rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.1/tests/gui/__init__.py
--rw-rw-rw-   0        0        0     2461 2024-05-03 13:07:26.000000 besser-1.1.1/tests/gui/gui_model.py
--rw-rw-rw-   0        0        0     5244 2024-05-03 13:07:26.000000 besser-1.1.1/tests/gui/test_gui.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.829900 besser-1.1.1/tests/notations/
--rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.1/tests/notations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.833133 besser-1.1.1/tests/object/
--rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.1/tests/object/__init__.py
--rw-rw-rw-   0        0        0    10448 2024-05-03 13:07:26.000000 besser-1.1.1/tests/object/library_object.py
--rw-rw-rw-   0        0        0     3843 2024-05-03 13:07:26.000000 besser-1.1.1/tests/object/test_object_mm.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.835146 besser-1.1.1/tests/ocl/
--rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.1/tests/ocl/__init__.py
--rw-rw-rw-   0        0        0     7566 2024-04-29 14:01:22.000000 besser-1.1.1/tests/ocl/test_ocl_parser.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.837599 besser-1.1.1/tests/structural/
--rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.1/tests/structural/__init__.py
--rw-rw-rw-   0        0        0    10023 2024-05-03 13:07:26.000000 besser-1.1.1/tests/structural/test_structural.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:29.830198 besser-1.1.2/
+-rw-rw-rw-   0        0        0     3777 2024-05-23 12:11:29.830198 besser-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2804 2024-04-29 14:01:22.000000 besser-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:29.737509 besser-1.1.2/besser/
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:29.745518 besser-1.1.2/besser/BUML/
+-rw-rw-rw-   0        0        0        0 2023-11-29 15:43:44.000000 besser-1.1.2/besser/BUML/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:29.746510 besser-1.1.2/besser/BUML/metamodel/
+-rw-rw-rw-   0        0        0        0 2023-10-23 15:26:16.000000 besser-1.1.2/besser/BUML/metamodel/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:29.747520 besser-1.1.2/besser/BUML/metamodel/gui/
+-rw-rw-rw-   0        0        0       29 2024-03-07 10:53:16.000000 besser-1.1.2/besser/BUML/metamodel/gui/__init__.py
+-rw-rw-rw-   0        0        0    25750 2024-04-29 14:01:22.000000 besser-1.1.2/besser/BUML/metamodel/gui/graphical_ui.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:29.750517 besser-1.1.2/besser/BUML/metamodel/object/
+-rw-rw-rw-   0        0        0       21 2024-03-07 08:52:50.000000 besser-1.1.2/besser/BUML/metamodel/object/__init__.py
+-rw-rw-rw-   0        0        0    10058 2024-04-29 14:01:22.000000 besser-1.1.2/besser/BUML/metamodel/object/object.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:29.753532 besser-1.1.2/besser/BUML/metamodel/ocl/
+-rw-rw-rw-   0        0        0       20 2024-04-29 14:01:22.000000 besser-1.1.2/besser/BUML/metamodel/ocl/__init__.py
+-rw-rw-rw-   0        0        0    18910 2024-04-29 14:01:22.000000 besser-1.1.2/besser/BUML/metamodel/ocl/rules.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:29.755575 besser-1.1.2/besser/BUML/metamodel/structural/
+-rw-rw-rw-   0        0        0       25 2024-04-29 14:01:22.000000 besser-1.1.2/besser/BUML/metamodel/structural/__init__.py
+-rw-rw-rw-   0        0        0    42620 2024-05-07 13:15:11.000000 besser-1.1.2/besser/BUML/metamodel/structural/structural.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:29.757574 besser-1.1.2/besser/BUML/notations/
+-rw-rw-rw-   0        0        0        0 2023-10-23 15:26:16.000000 besser-1.1.2/besser/BUML/notations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:29.761581 besser-1.1.2/besser/BUML/notations/objectPlantUML/
+-rw-rw-rw-   0        0        0     5938 2024-04-29 14:01:22.000000 besser-1.1.2/besser/BUML/notations/objectPlantUML/ODLexer.py
+-rw-rw-rw-   0        0        0     4976 2024-05-07 13:15:11.000000 besser-1.1.2/besser/BUML/notations/objectPlantUML/ODListener.py
+-rw-rw-rw-   0        0        0    25828 2024-04-29 14:01:22.000000 besser-1.1.2/besser/BUML/notations/objectPlantUML/ODParser.py
+-rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.2/besser/BUML/notations/objectPlantUML/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:29.771202 besser-1.1.2/besser/BUML/notations/ocl/
+-rw-rw-rw-   0        0        0    23268 2024-04-29 14:01:22.000000 besser-1.1.2/besser/BUML/notations/ocl/BOCLLexer.py
+-rw-rw-rw-   0        0        0    41633 2024-04-29 14:01:22.000000 besser-1.1.2/besser/BUML/notations/ocl/BOCLListener.py
+-rw-rw-rw-   0        0        0   212929 2024-04-29 14:01:22.000000 besser-1.1.2/besser/BUML/notations/ocl/BOCLParser.py
+-rw-rw-rw-   0        0        0     4732 2024-04-29 14:01:22.000000 besser-1.1.2/besser/BUML/notations/ocl/FactoryInstance.py
+-rw-rw-rw-   0        0        0     1080 2024-04-29 14:01:22.000000 besser-1.1.2/besser/BUML/notations/ocl/OCLWrapper.py
+-rw-rw-rw-   0        0        0    12723 2024-04-29 14:01:22.000000 besser-1.1.2/besser/BUML/notations/ocl/RootHandler.py
+-rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.2/besser/BUML/notations/ocl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:29.778210 besser-1.1.2/besser/BUML/notations/structuralPlantUML/
+-rw-rw-rw-   0        0        0    10331 2024-04-29 14:01:22.000000 besser-1.1.2/besser/BUML/notations/structuralPlantUML/PlantUMLLexer.py
+-rw-rw-rw-   0        0        0     6394 2024-04-29 14:01:22.000000 besser-1.1.2/besser/BUML/notations/structuralPlantUML/PlantUMLListener.py
+-rw-rw-rw-   0        0        0    51575 2024-04-29 14:01:22.000000 besser-1.1.2/besser/BUML/notations/structuralPlantUML/PlantUMLParser.py
+-rw-rw-rw-   0        0        0      203 2024-04-29 14:01:22.000000 besser-1.1.2/besser/BUML/notations/structuralPlantUML/__init__.py
+-rw-rw-rw-   0        0        0     9094 2024-05-07 13:15:11.000000 besser-1.1.2/besser/BUML/notations/structuralPlantUML/plantUML_buml_listener.py
+-rw-rw-rw-   0        0        0     1432 2024-04-29 14:01:22.000000 besser-1.1.2/besser/BUML/notations/structuralPlantUML/plantuml_to_buml.py
+-rw-rw-rw-   0        0        0        0 2024-01-15 16:06:49.000000 besser-1.1.2/besser/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:29.780202 besser-1.1.2/besser/generators/
+-rw-rw-rw-   0        0        0       34 2023-10-23 15:26:16.000000 besser-1.1.2/besser/generators/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:29.782203 besser-1.1.2/besser/generators/backend/
+-rw-rw-rw-   0        0        0       32 2024-05-23 08:57:34.000000 besser-1.1.2/besser/generators/backend/__init__.py
+-rw-rw-rw-   0        0        0     3276 2024-05-23 08:57:34.000000 besser-1.1.2/besser/generators/backend/backend_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:29.784208 besser-1.1.2/besser/generators/django/
+-rw-rw-rw-   0        0        0       31 2023-11-24 11:35:33.000000 besser-1.1.2/besser/generators/django/__init__.py
+-rw-rw-rw-   0        0        0     1756 2024-01-15 16:11:55.000000 besser-1.1.2/besser/generators/django/django_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:29.787203 besser-1.1.2/besser/generators/django/templates/
+-rw-rw-rw-   0        0        0        0 2024-01-05 16:17:26.000000 besser-1.1.2/besser/generators/django/templates/__init__.py
+-rw-rw-rw-   0        0        0      608 2023-11-24 11:35:33.000000 besser-1.1.2/besser/generators/django/templates/django_fields.py.j2
+-rw-rw-rw-   0        0        0     3595 2024-05-23 09:56:48.000000 besser-1.1.2/besser/generators/django/templates/django_template.py.j2
+-rw-rw-rw-   0        0        0     1166 2024-04-29 14:01:22.000000 besser-1.1.2/besser/generators/generator_interface.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:29.789196 besser-1.1.2/besser/generators/pydantic_classes/
+-rw-rw-rw-   0        0        0       41 2024-05-07 13:15:11.000000 besser-1.1.2/besser/generators/pydantic_classes/__init__.py
+-rw-rw-rw-   0        0        0     2593 2024-05-07 13:15:11.000000 besser-1.1.2/besser/generators/pydantic_classes/pydantic_classes_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:29.791204 besser-1.1.2/besser/generators/pydantic_classes/templates/
+-rw-rw-rw-   0        0        0        0 2024-05-07 13:15:11.000000 besser-1.1.2/besser/generators/pydantic_classes/templates/__init__.py
+-rw-rw-rw-   0        0        0     3409 2024-05-07 13:15:11.000000 besser-1.1.2/besser/generators/pydantic_classes/templates/pydantic_classes_template.py.j2
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:29.793155 besser-1.1.2/besser/generators/python_classes/
+-rw-rw-rw-   0        0        0       39 2023-11-03 14:54:15.000000 besser-1.1.2/besser/generators/python_classes/__init__.py
+-rw-rw-rw-   0        0        0     1722 2024-05-07 13:15:11.000000 besser-1.1.2/besser/generators/python_classes/python_classes_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:29.797197 besser-1.1.2/besser/generators/python_classes/templates/
+-rw-rw-rw-   0        0        0        0 2024-01-05 16:17:26.000000 besser-1.1.2/besser/generators/python_classes/templates/__init__.py
+-rw-rw-rw-   0        0        0     1461 2024-01-05 14:02:17.000000 besser-1.1.2/besser/generators/python_classes/templates/class_parameters.py.j2
+-rw-rw-rw-   0        0        0     1496 2024-01-04 17:15:56.000000 besser-1.1.2/besser/generators/python_classes/templates/python_classes_template.py.j2
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:29.799201 besser-1.1.2/besser/generators/rest_api/
+-rw-rw-rw-   0        0        0       33 2024-03-07 08:29:25.000000 besser-1.1.2/besser/generators/rest_api/__init__.py
+-rw-rw-rw-   0        0        0     4716 2024-05-07 13:15:11.000000 besser-1.1.2/besser/generators/rest_api/rest_api_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:29.803206 besser-1.1.2/besser/generators/rest_api/templates/
+-rw-rw-rw-   0        0        0        0 2024-03-07 08:29:25.000000 besser-1.1.2/besser/generators/rest_api/templates/__init__.py
+-rw-rw-rw-   0        0        0    11014 2024-05-07 13:15:11.000000 besser-1.1.2/besser/generators/rest_api/templates/backend_fast_api_template.py.j2
+-rw-rw-rw-   0        0        0     4987 2024-05-07 13:15:11.000000 besser-1.1.2/besser/generators/rest_api/templates/fast_api_template.py.j2
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:29.805155 besser-1.1.2/besser/generators/sql/
+-rw-rw-rw-   0        0        0       28 2023-11-03 14:54:15.000000 besser-1.1.2/besser/generators/sql/__init__.py
+-rw-rw-rw-   0        0        0     2191 2024-01-15 16:14:26.000000 besser-1.1.2/besser/generators/sql/sql_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:29.809199 besser-1.1.2/besser/generators/sql/templates/
+-rw-rw-rw-   0        0        0        0 2024-01-05 16:17:26.000000 besser-1.1.2/besser/generators/sql/templates/__init__.py
+-rw-rw-rw-   0        0        0     4633 2023-11-24 11:35:33.000000 besser-1.1.2/besser/generators/sql/templates/sql_dialects.sql.j2
+-rw-rw-rw-   0        0        0     3608 2023-11-24 11:35:33.000000 besser-1.1.2/besser/generators/sql/templates/sql_template.sql.j2
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:29.812202 besser-1.1.2/besser/generators/sql_alchemy/
+-rw-rw-rw-   0        0        0       36 2023-11-23 14:47:36.000000 besser-1.1.2/besser/generators/sql_alchemy/__init__.py
+-rw-rw-rw-   0        0        0     1994 2024-01-15 16:14:45.000000 besser-1.1.2/besser/generators/sql_alchemy/sql_alchemy_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:29.814197 besser-1.1.2/besser/generators/sql_alchemy/templates/
+-rw-rw-rw-   0        0        0        0 2024-01-05 16:17:26.000000 besser-1.1.2/besser/generators/sql_alchemy/templates/__init__.py
+-rw-rw-rw-   0        0        0     3695 2024-05-07 13:15:11.000000 besser-1.1.2/besser/generators/sql_alchemy/templates/sql_alchemy_template.py.j2
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:29.817197 besser-1.1.2/besser/utilities/
+-rw-rw-rw-   0        0        0       50 2024-01-04 13:03:26.000000 besser-1.1.2/besser/utilities/__init__.py
+-rw-rw-rw-   0        0        0     2897 2024-05-07 13:15:11.000000 besser-1.1.2/besser/utilities/image_to_buml.py
+-rw-rw-rw-   0        0        0     2106 2024-01-15 16:16:07.000000 besser-1.1.2/besser/utilities/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:29.829215 besser-1.1.2/besser.egg-info/
+-rw-rw-rw-   0        0        0     3777 2024-05-23 12:11:29.000000 besser-1.1.2/besser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3529 2024-05-23 12:11:29.000000 besser-1.1.2/besser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 12:11:29.000000 besser-1.1.2/besser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      263 2024-05-23 12:11:29.000000 besser-1.1.2/besser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-23 12:11:29.000000 besser-1.1.2/besser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       97 2023-10-23 15:26:16.000000 besser-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      277 2024-05-07 13:15:11.000000 besser-1.1.2/requirements.txt
+-rw-rw-rw-   0        0        0      659 2024-05-23 12:11:29.831197 besser-1.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:29.818208 besser-1.1.2/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.2/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:29.821199 besser-1.1.2/tests/gui/
+-rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.2/tests/gui/__init__.py
+-rw-rw-rw-   0        0        0     2461 2024-05-07 13:15:11.000000 besser-1.1.2/tests/gui/gui_model.py
+-rw-rw-rw-   0        0        0     5244 2024-05-07 13:15:11.000000 besser-1.1.2/tests/gui/test_gui.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:29.822198 besser-1.1.2/tests/notations/
+-rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.2/tests/notations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:29.824210 besser-1.1.2/tests/object/
+-rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.2/tests/object/__init__.py
+-rw-rw-rw-   0        0        0    10453 2024-05-07 13:15:11.000000 besser-1.1.2/tests/object/library_object.py
+-rw-rw-rw-   0        0        0     3843 2024-05-07 13:15:11.000000 besser-1.1.2/tests/object/test_object_mm.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:29.826209 besser-1.1.2/tests/ocl/
+-rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.2/tests/ocl/__init__.py
+-rw-rw-rw-   0        0        0     7566 2024-04-29 14:01:22.000000 besser-1.1.2/tests/ocl/test_ocl_parser.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:11:29.827205 besser-1.1.2/tests/structural/
+-rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.2/tests/structural/__init__.py
+-rw-rw-rw-   0        0        0    10023 2024-05-07 13:15:11.000000 besser-1.1.2/tests/structural/test_structural.py
```

### Comparing `besser-1.1.1/PKG-INFO` & `besser-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: besser
-Version: 1.1.1
+Version: 1.1.2
 Summary: BESSER
 Author: Luxembourg Institute of Science and Technology
 License: MIT
 Project-URL: Documentation, https://besser.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/BESSER-PEARL/BESSER
 Project-URL: Bug Tracker, https://github.com/BESSER-PEARL/BESSER/issues
 Keywords: uml,code generation,python
```

### Comparing `besser-1.1.1/README.md` & `besser-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/BUML/metamodel/gui/graphical_ui.py` & `besser-1.1.2/besser/BUML/metamodel/gui/graphical_ui.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/BUML/metamodel/object/object.py` & `besser-1.1.2/besser/BUML/metamodel/object/object.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/BUML/metamodel/ocl/rules.py` & `besser-1.1.2/besser/BUML/metamodel/ocl/rules.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/BUML/metamodel/structural/structural.py` & `besser-1.1.2/besser/BUML/metamodel/structural/structural.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/BUML/notations/objectPlantUML/ODLexer.py` & `besser-1.1.2/besser/BUML/notations/objectPlantUML/ODLexer.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/BUML/notations/objectPlantUML/ODListener.py` & `besser-1.1.2/besser/BUML/notations/objectPlantUML/ODListener.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/BUML/notations/objectPlantUML/ODParser.py` & `besser-1.1.2/besser/BUML/notations/objectPlantUML/ODParser.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/BUML/notations/ocl/BOCLLexer.py` & `besser-1.1.2/besser/BUML/notations/ocl/BOCLLexer.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/BUML/notations/ocl/BOCLListener.py` & `besser-1.1.2/besser/BUML/notations/ocl/BOCLListener.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/BUML/notations/ocl/BOCLParser.py` & `besser-1.1.2/besser/BUML/notations/ocl/BOCLParser.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/BUML/notations/ocl/FactoryInstance.py` & `besser-1.1.2/besser/BUML/notations/ocl/FactoryInstance.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/BUML/notations/ocl/OCLWrapper.py` & `besser-1.1.2/besser/BUML/notations/ocl/OCLWrapper.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/BUML/notations/ocl/RootHandler.py` & `besser-1.1.2/besser/BUML/notations/ocl/RootHandler.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/BUML/notations/structuralPlantUML/PlantUMLLexer.py` & `besser-1.1.2/besser/BUML/notations/structuralPlantUML/PlantUMLLexer.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/BUML/notations/structuralPlantUML/PlantUMLListener.py` & `besser-1.1.2/besser/BUML/notations/structuralPlantUML/PlantUMLListener.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/BUML/notations/structuralPlantUML/PlantUMLParser.py` & `besser-1.1.2/besser/BUML/notations/structuralPlantUML/PlantUMLParser.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/BUML/notations/structuralPlantUML/plantUML_buml_listener.py` & `besser-1.1.2/besser/BUML/notations/structuralPlantUML/plantUML_buml_listener.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/BUML/notations/structuralPlantUML/plantuml_to_buml.py` & `besser-1.1.2/besser/BUML/notations/structuralPlantUML/plantuml_to_buml.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/generators/backend/backend_generator.py` & `besser-1.1.2/besser/generators/backend/backend_generator.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/generators/django/django_generator.py` & `besser-1.1.2/besser/generators/django/django_generator.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/generators/django/templates/django_fields.py.j2` & `besser-1.1.2/besser/generators/django/templates/django_fields.py.j2`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/generators/django/templates/django_template.py.j2` & `besser-1.1.2/besser/generators/django/templates/django_template.py.j2`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,16 @@
             {% set class2_name = ns.end2.type.name %}
             {% if ns.end1.multiplicity.max > 1 and ns.end2.multiplicity.max > 1 %}
             {# N:M Relationship: Use ManyToManyField in Django #}
     {{ ns.end2.name.replace(' ', '_') }} = models.ManyToManyField('{{ class2_name }}'{% if ns.end2.multiplicity.min == 0 %}, blank=True, null=True{% endif %})
                 {% do processed_associations.append(association.name) %}
             {% elif ns.end1.multiplicity.max > 1 and ns.end2.multiplicity.max == 1 %}
             {# N:1 Relationship: Use ForeignKey in Django #}
-    {{ ns.end2.name.replace(' ', '_') }} = models.ForeignKey('{{ class2_name }}'{% if ns.end2.is_composite %}, on_delete=models.CASCADE{% endif %}
-                {%- if ns.end2.multiplicity.min == 0 %}, blank=True, null=True{% endif %})
+    {{ ns.end2.name.replace(' ', '_') }} = models.ForeignKey('{{ class2_name }}', on_delete=models.{% if ns.end2.is_composite %}CASCADE
+                {%- elif ns.end2.multiplicity.min == 0%}SET_NULL, blank=True, null=True{% else %}PROTECT{% endif %})
                 {% do processed_associations.append(association.name) %}
             {% elif ns.end1.multiplicity.max == 1 and ns.end2.multiplicity.max == 1 %}
             {# 1:1 Relationship: Use OneToOneField in Django #}
     {{ ns.end2.name.replace(' ', '_') }} = models.OneToOneField('{{ class2_name }}'{% if ns.end2.is_composite %}, on_delete=models.CASCADE{% endif %}
                 {%- if ns.end2.multiplicity.min == 0 %}, blank=True, null=True{% endif %})
                 {% do processed_associations.append(association.name) %}
             {% endif %}
```

### Comparing `besser-1.1.1/besser/generators/generator_interface.py` & `besser-1.1.2/besser/generators/generator_interface.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/generators/pydantic_classes/pydantic_classes_generator.py` & `besser-1.1.2/besser/generators/pydantic_classes/pydantic_classes_generator.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/generators/pydantic_classes/templates/pydantic_classes_template.py.j2` & `besser-1.1.2/besser/generators/pydantic_classes/templates/pydantic_classes_template.py.j2`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/generators/python_classes/python_classes_generator.py` & `besser-1.1.2/besser/generators/python_classes/python_classes_generator.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/generators/python_classes/templates/class_parameters.py.j2` & `besser-1.1.2/besser/generators/python_classes/templates/class_parameters.py.j2`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/generators/python_classes/templates/python_classes_template.py.j2` & `besser-1.1.2/besser/generators/python_classes/templates/python_classes_template.py.j2`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/generators/rest_api/rest_api_generator.py` & `besser-1.1.2/besser/generators/rest_api/rest_api_generator.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/generators/rest_api/templates/backend_fast_api_template.py.j2` & `besser-1.1.2/besser/generators/rest_api/templates/backend_fast_api_template.py.j2`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/generators/rest_api/templates/fast_api_template.py.j2` & `besser-1.1.2/besser/generators/rest_api/templates/fast_api_template.py.j2`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/generators/sql/sql_generator.py` & `besser-1.1.2/besser/generators/sql/sql_generator.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/generators/sql/templates/sql_dialects.sql.j2` & `besser-1.1.2/besser/generators/sql/templates/sql_dialects.sql.j2`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/generators/sql/templates/sql_template.sql.j2` & `besser-1.1.2/besser/generators/sql/templates/sql_template.sql.j2`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/generators/sql_alchemy/sql_alchemy_generator.py` & `besser-1.1.2/besser/generators/sql_alchemy/sql_alchemy_generator.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/generators/sql_alchemy/templates/sql_alchemy_template.py.j2` & `besser-1.1.2/besser/generators/sql_alchemy/templates/sql_alchemy_template.py.j2`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/utilities/image_to_buml.py` & `besser-1.1.2/besser/utilities/image_to_buml.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser/utilities/utils.py` & `besser-1.1.2/besser/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/besser.egg-info/PKG-INFO` & `besser-1.1.2/besser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: besser
-Version: 1.1.1
+Version: 1.1.2
 Summary: BESSER
 Author: Luxembourg Institute of Science and Technology
 License: MIT
 Project-URL: Documentation, https://besser.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/BESSER-PEARL/BESSER
 Project-URL: Bug Tracker, https://github.com/BESSER-PEARL/BESSER/issues
 Keywords: uml,code generation,python
```

### Comparing `besser-1.1.1/besser.egg-info/SOURCES.txt` & `besser-1.1.2/besser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/setup.cfg` & `besser-1.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 6573 7365 720d 0a76 6572 7369   = besser..versi
-00000020: 6f6e 203d 2031 2e31 2e31 0d0a 6175 7468  on = 1.1.1..auth
+00000020: 6f6e 203d 2031 2e31 2e32 0d0a 6175 7468  on = 1.1.2..auth
 00000030: 6f72 203d 204c 7578 656d 626f 7572 6720  or = Luxembourg 
 00000040: 496e 7374 6974 7574 6520 6f66 2053 6369  Institute of Sci
 00000050: 656e 6365 2061 6e64 2054 6563 686e 6f6c  ence and Technol
 00000060: 6f67 790d 0a64 6573 6372 6970 7469 6f6e  ogy..description
 00000070: 203d 2042 4553 5345 520d 0a6c 6f6e 675f   = BESSER..long_
 00000080: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
 00000090: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
```

### Comparing `besser-1.1.1/tests/gui/gui_model.py` & `besser-1.1.2/tests/gui/gui_model.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/tests/gui/test_gui.py` & `besser-1.1.2/tests/gui/test_gui.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/tests/object/library_object.py` & `besser-1.1.2/tests/object/library_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 # Library-Book association definition
 located_in: Property = Property(name="locatedIn",type=library, multiplicity=Multiplicity(1, 1))
 has: Property = Property(name="has", type=book, multiplicity=Multiplicity(0, "*"))
 lib_book_association: BinaryAssociation = BinaryAssociation(name="lib_book_assoc", ends={located_in, has})
 
 # Book-Author association definition
 publishes: Property = Property(name="publishes", type=book, multiplicity=Multiplicity(0, "*"))
-writed_by: Property = Property(name="writedBy", type=author, multiplicity=Multiplicity(1, "*"))
-book_author_association: BinaryAssociation = BinaryAssociation(name="book_author_assoc", ends={writed_by, publishes})
+written_by: Property = Property(name="writtenBy", type=author, multiplicity=Multiplicity(1, "*"))
+book_author_association: BinaryAssociation = BinaryAssociation(name="book_author_assoc", ends={written_by, publishes})
 
 constraintPageNumber: Constraint = Constraint(name = "libraryPageNumber",context=library,expression="context Library inv inv1: self.has ->forAll(b:Book|b.pages>0)",language="OCL")
 
 constraintBookPageNumber: Constraint = Constraint(name = "BookPageNumber",context=book,expression="context Book inv inv2: self.pages>0",language="OCL")
 
 constraintTitleIncorrect: Constraint = Constraint(name = "BookTitleInc",context=book,expression="context Book inv inv2: self.title= 'NI')",language="OCL")
 
@@ -133,25 +133,25 @@
 author_obj_name: AttributeLink = AttributeLink(attribute=author_name, value=DataValue(classifier=t_str, value="John Doe"))
 author_obj_email: AttributeLink = AttributeLink(attribute=email, value=DataValue(classifier=t_str, value="john@doe.com"))
 # Author object
 author_obj: Object = Object(name="Author Object", classifier=author, slots=[author_obj_name, author_obj_email])
 
 # Book object and Author object link
 book_link_end1: LinkEnd = LinkEnd(name="book_end1", association_end=publishes, object=book_obj)
-author_link_end: LinkEnd = LinkEnd(name="author_end", association_end=writed_by, object=author_obj)
+author_link_end: LinkEnd = LinkEnd(name="author_end", association_end=written_by, object=author_obj)
 author_book_link: Link = Link(name="author_book_link", association=book_author_association, connections=[book_link_end1,author_link_end])
 
 # Book Library and Book object link
 book_link_end2: LinkEnd = LinkEnd(name="book_end2", association_end=has, object=book_obj)
 library_link_end: LinkEnd = LinkEnd(name="library_end", association_end=located_in, object=library_obj)
 library_book_link: Link = Link(name="library_book_link", association=book_author_association, connections=[book_link_end2,library_link_end])
 
 # Book object and Author object link
 book_link_end2: LinkEnd = LinkEnd(name="book_end3", association_end=publishes, object=book_obj_2)
-author_link_end2: LinkEnd = LinkEnd(name="author_end2", association_end=writed_by, object=author_obj)
+author_link_end2: LinkEnd = LinkEnd(name="author_end2", association_end=written_by, object=author_obj)
 author_book_link2: Link = Link(name="author_book_link2", association=book_author_association, connections=[book_link_end2,author_link_end2])
 
 # Book Library and Book object link
 book_link_end3: LinkEnd = LinkEnd(name="book_end4", association_end=has, object=book_obj_2)
 library_link_end3: LinkEnd = LinkEnd(name="library_end3", association_end=located_in, object=library_obj)
 library_book_link3: Link = Link(name="library_book_link3", association=book_author_association, connections=[book_link_end3,library_link_end3])
```

### Comparing `besser-1.1.1/tests/object/test_object_mm.py` & `besser-1.1.2/tests/object/test_object_mm.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/tests/ocl/test_ocl_parser.py` & `besser-1.1.2/tests/ocl/test_ocl_parser.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.1/tests/structural/test_structural.py` & `besser-1.1.2/tests/structural/test_structural.py`

 * *Files identical despite different names*

