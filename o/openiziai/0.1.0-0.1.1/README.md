# Comparing `tmp/openiziai-0.1.0.tar.gz` & `tmp/openiziai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openiziai-0.1.0.tar", max compression
+gzip compressed data, was "openiziai-0.1.1.tar", max compression
```

## Comparing `openiziai-0.1.0.tar` & `openiziai-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1088 2024-05-21 22:32:24.881445 openiziai-0.1.0/LICENSE
--rw-r--r--   0        0        0     5263 2024-05-21 22:32:24.881445 openiziai-0.1.0/README.md
--rw-r--r--   0        0        0      186 2024-05-21 22:32:24.881445 openiziai-0.1.0/openiziai/__init__.py
--rw-r--r--   0        0        0      158 2024-05-21 22:32:24.881445 openiziai-0.1.0/openiziai/agents/__init__.py
--rw-r--r--   0        0        0     5661 2024-05-21 22:32:24.881445 openiziai-0.1.0/openiziai/agents/agent.py
--rw-r--r--   0        0        0     2656 2024-05-21 22:32:24.881445 openiziai-0.1.0/openiziai/agents/manager.py
--rw-r--r--   0        0        0      149 2024-05-21 22:32:24.881445 openiziai-0.1.0/openiziai/contexts/__init__.py
--rw-r--r--   0        0        0      417 2024-05-21 22:32:24.881445 openiziai-0.1.0/openiziai/contexts/contexts.py
--rw-r--r--   0        0        0     2341 2024-05-21 22:32:24.881445 openiziai-0.1.0/openiziai/contexts/handler.py
--rw-r--r--   0        0        0     4933 2024-05-21 22:32:24.881445 openiziai-0.1.0/openiziai/fine_tuning.py
--rw-r--r--   0        0        0      953 2024-05-21 22:32:24.881445 openiziai-0.1.0/openiziai/schemas.py
--rw-r--r--   0        0        0      242 2024-05-21 22:32:24.881445 openiziai-0.1.0/openiziai/task.py
--rw-r--r--   0        0        0      193 2024-05-21 22:32:24.881445 openiziai-0.1.0/openiziai/tools/__init__.py
--rw-r--r--   0        0        0      992 2024-05-21 22:32:24.881445 openiziai-0.1.0/openiziai/tools/prep_data.py
--rw-r--r--   0        0        0    11162 2024-05-21 22:32:24.881445 openiziai-0.1.0/openiziai/tools/train_data.py
--rw-r--r--   0        0        0      855 2024-05-21 22:32:24.881445 openiziai-0.1.0/openiziai/utils.py
--rw-r--r--   0        0        0     1703 2024-05-21 22:32:24.881445 openiziai-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6420 1970-01-01 00:00:00.000000 openiziai-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1088 2024-05-23 13:42:39.752021 openiziai-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5375 2024-05-23 13:42:39.752021 openiziai-0.1.1/README.md
+-rw-r--r--   0        0        0      186 2024-05-23 13:42:39.756021 openiziai-0.1.1/openiziai/__init__.py
+-rw-r--r--   0        0        0      158 2024-05-23 13:42:39.756021 openiziai-0.1.1/openiziai/agents/__init__.py
+-rw-r--r--   0        0        0     5532 2024-05-23 13:42:39.756021 openiziai-0.1.1/openiziai/agents/agent.py
+-rw-r--r--   0        0        0     2656 2024-05-23 13:42:39.756021 openiziai-0.1.1/openiziai/agents/manager.py
+-rw-r--r--   0        0        0      149 2024-05-23 13:42:39.756021 openiziai-0.1.1/openiziai/contexts/__init__.py
+-rw-r--r--   0        0        0      417 2024-05-23 13:42:39.756021 openiziai-0.1.1/openiziai/contexts/contexts.py
+-rw-r--r--   0        0        0     2341 2024-05-23 13:42:39.756021 openiziai-0.1.1/openiziai/contexts/handler.py
+-rw-r--r--   0        0        0     4933 2024-05-23 13:42:39.756021 openiziai-0.1.1/openiziai/fine_tuning.py
+-rw-r--r--   0        0        0      953 2024-05-23 13:42:39.756021 openiziai-0.1.1/openiziai/schemas.py
+-rw-r--r--   0        0        0      242 2024-05-23 13:42:39.756021 openiziai-0.1.1/openiziai/task.py
+-rw-r--r--   0        0        0      193 2024-05-23 13:42:39.756021 openiziai-0.1.1/openiziai/tools/__init__.py
+-rw-r--r--   0        0        0      992 2024-05-23 13:42:39.756021 openiziai-0.1.1/openiziai/tools/prep_data.py
+-rw-r--r--   0        0        0    11162 2024-05-23 13:42:39.756021 openiziai-0.1.1/openiziai/tools/train_data.py
+-rw-r--r--   0        0        0      855 2024-05-23 13:42:39.756021 openiziai-0.1.1/openiziai/utils.py
+-rw-r--r--   0        0        0     1703 2024-05-23 13:42:39.756021 openiziai-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6532 1970-01-01 00:00:00.000000 openiziai-0.1.1/PKG-INFO
```

### Comparing `openiziai-0.1.0/LICENSE` & `openiziai-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openiziai-0.1.0/README.md` & `openiziai-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 # OPENIZIAI
 
 ![Static Badge](https://img.shields.io/badge/python-3.11%7C3.12-blue)
 [![CI](https://github.com/RWallan/openiziai/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/RWallan/openiziai/actions/workflows/ci.yaml)
 [![codecov](https://codecov.io/github/RWallan/openiziai/branch/main/graph/badge.svg?token=FYZ1IOHC9Y)](https://codecov.io/github/RWallan/openiziai)
 ![GitHub License](https://img.shields.io/github/license/RWallan/openiziai)
+![PyPI - Version](https://img.shields.io/pypi/v/openiziai)
 
 O projeto ainda está em suas primeiras versões. Isso significa que o projeto está em constante mudanças e todo feedback é bem vindo!
 
 ### Utilize seus modelos LLM com o que quiser e como quiser
 
 OpeniziAI é um projeto que disponibiliza uma interface que implementa práticas de _prompt enginnering_ para ser capaz de:
 
 - Criar dados de treino para fine tuning
 
 - Aplicar fine tuning nos seus dados
 
 - Criar agentes especializados
 
+## Como instalar
+
+```bash
+pip install openiziai
+```
+
 ## Como usar
 
 ```python
 import openiziai # Importe a biblioteca
 from openai import OpenAI
 
 client = OpenAI() # Instancie o client da OpenAI com seu token
```

### Comparing `openiziai-0.1.0/openiziai/agents/agent.py` & `openiziai-0.1.1/openiziai/agents/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,32 +130,27 @@
             max_tokens (int): Máximo de tokens que deve conter nas respostas.
                 Valores maiores trarão respostas maiores porém terá maior
                 custo.
 
         Returns:
             PromptResponse: Informações do prompt construído.
         """
+        messages = [{'role': 'system', 'content': self._template}]
         if history:
             _history = [m.model_dump() for m in history]
-            messages = [{'role': 'system', 'content': self._template}].extend(
-                _history
-            )
+            messages.extend(_history)
             _prompt = _history[-1].get('content')
         elif prompt:
             _prompt = prompt
-            messages = [
-                {
-                    'role': 'system',
-                    'content': self._template,
-                },
+            messages.extend([
                 {
                     'role': 'user',
                     'content': _prompt,
                 },
-            ]
+            ])
         else:
             raise ValueError('`prompt` ou `history` precisam ser passados.')
 
         result = self.client.chat.completions.create(
             messages=messages,  # pyright: ignore
             model=self._fine_tuned_model,
             temperature=temperature,
```

### Comparing `openiziai-0.1.0/openiziai/agents/manager.py` & `openiziai-0.1.1/openiziai/agents/manager.py`

 * *Files identical despite different names*

### Comparing `openiziai-0.1.0/openiziai/contexts/handler.py` & `openiziai-0.1.1/openiziai/contexts/handler.py`

 * *Files identical despite different names*

### Comparing `openiziai-0.1.0/openiziai/fine_tuning.py` & `openiziai-0.1.1/openiziai/fine_tuning.py`

 * *Files identical despite different names*

### Comparing `openiziai-0.1.0/openiziai/schemas.py` & `openiziai-0.1.1/openiziai/schemas.py`

 * *Files identical despite different names*

### Comparing `openiziai-0.1.0/openiziai/tools/prep_data.py` & `openiziai-0.1.1/openiziai/tools/prep_data.py`

 * *Files identical despite different names*

### Comparing `openiziai-0.1.0/openiziai/tools/train_data.py` & `openiziai-0.1.1/openiziai/tools/train_data.py`

 * *Files identical despite different names*

### Comparing `openiziai-0.1.0/openiziai/utils.py` & `openiziai-0.1.1/openiziai/utils.py`

 * *Files identical despite different names*

### Comparing `openiziai-0.1.0/pyproject.toml` & `openiziai-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openiziai"
-version = "0.1.0"
+version = "0.1.1"
 description = "Interface para se comunicar com a api da OpenAI adotando as melhores práticas de LLM para criar e se comunicar com um agente."
 authors = ["RWallan <3am.richardwallan@gmail.com>"]
 readme = "README.md"
 packages = [{include = "openiziai"}]
 license = "MIT"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `openiziai-0.1.0/PKG-INFO` & `openiziai-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openiziai
-Version: 0.1.0
+Version: 0.1.1
 Summary: Interface para se comunicar com a api da OpenAI adotando as melhores práticas de LLM para criar e se comunicar com um agente.
 License: MIT
 Author: RWallan
 Author-email: 3am.richardwallan@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -26,27 +26,34 @@
 
 # OPENIZIAI
 
 ![Static Badge](https://img.shields.io/badge/python-3.11%7C3.12-blue)
 [![CI](https://github.com/RWallan/openiziai/actions/workflows/ci.yaml/badge.svg?branch=main)](https://github.com/RWallan/openiziai/actions/workflows/ci.yaml)
 [![codecov](https://codecov.io/github/RWallan/openiziai/branch/main/graph/badge.svg?token=FYZ1IOHC9Y)](https://codecov.io/github/RWallan/openiziai)
 ![GitHub License](https://img.shields.io/github/license/RWallan/openiziai)
+![PyPI - Version](https://img.shields.io/pypi/v/openiziai)
 
 O projeto ainda está em suas primeiras versões. Isso significa que o projeto está em constante mudanças e todo feedback é bem vindo!
 
 ### Utilize seus modelos LLM com o que quiser e como quiser
 
 OpeniziAI é um projeto que disponibiliza uma interface que implementa práticas de _prompt enginnering_ para ser capaz de:
 
 - Criar dados de treino para fine tuning
 
 - Aplicar fine tuning nos seus dados
 
 - Criar agentes especializados
 
+## Como instalar
+
+```bash
+pip install openiziai
+```
+
 ## Como usar
 
 ```python
 import openiziai # Importe a biblioteca
 from openai import OpenAI
 
 client = OpenAI() # Instancie o client da OpenAI com seu token
```

