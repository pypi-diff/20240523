# Comparing `tmp/sentier_glossary-0.5.0.tar.gz` & `tmp/sentier_glossary-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentier_glossary-0.5.0.tar", last modified: Thu May 23 19:14:29 2024, max compression
+gzip compressed data, was "sentier_glossary-0.5.1.tar", last modified: Thu May 23 19:49:05 2024, max compression
```

## Comparing `sentier_glossary-0.5.0.tar` & `sentier_glossary-0.5.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:14:29.581869 sentier_glossary-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-23 19:14:22.000000 sentier_glossary-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:14:22.000000 sentier_glossary-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-05-23 19:14:29.581869 sentier_glossary-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-05-23 19:14:22.000000 sentier_glossary-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-23 19:14:22.000000 sentier_glossary-0.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:14:29.581869 sentier_glossary-0.5.0/sentier_glossary/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-23 19:14:22.000000 sentier_glossary-0.5.0/sentier_glossary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-05-23 19:14:22.000000 sentier_glossary-0.5.0/sentier_glossary/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-23 19:14:22.000000 sentier_glossary-0.5.0/sentier_glossary/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:14:29.581869 sentier_glossary-0.5.0/sentier_glossary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-05-23 19:14:29.000000 sentier_glossary-0.5.0/sentier_glossary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-23 19:14:29.000000 sentier_glossary-0.5.0/sentier_glossary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 19:14:29.000000 sentier_glossary-0.5.0/sentier_glossary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-23 19:14:29.000000 sentier_glossary-0.5.0/sentier_glossary.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-23 19:14:29.000000 sentier_glossary-0.5.0/sentier_glossary.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 19:14:29.585869 sentier_glossary-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:49:05.968238 sentier_glossary-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-23 19:49:02.000000 sentier_glossary-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:49:02.000000 sentier_glossary-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-05-23 19:49:05.968238 sentier_glossary-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-05-23 19:49:02.000000 sentier_glossary-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-23 19:49:02.000000 sentier_glossary-0.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:49:05.968238 sentier_glossary-0.5.1/sentier_glossary/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-23 19:49:02.000000 sentier_glossary-0.5.1/sentier_glossary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10351 2024-05-23 19:49:02.000000 sentier_glossary-0.5.1/sentier_glossary/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-23 19:49:02.000000 sentier_glossary-0.5.1/sentier_glossary/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:49:05.968238 sentier_glossary-0.5.1/sentier_glossary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-05-23 19:49:05.000000 sentier_glossary-0.5.1/sentier_glossary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-23 19:49:05.000000 sentier_glossary-0.5.1/sentier_glossary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 19:49:05.000000 sentier_glossary-0.5.1/sentier_glossary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-23 19:49:05.000000 sentier_glossary-0.5.1/sentier_glossary.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-23 19:49:05.000000 sentier_glossary-0.5.1/sentier_glossary.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 19:49:05.968238 sentier_glossary-0.5.1/setup.cfg
```

### Comparing `sentier_glossary-0.5.0/LICENSE` & `sentier_glossary-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sentier_glossary-0.5.0/PKG-INFO` & `sentier_glossary-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentier_glossary
-Version: 0.5.0
+Version: 0.5.1
 Summary: Client interface to sentier.dev sustainability assessment glossary
 Author-email: João Gonçalves <jsvgoncalves@gmail.com>, Chris Mutel <cmutel@gmail.com>
 Maintainer-email: João Gonçalves <jsvgoncalves@gmail.com>, Chris Mutel <cmutel@gmail.com>
 Project-URL: source, https://github.com/Depart-de-Sentier/sentier_glossary
 Project-URL: homepage, https://github.com/Depart-de-Sentier/sentier_glossary
 Project-URL: tracker, https://github.com/Depart-de-Sentier/sentier_glossary/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sentier_glossary-0.5.0/README.md` & `sentier_glossary-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `sentier_glossary-0.5.0/pyproject.toml` & `sentier_glossary-0.5.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -69,21 +69,24 @@
 include-package-data = true
 packages = ["sentier_glossary"]
 
 [tool.setuptools.dynamic]
 version = {attr = "sentier_glossary.__version__"}
 
 [tool.pytest.ini_options]
-addopts = "--cov sentier_glossary --cov-report term-missing --verbose"
+addopts = "--cov sentier_glossary --cov-report term-missing --verbose -m \"not slow\""
 norecursedirs = [
     "dist",
     "build",
     ".tox"
 ]
 testpaths = ["tests/*/*.py"]
+markers = [
+    "slow: marks tests as slow (run all with '-m \"slow or not slow\"')",
+]
 
 [tool.flake8]
 # Some sane defaults for the code style checker flake8
 max_line_length = 100
 extend_ignore = ["E203", "W503"]
 # ^  Black-compatible
 #    E203 and W503 have edge cases handled by black
```

### Comparing `sentier_glossary-0.5.0/sentier_glossary/main.py` & `sentier_glossary-0.5.1/sentier_glossary/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         code = language_code or locale.getlocale()[0] or self._cfg.fallback_language
         if isinstance(code, str) and len(code) >= 2:
             return code[:2].lower()
         raise ValueError(f"Invalid language code {code} found; set locale or `default_language`")
 
     def set_language_code(self, language_code: str) -> None:
         """Override language code from system locale or input argument."""
-        if not isinstance(language_code, str) and len(language_code) >= 2:
+        if not (isinstance(language_code, str) and len(language_code) >= 2):
             raise ValueError(
                 f"Invalid language code {language_code} given. Must be `str` of length two."
             )
         self.language_code = language_code[:2].lower()
         if self._semantic_search:
             warnings.warn(
                 f"""Semantic search cache is stale and disabled. Please reenable with
@@ -76,49 +76,54 @@
                         self._catalogues[cs.value][concept[label]].append(concept)
 
     def schemes(self) -> list[dict]:
         """Get all concept schemes, regardless of type"""
         return self._requests_get("schemes")
 
     def concepts_for_scheme(self, scheme_iri: str | Enum) -> list[dict]:
+        """Return a list of concepts for a given scheme.
+
+        Args:
+            scheme_iri (str): the scheme IRI
+
+        Returns:
+            A list of dictionaries of concepts in the scheme
+
+        Raises:
+            ValueError: The IRI is not valid
+            requests.exceptionsRequestException: The requested resource was not found
+
+        """
         if isinstance(scheme_iri, Enum):
             scheme_iri = scheme_iri.value
         self._validate_iri(scheme_iri)
-        data = self._requests_get("concepts", {"concept_scheme_iri": scheme_iri})
-        if not data and scheme_iri not in {obj["iri"] for obj in self.schemes()}:
-            raise KeyError(f"Given concept scheme IRI '{scheme_iri}' not present in glossary")
-        return data
+        return self._requests_get("concepts", {"concept_scheme_iri": scheme_iri})
 
     def concept(self, concept_iri: str) -> dict:
         """Return a single concept resource.
 
         Args:
-            query (str): the search query string
-            scope (str, CommonSchemes, None): If given, limit the search to one concept scheme
+            concept_iri (str): the concept IRI
 
         Returns:
             A dictionary of the requested resource
 
         Raises:
             ValueError: The IRI is not valid
-            KeyError: The requested resource was not found
+            requests.exceptionsRequestException: The requested resource was not found
 
         """
         self._validate_iri(concept_iri)
-        data = self._requests_get("concept", {"concept_iri": concept_iri})
-        if not data:
-            raise KeyError(f"Given concept IRI '{concept_iri}' not present in glossary")
-        return data
+        return self._requests_get("concept", {"concept_iri": concept_iri})
 
     def search(self, query: str) -> list[dict]:
         """Search the the concept library using the `/search` endpoint.
 
         Args:
             query (str): the search query string
-            scope (str, CommonSchemes, None): If given, limit the search to one concept scheme
 
         Returns:
             list of resources matching the search query.
         """
         return self._requests_get("search", {"search_term": query})
 
     def semantic_search(
```

### Comparing `sentier_glossary-0.5.0/sentier_glossary.egg-info/PKG-INFO` & `sentier_glossary-0.5.1/sentier_glossary.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentier_glossary
-Version: 0.5.0
+Version: 0.5.1
 Summary: Client interface to sentier.dev sustainability assessment glossary
 Author-email: João Gonçalves <jsvgoncalves@gmail.com>, Chris Mutel <cmutel@gmail.com>
 Maintainer-email: João Gonçalves <jsvgoncalves@gmail.com>, Chris Mutel <cmutel@gmail.com>
 Project-URL: source, https://github.com/Depart-de-Sentier/sentier_glossary
 Project-URL: homepage, https://github.com/Depart-de-Sentier/sentier_glossary
 Project-URL: tracker, https://github.com/Depart-de-Sentier/sentier_glossary/issues
 Classifier: Development Status :: 4 - Beta
```

