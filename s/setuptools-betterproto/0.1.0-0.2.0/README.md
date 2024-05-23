# Comparing `tmp/setuptools-betterproto-0.1.0.tar.gz` & `tmp/setuptools-betterproto-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools-betterproto-0.1.0.tar", last modified: Wed May 15 12:51:52 2024, max compression
+gzip compressed data, was "setuptools-betterproto-0.2.0.tar", last modified: Thu May 23 08:51:45 2024, max compression
```

## Comparing `setuptools-betterproto-0.1.0.tar` & `setuptools-betterproto-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:51:52.743488 setuptools-betterproto-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-15 12:51:47.000000 setuptools-betterproto-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-15 12:51:47.000000 setuptools-betterproto-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-15 12:51:52.743488 setuptools-betterproto-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-05-15 12:51:47.000000 setuptools-betterproto-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-15 12:51:47.000000 setuptools-betterproto-0.1.0/RELEASE_NOTES.md
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-15 12:51:47.000000 setuptools-betterproto-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 12:51:52.743488 setuptools-betterproto-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:51:52.739488 setuptools-betterproto-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:51:52.743488 setuptools-betterproto-0.1.0/src/setuptools_betterproto/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-15 12:51:47.000000 setuptools-betterproto-0.1.0/src/setuptools_betterproto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-05-15 12:51:47.000000 setuptools-betterproto-0.1.0/src/setuptools_betterproto/_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-15 12:51:47.000000 setuptools-betterproto-0.1.0/src/setuptools_betterproto/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-15 12:51:47.000000 setuptools-betterproto-0.1.0/src/setuptools_betterproto/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 12:51:47.000000 setuptools-betterproto-0.1.0/src/setuptools_betterproto/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 12:51:52.743488 setuptools-betterproto-0.1.0/src/setuptools_betterproto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-15 12:51:52.000000 setuptools-betterproto-0.1.0/src/setuptools_betterproto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-15 12:51:52.000000 setuptools-betterproto-0.1.0/src/setuptools_betterproto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 12:51:52.000000 setuptools-betterproto-0.1.0/src/setuptools_betterproto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-15 12:51:52.000000 setuptools-betterproto-0.1.0/src/setuptools_betterproto.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-15 12:51:52.000000 setuptools-betterproto-0.1.0/src/setuptools_betterproto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-15 12:51:52.000000 setuptools-betterproto-0.1.0/src/setuptools_betterproto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:51:45.913051 setuptools-betterproto-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-23 08:51:38.000000 setuptools-betterproto-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-23 08:51:38.000000 setuptools-betterproto-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-05-23 08:51:45.913051 setuptools-betterproto-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-23 08:51:38.000000 setuptools-betterproto-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-23 08:51:38.000000 setuptools-betterproto-0.2.0/RELEASE_NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-05-23 08:51:38.000000 setuptools-betterproto-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 08:51:45.913051 setuptools-betterproto-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:51:45.909051 setuptools-betterproto-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:51:45.909051 setuptools-betterproto-0.2.0/src/setuptools_betterproto/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-23 08:51:38.000000 setuptools-betterproto-0.2.0/src/setuptools_betterproto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-23 08:51:38.000000 setuptools-betterproto-0.2.0/src/setuptools_betterproto/_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-05-23 08:51:38.000000 setuptools-betterproto-0.2.0/src/setuptools_betterproto/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-23 08:51:38.000000 setuptools-betterproto-0.2.0/src/setuptools_betterproto/_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-23 08:51:38.000000 setuptools-betterproto-0.2.0/src/setuptools_betterproto/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:51:38.000000 setuptools-betterproto-0.2.0/src/setuptools_betterproto/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:51:45.913051 setuptools-betterproto-0.2.0/src/setuptools_betterproto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-05-23 08:51:45.000000 setuptools-betterproto-0.2.0/src/setuptools_betterproto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-23 08:51:45.000000 setuptools-betterproto-0.2.0/src/setuptools_betterproto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 08:51:45.000000 setuptools-betterproto-0.2.0/src/setuptools_betterproto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-23 08:51:45.000000 setuptools-betterproto-0.2.0/src/setuptools_betterproto.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-23 08:51:45.000000 setuptools-betterproto-0.2.0/src/setuptools_betterproto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-23 08:51:45.000000 setuptools-betterproto-0.2.0/src/setuptools_betterproto.egg-info/top_level.txt
```

### Comparing `setuptools-betterproto-0.1.0/LICENSE` & `setuptools-betterproto-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools-betterproto-0.1.0/PKG-INFO` & `setuptools-betterproto-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-betterproto
-Version: 0.1.0
+Version: 0.2.0
 Summary: A modern setuptools plugin to generate Python files from proto files using betterproto
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Documentation, https://frequenz-floss.github.io/setuptools-betterproto/
 Project-URL: Changelog, https://github.com/frequenz-floss/setuptools-betterproto/releases
 Project-URL: Issues, https://github.com/frequenz-floss/setuptools-betterproto/issues
 Project-URL: Repository, https://github.com/frequenz-floss/setuptools-betterproto
@@ -92,34 +92,26 @@
 
 You should add [betterproto] as a dependency too, for example:
 
 ```toml
 dependencies = ["betterproto == 2.0.0b6"]
 ```
 
-You probably also need to add the protobuf files to the `MANIFEST.in` file, so
-they are included in the source distribution. For example (following our
-customized example):
-
-```plaintext
-recursive-include proto *.proto
-```
-
 Once this is done, the conversion of the proto files to Python files should be
 automatic. Just try building the package with:
 
 ```sh
 python -m pip install build
 python -m build
 ```
 
 A new command to generate the files will be also added to `setuptools`, you can
 run it manually with:
 ```sh
-python -c 'import setuptools; setuptools.setup()' build_betterproto
+python -c 'import setuptools; setuptools.setup()' compile_betterproto
 ```
 
 You can also pass the configuration options via command line for quick testing,
 try passing `--help` at the end of the command to see the available options.
 
 ## Contributing
```

### Comparing `setuptools-betterproto-0.1.0/README.md` & `setuptools-betterproto-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -60,34 +60,26 @@
 
 You should add [betterproto] as a dependency too, for example:
 
 ```toml
 dependencies = ["betterproto == 2.0.0b6"]
 ```
 
-You probably also need to add the protobuf files to the `MANIFEST.in` file, so
-they are included in the source distribution. For example (following our
-customized example):
-
-```plaintext
-recursive-include proto *.proto
-```
-
 Once this is done, the conversion of the proto files to Python files should be
 automatic. Just try building the package with:
 
 ```sh
 python -m pip install build
 python -m build
 ```
 
 A new command to generate the files will be also added to `setuptools`, you can
 run it manually with:
 ```sh
-python -c 'import setuptools; setuptools.setup()' build_betterproto
+python -c 'import setuptools; setuptools.setup()' compile_betterproto
 ```
 
 You can also pass the configuration options via command line for quick testing,
 try passing `--help` at the end of the command to see the available options.
 
 ## Contributing
```

### Comparing `setuptools-betterproto-0.1.0/pyproject.toml` & `setuptools-betterproto-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -42,16 +42,20 @@
 ]
 dynamic = ["version"]
 
 [[project.authors]]
 name = "Frequenz Energy-as-a-Service GmbH"
 email = "floss@frequenz.com"
 
+[project.entry-points."setuptools.finalize_distribution_options"]
+finalize_distribution_options_betterproto = "setuptools_betterproto:finalize_distribution_options"
+
 [project.entry-points."distutils.commands"]
-build_betterproto = "setuptools_betterproto:CompileProto"
+compile_betterproto = "setuptools_betterproto:CompileBetterproto"
+add_proto_files = "setuptools_betterproto:AddProtoFiles"
 
 [project.optional-dependencies]
 dev-flake8 = [
   "flake8 == 7.0.0",
   "flake8-docstrings == 1.7.0",
   "flake8-pyproject == 1.2.3",  # For reading the flake8 config from pyproject.toml
   "pydoclint == 0.4.1",
```

### Comparing `setuptools-betterproto-0.1.0/src/setuptools_betterproto/_config.py` & `setuptools-betterproto-0.2.0/src/setuptools_betterproto/_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # License: MIT
 # Copyright © 2024 Frequenz Energy-as-a-Service GmbH
 
 """Manages the configuration to generate files from the protobuf files."""
 
 import dataclasses
 import logging
+import pathlib
 import tomllib
 from collections.abc import Sequence
 from typing import Any, Self
 
 _logger = logging.getLogger(__name__)
 
 
@@ -71,7 +72,46 @@
                 "WARNING: There are some configuration keys in pyproject.toml we don't "
                 "know about and will be ignored: %s",
                 ", ".join(f"'{k}'" for k in unknown_keys),
             )
 
         attrs = dict(defaults, **{k: config[k] for k in (known_keys & config_keys)})
         return dataclasses.replace(default, **attrs)
+
+    @classmethod
+    def from_strings(
+        cls, *, proto_path: str, proto_glob: str, include_paths: str, out_path: str
+    ) -> Self:
+        """Create a new configuration from plain strings.
+
+        Args:
+            proto_path: The path of the root directory containing the protobuf files.
+            proto_glob: The glob pattern to use to find the protobuf files.
+            include_paths: The paths to add to the include path when compiling the
+                protobuf files.
+            out_path: The path of the root directory where the Python files will be
+                generated.
+
+        Returns:
+            The configuration.
+        """
+        return cls(
+            proto_path=proto_path,
+            proto_glob=proto_glob,
+            include_paths=[p.strip() for p in include_paths.split(",")],
+            out_path=out_path,
+        )
+
+    @property
+    def expanded_proto_files(self) -> list[str]:
+        """The files in the `proto_path` expanded according to the configured glob."""
+        proto_path = pathlib.Path(self.proto_path)
+        return [str(proto_file) for proto_file in proto_path.rglob(self.proto_glob)]
+
+    @property
+    def expanded_include_files(self) -> list[str]:
+        """The files in the `include_paths` expanded according to the configured glob."""
+        return [
+            str(proto_file)
+            for include_path in map(pathlib.Path, self.include_paths)
+            for proto_file in include_path.rglob(self.proto_glob)
+        ]
```

### Comparing `setuptools-betterproto-0.1.0/src/setuptools_betterproto.egg-info/PKG-INFO` & `setuptools-betterproto-0.2.0/src/setuptools_betterproto.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-betterproto
-Version: 0.1.0
+Version: 0.2.0
 Summary: A modern setuptools plugin to generate Python files from proto files using betterproto
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Documentation, https://frequenz-floss.github.io/setuptools-betterproto/
 Project-URL: Changelog, https://github.com/frequenz-floss/setuptools-betterproto/releases
 Project-URL: Issues, https://github.com/frequenz-floss/setuptools-betterproto/issues
 Project-URL: Repository, https://github.com/frequenz-floss/setuptools-betterproto
@@ -92,34 +92,26 @@
 
 You should add [betterproto] as a dependency too, for example:
 
 ```toml
 dependencies = ["betterproto == 2.0.0b6"]
 ```
 
-You probably also need to add the protobuf files to the `MANIFEST.in` file, so
-they are included in the source distribution. For example (following our
-customized example):
-
-```plaintext
-recursive-include proto *.proto
-```
-
 Once this is done, the conversion of the proto files to Python files should be
 automatic. Just try building the package with:
 
 ```sh
 python -m pip install build
 python -m build
 ```
 
 A new command to generate the files will be also added to `setuptools`, you can
 run it manually with:
 ```sh
-python -c 'import setuptools; setuptools.setup()' build_betterproto
+python -c 'import setuptools; setuptools.setup()' compile_betterproto
 ```
 
 You can also pass the configuration options via command line for quick testing,
 try passing `--help` at the end of the command to see the available options.
 
 ## Contributing
```

### Comparing `setuptools-betterproto-0.1.0/src/setuptools_betterproto.egg-info/SOURCES.txt` & `setuptools-betterproto-0.2.0/src/setuptools_betterproto.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 RELEASE_NOTES.md
 pyproject.toml
 src/setuptools_betterproto/__init__.py
 src/setuptools_betterproto/_command.py
 src/setuptools_betterproto/_config.py
+src/setuptools_betterproto/_install.py
 src/setuptools_betterproto/conftest.py
 src/setuptools_betterproto/py.typed
 src/setuptools_betterproto.egg-info/PKG-INFO
 src/setuptools_betterproto.egg-info/SOURCES.txt
 src/setuptools_betterproto.egg-info/dependency_links.txt
 src/setuptools_betterproto.egg-info/entry_points.txt
 src/setuptools_betterproto.egg-info/requires.txt
```

### Comparing `setuptools-betterproto-0.1.0/src/setuptools_betterproto.egg-info/requires.txt` & `setuptools-betterproto-0.2.0/src/setuptools_betterproto.egg-info/requires.txt`

 * *Files identical despite different names*

