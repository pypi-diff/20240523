# Comparing `tmp/hatch_datavolo_nar-0.1.0.tar.gz` & `tmp/hatch_datavolo_nar-0.1.1.tar.gz`

## Comparing `hatch_datavolo_nar-0.1.0.tar` & `hatch_datavolo_nar-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 hatch_datavolo_nar-0.1.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 hatch_datavolo_nar-0.1.0/.github/workflows/build.yml
--rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 hatch_datavolo_nar-0.1.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 hatch_datavolo_nar-0.1.0/src/hatch_datavolo_nar/__about__.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 hatch_datavolo_nar-0.1.0/src/hatch_datavolo_nar/__init__.py
--rw-r--r--   0        0        0     5643 2020-02-02 00:00:00.000000 hatch_datavolo_nar-0.1.0/src/hatch_datavolo_nar/builder.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 hatch_datavolo_nar-0.1.0/src/hatch_datavolo_nar/hooks.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 hatch_datavolo_nar-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 hatch_datavolo_nar-0.1.0/tests/test_builder.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 hatch_datavolo_nar-0.1.0/tests/test_hooks.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 hatch_datavolo_nar-0.1.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 hatch_datavolo_nar-0.1.0/LICENSE
--rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 hatch_datavolo_nar-0.1.0/README.md
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 hatch_datavolo_nar-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    17156 2020-02-02 00:00:00.000000 hatch_datavolo_nar-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 hatch_datavolo_nar-0.1.1/.github/CODEOWNERS
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 hatch_datavolo_nar-0.1.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 hatch_datavolo_nar-0.1.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 hatch_datavolo_nar-0.1.1/src/hatch_datavolo_nar/__about__.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 hatch_datavolo_nar-0.1.1/src/hatch_datavolo_nar/__init__.py
+-rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 hatch_datavolo_nar-0.1.1/src/hatch_datavolo_nar/builder.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 hatch_datavolo_nar-0.1.1/src/hatch_datavolo_nar/hooks.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 hatch_datavolo_nar-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     5583 2020-02-02 00:00:00.000000 hatch_datavolo_nar-0.1.1/tests/test_builder.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 hatch_datavolo_nar-0.1.1/tests/test_hooks.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 hatch_datavolo_nar-0.1.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 hatch_datavolo_nar-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 hatch_datavolo_nar-0.1.1/README.md
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 hatch_datavolo_nar-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    17396 2020-02-02 00:00:00.000000 hatch_datavolo_nar-0.1.1/PKG-INFO
```

### Comparing `hatch_datavolo_nar-0.1.0/.github/workflows/build.yml` & `hatch_datavolo_nar-0.1.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `hatch_datavolo_nar-0.1.0/.github/workflows/release.yml` & `hatch_datavolo_nar-0.1.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `hatch_datavolo_nar-0.1.0/src/hatch_datavolo_nar/builder.py` & `hatch_datavolo_nar-0.1.1/src/hatch_datavolo_nar/builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # SPDX-FileCopyrightText: 2024 Datavolo Inc.
 #
 # SPDX-License-Identifier: Apache-2.0
 
 import io
 import os
 import sys
-import time
 from collections.abc import Callable, Generator
 from contextlib import contextmanager
 from pathlib import Path
 from shlex import quote
 from shutil import rmtree
 from subprocess import PIPE, check_call
 from typing import Any
-from zipfile import ZIP_DEFLATED, ZipFile, ZipInfo
+from zipfile import ZIP_DEFLATED, ZipFile
 
 from hatchling.builders.config import BuilderConfig
 from hatchling.builders.plugin.interface import BuilderInterface
 from hatchling.builders.utils import normalize_archive_path
 from hatchling.metadata.core import ProjectMetadata
 
 
 class NarBundle:
+    DIRECTORY_MODE = 0o755
+
     def __init__(self, zip_descriptor: ZipFile):
         self.zip_descriptor = zip_descriptor
         self.directories_added: list[str] = []
 
     def add_entry(self, path: Path, archive_name: str) -> None:
         normalized_archive_name = normalize_archive_path(archive_name)
 
@@ -38,19 +39,16 @@
             if parent_dir_name not in self.directories_added:
                 self.mkdir(parent_dir_name)
                 self.directories_added.append(parent_dir_name)
 
         self.zip_descriptor.write(path, normalized_archive_name)
 
     def mkdir(self, directory_name: str) -> None:
-        now = time.localtime()
-        date_time = now[0:6]
-        archive_info = ZipInfo(f"{directory_name}/", date_time)
-        archive_info.CRC = 0
-        self.zip_descriptor.mkdir(archive_info)
+        directory_mode = self.DIRECTORY_MODE
+        self.zip_descriptor.mkdir(directory_name, mode=directory_mode)
 
     def write_manifest(self, metadata: ProjectMetadata) -> None:
         manifest_dir = "META-INF"
         self.mkdir(manifest_dir)
 
         manifest_lines = [
             "Manifest-Version: 1.0",
```

### Comparing `hatch_datavolo_nar-0.1.0/tests/test_builder.py` & `hatch_datavolo_nar-0.1.1/tests/test_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -133,14 +133,20 @@
         assert f"{source_dir}/{record_package}/{record_processor_name}" in nar_entries
         assert "META-INF/" in nar_entries
         assert "NAR-INF/" in nar_entries
         assert "NAR-INF/bundled-dependencies/" in nar_entries
         assert "NAR-INF/bundled-dependencies/bech32/" in nar_entries
         assert "NAR-INF/bundled-dependencies/bech32/__init__.py" in nar_entries
 
+        meta_dir_info = nar.getinfo("META-INF/")
+
+        expected_directory_mode = 0o755
+        expected_external_attr = ((0o40000 | expected_directory_mode) & 0xFFFF) << 16 | 0x10
+        assert meta_dir_info.external_attr == expected_external_attr
+
     cache_path = dist_path / "pip-cache"
     assert cache_path.is_dir()
 
     builder.clean(dist_path.as_posix(), [])
 
     assert not cache_path.is_dir()
```

### Comparing `hatch_datavolo_nar-0.1.0/.gitignore` & `hatch_datavolo_nar-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hatch_datavolo_nar-0.1.0/LICENSE` & `hatch_datavolo_nar-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hatch_datavolo_nar-0.1.0/README.md` & `hatch_datavolo_nar-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 This project provides a [Builder](https://hatch.pypa.io/latest/plugins/builder/reference/) plugin
 for the [Hatch](https://hatch.pypa.io/latest/) Python project manager that enables building packaged
 archives for [Apache NiFi](https://nifi.apache.org). The NAR format uses the
 [ZIP](https://en.wikipedia.org/wiki/ZIP_(file_format)) file structure, containing a manifest
 and NiFi components with dependencies.
 
+[![pypi](https://img.shields.io/pypi/v/hatch-datavolo-nar.svg)](https://pypi.org/project/hatch-datavolo-nar/)
+[![python-versions](https://img.shields.io/pypi/pyversions/hatch-datavolo-nar.svg)](https://pypi.org/project/hatch-datavolo-nar/)
 [![build](https://github.com/datavolo-io/hatch-datavolo-nar/actions/workflows/build.yml/badge.svg)](https://github.com/datavolo-io/hatch-datavolo-nar/actions/workflows/build.yml)
 [![license](https://img.shields.io/github/license/datavolo-io/hatch-datavolo-nar)](https://github.com/datavolo-io/hatch-datavolo-nar/blob/main/LICENSE)
 [![Hatch](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy)
 
 ## Integrating
```

### Comparing `hatch_datavolo_nar-0.1.0/pyproject.toml` & `hatch_datavolo_nar-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hatch_datavolo_nar-0.1.0/PKG-INFO` & `hatch_datavolo_nar-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hatch-datavolo-nar
-Version: 0.1.0
+Version: 0.1.1
 Summary: Hatch plugin for building Apache NiFi NAR bundles
 Project-URL: Issues, https://github.com/datavolo-io/hatch-datavolo-nar/issues
 Project-URL: Source, https://github.com/datavolo-io/hatch-datavolo-nar
 Author-email: Datavolo Developers <dev@datavolo.io>
 Maintainer-email: Datavolo Developers <dev@datavolo.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
@@ -224,14 +224,16 @@
 
 This project provides a [Builder](https://hatch.pypa.io/latest/plugins/builder/reference/) plugin
 for the [Hatch](https://hatch.pypa.io/latest/) Python project manager that enables building packaged
 archives for [Apache NiFi](https://nifi.apache.org). The NAR format uses the
 [ZIP](https://en.wikipedia.org/wiki/ZIP_(file_format)) file structure, containing a manifest
 and NiFi components with dependencies.
 
+[![pypi](https://img.shields.io/pypi/v/hatch-datavolo-nar.svg)](https://pypi.org/project/hatch-datavolo-nar/)
+[![python-versions](https://img.shields.io/pypi/pyversions/hatch-datavolo-nar.svg)](https://pypi.org/project/hatch-datavolo-nar/)
 [![build](https://github.com/datavolo-io/hatch-datavolo-nar/actions/workflows/build.yml/badge.svg)](https://github.com/datavolo-io/hatch-datavolo-nar/actions/workflows/build.yml)
 [![license](https://img.shields.io/github/license/datavolo-io/hatch-datavolo-nar)](https://github.com/datavolo-io/hatch-datavolo-nar/blob/main/LICENSE)
 [![Hatch](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy)
 
 ## Integrating
```

