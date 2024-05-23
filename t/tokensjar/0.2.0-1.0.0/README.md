# Comparing `tmp/tokensjar-0.2.0.tar.gz` & `tmp/tokensjar-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokensjar-0.2.0.tar", last modified: Mon Nov  1 00:07:00 2021, max compression
+gzip compressed data, was "tokensjar-1.0.0.tar", last modified: Thu May 23 13:31:13 2024, max compression
```

## Comparing `tokensjar-0.2.0.tar` & `tokensjar-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2021-11-01 00:07:00.354289 tokensjar-0.2.0/
--rw-rw-rw-   0        0        0    35823 2021-10-31 17:58:46.000000 tokensjar-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     4278 2021-11-01 00:07:00.354289 tokensjar-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3678 2021-10-31 23:49:14.000000 tokensjar-0.2.0/README.md
--rw-rw-rw-   0        0        0      108 2021-10-31 18:00:24.000000 tokensjar-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      735 2021-11-01 00:07:00.356283 tokensjar-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2021-11-01 00:07:00.331359 tokensjar-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2021-11-01 00:07:00.343318 tokensjar-0.2.0/src/tokensjar/
--rw-rw-rw-   0        0        0       24 2021-10-31 23:59:44.000000 tokensjar-0.2.0/src/tokensjar/__init__.py
--rw-rw-rw-   0        0        0     3761 2021-10-31 23:58:15.000000 tokensjar-0.2.0/src/tokensjar/tokensjar.py
-drwxrwxrwx   0        0        0        0 2021-11-01 00:07:00.353290 tokensjar-0.2.0/src/tokensjar.egg-info/
--rw-rw-rw-   0        0        0     4278 2021-11-01 00:07:00.000000 tokensjar-0.2.0/src/tokensjar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2021-11-01 00:07:00.000000 tokensjar-0.2.0/src/tokensjar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-11-01 00:07:00.000000 tokensjar-0.2.0/src/tokensjar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2021-11-01 00:07:00.000000 tokensjar-0.2.0/src/tokensjar.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2021-11-01 00:07:00.000000 tokensjar-0.2.0/src/tokensjar.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 13:31:13.936127 tokensjar-1.0.0/
+-rw-rw-rw-   0        0        0    35823 2024-05-23 12:13:07.000000 tokensjar-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     4132 2024-05-23 13:31:13.935126 tokensjar-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3569 2024-05-23 13:24:54.000000 tokensjar-1.0.0/README.md
+-rw-rw-rw-   0        0        0      108 2024-05-23 12:13:07.000000 tokensjar-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      700 2024-05-23 13:31:13.937127 tokensjar-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-23 13:31:13.919350 tokensjar-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-23 13:31:13.927348 tokensjar-1.0.0/src/tokensjar/
+-rw-rw-rw-   0        0        0       31 2024-05-23 13:24:54.000000 tokensjar-1.0.0/src/tokensjar/__init__.py
+-rw-rw-rw-   0        0        0     3817 2024-05-23 13:24:54.000000 tokensjar-1.0.0/src/tokensjar/tokensjar.py
+drwxrwxrwx   0        0        0        0 2024-05-23 13:31:13.934126 tokensjar-1.0.0/src/tokensjar.egg-info/
+-rw-rw-rw-   0        0        0     4132 2024-05-23 13:31:13.000000 tokensjar-1.0.0/src/tokensjar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2024-05-23 13:31:13.000000 tokensjar-1.0.0/src/tokensjar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 13:31:13.000000 tokensjar-1.0.0/src/tokensjar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-23 13:31:13.000000 tokensjar-1.0.0/src/tokensjar.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 13:31:13.933128 tokensjar-1.0.0/tests/
+-rw-rw-rw-   0        0        0     3606 2024-05-23 13:18:06.000000 tokensjar-1.0.0/tests/test_tokensjar.py
```

### Comparing `tokensjar-0.2.0/LICENSE` & `tokensjar-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tokensjar-0.2.0/PKG-INFO` & `tokensjar-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: tokensjar
-Version: 0.2.0
+Version: 1.0.0
 Summary: A micro token interpretor/manipulator for Python
 Home-page: https://github.com/tcladet/tokensjar
 Author: Tristan Cladet
 Author-email: tristan.cladet@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/tcladet/tokensjar
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # tokensjar
 
 `tokensjar` is a pure Python module dedicated to generate, manipulate and interpret expressions following environment variables creation rules. This module is really useful if you need to develop a tool that can prepare the session environment variables for a specific usage.
 
@@ -80,15 +78,15 @@
 print(jar.tokens_interpreted['T12'])
 # Output: Token1/Token2
 
 result = jar.interpret('Joe said: $(HELLO) $(T12)')
 # Output: Joe said: Hello: Token1/Token2
 ```
 
- Take care to not introduce cyclic dependencies between tokens! The topological sort is handled by Eric V. Smith `toposort` Python package ([Link](https://pypi.org/project/toposort)).
+> :warning: Take care to not introduce cyclic dependencies between tokens!
 
  ```python
 from tokensjar import TokensJar
 
 
 jar = TokensJar()
 jar.add_raw_value('T1', '$(T2)')
@@ -121,8 +119,7 @@
 ## Upload the project
 
 The project can be uploaded using `twine` (listed in `dist-requirements.txt`) by running the following command:
 
 ```
 python -m twine upload dist/*
 ```
-
```

### Comparing `tokensjar-0.2.0/README.md` & `tokensjar-1.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 print(jar.tokens_interpreted['T12'])
 # Output: Token1/Token2
 
 result = jar.interpret('Joe said: $(HELLO) $(T12)')
 # Output: Joe said: Hello: Token1/Token2
 ```
 
- Take care to not introduce cyclic dependencies between tokens! The topological sort is handled by Eric V. Smith `toposort` Python package ([Link](https://pypi.org/project/toposort)).
+> :warning: Take care to not introduce cyclic dependencies between tokens!
 
  ```python
 from tokensjar import TokensJar
 
 
 jar = TokensJar()
 jar.add_raw_value('T1', '$(T2)')
```

### Comparing `tokensjar-0.2.0/setup.cfg` & `tokensjar-1.0.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 6f6b 656e 736a 6172 0d0a 7665   = tokensjar..ve
-00000020: 7273 696f 6e20 3d20 302e 322e 300d 0a61  rsion = 0.2.0..a
+00000020: 7273 696f 6e20 3d20 312e 302e 300d 0a61  rsion = 1.0.0..a
 00000030: 7574 686f 7220 3d20 5472 6973 7461 6e20  uthor = Tristan 
 00000040: 436c 6164 6574 0d0a 6175 7468 6f72 5f65  Cladet..author_e
 00000050: 6d61 696c 203d 2074 7269 7374 616e 2e63  mail = tristan.c
 00000060: 6c61 6465 7440 676d 6169 6c2e 636f 6d0d  ladet@gmail.com.
 00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
 00000080: 206d 6963 726f 2074 6f6b 656e 2069 6e74   micro token int
 00000090: 6572 7072 6574 6f72 2f6d 616e 6970 756c  erpretor/manipul
@@ -20,27 +20,25 @@
 00000130: 7072 6f6a 6563 745f 7572 6c73 203d 200d  project_urls = .
 00000140: 0a09 4275 6720 5472 6163 6b65 7220 3d20  ..Bug Tracker = 
 00000150: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
 00000160: 6f6d 2f74 636c 6164 6574 2f74 6f6b 656e  om/tcladet/token
 00000170: 736a 6172 0d0a 636c 6173 7369 6669 6572  sjar..classifier
 00000180: 7320 3d20 0d0a 0950 726f 6772 616d 6d69  s = ...Programmi
 00000190: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000001a0: 7974 686f 6e20 3a3a 2033 2e38 0d0a 094c  ython :: 3.8...L
-000001b0: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
-000001c0: 7072 6f76 6564 203a 3a20 474e 5520 4765  proved :: GNU Ge
-000001d0: 6e65 7261 6c20 5075 626c 6963 204c 6963  neral Public Lic
-000001e0: 656e 7365 2076 3320 2847 504c 7633 290d  ense v3 (GPLv3).
-000001f0: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
-00000200: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
-00000210: 6465 6e74 0d0a 0d0a 5b6f 7074 696f 6e73  dent....[options
-00000220: 5d0d 0a70 6163 6b61 6765 5f64 6972 203d  ]..package_dir =
-00000230: 200d 0a09 3d20 7372 630d 0a70 6163 6b61   ...= src..packa
-00000240: 6765 7320 3d20 6669 6e64 3a0d 0a70 7974  ges = find:..pyt
-00000250: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
-00000260: 3d33 2e38 0d0a 696e 7374 616c 6c5f 7265  =3.8..install_re
-00000270: 7175 6972 6573 203d 200d 0a09 746f 706f  quires = ...topo
-00000280: 736f 7274 3d3d 312e 370d 0a0d 0a5b 6f70  sort==1.7....[op
-00000290: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
-000002a0: 696e 645d 0d0a 7768 6572 6520 3d20 7372  ind]..where = sr
-000002b0: 630d 0a0d 0a5b 6567 675f 696e 666f 5d0d  c....[egg_info].
-000002c0: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
-000002d0: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
+000001a0: 7974 686f 6e20 3a3a 2033 2e31 310d 0a09  ython :: 3.11...
+000001b0: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
+000001c0: 7070 726f 7665 6420 3a3a 2047 4e55 2047  pproved :: GNU G
+000001d0: 656e 6572 616c 2050 7562 6c69 6320 4c69  eneral Public Li
+000001e0: 6365 6e73 6520 7633 2028 4750 4c76 3329  cense v3 (GPLv3)
+000001f0: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
+00000200: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
+00000210: 6e64 656e 740d 0a0d 0a5b 6f70 7469 6f6e  ndent....[option
+00000220: 735d 0d0a 7061 636b 6167 655f 6469 7220  s]..package_dir 
+00000230: 3d20 0d0a 093d 2073 7263 0d0a 7061 636b  = ...= src..pack
+00000240: 6167 6573 203d 2066 696e 643a 0d0a 7079  ages = find:..py
+00000250: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
+00000260: 3e3d 332e 3131 0d0a 0d0a 5b6f 7074 696f  >=3.11....[optio
+00000270: 6e73 2e70 6163 6b61 6765 732e 6669 6e64  ns.packages.find
+00000280: 5d0d 0a77 6865 7265 203d 2073 7263 0d0a  ]..where = src..
+00000290: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
+000002a0: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
+000002b0: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
```

### Comparing `tokensjar-0.2.0/src/tokensjar/tokensjar.py` & `tokensjar-1.0.0/src/tokensjar/tokensjar.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import re
 from collections import defaultdict
+from graphlib import TopologicalSorter
 
 
 RX_TOKEN_PATTERN = re.compile(r'\$\(([^\)]+)\)')
 
 
 class TokensJarError(Exception):
     pass
@@ -87,20 +88,20 @@
         # Create dependency graph
         nodes = {n: set() for n in tokens.keys()}
         for t, value in tokens.items():
             dep_tokens = RX_TOKEN_PATTERN.findall(value)
             for token in dep_tokens:
                 nodes[t].add(token)
         # Sort nodes
-        from toposort import toposort_flatten
-        tokens_sorted = reversed(toposort_flatten(nodes))
+        sorter = TopologicalSorter(nodes)
+        tokens_sorted = list(reversed(list(sorter.static_order())))
         for ts in tokens_sorted:
             expression = expression.replace(f'$({ts})', tokens[ts])
         return expression
 
     @property
-    def tokens_interpreted(self) -> dict:
+    def tokens_interpreted(self) -> dict[str, str]:
         """The dictionary of all tokens interpreted."""
         tokens = self.__get_tokens()
         for t, value in tokens.items():
             tokens[t] = self.interpret(value)
         return tokens
```

### Comparing `tokensjar-0.2.0/src/tokensjar.egg-info/PKG-INFO` & `tokensjar-1.0.0/src/tokensjar.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: tokensjar
-Version: 0.2.0
+Version: 1.0.0
 Summary: A micro token interpretor/manipulator for Python
 Home-page: https://github.com/tcladet/tokensjar
 Author: Tristan Cladet
 Author-email: tristan.cladet@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/tcladet/tokensjar
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # tokensjar
 
 `tokensjar` is a pure Python module dedicated to generate, manipulate and interpret expressions following environment variables creation rules. This module is really useful if you need to develop a tool that can prepare the session environment variables for a specific usage.
 
@@ -80,15 +78,15 @@
 print(jar.tokens_interpreted['T12'])
 # Output: Token1/Token2
 
 result = jar.interpret('Joe said: $(HELLO) $(T12)')
 # Output: Joe said: Hello: Token1/Token2
 ```
 
- Take care to not introduce cyclic dependencies between tokens! The topological sort is handled by Eric V. Smith `toposort` Python package ([Link](https://pypi.org/project/toposort)).
+> :warning: Take care to not introduce cyclic dependencies between tokens!
 
  ```python
 from tokensjar import TokensJar
 
 
 jar = TokensJar()
 jar.add_raw_value('T1', '$(T2)')
@@ -121,8 +119,7 @@
 ## Upload the project
 
 The project can be uploaded using `twine` (listed in `dist-requirements.txt`) by running the following command:
 
 ```
 python -m twine upload dist/*
 ```
-
```

