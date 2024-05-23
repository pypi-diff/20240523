# Comparing `tmp/foundationallm-0.7.1.tar.gz` & `tmp/foundationallm-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foundationallm-0.7.1.tar", last modified: Fri May  3 19:45:17 2024, max compression
+gzip compressed data, was "foundationallm-0.7.2.tar", last modified: Thu May 23 11:21:01 2024, max compression
```

## Comparing `foundationallm-0.7.1.tar` & `foundationallm-0.7.2.tar`

### file list

```diff
@@ -1,96 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 19:45:17.111750 foundationallm-0.7.1/
--rw-rw-rw-   0        0        0      201 2024-05-03 10:37:29.000000 foundationallm-0.7.1/LICENSE
--rw-rw-rw-   0        0        0      633 2024-05-03 19:45:17.110754 foundationallm-0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0       88 2024-05-03 10:38:21.000000 foundationallm-0.7.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 19:45:16.692295 foundationallm-0.7.1/env/
-drwxrwxrwx   0        0        0        0 2024-05-03 19:45:16.692295 foundationallm-0.7.1/env/Lib/
-drwxrwxrwx   0        0        0        0 2024-05-03 19:45:16.695287 foundationallm-0.7.1/env/Lib/site-packages/
-drwxrwxrwx   0        0        0        0 2024-05-03 19:45:16.692295 foundationallm-0.7.1/env/Lib/site-packages/effdet/
-drwxrwxrwx   0        0        0        0 2024-05-03 19:45:16.733390 foundationallm-0.7.1/env/Lib/site-packages/effdet/config/
--rw-rw-rw-   0        0        0      247 2024-03-03 18:44:27.000000 foundationallm-0.7.1/env/Lib/site-packages/effdet/config/__init__.py
--rw-rw-rw-   0        0        0      178 2024-03-03 18:44:27.000000 foundationallm-0.7.1/env/Lib/site-packages/effdet/config/config_utils.py
--rw-rw-rw-   0        0        0     6758 2024-03-03 18:44:27.000000 foundationallm-0.7.1/env/Lib/site-packages/effdet/config/fpn_config.py
--rw-rw-rw-   0        0        0    26363 2024-03-03 18:44:27.000000 foundationallm-0.7.1/env/Lib/site-packages/effdet/config/model_config.py
--rw-rw-rw-   0        0        0      798 2024-03-03 18:44:27.000000 foundationallm-0.7.1/env/Lib/site-packages/effdet/config/train_config.py
-drwxrwxrwx   0        0        0        0 2024-05-03 19:45:16.693292 foundationallm-0.7.1/env/Lib/site-packages/fontTools/
-drwxrwxrwx   0        0        0        0 2024-05-03 19:45:16.739434 foundationallm-0.7.1/env/Lib/site-packages/fontTools/config/
--rw-rw-rw-   0        0        0     2718 2024-03-03 18:42:07.000000 foundationallm-0.7.1/env/Lib/site-packages/fontTools/config/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 19:45:16.693292 foundationallm-0.7.1/env/Lib/site-packages/pandas/
-drwxrwxrwx   0        0        0        0 2024-05-03 19:45:16.772483 foundationallm-0.7.1/env/Lib/site-packages/pandas/_config/
--rw-rw-rw-   0        0        0     1179 2024-03-03 18:43:15.000000 foundationallm-0.7.1/env/Lib/site-packages/pandas/_config/__init__.py
--rw-rw-rw-   0        0        0    25435 2024-03-03 18:43:15.000000 foundationallm-0.7.1/env/Lib/site-packages/pandas/_config/config.py
--rw-rw-rw-   0        0        0      668 2024-03-03 18:43:15.000000 foundationallm-0.7.1/env/Lib/site-packages/pandas/_config/dates.py
--rw-rw-rw-   0        0        0     1804 2024-03-03 18:43:15.000000 foundationallm-0.7.1/env/Lib/site-packages/pandas/_config/display.py
--rw-rw-rw-   0        0        0     5190 2024-03-03 18:43:15.000000 foundationallm-0.7.1/env/Lib/site-packages/pandas/_config/localization.py
-drwxrwxrwx   0        0        0        0 2024-05-03 19:45:16.694291 foundationallm-0.7.1/env/Lib/site-packages/pandas/tests/
-drwxrwxrwx   0        0        0        0 2024-05-03 19:45:16.791474 foundationallm-0.7.1/env/Lib/site-packages/pandas/tests/config/
--rw-rw-rw-   0        0        0        0 2024-03-03 18:43:14.000000 foundationallm-0.7.1/env/Lib/site-packages/pandas/tests/config/__init__.py
--rw-rw-rw-   0        0        0    15858 2024-03-03 18:43:14.000000 foundationallm-0.7.1/env/Lib/site-packages/pandas/tests/config/test_config.py
--rw-rw-rw-   0        0        0     4479 2024-03-03 18:43:14.000000 foundationallm-0.7.1/env/Lib/site-packages/pandas/tests/config/test_localization.py
-drwxrwxrwx   0        0        0        0 2024-05-03 19:45:16.694291 foundationallm-0.7.1/env/Lib/site-packages/pylint/
-drwxrwxrwx   0        0        0        0 2024-05-03 19:45:16.884487 foundationallm-0.7.1/env/Lib/site-packages/pylint/config/
--rw-rw-rw-   0        0        0      387 2024-03-03 18:42:29.000000 foundationallm-0.7.1/env/Lib/site-packages/pylint/config/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 19:45:16.927090 foundationallm-0.7.1/env/Lib/site-packages/pylint/config/_pylint_config/
--rw-rw-rw-   0        0        0      571 2024-03-03 18:42:29.000000 foundationallm-0.7.1/env/Lib/site-packages/pylint/config/_pylint_config/__init__.py
--rw-rw-rw-   0        0        0     1718 2024-03-03 18:42:29.000000 foundationallm-0.7.1/env/Lib/site-packages/pylint/config/_pylint_config/generate_command.py
--rw-rw-rw-   0        0        0     2007 2024-03-03 18:42:29.000000 foundationallm-0.7.1/env/Lib/site-packages/pylint/config/_pylint_config/help_message.py
--rw-rw-rw-   0        0        0      855 2024-03-03 18:42:29.000000 foundationallm-0.7.1/env/Lib/site-packages/pylint/config/_pylint_config/main.py
--rw-rw-rw-   0        0        0     1613 2024-03-03 18:42:29.000000 foundationallm-0.7.1/env/Lib/site-packages/pylint/config/_pylint_config/setup.py
--rw-rw-rw-   0        0        0     3662 2024-03-03 18:42:29.000000 foundationallm-0.7.1/env/Lib/site-packages/pylint/config/_pylint_config/utils.py
--rw-rw-rw-   0        0        0    14816 2024-03-03 18:42:29.000000 foundationallm-0.7.1/env/Lib/site-packages/pylint/config/argument.py
--rw-rw-rw-   0        0        0    15085 2024-03-03 18:42:29.000000 foundationallm-0.7.1/env/Lib/site-packages/pylint/config/arguments_manager.py
--rw-rw-rw-   0        0        0     2392 2024-03-03 18:42:29.000000 foundationallm-0.7.1/env/Lib/site-packages/pylint/config/arguments_provider.py
--rw-rw-rw-   0        0        0    13391 2024-03-03 18:42:29.000000 foundationallm-0.7.1/env/Lib/site-packages/pylint/config/callback_actions.py
--rw-rw-rw-   0        0        0     4532 2024-03-03 18:42:29.000000 foundationallm-0.7.1/env/Lib/site-packages/pylint/config/config_file_parser.py
--rw-rw-rw-   0        0        0     7316 2024-03-03 18:42:29.000000 foundationallm-0.7.1/env/Lib/site-packages/pylint/config/config_initialization.py
--rw-rw-rw-   0        0        0     2983 2024-03-03 18:42:29.000000 foundationallm-0.7.1/env/Lib/site-packages/pylint/config/deprecation_actions.py
--rw-rw-rw-   0        0        0      826 2024-03-03 18:42:29.000000 foundationallm-0.7.1/env/Lib/site-packages/pylint/config/exceptions.py
--rw-rw-rw-   0        0        0     4423 2024-03-03 18:42:29.000000 foundationallm-0.7.1/env/Lib/site-packages/pylint/config/find_default_config_files.py
--rw-rw-rw-   0        0        0     2583 2024-03-03 18:42:29.000000 foundationallm-0.7.1/env/Lib/site-packages/pylint/config/help_formatter.py
--rw-rw-rw-   0        0        0     8774 2024-03-03 18:42:29.000000 foundationallm-0.7.1/env/Lib/site-packages/pylint/config/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-03 19:45:16.695287 foundationallm-0.7.1/env/Lib/site-packages/setuptools/
-drwxrwxrwx   0        0        0        0 2024-05-03 19:45:16.961627 foundationallm-0.7.1/env/Lib/site-packages/setuptools/config/
--rw-rw-rw-   0        0        0     1121 2024-03-03 18:39:26.000000 foundationallm-0.7.1/env/Lib/site-packages/setuptools/config/__init__.py
--rw-rw-rw-   0        0        0    13398 2024-03-03 18:39:26.000000 foundationallm-0.7.1/env/Lib/site-packages/setuptools/config/_apply_pyprojecttoml.py
--rw-rw-rw-   0        0        0    16319 2024-03-03 18:39:26.000000 foundationallm-0.7.1/env/Lib/site-packages/setuptools/config/expand.py
--rw-rw-rw-   0        0        0    19304 2024-03-03 18:39:26.000000 foundationallm-0.7.1/env/Lib/site-packages/setuptools/config/pyprojecttoml.py
--rw-rw-rw-   0        0        0    25198 2024-03-03 18:39:26.000000 foundationallm-0.7.1/env/Lib/site-packages/setuptools/config/setupcfg.py
-drwxrwxrwx   0        0        0        0 2024-05-03 19:45:16.695287 foundationallm-0.7.1/env/Lib/site-packages/torch/
-drwxrwxrwx   0        0        0        0 2024-05-03 19:45:16.695287 foundationallm-0.7.1/env/Lib/site-packages/torch/ao/
-drwxrwxrwx   0        0        0        0 2024-05-03 19:45:16.696284 foundationallm-0.7.1/env/Lib/site-packages/torch/ao/quantization/
-drwxrwxrwx   0        0        0        0 2024-05-03 19:45:17.037929 foundationallm-0.7.1/env/Lib/site-packages/torch/ao/quantization/backend_config/
--rw-rw-rw-   0        0        0      912 2024-03-03 18:42:57.000000 foundationallm-0.7.1/env/Lib/site-packages/torch/ao/quantization/backend_config/__init__.py
--rw-rw-rw-   0        0        0    27710 2024-03-03 18:42:57.000000 foundationallm-0.7.1/env/Lib/site-packages/torch/ao/quantization/backend_config/_common_operator_config_utils.py
--rw-rw-rw-   0        0        0     6466 2024-03-03 18:42:57.000000 foundationallm-0.7.1/env/Lib/site-packages/torch/ao/quantization/backend_config/_qnnpack_pt2e.py
--rw-rw-rw-   0        0        0    31124 2024-03-03 18:42:57.000000 foundationallm-0.7.1/env/Lib/site-packages/torch/ao/quantization/backend_config/backend_config.py
--rw-rw-rw-   0        0        0    17447 2024-03-03 18:42:57.000000 foundationallm-0.7.1/env/Lib/site-packages/torch/ao/quantization/backend_config/executorch.py
--rw-rw-rw-   0        0        0     4239 2024-03-03 18:42:57.000000 foundationallm-0.7.1/env/Lib/site-packages/torch/ao/quantization/backend_config/fbgemm.py
--rw-rw-rw-   0        0        0     8252 2024-03-03 18:42:57.000000 foundationallm-0.7.1/env/Lib/site-packages/torch/ao/quantization/backend_config/native.py
--rw-rw-rw-   0        0        0        0 2024-03-03 18:42:57.000000 foundationallm-0.7.1/env/Lib/site-packages/torch/ao/quantization/backend_config/observation_type.py
--rw-rw-rw-   0        0        0    19692 2024-03-03 18:42:57.000000 foundationallm-0.7.1/env/Lib/site-packages/torch/ao/quantization/backend_config/onednn.py
--rw-rw-rw-   0        0        0     5499 2024-03-03 18:42:57.000000 foundationallm-0.7.1/env/Lib/site-packages/torch/ao/quantization/backend_config/qnnpack.py
--rw-rw-rw-   0        0        0     2964 2024-03-03 18:42:57.000000 foundationallm-0.7.1/env/Lib/site-packages/torch/ao/quantization/backend_config/tensorrt.py
--rw-rw-rw-   0        0        0    12621 2024-03-03 18:42:57.000000 foundationallm-0.7.1/env/Lib/site-packages/torch/ao/quantization/backend_config/utils.py
--rw-rw-rw-   0        0        0     3897 2024-03-03 18:42:57.000000 foundationallm-0.7.1/env/Lib/site-packages/torch/ao/quantization/backend_config/x86.py
-drwxrwxrwx   0        0        0        0 2024-05-03 19:45:16.697282 foundationallm-0.7.1/foundationallm/
-drwxrwxrwx   0        0        0        0 2024-05-03 19:45:17.075847 foundationallm-0.7.1/foundationallm/config/
--rw-rw-rw-   0        0        0      177 2024-03-03 18:33:11.000000 foundationallm-0.7.1/foundationallm/config/__init__.py
--rw-rw-rw-   0        0        0     4874 2024-03-03 18:33:11.000000 foundationallm-0.7.1/foundationallm/config/configuration.py
--rw-rw-rw-   0        0        0      605 2024-03-03 18:33:11.000000 foundationallm-0.7.1/foundationallm/config/context.py
--rw-rw-rw-   0        0        0      378 2024-03-05 18:20:28.000000 foundationallm-0.7.1/foundationallm/config/environment_variables.py
--rw-rw-rw-   0        0        0      556 2024-03-03 18:33:11.000000 foundationallm-0.7.1/foundationallm/config/user_identity.py
-drwxrwxrwx   0        0        0        0 2024-05-03 19:45:16.697282 foundationallm-0.7.1/foundationallm/models/
-drwxrwxrwx   0        0        0        0 2024-05-03 19:45:17.108783 foundationallm-0.7.1/foundationallm/models/orchestration/
--rw-rw-rw-   0        0        0      308 2024-05-03 19:44:44.000000 foundationallm-0.7.1/foundationallm/models/orchestration/__init__.py
--rw-rw-rw-   0        0        0      272 2024-04-16 19:16:39.000000 foundationallm-0.7.1/foundationallm/models/orchestration/citation.py
--rw-rw-rw-   0        0        0      464 2024-05-03 09:01:18.000000 foundationallm-0.7.1/foundationallm/models/orchestration/completion_request_base.py
--rw-rw-rw-   0        0        0      523 2024-04-16 19:16:39.000000 foundationallm-0.7.1/foundationallm/models/orchestration/completion_response.py
--rw-rw-rw-   0        0        0      370 2024-03-03 18:33:11.000000 foundationallm-0.7.1/foundationallm/models/orchestration/message_history_item.py
--rw-rw-rw-   0        0        0      838 2024-05-03 09:01:18.000000 foundationallm-0.7.1/foundationallm/models/orchestration/orchestration_settings.py
-drwxrwxrwx   0        0        0        0 2024-05-03 19:45:17.109756 foundationallm-0.7.1/foundationallm.egg-info/
--rw-rw-rw-   0        0        0      633 2024-05-03 19:45:16.000000 foundationallm-0.7.1/foundationallm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3702 2024-05-03 19:45:16.000000 foundationallm-0.7.1/foundationallm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 19:45:16.000000 foundationallm-0.7.1/foundationallm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-03 19:45:16.000000 foundationallm-0.7.1/foundationallm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      614 2024-05-03 19:44:57.000000 foundationallm-0.7.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-03 19:45:17.111750 foundationallm-0.7.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-23 11:21:01.044038 foundationallm-0.7.2/
+-rw-rw-rw-   0        0        0      201 2024-05-07 13:15:07.000000 foundationallm-0.7.2/LICENSE
+-rw-rw-rw-   0        0        0      633 2024-05-23 11:21:01.043037 foundationallm-0.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0       88 2024-05-07 13:15:07.000000 foundationallm-0.7.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 11:21:00.929906 foundationallm-0.7.2/foundationallm/
+drwxrwxrwx   0        0        0        0 2024-05-23 11:21:00.987907 foundationallm-0.7.2/foundationallm/config/
+-rw-rw-rw-   0        0        0      177 2023-12-14 16:50:30.000000 foundationallm-0.7.2/foundationallm/config/__init__.py
+-rw-rw-rw-   0        0        0     4874 2024-05-23 11:10:06.000000 foundationallm-0.7.2/foundationallm/config/configuration.py
+-rw-rw-rw-   0        0        0      605 2023-12-14 16:50:30.000000 foundationallm-0.7.2/foundationallm/config/context.py
+-rw-rw-rw-   0        0        0      378 2024-03-15 16:01:06.000000 foundationallm-0.7.2/foundationallm/config/environment_variables.py
+-rw-rw-rw-   0        0        0      556 2023-12-14 16:50:30.000000 foundationallm-0.7.2/foundationallm/config/user_identity.py
+drwxrwxrwx   0        0        0        0 2024-05-23 11:21:00.930906 foundationallm-0.7.2/foundationallm/models/
+drwxrwxrwx   0        0        0        0 2024-05-23 11:21:01.039037 foundationallm-0.7.2/foundationallm/models/orchestration/
+-rw-rw-rw-   0        0        0      357 2024-05-07 13:15:07.000000 foundationallm-0.7.2/foundationallm/models/orchestration/__init__.py
+-rw-rw-rw-   0        0        0      272 2024-04-24 17:34:13.000000 foundationallm-0.7.2/foundationallm/models/orchestration/citation.py
+-rw-rw-rw-   0        0        0      502 2024-05-07 13:15:07.000000 foundationallm-0.7.2/foundationallm/models/orchestration/completion_request_base.py
+-rw-rw-rw-   0        0        0      523 2024-04-24 17:34:13.000000 foundationallm-0.7.2/foundationallm/models/orchestration/completion_response.py
+-rw-rw-rw-   0        0        0      479 2024-05-07 13:15:07.000000 foundationallm-0.7.2/foundationallm/models/orchestration/endpoint_settings.py
+-rw-rw-rw-   0        0        0      370 2023-12-14 16:50:30.000000 foundationallm-0.7.2/foundationallm/models/orchestration/message_history_item.py
+-rw-rw-rw-   0        0        0      939 2024-05-07 13:15:07.000000 foundationallm-0.7.2/foundationallm/models/orchestration/orchestration_settings.py
+drwxrwxrwx   0        0        0        0 2024-05-23 11:21:01.041038 foundationallm-0.7.2/foundationallm.egg-info/
+-rw-rw-rw-   0        0        0      633 2024-05-23 11:21:00.000000 foundationallm-0.7.2/foundationallm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2024-05-23 11:21:00.000000 foundationallm-0.7.2/foundationallm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 11:21:00.000000 foundationallm-0.7.2/foundationallm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-23 11:21:00.000000 foundationallm-0.7.2/foundationallm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      614 2024-05-23 11:20:33.000000 foundationallm-0.7.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-23 11:21:01.044038 foundationallm-0.7.2/setup.cfg
```

### Comparing `foundationallm-0.7.1/PKG-INFO` & `foundationallm-0.7.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foundationallm
-Version: 0.7.1
+Version: 0.7.2
 Summary: Enables integration with the FoundationaLLM platform.
 Author-email: FoundationaLLM <dev@foundationallm.ai>
 Project-URL: Homepage, https://foundationallm.ai
 Project-URL: Issues, https://github.com/solliancenet/foundationallm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `foundationallm-0.7.1/foundationallm/config/configuration.py` & `foundationallm-0.7.2/foundationallm/config/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 )
 from azure.identity import DefaultAzureCredential
 
 class Configuration():
     def __init__(self):
         """Init"""
         try:
-            app_config_uri = os.environ['foundationallm-app-configuration-uri']
+            app_config_uri = os.environ['FOUNDATIONALLM_APP_CONFIGURATION_URI']
         except Exception as e:
             raise e
 
         credential = DefaultAzureCredential(
             exclude_environment_credential=True)
 
         # Connect to Azure App Configuration.
```

### Comparing `foundationallm-0.7.1/foundationallm/config/context.py` & `foundationallm-0.7.2/foundationallm/config/context.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.1/foundationallm/config/user_identity.py` & `foundationallm-0.7.2/foundationallm/config/user_identity.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.1/foundationallm/models/orchestration/completion_response.py` & `foundationallm-0.7.2/foundationallm/models/orchestration/completion_response.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.1/foundationallm.egg-info/PKG-INFO` & `foundationallm-0.7.2/foundationallm.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foundationallm
-Version: 0.7.1
+Version: 0.7.2
 Summary: Enables integration with the FoundationaLLM platform.
 Author-email: FoundationaLLM <dev@foundationallm.ai>
 Project-URL: Homepage, https://foundationallm.ai
 Project-URL: Issues, https://github.com/solliancenet/foundationallm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `foundationallm-0.7.1/pyproject.toml` & `foundationallm-0.7.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "foundationallm"
-version = "0.7.1"
+version = "0.7.2"
 authors = [
   { name="FoundationaLLM", email="dev@foundationallm.ai" },
 ]
 description = "Enables integration with the FoundationaLLM platform."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

