# Comparing `tmp/sentier_glossary-0.4.1.tar.gz` & `tmp/sentier_glossary-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentier_glossary-0.4.1.tar", last modified: Wed May 22 17:11:15 2024, max compression
+gzip compressed data, was "sentier_glossary-0.5.0.tar", last modified: Thu May 23 19:14:29 2024, max compression
```

## Comparing `sentier_glossary-0.4.1.tar` & `sentier_glossary-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:11:15.919915 sentier_glossary-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-22 17:11:12.000000 sentier_glossary-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 17:11:12.000000 sentier_glossary-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8195 2024-05-22 17:11:15.919915 sentier_glossary-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-05-22 17:11:12.000000 sentier_glossary-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-22 17:11:12.000000 sentier_glossary-0.4.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:11:15.919915 sentier_glossary-0.4.1/sentier_glossary/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-22 17:11:12.000000 sentier_glossary-0.4.1/sentier_glossary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-05-22 17:11:12.000000 sentier_glossary-0.4.1/sentier_glossary/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-22 17:11:12.000000 sentier_glossary-0.4.1/sentier_glossary/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:11:15.919915 sentier_glossary-0.4.1/sentier_glossary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8195 2024-05-22 17:11:15.000000 sentier_glossary-0.4.1/sentier_glossary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-22 17:11:15.000000 sentier_glossary-0.4.1/sentier_glossary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 17:11:15.000000 sentier_glossary-0.4.1/sentier_glossary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-22 17:11:15.000000 sentier_glossary-0.4.1/sentier_glossary.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 17:11:15.000000 sentier_glossary-0.4.1/sentier_glossary.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 17:11:15.919915 sentier_glossary-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:14:29.581869 sentier_glossary-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-23 19:14:22.000000 sentier_glossary-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:14:22.000000 sentier_glossary-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-05-23 19:14:29.581869 sentier_glossary-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-05-23 19:14:22.000000 sentier_glossary-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-23 19:14:22.000000 sentier_glossary-0.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:14:29.581869 sentier_glossary-0.5.0/sentier_glossary/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-23 19:14:22.000000 sentier_glossary-0.5.0/sentier_glossary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-05-23 19:14:22.000000 sentier_glossary-0.5.0/sentier_glossary/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-23 19:14:22.000000 sentier_glossary-0.5.0/sentier_glossary/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:14:29.581869 sentier_glossary-0.5.0/sentier_glossary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-05-23 19:14:29.000000 sentier_glossary-0.5.0/sentier_glossary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-23 19:14:29.000000 sentier_glossary-0.5.0/sentier_glossary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 19:14:29.000000 sentier_glossary-0.5.0/sentier_glossary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-23 19:14:29.000000 sentier_glossary-0.5.0/sentier_glossary.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-23 19:14:29.000000 sentier_glossary-0.5.0/sentier_glossary.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 19:14:29.585869 sentier_glossary-0.5.0/setup.cfg
```

### Comparing `sentier_glossary-0.4.1/LICENSE` & `sentier_glossary-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sentier_glossary-0.4.1/PKG-INFO` & `sentier_glossary-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentier_glossary
-Version: 0.4.1
+Version: 0.5.0
 Summary: Client interface to sentier.dev sustainability assessment glossary
 Author-email: João Gonçalves <jsvgoncalves@gmail.com>, Chris Mutel <cmutel@gmail.com>
 Maintainer-email: João Gonçalves <jsvgoncalves@gmail.com>, Chris Mutel <cmutel@gmail.com>
 Project-URL: source, https://github.com/Depart-de-Sentier/sentier_glossary
 Project-URL: homepage, https://github.com/Depart-de-Sentier/sentier_glossary
 Project-URL: tracker, https://github.com/Depart-de-Sentier/sentier_glossary/issues
 Classifier: Development Status :: 4 - Beta
@@ -19,14 +19,15 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic-settings
 Requires-Dist: requests
 Requires-Dist: sentence_transformers
 Requires-Dist: torch
+Requires-Dist: pandas
 Provides-Extra: testing
 Requires-Dist: sentier_glossary; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: python-coveralls; extra == "testing"
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
```

### Comparing `sentier_glossary-0.4.1/README.md` & `sentier_glossary-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `sentier_glossary-0.4.1/pyproject.toml` & `sentier_glossary-0.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 dependencies = [
     # dependencies as strings with quotes, e.g. "foo"
     # You can add version requirements like "foo>2.0"
     "pydantic-settings",
     "requests",
     "sentence_transformers",
     "torch",
+    "pandas",
 ]
 
 [project.urls]
 source = "https://github.com/Depart-de-Sentier/sentier_glossary"
 homepage = "https://github.com/Depart-de-Sentier/sentier_glossary"
 tracker = "https://github.com/Depart-de-Sentier/sentier_glossary/issues"
```

### Comparing `sentier_glossary-0.4.1/sentier_glossary/main.py` & `sentier_glossary-0.5.0/sentier_glossary/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,90 +1,43 @@
-import itertools
 import locale
 import warnings
 from collections import defaultdict
 from enum import Enum
 from functools import reduce
 from urllib.parse import urljoin
 
+import pandas as pd
 import requests
 import torch
 from sentence_transformers import SentenceTransformer, util  # type: ignore
 
 from sentier_glossary.settings import Settings
 
 
 class CommonSchemes(Enum):
     cn2024 = "http://data.europa.eu/xsp/cn2024/cn2024"
     nace21 = "http://data.europa.eu/ux2/nace2.1/nace2.1"
     low2015 = "http://data.europa.eu/6p8/low2015/scheme"
     icst2009 = "http://data.europa.eu/z1e/icstcom2009/icst"
     prodcom2023 = "http://data.europa.eu/qw1/prodcom2023/prodcom2023"
     isic4 = "https://unstats.un.org/classifications/ISIC/rev4/scheme"
-
-
-DEFAULT_COMPONENTS = {
-    "process": CommonSchemes.cn2024,
-    "product": CommonSchemes.nace21,
-    "unit": None,
-    "place": None,
-}
+    icc11 = "https://stats.fao.org/classifications/ICC/v1.1/scheme"
+    wca2020 = "https://stats.fao.org/classifications/WCA2020/crops/scheme"
 
 
 class GlossaryAPI:
     def __init__(self, cfg: Settings | None = None, language_code: str | None = None):
         self._cfg = cfg if cfg is not None else Settings()
         if not self._cfg.base_url.endswith("/"):
             self._cfg.base_url += "/"
 
         self._semantic_search = False
         self.language_code = self.get_language_code(language_code)
         print(f"Using language code '{self.language_code}'; change with `set_language_code()`")
 
-    def _requests_get(self, url: str, params: dict | None = None) -> dict:
-        """Perform a `requests.get(api_url, …)` with given parameters.
-
-        Args:
-            url: The API endpoint.
-            params: Any additional parameters to pass.
-
-        Returns:
-            dict: A dictionary containing the parsed JSON response.
-
-        Raises:
-            requests.exceptions.RequestException: If there is an error with the request,
-            such as a connection error or an invalid URL.
-
-        """
-        params = self._params | params if params is not None else self._params
-        response = requests.get(
-            reduce(urljoin, [self._cfg.base_url, f"{self._cfg.api_version}/", url]),
-            params=params,
-        )
-        try:
-            response.raise_for_status()
-        except requests.exceptions.RequestException as error:
-            msg = f"Error fetching data: {error}"
-            if response is not None:
-                status_code = response.status_code
-                msg += f"\nHTTP {status_code}"
-                if 400 <= status_code < 600:
-                    try:
-                        error_data = response.json()
-                        msg += f"\nResponse: {error_data}"
-                    except ValueError:
-                        msg += f"\nResponse: {response.text}"
-            raise requests.exceptions.RequestException(msg) from error
-        return response.json()
-
-    @property
-    def _params(self) -> dict:
-        """Default parameters for every request."""
-        return {"lang": self.language_code}
-
     def get_language_code(self, language_code: str | None = None) -> str:
         """Get 2-letter (Set 1) ISO 639 language code."""
         code = language_code or locale.getlocale()[0] or self._cfg.fallback_language
         if isinstance(code, str) and len(code) >= 2:
             return code[:2].lower()
         raise ValueError(f"Invalid language code {code} found; set locale or `default_language`")
 
@@ -101,20 +54,19 @@
                 `setup_semantic_search()` to use semantic search with {self.language_code}."""
             )
             self._semantic_search = False
 
     def setup_semantic_search(
         self,
         model_id: str = "all-mpnet-base-v2",
-        components: dict[str, CommonSchemes | None] = DEFAULT_COMPONENTS,
     ) -> None:
         """Download data and metadata to perform semantic search queries"""
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", category=FutureWarning)
-            self._embedder = SentenceTransformer("all-MiniLM-L6-v2")
+            self._embedder = SentenceTransformer(model_id)
 
         self._catalogues: dict[str, str] = {}
         self._embeddings: dict[str, torch.Tensor] = {}
         self._semantic_search = True
 
         for cs in CommonSchemes:
             self._catalogues[cs.value] = defaultdict(list)
@@ -123,32 +75,19 @@
                     if concept.get(label):
                         self._catalogues[cs.value][concept[label]].append(concept)
 
     def schemes(self) -> list[dict]:
         """Get all concept schemes, regardless of type"""
         return self._requests_get("schemes")
 
-    def _validate_iri(self, iri: str) -> None:
-        """Basic IRI validation.
-
-        Args:
-            iri (str): The [IRI](https://en.wikipedia.org/wiki/Internationalized_Resource_Identifier)
-
-        Raises:
-            ValueError: The IRI is not valid
-            KeyError: The requested resource was not found
-
-        """
-        pass
-
     def concepts_for_scheme(self, scheme_iri: str | Enum) -> list[dict]:
         if isinstance(scheme_iri, Enum):
             scheme_iri = scheme_iri.value
         self._validate_iri(scheme_iri)
-        data = self._requests_get("concepts", {"concept_scheme_iri": scheme_iri})["concepts"]
+        data = self._requests_get("concepts", {"concept_scheme_iri": scheme_iri})
         if not data and scheme_iri not in {obj["iri"] for obj in self.schemes()}:
             raise KeyError(f"Given concept scheme IRI '{scheme_iri}' not present in glossary")
         return data
 
     def concept(self, concept_iri: str) -> dict:
         """Return a single concept resource.
 
@@ -179,15 +118,19 @@
 
         Returns:
             list of resources matching the search query.
         """
         return self._requests_get("search", {"search_term": query})
 
     def semantic_search(
-        self, query: str, scope: str | CommonSchemes | None = None, min_num_results: int = 10
+        self,
+        query: str,
+        scope: str | CommonSchemes | None = None,
+        dataframe: bool = False,
+        min_num_results: int = 10,
     ) -> list[dict]:
         """Perform semantic search query.
 
         Stolen shamelessly from https://www.sbert.net/examples/applications/semantic-search/README.html#semantic-search.
 
         Args:
             query (str): the search query string
@@ -209,13 +152,116 @@
         num_results = min(min_num_results, len(corpus))
         # Creating embeddings is relatively expensive
         if scope not in self._embeddings:
             self._embeddings[scope] = self._embedder.encode(corpus, convert_to_tensor=True)
         query_embedding = self._embedder.encode(query, convert_to_tensor=True)
 
         cos_scores = util.cos_sim(query_embedding, self._embeddings[scope])[0]
-        return list(
-            itertools.chain(
-                self._catalogues[scope][corpus[idx.item()]]
-                for idx in torch.topk(cos_scores, k=num_results)[1]
+        object_lists = [
+            self._catalogues[scope][corpus[idx.item()]]
+            for idx in torch.topk(cos_scores, k=num_results)[1]
+        ]
+        results = list(
+            {
+                obj["iri"]: self._fill_out_concept_broader_relationships(self.concept(obj["iri"]))
+                for lst in object_lists
+                for obj in lst
+            }.values()
+        )
+        if dataframe:
+            return pd.DataFrame(
+                [
+                    {
+                        "prefLabel": obj.get("prefLabel"),
+                        "completeLabel": self._complete_label(obj),
+                        "broader_iri": (
+                            obj["broader"][0].get("iri", None) if obj.get("broader") else None
+                        ),
+                        "broader_prefLabel": (
+                            obj["broader"][0].get("prefLabel", None) if obj.get("broader") else None
+                        ),
+                        "iri": obj["iri"],
+                    }
+                    for obj in results
+                ]
             )
+        return results
+
+    def _requests_get(self, url: str, params: dict | None = None) -> dict:
+        """Perform a `requests.get(api_url, …)` with given parameters.
+
+        Args:
+            url: The API endpoint.
+            params: Any additional parameters to pass.
+
+        Returns:
+            dict: A dictionary containing the parsed JSON response.
+
+        Raises:
+            requests.exceptions.RequestException: If there is an error with the request,
+            such as a connection error or an invalid URL.
+
+        """
+        params = self._params | params if params is not None else self._params
+        response = requests.get(
+            reduce(urljoin, [self._cfg.base_url, f"{self._cfg.api_version}/", url]),
+            params=params,
+            timeout=10,
         )
+        try:
+            response.raise_for_status()
+        except requests.exceptions.RequestException as error:
+            msg = f"Error fetching data: {error}"
+            if response is not None:
+                status_code = response.status_code
+                msg += f"\nHTTP {status_code}"
+                if 400 <= status_code < 600:
+                    try:
+                        error_data = response.json()
+                        msg += f"\nResponse: {error_data}"
+                    except ValueError:
+                        msg += f"\nResponse: {response.text}"
+            raise requests.exceptions.RequestException(msg) from error
+        return response.json()
+
+    def _complete_label(self, data: dict) -> str:
+        if len(data.get("broader", [])):
+            return (
+                " ⧺ ".join([obj["prefLabel"] for obj in data["broader"]])
+                + " ⧺ "
+                + data["prefLabel"]
+            )
+        return data["prefLabel"]
+
+    @property
+    def _params(self) -> dict:
+        """Default parameters for every request."""
+        return {"lang": self.language_code}
+
+    def _validate_iri(self, iri: str) -> None:
+        """Basic IRI validation.
+
+        # TBD
+
+        Args:
+            iri (str): The [IRI](https://en.wikipedia.org/wiki/Internationalized_Resource_Identifier)
+
+        Raises:
+            ValueError: The IRI is not valid
+            KeyError: The requested resource was not found
+
+        """
+
+    def _fill_out_concept_broader_relationships(
+        self, data: dict, attributes: list[str] | None = None
+    ) -> dict:
+        """Add some additional information about broader relations of a concept"""
+        if attributes is None:
+            attributes = ["iri", "prefLabel"]
+        if "relations" in data:
+            broader = [
+                self.concept(obj["target_concept_iri"])
+                for obj in data["relations"]
+                if obj["type"] == "broader" and obj["source_concept_iri"] == data["iri"]
+            ]
+            data["broader"] = [{key: obj.get(key) for key in attributes} for obj in broader]
+        return data
```

### Comparing `sentier_glossary-0.4.1/sentier_glossary.egg-info/PKG-INFO` & `sentier_glossary-0.5.0/sentier_glossary.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentier_glossary
-Version: 0.4.1
+Version: 0.5.0
 Summary: Client interface to sentier.dev sustainability assessment glossary
 Author-email: João Gonçalves <jsvgoncalves@gmail.com>, Chris Mutel <cmutel@gmail.com>
 Maintainer-email: João Gonçalves <jsvgoncalves@gmail.com>, Chris Mutel <cmutel@gmail.com>
 Project-URL: source, https://github.com/Depart-de-Sentier/sentier_glossary
 Project-URL: homepage, https://github.com/Depart-de-Sentier/sentier_glossary
 Project-URL: tracker, https://github.com/Depart-de-Sentier/sentier_glossary/issues
 Classifier: Development Status :: 4 - Beta
@@ -19,14 +19,15 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic-settings
 Requires-Dist: requests
 Requires-Dist: sentence_transformers
 Requires-Dist: torch
+Requires-Dist: pandas
 Provides-Extra: testing
 Requires-Dist: sentier_glossary; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: python-coveralls; extra == "testing"
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
```

