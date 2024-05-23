# Comparing `tmp/sqliteimport-0.1.0.tar.gz` & `tmp/sqliteimport-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqliteimport-0.1.0.tar", max compression
+gzip compressed data, was "sqliteimport-0.2.0.tar", max compression
```

## Comparing `sqliteimport-0.1.0.tar` & `sqliteimport-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     1089 2024-05-15 00:04:16.095343 sqliteimport-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     1051 2024-05-22 13:49:10.539680 sqliteimport-0.1.0/README.rst
--rw-r--r--   0        0        0     1421 2024-05-22 13:53:18.508463 sqliteimport-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      216 2024-05-16 17:57:35.619910 sqliteimport-0.1.0/src/sqliteimport/__init__.py
--rw-r--r--   0        0        0     1594 2024-05-17 14:43:37.393516 sqliteimport-0.1.0/src/sqliteimport/importer.py
--rw-r--r--   0        0        0        0 2024-05-16 17:57:35.619910 sqliteimport-0.1.0/src/sqliteimport/py.typed
--rw-r--r--   0        0        0     1761 1970-01-01 00:00:00.000000 sqliteimport-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-05-15 00:04:16.095343 sqliteimport-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     1164 2024-05-23 14:28:47.027572 sqliteimport-0.2.0/README.rst
+-rw-r--r--   0        0        0     1564 2024-05-23 14:28:47.027572 sqliteimport-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      216 2024-05-16 17:57:35.619910 sqliteimport-0.2.0/src/sqliteimport/__init__.py
+-rw-r--r--   0        0        0       31 2024-05-23 14:28:47.027572 sqliteimport-0.2.0/src/sqliteimport/__main__.py
+-rw-r--r--   0        0        0     2564 2024-05-23 14:28:47.027572 sqliteimport-0.2.0/src/sqliteimport/cli.py
+-rw-r--r--   0        0        0     2110 2024-05-23 14:28:47.027572 sqliteimport-0.2.0/src/sqliteimport/importer.py
+-rw-r--r--   0        0        0        0 2024-05-16 17:57:35.619910 sqliteimport-0.2.0/src/sqliteimport/py.typed
+-rw-r--r--   0        0        0     1941 1970-01-01 00:00:00.000000 sqliteimport-0.2.0/PKG-INFO
```

### Comparing `sqliteimport-0.1.0/LICENSE.txt` & `sqliteimport-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sqliteimport-0.1.0/README.rst` & `sqliteimport-0.2.0/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -16,51 +16,58 @@
 000000f0: 6162 6173 6573 2e2a 0a0a 2d2d 2d2d 2d2d  abases.*..------
 00000100: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00000110: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00000120: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00000130: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00000140: 2d2d 2d2d 2d2d 2d2d 2d0a 0a44 656d 6f20  ---------..Demo 
 00000150: 7573 6167 6520 6578 616d 706c 652c 2075  usage example, u
-00000160: 7369 6e67 2063 6f64 6520 696e 2060 7468  sing code in `th
-00000170: 6520 7371 6c69 7465 696d 706f 7274 2072  e sqliteimport r
-00000180: 6570 6f73 6974 6f72 7960 5f3a 0a0a 2e2e  epository`_:....
-00000190: 2020 636f 6465 2d62 6c6f 636b 3a3a 2062    code-block:: b
-000001a0: 6173 680a 0a20 2020 2023 2049 6e73 7461  ash..    # Insta
-000001b0: 6c6c 2027 7265 7175 6573 7473 2720 696e  ll 'requests' in
-000001c0: 2061 2073 7461 6e64 616c 6f6e 6520 6469   a standalone di
-000001d0: 7265 6374 6f72 792e 0a20 2020 2070 6970  rectory..    pip
-000001e0: 2069 6e73 7461 6c6c 202d 2d74 6172 6765   install --targe
-000001f0: 743d 7361 6d70 6c65 2072 6571 7565 7374  t=sample request
-00000200: 730a 0a20 2020 2023 2047 656e 6572 6174  s..    # Generat
-00000210: 6520 6120 7371 6c69 7465 2064 6174 6162  e a sqlite datab
-00000220: 6173 6520 636f 6e74 6169 6e69 6e67 2074  ase containing t
-00000230: 6865 2069 6e73 7461 6c6c 6564 2070 6163  he installed pac
-00000240: 6b61 6765 732e 0a20 2020 2070 7974 686f  kages..    pytho
-00000250: 6e20 6765 6e65 7261 7465 2d73 616d 706c  n generate-sampl
-00000260: 652e 7079 0a0a 2020 2020 2320 4465 6d6f  e.py..    # Demo
-00000270: 6e73 7472 6174 6520 7468 6174 2069 6d70  nstrate that imp
-00000280: 6f72 7469 6e67 2066 726f 6d20 6120 6461  orting from a da
-00000290: 7461 6261 7365 2077 6f72 6b73 2e0a 2020  tabase works..  
-000002a0: 2020 7079 7468 6f6e 2064 656d 6f2e 7079    python demo.py
-000002b0: 0a0a 0a54 6869 7320 6973 2074 6865 206f  ...This is the o
-000002c0: 7574 7075 743a 0a0a 2e2e 2020 636f 6465  utput:....  code
-000002d0: 2d62 6c6f 636b 3a3a 2063 6f6e 736f 6c65  -block:: console
-000002e0: 0a0a 2020 2020 2420 7079 7468 6f6e 2064  ..    $ python d
-000002f0: 656d 6f2e 7079 0a20 2020 2054 6865 2072  emo.py.    The r
-00000300: 6571 7565 7374 7320 6d6f 6475 6c65 206f  equests module o
-00000310: 626a 6563 743a 0a20 2020 203c 6d6f 6475  bject:.    <modu
-00000320: 6c65 2027 7265 7175 6573 7473 2720 2873  le 'requests' (s
-00000330: 616d 706c 652e 7371 6c69 7465 3329 3e0a  ample.sqlite3)>.
-00000340: 0a20 2020 2046 6972 7374 206c 696e 6520  .    First line 
-00000350: 6f66 2074 6865 2048 544d 4c20 7265 7370  of the HTML resp
-00000360: 6f6e 7365 3a0a 2020 2020 3c21 444f 4354  onse:.    <!DOCT
-00000370: 5950 4520 6874 6d6c 3e0a 0a2e 2e20 2077  YPE html>....  w
-00000380: 6172 6e69 6e67 3a3a 0a0a 2020 2020 5468  arning::..    Th
-00000390: 6520 6461 7461 6261 7365 2066 6f72 6d61  e database forma
-000003a0: 7420 6973 206c 696b 656c 7920 746f 2063  t is likely to c
-000003b0: 6861 6e67 6520 6173 2074 6865 2070 726f  hange as the pro
-000003c0: 6a65 6374 206d 6174 7572 6573 2e0a 0a2e  ject matures....
-000003d0: 2e20 205f 7468 6520 7371 6c69 7465 696d  .  _the sqliteim
-000003e0: 706f 7274 2072 6570 6f73 6974 6f72 793a  port repository:
-000003f0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000400: 636f 6d2f 6b75 7274 6d63 6b65 652f 7371  com/kurtmckee/sq
-00000410: 6c69 7465 696d 706f 7274 0a              liteimport.
+00000160: 7369 6e67 2060 6064 656d 6f2e 7079 6060  sing ``demo.py``
+00000170: 2069 6e20 6074 6865 2073 716c 6974 6569   in `the sqlitei
+00000180: 6d70 6f72 7420 7265 706f 7369 746f 7279  mport repository
+00000190: 605f 3a0a 0a2e 2e20 2063 6f64 652d 626c  `_:....  code-bl
+000001a0: 6f63 6b3a 3a20 6261 7368 0a0a 2020 2020  ock:: bash..    
+000001b0: 2320 456e 7375 7265 2073 716c 6974 6569  # Ensure sqlitei
+000001c0: 6d70 6f72 7420 6973 2069 6e73 7461 6c6c  mport is install
+000001d0: 6564 2077 6974 6820 7468 6520 2763 6c69  ed with the 'cli
+000001e0: 2720 6578 7472 612e 0a20 2020 2070 6970  ' extra..    pip
+000001f0: 2069 6e73 7461 6c6c 2073 716c 6974 6569   install sqlitei
+00000200: 6d70 6f72 745b 636c 695d 0a0a 2020 2020  mport[cli]..    
+00000210: 2320 496e 7374 616c 6c20 2772 6571 7565  # Install 'reque
+00000220: 7374 7327 2069 6e20 6120 7374 616e 6461  sts' in a standa
+00000230: 6c6f 6e65 2064 6972 6563 746f 7279 2e0a  lone directory..
+00000240: 2020 2020 7069 7020 696e 7374 616c 6c20      pip install 
+00000250: 2d2d 7461 7267 6574 3d73 616d 706c 6520  --target=sample 
+00000260: 7265 7175 6573 7473 0a0a 2020 2020 2320  requests..    # 
+00000270: 4765 6e65 7261 7465 2061 2073 716c 6974  Generate a sqlit
+00000280: 6520 6461 7461 6261 7365 2063 6f6e 7461  e database conta
+00000290: 696e 696e 6720 7468 6520 696e 7374 616c  ining the instal
+000002a0: 6c65 6420 7061 636b 6167 6573 2e0a 2020  led packages..  
+000002b0: 2020 7371 6c69 7465 696d 706f 7274 2062    sqliteimport b
+000002c0: 756e 646c 6520 7361 6d70 6c65 2073 616d  undle sample sam
+000002d0: 706c 652e 7371 6c69 7465 330a 0a20 2020  ple.sqlite3..   
+000002e0: 2023 2044 656d 6f6e 7374 7261 7465 2074   # Demonstrate t
+000002f0: 6861 7420 696d 706f 7274 696e 6720 6672  hat importing fr
+00000300: 6f6d 2061 2064 6174 6162 6173 6520 776f  om a database wo
+00000310: 726b 732e 0a20 2020 2070 7974 686f 6e20  rks..    python 
+00000320: 6465 6d6f 2e70 7920 7361 6d70 6c65 2e73  demo.py sample.s
+00000330: 716c 6974 6533 0a0a 0a54 6869 7320 6973  qlite3...This is
+00000340: 2074 6865 206f 7574 7075 743a 0a0a 2e2e   the output:....
+00000350: 2020 636f 6465 2d62 6c6f 636b 3a3a 2063    code-block:: c
+00000360: 6f6e 736f 6c65 0a0a 2020 2020 2420 7079  onsole..    $ py
+00000370: 7468 6f6e 2064 656d 6f2e 7079 0a20 2020  thon demo.py.   
+00000380: 2054 6865 2072 6571 7565 7374 7320 6d6f   The requests mo
+00000390: 6475 6c65 206f 626a 6563 743a 0a20 2020  dule object:.   
+000003a0: 203c 6d6f 6475 6c65 2027 7265 7175 6573   <module 'reques
+000003b0: 7473 2720 2873 616d 706c 652e 7371 6c69  ts' (sample.sqli
+000003c0: 7465 3329 3e0a 0a20 2020 2052 6571 7565  te3)>..    Reque
+000003d0: 7374 696e 6720 6120 7765 6270 6167 652e  sting a webpage.
+000003e0: 2e2e 7375 6363 6573 7321 0a0a 2e2e 2020  ..success!....  
+000003f0: 7761 726e 696e 673a 3a0a 0a20 2020 2054  warning::..    T
+00000400: 6865 2064 6174 6162 6173 6520 666f 726d  he database form
+00000410: 6174 2069 7320 6c69 6b65 6c79 2074 6f20  at is likely to 
+00000420: 6368 616e 6765 2061 7320 7468 6520 7072  change as the pr
+00000430: 6f6a 6563 7420 6d61 7475 7265 732e 0a0a  oject matures...
+00000440: 2e2e 2020 5f74 6865 2073 716c 6974 6569  ..  _the sqlitei
+00000450: 6d70 6f72 7420 7265 706f 7369 746f 7279  mport repository
+00000460: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+00000470: 2e63 6f6d 2f6b 7572 746d 636b 6565 2f73  .com/kurtmckee/s
+00000480: 716c 6974 6569 6d70 6f72 740a            qliteimport.
```

### Comparing `sqliteimport-0.1.0/pyproject.toml` & `sqliteimport-0.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 [tool.poetry]
 name = "sqliteimport"
-version = "0.1.0"
+version = "0.2.0"
 description = "Import Python code from sqlite databases"
 authors = ["Kurt McKee <contactme@kurtmckee.org>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/kurtmckee/sqliteimport"
 homepage = "https://github.com/kurtmckee/sqliteimport"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
+click = {version = "^8", optional = true}
+
+[tool.poetry.extras]
+cli = ["click"]
+
+[tool.poetry.scripts]
+sqliteimport = "sqliteimport.cli:group"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 # Coverage
@@ -32,15 +39,15 @@
 source = [
     "src",
     "*/site-packages",
 ]
 
 [tool.coverage.report]
 skip_covered = true
-fail_under = 69
+fail_under = 29
 
 
 # Mypy
 # ----
 
 [tool.mypy]
 packages = "sqliteimport"
```

### Comparing `sqliteimport-0.1.0/src/sqliteimport/importer.py` & `sqliteimport-0.2.0/src/sqliteimport/importer.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,25 +2,31 @@
 # Copyright 2024 Kurt McKee <contactme@kurtmckee.org>
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import importlib.abc
 import importlib.machinery
+import os.path
 import pathlib
 import sqlite3
 import sys
 import types
 import typing
 
 
 class SqliteFinder(importlib.abc.MetaPathFinder):
-    def __init__(self, database: pathlib.Path) -> None:
-        self.database = database
-        self.connection = sqlite3.connect(database)
+    def __init__(self, database: pathlib.Path | sqlite3.Connection) -> None:
+        if isinstance(database, pathlib.Path):
+            self.database = database
+            self.connection = sqlite3.connect(database)
+        else:  # isinstance(database, sqlite3.Connection)
+            _, _, path = database.execute("PRAGMA database_list;").fetchone()
+            self.database = pathlib.Path(path)
+            self.connection = database
 
     def find_spec(
         self,
         fullname: str,
         path: typing.Sequence[str] | None,
         target: types.ModuleType | None = None,
     ) -> importlib.machinery.ModuleSpec | None:
@@ -46,9 +52,13 @@
     def create_module(self, spec: importlib.machinery.ModuleSpec) -> None:
         return None
 
     def exec_module(self, module: types.ModuleType) -> None:
         exec(self.source, module.__dict__)
 
 
-def load(database: pathlib.Path | str) -> None:
-    sys.meta_path.append(SqliteFinder(pathlib.Path(database)))
+def load(database: pathlib.Path | str | sqlite3.Connection) -> None:
+    if isinstance(database, (pathlib.Path, str)):
+        if not os.path.isfile(database):
+            raise FileNotFoundError(f"{database} must exist.")
+        database = pathlib.Path(database)
+    sys.meta_path.append(SqliteFinder(database))
```

### Comparing `sqliteimport-0.1.0/PKG-INFO` & `sqliteimport-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7371 6c69  : 2.1.Name: sqli
 00000020: 7465 696d 706f 7274 0a56 6572 7369 6f6e  teimport.Version
-00000030: 3a20 302e 312e 300a 5375 6d6d 6172 793a  : 0.1.0.Summary:
+00000030: 3a20 302e 322e 300a 5375 6d6d 6172 793a  : 0.2.0.Summary:
 00000040: 2049 6d70 6f72 7420 5079 7468 6f6e 2063   Import Python c
 00000050: 6f64 6520 6672 6f6d 2073 716c 6974 6520  ode from sqlite 
 00000060: 6461 7461 6261 7365 730a 486f 6d65 2d70  databases.Home-p
 00000070: 6167 653a 2068 7474 7073 3a2f 2f67 6974  age: https://git
 00000080: 6875 622e 636f 6d2f 6b75 7274 6d63 6b65  hub.com/kurtmcke
 00000090: 652f 7371 6c69 7465 696d 706f 7274 0a4c  e/sqliteimport.L
 000000a0: 6963 656e 7365 3a20 4d49 540a 4175 7468  icense: MIT.Auth
@@ -31,81 +31,92 @@
 000001e0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
 000001f0: 2033 2e31 300a 436c 6173 7369 6669 6572   3.10.Classifier
 00000200: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
 00000210: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
 00000220: 203a 3a20 332e 3131 0a43 6c61 7373 6966   :: 3.11.Classif
 00000230: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
 00000240: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000250: 686f 6e20 3a3a 2033 2e31 320a 5072 6f6a  hon :: 3.12.Proj
-00000260: 6563 742d 5552 4c3a 2052 6570 6f73 6974  ect-URL: Reposit
-00000270: 6f72 792c 2068 7474 7073 3a2f 2f67 6974  ory, https://git
-00000280: 6875 622e 636f 6d2f 6b75 7274 6d63 6b65  hub.com/kurtmcke
-00000290: 652f 7371 6c69 7465 696d 706f 7274 0a44  e/sqliteimport.D
-000002a0: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
-000002b0: 6e74 2d54 7970 653a 2074 6578 742f 782d  nt-Type: text/x-
-000002c0: 7273 740a 0a2e 2e0a 2020 2020 5468 6973  rst.....    This
-000002d0: 2066 696c 6520 6973 2061 2070 6172 7420   file is a part 
-000002e0: 6f66 2073 716c 6974 6569 6d70 6f72 7420  of sqliteimport 
-000002f0: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
-00000300: 636f 6d2f 6b75 7274 6d63 6b65 652f 7371  com/kurtmckee/sq
-00000310: 6c69 7465 696d 706f 7274 3e0a 2020 2020  liteimport>.    
-00000320: 436f 7079 7269 6768 7420 3230 3234 204b  Copyright 2024 K
-00000330: 7572 7420 4d63 4b65 6520 3c63 6f6e 7461  urt McKee <conta
-00000340: 6374 6d65 406b 7572 746d 636b 6565 2e6f  ctme@kurtmckee.o
-00000350: 7267 3e0a 2020 2020 5350 4458 2d4c 6963  rg>.    SPDX-Lic
-00000360: 656e 7365 2d49 6465 6e74 6966 6965 723a  ense-Identifier:
-00000370: 204d 4954 0a0a 0a73 716c 6974 6569 6d70   MIT...sqliteimp
-00000380: 6f72 740a 2323 2323 2323 2323 2323 2323  ort.############
-00000390: 0a0a 2a49 6d70 6f72 7420 5079 7468 6f6e  ..*Import Python
-000003a0: 2063 6f64 6520 6672 6f6d 2073 716c 6974   code from sqlit
-000003b0: 6520 6461 7461 6261 7365 732e 2a0a 0a2d  e databases.*..-
-000003c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000003d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000003e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000003f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000400: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  --------------..
-00000410: 4465 6d6f 2075 7361 6765 2065 7861 6d70  Demo usage examp
-00000420: 6c65 2c20 7573 696e 6720 636f 6465 2069  le, using code i
-00000430: 6e20 6074 6865 2073 716c 6974 6569 6d70  n `the sqliteimp
-00000440: 6f72 7420 7265 706f 7369 746f 7279 605f  ort repository`_
-00000450: 3a0a 0a2e 2e20 2063 6f64 652d 626c 6f63  :....  code-bloc
-00000460: 6b3a 3a20 6261 7368 0a0a 2020 2020 2320  k:: bash..    # 
-00000470: 496e 7374 616c 6c20 2772 6571 7565 7374  Install 'request
-00000480: 7327 2069 6e20 6120 7374 616e 6461 6c6f  s' in a standalo
-00000490: 6e65 2064 6972 6563 746f 7279 2e0a 2020  ne directory..  
-000004a0: 2020 7069 7020 696e 7374 616c 6c20 2d2d    pip install --
-000004b0: 7461 7267 6574 3d73 616d 706c 6520 7265  target=sample re
-000004c0: 7175 6573 7473 0a0a 2020 2020 2320 4765  quests..    # Ge
-000004d0: 6e65 7261 7465 2061 2073 716c 6974 6520  nerate a sqlite 
-000004e0: 6461 7461 6261 7365 2063 6f6e 7461 696e  database contain
-000004f0: 696e 6720 7468 6520 696e 7374 616c 6c65  ing the installe
-00000500: 6420 7061 636b 6167 6573 2e0a 2020 2020  d packages..    
-00000510: 7079 7468 6f6e 2067 656e 6572 6174 652d  python generate-
-00000520: 7361 6d70 6c65 2e70 790a 0a20 2020 2023  sample.py..    #
-00000530: 2044 656d 6f6e 7374 7261 7465 2074 6861   Demonstrate tha
-00000540: 7420 696d 706f 7274 696e 6720 6672 6f6d  t importing from
-00000550: 2061 2064 6174 6162 6173 6520 776f 726b   a database work
-00000560: 732e 0a20 2020 2070 7974 686f 6e20 6465  s..    python de
-00000570: 6d6f 2e70 790a 0a0a 5468 6973 2069 7320  mo.py...This is 
-00000580: 7468 6520 6f75 7470 7574 3a0a 0a2e 2e20  the output:.... 
-00000590: 2063 6f64 652d 626c 6f63 6b3a 3a20 636f   code-block:: co
-000005a0: 6e73 6f6c 650a 0a20 2020 2024 2070 7974  nsole..    $ pyt
-000005b0: 686f 6e20 6465 6d6f 2e70 790a 2020 2020  hon demo.py.    
-000005c0: 5468 6520 7265 7175 6573 7473 206d 6f64  The requests mod
-000005d0: 756c 6520 6f62 6a65 6374 3a0a 2020 2020  ule object:.    
-000005e0: 3c6d 6f64 756c 6520 2772 6571 7565 7374  <module 'request
-000005f0: 7327 2028 7361 6d70 6c65 2e73 716c 6974  s' (sample.sqlit
-00000600: 6533 293e 0a0a 2020 2020 4669 7273 7420  e3)>..    First 
-00000610: 6c69 6e65 206f 6620 7468 6520 4854 4d4c  line of the HTML
-00000620: 2072 6573 706f 6e73 653a 0a20 2020 203c   response:.    <
-00000630: 2144 4f43 5459 5045 2068 746d 6c3e 0a0a  !DOCTYPE html>..
-00000640: 2e2e 2020 7761 726e 696e 673a 3a0a 0a20  ..  warning::.. 
-00000650: 2020 2054 6865 2064 6174 6162 6173 6520     The database 
-00000660: 666f 726d 6174 2069 7320 6c69 6b65 6c79  format is likely
-00000670: 2074 6f20 6368 616e 6765 2061 7320 7468   to change as th
-00000680: 6520 7072 6f6a 6563 7420 6d61 7475 7265  e project mature
-00000690: 732e 0a0a 2e2e 2020 5f74 6865 2073 716c  s.....  _the sql
-000006a0: 6974 6569 6d70 6f72 7420 7265 706f 7369  iteimport reposi
-000006b0: 746f 7279 3a20 6874 7470 733a 2f2f 6769  tory: https://gi
-000006c0: 7468 7562 2e63 6f6d 2f6b 7572 746d 636b  thub.com/kurtmck
-000006d0: 6565 2f73 716c 6974 6569 6d70 6f72 740a  ee/sqliteimport.
-000006e0: 0a                                       .
+00000250: 686f 6e20 3a3a 2033 2e31 320a 5072 6f76  hon :: 3.12.Prov
+00000260: 6964 6573 2d45 7874 7261 3a20 636c 690a  ides-Extra: cli.
+00000270: 5265 7175 6972 6573 2d44 6973 743a 2063  Requires-Dist: c
+00000280: 6c69 636b 2028 3e3d 382c 3c39 2920 3b20  lick (>=8,<9) ; 
+00000290: 6578 7472 6120 3d3d 2022 636c 6922 0a50  extra == "cli".P
+000002a0: 726f 6a65 6374 2d55 524c 3a20 5265 706f  roject-URL: Repo
+000002b0: 7369 746f 7279 2c20 6874 7470 733a 2f2f  sitory, https://
+000002c0: 6769 7468 7562 2e63 6f6d 2f6b 7572 746d  github.com/kurtm
+000002d0: 636b 6565 2f73 716c 6974 6569 6d70 6f72  ckee/sqliteimpor
+000002e0: 740a 4465 7363 7269 7074 696f 6e2d 436f  t.Description-Co
+000002f0: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
+00000300: 2f78 2d72 7374 0a0a 2e2e 0a20 2020 2054  /x-rst.....    T
+00000310: 6869 7320 6669 6c65 2069 7320 6120 7061  his file is a pa
+00000320: 7274 206f 6620 7371 6c69 7465 696d 706f  rt of sqliteimpo
+00000330: 7274 203c 6874 7470 733a 2f2f 6769 7468  rt <https://gith
+00000340: 7562 2e63 6f6d 2f6b 7572 746d 636b 6565  ub.com/kurtmckee
+00000350: 2f73 716c 6974 6569 6d70 6f72 743e 0a20  /sqliteimport>. 
+00000360: 2020 2043 6f70 7972 6967 6874 2032 3032     Copyright 202
+00000370: 3420 4b75 7274 204d 634b 6565 203c 636f  4 Kurt McKee <co
+00000380: 6e74 6163 746d 6540 6b75 7274 6d63 6b65  ntactme@kurtmcke
+00000390: 652e 6f72 673e 0a20 2020 2053 5044 582d  e.org>.    SPDX-
+000003a0: 4c69 6365 6e73 652d 4964 656e 7469 6669  License-Identifi
+000003b0: 6572 3a20 4d49 540a 0a0a 7371 6c69 7465  er: MIT...sqlite
+000003c0: 696d 706f 7274 0a23 2323 2323 2323 2323  import.#########
+000003d0: 2323 230a 0a2a 496d 706f 7274 2050 7974  ###..*Import Pyt
+000003e0: 686f 6e20 636f 6465 2066 726f 6d20 7371  hon code from sq
+000003f0: 6c69 7465 2064 6174 6162 6173 6573 2e2a  lite databases.*
+00000400: 0a0a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ..--------------
+00000410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000430: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000440: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000450: 2d0a 0a44 656d 6f20 7573 6167 6520 6578  -..Demo usage ex
+00000460: 616d 706c 652c 2075 7369 6e67 2060 6064  ample, using ``d
+00000470: 656d 6f2e 7079 6060 2069 6e20 6074 6865  emo.py`` in `the
+00000480: 2073 716c 6974 6569 6d70 6f72 7420 7265   sqliteimport re
+00000490: 706f 7369 746f 7279 605f 3a0a 0a2e 2e20  pository`_:.... 
+000004a0: 2063 6f64 652d 626c 6f63 6b3a 3a20 6261   code-block:: ba
+000004b0: 7368 0a0a 2020 2020 2320 456e 7375 7265  sh..    # Ensure
+000004c0: 2073 716c 6974 6569 6d70 6f72 7420 6973   sqliteimport is
+000004d0: 2069 6e73 7461 6c6c 6564 2077 6974 6820   installed with 
+000004e0: 7468 6520 2763 6c69 2720 6578 7472 612e  the 'cli' extra.
+000004f0: 0a20 2020 2070 6970 2069 6e73 7461 6c6c  .    pip install
+00000500: 2073 716c 6974 6569 6d70 6f72 745b 636c   sqliteimport[cl
+00000510: 695d 0a0a 2020 2020 2320 496e 7374 616c  i]..    # Instal
+00000520: 6c20 2772 6571 7565 7374 7327 2069 6e20  l 'requests' in 
+00000530: 6120 7374 616e 6461 6c6f 6e65 2064 6972  a standalone dir
+00000540: 6563 746f 7279 2e0a 2020 2020 7069 7020  ectory..    pip 
+00000550: 696e 7374 616c 6c20 2d2d 7461 7267 6574  install --target
+00000560: 3d73 616d 706c 6520 7265 7175 6573 7473  =sample requests
+00000570: 0a0a 2020 2020 2320 4765 6e65 7261 7465  ..    # Generate
+00000580: 2061 2073 716c 6974 6520 6461 7461 6261   a sqlite databa
+00000590: 7365 2063 6f6e 7461 696e 696e 6720 7468  se containing th
+000005a0: 6520 696e 7374 616c 6c65 6420 7061 636b  e installed pack
+000005b0: 6167 6573 2e0a 2020 2020 7371 6c69 7465  ages..    sqlite
+000005c0: 696d 706f 7274 2062 756e 646c 6520 7361  import bundle sa
+000005d0: 6d70 6c65 2073 616d 706c 652e 7371 6c69  mple sample.sqli
+000005e0: 7465 330a 0a20 2020 2023 2044 656d 6f6e  te3..    # Demon
+000005f0: 7374 7261 7465 2074 6861 7420 696d 706f  strate that impo
+00000600: 7274 696e 6720 6672 6f6d 2061 2064 6174  rting from a dat
+00000610: 6162 6173 6520 776f 726b 732e 0a20 2020  abase works..   
+00000620: 2070 7974 686f 6e20 6465 6d6f 2e70 7920   python demo.py 
+00000630: 7361 6d70 6c65 2e73 716c 6974 6533 0a0a  sample.sqlite3..
+00000640: 0a54 6869 7320 6973 2074 6865 206f 7574  .This is the out
+00000650: 7075 743a 0a0a 2e2e 2020 636f 6465 2d62  put:....  code-b
+00000660: 6c6f 636b 3a3a 2063 6f6e 736f 6c65 0a0a  lock:: console..
+00000670: 2020 2020 2420 7079 7468 6f6e 2064 656d      $ python dem
+00000680: 6f2e 7079 0a20 2020 2054 6865 2072 6571  o.py.    The req
+00000690: 7565 7374 7320 6d6f 6475 6c65 206f 626a  uests module obj
+000006a0: 6563 743a 0a20 2020 203c 6d6f 6475 6c65  ect:.    <module
+000006b0: 2027 7265 7175 6573 7473 2720 2873 616d   'requests' (sam
+000006c0: 706c 652e 7371 6c69 7465 3329 3e0a 0a20  ple.sqlite3)>.. 
+000006d0: 2020 2052 6571 7565 7374 696e 6720 6120     Requesting a 
+000006e0: 7765 6270 6167 652e 2e2e 7375 6363 6573  webpage...succes
+000006f0: 7321 0a0a 2e2e 2020 7761 726e 696e 673a  s!....  warning:
+00000700: 3a0a 0a20 2020 2054 6865 2064 6174 6162  :..    The datab
+00000710: 6173 6520 666f 726d 6174 2069 7320 6c69  ase format is li
+00000720: 6b65 6c79 2074 6f20 6368 616e 6765 2061  kely to change a
+00000730: 7320 7468 6520 7072 6f6a 6563 7420 6d61  s the project ma
+00000740: 7475 7265 732e 0a0a 2e2e 2020 5f74 6865  tures.....  _the
+00000750: 2073 716c 6974 6569 6d70 6f72 7420 7265   sqliteimport re
+00000760: 706f 7369 746f 7279 3a20 6874 7470 733a  pository: https:
+00000770: 2f2f 6769 7468 7562 2e63 6f6d 2f6b 7572  //github.com/kur
+00000780: 746d 636b 6565 2f73 716c 6974 6569 6d70  tmckee/sqliteimp
+00000790: 6f72 740a 0a                             ort..
```

