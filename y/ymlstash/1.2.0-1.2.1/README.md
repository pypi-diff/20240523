# Comparing `tmp/ymlstash-1.2.0.tar.gz` & `tmp/ymlstash-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ymlstash-1.2.0.tar", max compression
+gzip compressed data, was "ymlstash-1.2.1.tar", max compression
```

## Comparing `ymlstash-1.2.0.tar` & `ymlstash-1.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2024-05-07 18:56:12.873162 ymlstash-1.2.0/LICENSE
--rw-r--r--   0        0        0     1457 2024-05-09 09:50:41.964518 ymlstash-1.2.0/README.md
--rw-r--r--   0        0        0      572 2024-05-09 11:15:01.364528 ymlstash-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       50 2024-05-07 13:34:28.333474 ymlstash-1.2.0/ymlstash/__init__.py
--rw-r--r--   0        0        0     2526 2024-05-09 11:09:33.056267 ymlstash-1.2.0/ymlstash/stash.py
--rw-r--r--   0        0        0     2223 1970-01-01 00:00:00.000000 ymlstash-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-07 18:56:12.873162 ymlstash-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1900 2024-05-23 09:08:04.319656 ymlstash-1.2.1/README.md
+-rw-r--r--   0        0        0      588 2024-05-23 09:09:26.395768 ymlstash-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0       50 2024-05-07 13:34:28.333474 ymlstash-1.2.1/ymlstash/__init__.py
+-rw-r--r--   0        0        0     2526 2024-05-09 18:24:49.258631 ymlstash-1.2.1/ymlstash/stash.py
+-rw-r--r--   0        0        0     2666 1970-01-01 00:00:00.000000 ymlstash-1.2.1/PKG-INFO
```

### Comparing `ymlstash-1.2.0/LICENSE` & `ymlstash-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ymlstash-1.2.0/pyproject.toml` & `ymlstash-1.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "ymlstash"
-version = "1.2.0"
+version = "1.2.1"
 description = "A simple ORM-like utility for operating on local YAML files via Python dataclasses"
 authors = ["Yuval Adam <_@yuv.al>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/yuvadm/ymlstash"
 repository = "https://github.com/yuvadm/ymlstash"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pyyaml = "^6.0.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.0"
+ruff = "^0.4.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
```

### Comparing `ymlstash-1.2.0/ymlstash/stash.py` & `ymlstash-1.2.1/ymlstash/stash.py`

 * *Files identical despite different names*

### Comparing `ymlstash-1.2.0/PKG-INFO` & `ymlstash-1.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ymlstash
-Version: 1.2.0
+Version: 1.2.1
 Summary: A simple ORM-like utility for operating on local YAML files via Python dataclasses
 Home-page: https://github.com/yuvadm/ymlstash
 License: MIT
 Author: Yuval Adam
 Author-email: _@yuv.al
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -18,60 +18,70 @@
 Project-URL: Repository, https://github.com/yuvadm/ymlstash
 Description-Content-Type: text/markdown
 
 # ymlstash
 
 A simple ORM-like utility for operating on local YAML files via Python dataclasses.
 
+In the context of this library, a *stash* is a diretory in the filesystem that holds many `.yml` files that all adhere to the same structure.
+
+`ymlstash` simplifies the management of such a basic database of files.
+
 ## Install
 
 Package is published on PyPI - https://pypi.org/project/ymlstash/
 
 Install from pip or your favorite package manager:
 
 ```bash
 $ pip install ymlstash
 ```
 
 ## Usage
 
-Define a dataclass:
+Start by defining your model as a dataclass:
 
 ```python
 from dataclasses import dataclass
 from typing import ClassVar
 
 @dataclass
 class User:
     name: str
     age: int
     active: bool
     key: ClassVar[str] = "name"
 ```
 
-Note the special `key` field which is used to denote that `name` should be used as the primary key field. If an object has `name: "foo"`, it will be saved as `foo.yml` in the stash root directory.
+### Primary Keys
+
+Each model **must** include a primary key that will be used as the entry filename to uniquely access each record. 
+
+The recommended way do to this is with the special `key` field which is used to denote that `name` should be used as the primary key field. If an object has `name: "foo"`, it will be saved as `foo.yml` in the stash root directory.
+
+### Actions
 
 Instantiate a new object:
 
 ```python
 user = User(name="yuval", age=42, active=True)
 ```
 
 Save it to file:
 
 ```python
 from ymlstash import YmlStash
 
-stash = YmlStash(User, "path/to/db")
+stash = YmlStash(User, "path/to/db")  # path can either be a string or Path() object
 stash.save(user)
 ```
 
 This will create a `yuval.yml` file in the stash root directory.
 
-When saving to file, a `key` field must be present on the dataclass, otherwise an explicit `key` must be passed:
+If the `key` field is not present on the dataclass, an explicit `key` must be passed:
 
 ```python
 stash.save(obj, key="custom-key")
 ```
 
 Load from file:
 
@@ -87,15 +97,15 @@
 
 Delete a key:
 
 ```python
 stash.delete("foo")
 ```
 
-Check for key existance:
+Check for key existence:
 
 ```python
 stash.exists("foo")
 ```
 
 Drop all files (careful, this deletes everything):
```

