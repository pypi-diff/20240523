# Comparing `tmp/kimchima-0.5.1.tar.gz` & `tmp/kimchima-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kimchima-0.5.1.tar", max compression
+gzip compressed data, was "kimchima-0.5.2.tar", max compression
```

## Comparing `kimchima-0.5.1.tar` & `kimchima-0.5.2.tar`

### file list

```diff
@@ -1,31 +1,33 @@
--rw-r--r--   0        0        0    11343 2024-04-21 12:20:36.535643 kimchima-0.5.1/LICENSE
--rw-r--r--   0        0        0      908 2024-04-21 12:20:36.535643 kimchima-0.5.1/README.md
--rw-r--r--   0        0        0     2595 2024-04-21 12:20:36.535643 kimchima-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1091 2024-04-21 12:20:36.535643 kimchima-0.5.1/src/kimchima/__init__.py
--rw-r--r--   0        0        0        0 2024-04-21 12:20:36.535643 kimchima-0.5.1/src/kimchima/cmds/__init__.py
--rw-r--r--   0        0        0     1566 2024-04-21 12:20:36.535643 kimchima-0.5.1/src/kimchima/cmds/auto_cli.py
--rw-r--r--   0        0        0     1344 2024-04-21 12:20:36.535643 kimchima-0.5.1/src/kimchima/cmds/kimchima_cli.py
--rw-r--r--   0        0        0        0 2024-04-21 12:20:36.535643 kimchima-0.5.1/src/kimchima/models/__init__.py
--rw-r--r--   0        0        0     1284 2024-04-21 12:20:36.535643 kimchima-0.5.1/src/kimchima/pkg/__init__.py
--rw-r--r--   0        0        0     1669 2024-04-21 12:20:36.535643 kimchima-0.5.1/src/kimchima/pkg/chat_template_factory.py
--rw-r--r--   0        0        0     1598 2024-04-21 12:20:36.535643 kimchima-0.5.1/src/kimchima/pkg/devices.py
--rw-r--r--   0        0        0     3130 2024-04-21 12:20:36.535643 kimchima-0.5.1/src/kimchima/pkg/embedding_factory.py
--rw-r--r--   0        0        0     5564 2024-04-21 12:20:36.535643 kimchima-0.5.1/src/kimchima/pkg/logging.py
--rw-r--r--   0        0        0     5687 2024-04-21 12:20:36.535643 kimchima-0.5.1/src/kimchima/pkg/model_factory.py
--rw-r--r--   0        0        0     2665 2024-04-21 12:20:36.535643 kimchima-0.5.1/src/kimchima/pkg/pipelines_factory.py
--rw-r--r--   0        0        0     1821 2024-04-21 12:20:36.535643 kimchima-0.5.1/src/kimchima/pkg/quantization_factory.py
--rw-r--r--   0        0        0     2722 2024-04-21 12:20:36.535643 kimchima-0.5.1/src/kimchima/pkg/streamer_factory.py
--rw-r--r--   0        0        0     1660 2024-04-21 12:20:36.535643 kimchima-0.5.1/src/kimchima/pkg/tokenizer_factory.py
--rw-r--r--   0        0        0        0 2024-04-21 12:20:36.535643 kimchima-0.5.1/src/kimchima/tests/__init__.py
--rw-r--r--   0        0        0     2444 2024-04-21 12:20:36.535643 kimchima-0.5.1/src/kimchima/tests/test_chat_template_factory.py
--rw-r--r--   0        0        0     1818 2024-04-21 12:20:36.535643 kimchima-0.5.1/src/kimchima/tests/test_devices.py
--rw-r--r--   0        0        0     4307 2024-04-21 12:20:36.535643 kimchima-0.5.1/src/kimchima/tests/test_dialog.py
--rw-r--r--   0        0        0     3534 2024-04-21 12:20:36.535643 kimchima-0.5.1/src/kimchima/tests/test_downloadr.py
--rw-r--r--   0        0        0     2036 2024-04-21 12:20:36.535643 kimchima-0.5.1/src/kimchima/tests/test_embedding_factory.py
--rw-r--r--   0        0        0     1714 2024-04-21 12:20:36.535643 kimchima-0.5.1/src/kimchima/tests/test_model_factory.py
--rw-r--r--   0        0        0     3548 2024-04-21 12:20:36.535643 kimchima-0.5.1/src/kimchima/tests/test_pipelines_factory.py
--rw-r--r--   0        0        0     1084 2024-04-21 12:20:36.535643 kimchima-0.5.1/src/kimchima/tests/test_quantization_factory.py
--rw-r--r--   0        0        0      692 2024-04-21 12:20:36.535643 kimchima-0.5.1/src/kimchima/utils/__init__.py
--rw-r--r--   0        0        0     3694 2024-04-21 12:20:36.535643 kimchima-0.5.1/src/kimchima/utils/dialog.py
--rw-r--r--   0        0        0     5681 2024-04-21 12:20:36.535643 kimchima-0.5.1/src/kimchima/utils/downloader.py
--rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 kimchima-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11343 2024-05-23 15:22:19.160627 kimchima-0.5.2/LICENSE
+-rw-r--r--   0        0        0     1079 2024-05-23 15:22:19.160627 kimchima-0.5.2/README.md
+-rw-r--r--   0        0        0     2595 2024-05-23 15:22:19.160627 kimchima-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1118 2024-05-23 15:22:19.160627 kimchima-0.5.2/src/kimchima/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 15:22:19.160627 kimchima-0.5.2/src/kimchima/cmds/__init__.py
+-rw-r--r--   0        0        0     2866 2024-05-23 15:22:19.160627 kimchima-0.5.2/src/kimchima/cmds/auto_cli.py
+-rw-r--r--   0        0        0     1344 2024-05-23 15:22:19.160627 kimchima-0.5.2/src/kimchima/cmds/kimchima_cli.py
+-rw-r--r--   0        0        0        0 2024-05-23 15:22:19.160627 kimchima-0.5.2/src/kimchima/models/__init__.py
+-rw-r--r--   0        0        0     1366 2024-05-23 15:22:19.160627 kimchima-0.5.2/src/kimchima/pkg/__init__.py
+-rw-r--r--   0        0        0     1669 2024-05-23 15:22:19.160627 kimchima-0.5.2/src/kimchima/pkg/chat_template_factory.py
+-rw-r--r--   0        0        0    13702 2024-05-23 15:22:19.164627 kimchima-0.5.2/src/kimchima/pkg/cross_encoder_factory.py
+-rw-r--r--   0        0        0     1598 2024-05-23 15:22:19.164627 kimchima-0.5.2/src/kimchima/pkg/devices.py
+-rw-r--r--   0        0        0     3130 2024-05-23 15:22:19.164627 kimchima-0.5.2/src/kimchima/pkg/embedding_factory.py
+-rw-r--r--   0        0        0     5564 2024-05-23 15:22:19.164627 kimchima-0.5.2/src/kimchima/pkg/logging.py
+-rw-r--r--   0        0        0     5687 2024-05-23 15:22:19.164627 kimchima-0.5.2/src/kimchima/pkg/model_factory.py
+-rw-r--r--   0        0        0     2665 2024-05-23 15:22:19.164627 kimchima-0.5.2/src/kimchima/pkg/pipelines_factory.py
+-rw-r--r--   0        0        0     1821 2024-05-23 15:22:19.164627 kimchima-0.5.2/src/kimchima/pkg/quantization_factory.py
+-rw-r--r--   0        0        0     2722 2024-05-23 15:22:19.164627 kimchima-0.5.2/src/kimchima/pkg/streamer_factory.py
+-rw-r--r--   0        0        0     1660 2024-05-23 15:22:19.164627 kimchima-0.5.2/src/kimchima/pkg/tokenizer_factory.py
+-rw-r--r--   0        0        0        0 2024-05-23 15:22:19.164627 kimchima-0.5.2/src/kimchima/tests/__init__.py
+-rw-r--r--   0        0        0     2444 2024-05-23 15:22:19.164627 kimchima-0.5.2/src/kimchima/tests/test_chat_template_factory.py
+-rw-r--r--   0        0        0     1905 2024-05-23 15:22:19.164627 kimchima-0.5.2/src/kimchima/tests/test_cross_encoder_factory.py
+-rw-r--r--   0        0        0     1818 2024-05-23 15:22:19.164627 kimchima-0.5.2/src/kimchima/tests/test_devices.py
+-rw-r--r--   0        0        0     4307 2024-05-23 15:22:19.164627 kimchima-0.5.2/src/kimchima/tests/test_dialog.py
+-rw-r--r--   0        0        0     3534 2024-05-23 15:22:19.164627 kimchima-0.5.2/src/kimchima/tests/test_downloadr.py
+-rw-r--r--   0        0        0     2036 2024-05-23 15:22:19.164627 kimchima-0.5.2/src/kimchima/tests/test_embedding_factory.py
+-rw-r--r--   0        0        0     1714 2024-05-23 15:22:19.164627 kimchima-0.5.2/src/kimchima/tests/test_model_factory.py
+-rw-r--r--   0        0        0     3548 2024-05-23 15:22:19.164627 kimchima-0.5.2/src/kimchima/tests/test_pipelines_factory.py
+-rw-r--r--   0        0        0     1084 2024-05-23 15:22:19.164627 kimchima-0.5.2/src/kimchima/tests/test_quantization_factory.py
+-rw-r--r--   0        0        0      692 2024-05-23 15:22:19.164627 kimchima-0.5.2/src/kimchima/utils/__init__.py
+-rw-r--r--   0        0        0     3694 2024-05-23 15:22:19.164627 kimchima-0.5.2/src/kimchima/utils/dialog.py
+-rw-r--r--   0        0        0     5740 2024-05-23 15:22:19.164627 kimchima-0.5.2/src/kimchima/utils/downloader.py
+-rw-r--r--   0        0        0     1895 1970-01-01 00:00:00.000000 kimchima-0.5.2/PKG-INFO
```

### Comparing `kimchima-0.5.1/LICENSE` & `kimchima-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kimchima-0.5.1/README.md` & `kimchima-0.5.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # kimchima
 
 [![Backend CI/CD 🚀](https://github.com/Aisuko/kimchima/actions/workflows/ci.yml/badge.svg)](https://github.com/Aisuko/kimchima/actions/workflows/ci.yml)
 [![Release Drafter 🚀](https://github.com/Aisuko/kimchima/actions/workflows/release-drafter.yml/badge.svg)](https://github.com/Aisuko/kimchima/actions/workflows/release-drafter.yml)
+[![PyPI Release 🚀](https://github.com/SkywardAI/kimchima/actions/workflows/release.yml/badge.svg)](https://github.com/SkywardAI/kimchima/actions/workflows/release.yml)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 The collections of tools for ML model development.
 
 
 # Usage
```

### Comparing `kimchima-0.5.1/pyproject.toml` & `kimchima-0.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kimchima"
-version = "0.5.1"
+version = "0.5.2"
 description = "The collections of tools for ML model development."
 authors = ["Aisuko <urakiny@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/Aisuko/kimchi"
 repository = "https://github.com/Aisuko/kimchi"
 keywords = ["transformers", "pytorch"]
```

### Comparing `kimchima-0.5.1/src/kimchima/__init__.py` & `kimchima-0.5.2/src/kimchima/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
 from kimchima.utils import (
     Dialog,
     Downloader
     )
 
 __all__ = [
+    'CrossEncoderFactory',
     'ModelFactory', 
     'TokenizerFactory', 
     'EmbeddingsFactory',
     'QuantizationFactory',
     'StreamerFactory',
     'Devices',
     'PipelinesFactory',
```

### Comparing `kimchima-0.5.1/src/kimchima/cmds/kimchima_cli.py` & `kimchima-0.5.2/src/kimchima/cmds/kimchima_cli.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.5.1/src/kimchima/pkg/__init__.py` & `kimchima-0.5.2/src/kimchima/pkg/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,24 +13,26 @@
 # limitations under the License.
 
 
 # We want to import extra modules only in this module, let pkg module be a tool
 # module for the kimchima package.
 
 from .model_factory import ModelFactory
+from .cross_encoder_factory import CrossEncoderFactory
 from .tokenizer_factory import TokenizerFactory
 from .embedding_factory import EmbeddingsFactory
 from .quantization_factory import QuantizationFactory
 from .streamer_factory import StreamerFactory
 from .pipelines_factory import PipelinesFactory
 from .chat_template_factory import ChatTemplateFactory
 from .devices import Devices
 
 
 __all__ = [
+    'CrossEncoderFactory',
     'ModelFactory', 
     'TokenizerFactory', 
     'EmbeddingsFactory',
     'QuantizationFactory',
     'StreamerFactory',
     'PipelinesFactory',
     'ChatTemplateFactory',
```

### Comparing `kimchima-0.5.1/src/kimchima/pkg/chat_template_factory.py` & `kimchima-0.5.2/src/kimchima/pkg/chat_template_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.5.1/src/kimchima/pkg/devices.py` & `kimchima-0.5.2/src/kimchima/pkg/devices.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.5.1/src/kimchima/pkg/embedding_factory.py` & `kimchima-0.5.2/src/kimchima/pkg/embedding_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.5.1/src/kimchima/pkg/logging.py` & `kimchima-0.5.2/src/kimchima/pkg/logging.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.5.1/src/kimchima/pkg/model_factory.py` & `kimchima-0.5.2/src/kimchima/pkg/model_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.5.1/src/kimchima/pkg/pipelines_factory.py` & `kimchima-0.5.2/src/kimchima/pkg/pipelines_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.5.1/src/kimchima/pkg/quantization_factory.py` & `kimchima-0.5.2/src/kimchima/pkg/quantization_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.5.1/src/kimchima/pkg/streamer_factory.py` & `kimchima-0.5.2/src/kimchima/pkg/streamer_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.5.1/src/kimchima/pkg/tokenizer_factory.py` & `kimchima-0.5.2/src/kimchima/pkg/tokenizer_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.5.1/src/kimchima/tests/test_chat_template_factory.py` & `kimchima-0.5.2/src/kimchima/tests/test_chat_template_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.5.1/src/kimchima/tests/test_devices.py` & `kimchima-0.5.2/src/kimchima/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.5.1/src/kimchima/tests/test_dialog.py` & `kimchima-0.5.2/src/kimchima/tests/test_dialog.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.5.1/src/kimchima/tests/test_downloadr.py` & `kimchima-0.5.2/src/kimchima/tests/test_downloadr.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.5.1/src/kimchima/tests/test_embedding_factory.py` & `kimchima-0.5.2/src/kimchima/tests/test_embedding_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.5.1/src/kimchima/tests/test_model_factory.py` & `kimchima-0.5.2/src/kimchima/tests/test_model_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.5.1/src/kimchima/tests/test_pipelines_factory.py` & `kimchima-0.5.2/src/kimchima/tests/test_pipelines_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.5.1/src/kimchima/tests/test_quantization_factory.py` & `kimchima-0.5.2/src/kimchima/tests/test_quantization_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.5.1/src/kimchima/utils/__init__.py` & `kimchima-0.5.2/src/kimchima/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.5.1/src/kimchima/utils/dialog.py` & `kimchima-0.5.2/src/kimchima/utils/dialog.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.5.1/src/kimchima/utils/downloader.py` & `kimchima-0.5.2/src/kimchima/utils/downloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,16 +87,17 @@
 
         model_name=kwargs.pop("model_name", None)
         if model_name is None:
             raise ValueError("model_name is required")
         
         folder_name=kwargs.pop("folder_name", None)
         if folder_name is None:
-            #TODO folder_name equal to model_name will casue download issue
-            folder_name = model_name
+            raise ValueError("folder_name is required")
+        if model_name == folder_name:
+            raise ValueError("folder_name should not be equal to model_name")
 
         # save_pretrained only saves the model weights, not the configuration
         model=ModelFactory.auto_model(pretrained_model_name_or_path=model_name)
         model.save_pretrained(folder_name)
 
         tokenizer=TokenizerFactory.auto_tokenizer(pretrained_model_name_or_path=model_name)
         tokenizer.save_pretrained(folder_name + "/tmp1", legacy_format=False)
```

### Comparing `kimchima-0.5.1/PKG-INFO` & `kimchima-0.5.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kimchima
-Version: 0.5.1
+Version: 0.5.2
 Summary: The collections of tools for ML model development.
 Home-page: https://github.com/Aisuko/kimchi
 License: Apache-2.0
 Keywords: transformers,pytorch
 Author: Aisuko
 Author-email: urakiny@gmail.com
 Requires-Python: >=3.11,<4.0
@@ -21,14 +21,15 @@
 Project-URL: Repository, https://github.com/Aisuko/kimchi
 Description-Content-Type: text/markdown
 
 # kimchima
 
 [![Backend CI/CD 🚀](https://github.com/Aisuko/kimchima/actions/workflows/ci.yml/badge.svg)](https://github.com/Aisuko/kimchima/actions/workflows/ci.yml)
 [![Release Drafter 🚀](https://github.com/Aisuko/kimchima/actions/workflows/release-drafter.yml/badge.svg)](https://github.com/Aisuko/kimchima/actions/workflows/release-drafter.yml)
+[![PyPI Release 🚀](https://github.com/SkywardAI/kimchima/actions/workflows/release.yml/badge.svg)](https://github.com/SkywardAI/kimchima/actions/workflows/release.yml)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 The collections of tools for ML model development.
 
 
 # Usage
```

