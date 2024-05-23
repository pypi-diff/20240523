# Comparing `tmp/sentier_glossary-0.5.1.tar.gz` & `tmp/sentier_glossary-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentier_glossary-0.5.1.tar", last modified: Thu May 23 19:49:05 2024, max compression
+gzip compressed data, was "sentier_glossary-0.5.2.tar", last modified: Thu May 23 21:02:08 2024, max compression
```

## Comparing `sentier_glossary-0.5.1.tar` & `sentier_glossary-0.5.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:49:05.968238 sentier_glossary-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-23 19:49:02.000000 sentier_glossary-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:49:02.000000 sentier_glossary-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-05-23 19:49:05.968238 sentier_glossary-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-05-23 19:49:02.000000 sentier_glossary-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-23 19:49:02.000000 sentier_glossary-0.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:49:05.968238 sentier_glossary-0.5.1/sentier_glossary/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-23 19:49:02.000000 sentier_glossary-0.5.1/sentier_glossary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10351 2024-05-23 19:49:02.000000 sentier_glossary-0.5.1/sentier_glossary/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-23 19:49:02.000000 sentier_glossary-0.5.1/sentier_glossary/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:49:05.968238 sentier_glossary-0.5.1/sentier_glossary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-05-23 19:49:05.000000 sentier_glossary-0.5.1/sentier_glossary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-23 19:49:05.000000 sentier_glossary-0.5.1/sentier_glossary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 19:49:05.000000 sentier_glossary-0.5.1/sentier_glossary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-23 19:49:05.000000 sentier_glossary-0.5.1/sentier_glossary.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-23 19:49:05.000000 sentier_glossary-0.5.1/sentier_glossary.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 19:49:05.968238 sentier_glossary-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:02:08.250605 sentier_glossary-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-23 21:02:04.000000 sentier_glossary-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 21:02:04.000000 sentier_glossary-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-05-23 21:02:08.250605 sentier_glossary-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-05-23 21:02:04.000000 sentier_glossary-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-23 21:02:04.000000 sentier_glossary-0.5.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:02:08.250605 sentier_glossary-0.5.2/sentier_glossary/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-23 21:02:04.000000 sentier_glossary-0.5.2/sentier_glossary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10479 2024-05-23 21:02:04.000000 sentier_glossary-0.5.2/sentier_glossary/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-23 21:02:04.000000 sentier_glossary-0.5.2/sentier_glossary/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:02:08.250605 sentier_glossary-0.5.2/sentier_glossary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-05-23 21:02:08.000000 sentier_glossary-0.5.2/sentier_glossary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-23 21:02:08.000000 sentier_glossary-0.5.2/sentier_glossary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 21:02:08.000000 sentier_glossary-0.5.2/sentier_glossary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-23 21:02:08.000000 sentier_glossary-0.5.2/sentier_glossary.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-23 21:02:08.000000 sentier_glossary-0.5.2/sentier_glossary.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 21:02:08.250605 sentier_glossary-0.5.2/setup.cfg
```

### Comparing `sentier_glossary-0.5.1/LICENSE` & `sentier_glossary-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sentier_glossary-0.5.1/PKG-INFO` & `sentier_glossary-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentier_glossary
-Version: 0.5.1
+Version: 0.5.2
 Summary: Client interface to sentier.dev sustainability assessment glossary
 Author-email: João Gonçalves <jsvgoncalves@gmail.com>, Chris Mutel <cmutel@gmail.com>
 Maintainer-email: João Gonçalves <jsvgoncalves@gmail.com>, Chris Mutel <cmutel@gmail.com>
 Project-URL: source, https://github.com/Depart-de-Sentier/sentier_glossary
 Project-URL: homepage, https://github.com/Depart-de-Sentier/sentier_glossary
 Project-URL: tracker, https://github.com/Depart-de-Sentier/sentier_glossary/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sentier_glossary-0.5.1/README.md` & `sentier_glossary-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `sentier_glossary-0.5.1/pyproject.toml` & `sentier_glossary-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sentier_glossary-0.5.1/sentier_glossary/main.py` & `sentier_glossary-0.5.2/sentier_glossary/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import locale
 import warnings
 from collections import defaultdict
 from enum import Enum
 from functools import reduce
 from urllib.parse import urljoin
+import warnings
 
 import pandas as pd
 import requests
 import torch
 from sentence_transformers import SentenceTransformer, util  # type: ignore
 
 from sentier_glossary.settings import Settings
@@ -35,15 +36,19 @@
         print(f"Using language code '{self.language_code}'; change with `set_language_code()`")
 
     def get_language_code(self, language_code: str | None = None) -> str:
         """Get 2-letter (Set 1) ISO 639 language code."""
         code = language_code or locale.getlocale()[0] or self._cfg.fallback_language
         if isinstance(code, str) and len(code) >= 2:
             return code[:2].lower()
-        raise ValueError(f"Invalid language code {code} found; set locale or `default_language`")
+        warnings.warn(f"""
+            Unexpected language code encountered: '{code}'.
+            Switching to fallback: '{self._cfg.fallback_language}'
+        """)
+        return self._cfg.fallback_language
 
     def set_language_code(self, language_code: str) -> None:
         """Override language code from system locale or input argument."""
         if not (isinstance(language_code, str) and len(language_code) >= 2):
             raise ValueError(
                 f"Invalid language code {language_code} given. Must be `str` of length two."
             )
```

### Comparing `sentier_glossary-0.5.1/sentier_glossary.egg-info/PKG-INFO` & `sentier_glossary-0.5.2/sentier_glossary.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentier_glossary
-Version: 0.5.1
+Version: 0.5.2
 Summary: Client interface to sentier.dev sustainability assessment glossary
 Author-email: João Gonçalves <jsvgoncalves@gmail.com>, Chris Mutel <cmutel@gmail.com>
 Maintainer-email: João Gonçalves <jsvgoncalves@gmail.com>, Chris Mutel <cmutel@gmail.com>
 Project-URL: source, https://github.com/Depart-de-Sentier/sentier_glossary
 Project-URL: homepage, https://github.com/Depart-de-Sentier/sentier_glossary
 Project-URL: tracker, https://github.com/Depart-de-Sentier/sentier_glossary/issues
 Classifier: Development Status :: 4 - Beta
```

