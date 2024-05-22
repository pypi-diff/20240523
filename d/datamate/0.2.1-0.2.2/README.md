# Comparing `tmp/datamate-0.2.1.tar.gz` & `tmp/datamate-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamate-0.2.1.tar", last modified: Mon Apr 22 11:38:51 2024, max compression
+gzip compressed data, was "datamate-0.2.2.tar", last modified: Wed May 22 22:33:52 2024, max compression
```

## Comparing `datamate-0.2.1.tar` & `datamate-0.2.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 janne      (501) staff       (20)        0 2024-04-22 11:38:51.900633 datamate-0.2.1/
-drwxr-xr-x   0 janne      (501) staff       (20)        0 2024-04-22 11:38:51.891484 datamate-0.2.1/.github/
-drwxr-xr-x   0 janne      (501) staff       (20)        0 2024-04-22 11:38:51.892833 datamate-0.2.1/.github/workflows/
--rw-r--r--   0 janne      (501) staff       (20)     1064 2024-04-16 08:24:47.000000 datamate-0.2.1/.github/workflows/auto_test.yml
--rw-r--r--   0 janne      (501) staff       (20)      151 2024-04-22 10:30:01.000000 datamate-0.2.1/.gitignore
--rw-r--r--   0 janne      (501) staff       (20)      159 2024-04-22 10:30:01.000000 datamate-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 janne      (501) staff       (20)     4354 2024-04-22 11:38:51.900410 datamate-0.2.1/PKG-INFO
--rw-r--r--   0 janne      (501) staff       (20)     2473 2024-04-16 08:25:03.000000 datamate-0.2.1/README.md
-drwxr-xr-x   0 janne      (501) staff       (20)        0 2024-04-22 11:38:51.894424 datamate-0.2.1/datamate/
--rwx------   0 janne      (501) staff       (20)      647 2023-05-03 21:21:07.000000 datamate-0.2.1/datamate/__init__.py
--rw-r--r--   0 janne      (501) staff       (20)    62178 2024-04-22 10:31:26.000000 datamate-0.2.1/datamate/directory.py
--rwx------   0 janne      (501) staff       (20)    11921 2023-05-01 17:35:54.000000 datamate-0.2.1/datamate/namespaces.py
--rw-r--r--   0 janne      (501) staff       (20)      411 2024-04-22 11:38:51.000000 datamate-0.2.1/datamate/version.py
-drwxr-xr-x   0 janne      (501) staff       (20)        0 2024-04-22 11:38:51.898910 datamate-0.2.1/datamate.egg-info/
--rw-r--r--   0 janne      (501) staff       (20)     4354 2024-04-22 11:38:51.000000 datamate-0.2.1/datamate.egg-info/PKG-INFO
--rw-r--r--   0 janne      (501) staff       (20)      494 2024-04-22 11:38:51.000000 datamate-0.2.1/datamate.egg-info/SOURCES.txt
--rw-r--r--   0 janne      (501) staff       (20)        1 2024-04-22 11:38:51.000000 datamate-0.2.1/datamate.egg-info/dependency_links.txt
--rw-r--r--   0 janne      (501) staff       (20)      163 2024-04-22 11:38:51.000000 datamate-0.2.1/datamate.egg-info/requires.txt
--rw-r--r--   0 janne      (501) staff       (20)        9 2024-04-22 11:38:51.000000 datamate-0.2.1/datamate.egg-info/top_level.txt
-drwxr-xr-x   0 janne      (501) staff       (20)        0 2024-04-22 11:38:51.896455 datamate-0.2.1/examples/
--rwx------   0 janne      (501) staff       (20)   457250 2023-05-03 21:33:56.000000 datamate-0.2.1/examples/01. Introduction to Datamate.ipynb
--rwx------   0 janne      (501) staff       (20)   139159 2023-05-03 21:34:34.000000 datamate-0.2.1/examples/another thread.ipynb
--rw-r--r--   0 janne      (501) staff       (20)     1106 2024-04-22 10:31:26.000000 datamate-0.2.1/license
--rw-r--r--   0 janne      (501) staff       (20)      976 2024-04-22 11:32:52.000000 datamate-0.2.1/pyproject.toml
--rw-r--r--   0 janne      (501) staff       (20)       38 2024-04-22 11:38:51.900689 datamate-0.2.1/setup.cfg
-drwxr-xr-x   0 janne      (501) staff       (20)        0 2024-04-22 11:38:51.898633 datamate-0.2.1/tests/
--rwxr-xr-x   0 janne      (501) staff       (20)    32121 2024-04-16 08:25:03.000000 datamate-0.2.1/tests/test_directory.py
--rwx------   0 janne      (501) staff       (20)     3734 2023-05-03 21:20:00.000000 datamate-0.2.1/tests/test_namespaces.py
--rw-r--r--   0 janne      (501) staff       (20)      868 2024-04-16 08:25:03.000000 datamate-0.2.1/tests/test_swmr.py
+drwxr-xr-x   0 janne      (501) staff       (20)        0 2024-05-22 22:33:52.673049 datamate-0.2.2/
+drwxr-xr-x   0 janne      (501) staff       (20)        0 2024-05-22 22:33:52.664224 datamate-0.2.2/.github/
+drwxr-xr-x   0 janne      (501) staff       (20)        0 2024-05-22 22:33:52.665439 datamate-0.2.2/.github/workflows/
+-rw-r--r--   0 janne      (501) staff       (20)     1064 2024-04-16 08:24:47.000000 datamate-0.2.2/.github/workflows/auto_test.yml
+-rw-r--r--   0 janne      (501) staff       (20)      151 2024-04-22 10:30:01.000000 datamate-0.2.2/.gitignore
+-rw-r--r--   0 janne      (501) staff       (20)      159 2024-04-22 10:30:01.000000 datamate-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 janne      (501) staff       (20)     4501 2024-05-22 22:33:52.672855 datamate-0.2.2/PKG-INFO
+-rw-r--r--   0 janne      (501) staff       (20)     2473 2024-04-16 08:25:03.000000 datamate-0.2.2/README.md
+drwxr-xr-x   0 janne      (501) staff       (20)        0 2024-05-22 22:33:52.668013 datamate-0.2.2/datamate/
+-rw-r--r--   0 janne      (501) staff       (20)      683 2024-05-22 16:48:49.000000 datamate-0.2.2/datamate/__init__.py
+-rw-r--r--   0 janne      (501) staff       (20)    71743 2024-05-22 16:48:55.000000 datamate-0.2.2/datamate/directory.py
+-rwx------   0 janne      (501) staff       (20)    11921 2023-05-01 17:35:54.000000 datamate-0.2.2/datamate/namespaces.py
+-rw-r--r--   0 janne      (501) staff       (20)      411 2024-05-22 22:33:52.000000 datamate-0.2.2/datamate/version.py
+drwxr-xr-x   0 janne      (501) staff       (20)        0 2024-05-22 22:33:52.672144 datamate-0.2.2/datamate.egg-info/
+-rw-r--r--   0 janne      (501) staff       (20)     4501 2024-05-22 22:33:52.000000 datamate-0.2.2/datamate.egg-info/PKG-INFO
+-rw-r--r--   0 janne      (501) staff       (20)      494 2024-05-22 22:33:52.000000 datamate-0.2.2/datamate.egg-info/SOURCES.txt
+-rw-r--r--   0 janne      (501) staff       (20)        1 2024-05-22 22:33:52.000000 datamate-0.2.2/datamate.egg-info/dependency_links.txt
+-rw-r--r--   0 janne      (501) staff       (20)      171 2024-05-22 22:33:52.000000 datamate-0.2.2/datamate.egg-info/requires.txt
+-rw-r--r--   0 janne      (501) staff       (20)        9 2024-05-22 22:33:52.000000 datamate-0.2.2/datamate.egg-info/top_level.txt
+drwxr-xr-x   0 janne      (501) staff       (20)        0 2024-05-22 22:33:52.670432 datamate-0.2.2/examples/
+-rwx------   0 janne      (501) staff       (20)   457250 2023-05-03 21:33:56.000000 datamate-0.2.2/examples/01. Introduction to Datamate.ipynb
+-rwx------   0 janne      (501) staff       (20)   139159 2023-05-03 21:34:34.000000 datamate-0.2.2/examples/another thread.ipynb
+-rw-r--r--   0 janne      (501) staff       (20)     1106 2024-04-22 10:31:26.000000 datamate-0.2.2/license
+-rw-r--r--   0 janne      (501) staff       (20)      987 2024-05-22 16:48:49.000000 datamate-0.2.2/pyproject.toml
+-rw-r--r--   0 janne      (501) staff       (20)       38 2024-05-22 22:33:52.673090 datamate-0.2.2/setup.cfg
+drwxr-xr-x   0 janne      (501) staff       (20)        0 2024-05-22 22:33:52.671571 datamate-0.2.2/tests/
+-rwxr-xr-x   0 janne      (501) staff       (20)    36178 2024-05-22 16:48:49.000000 datamate-0.2.2/tests/test_directory.py
+-rwx------   0 janne      (501) staff       (20)     3734 2023-05-03 21:20:00.000000 datamate-0.2.2/tests/test_namespaces.py
+-rw-r--r--   0 janne      (501) staff       (20)      867 2024-05-22 16:48:49.000000 datamate-0.2.2/tests/test_swmr.py
```

### Comparing `datamate-0.2.1/.github/workflows/auto_test.yml` & `datamate-0.2.2/.github/workflows/auto_test.yml`

 * *Files identical despite different names*

### Comparing `datamate-0.2.1/PKG-INFO` & `datamate-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 Metadata-Version: 2.1
 Name: datamate
-Version: 0.2.1
+Version: 0.2.2
 Summary: A data organization and compilation system.
 Author: Janne K. Lappalainen, Mason McGill
 License: MIT License
         
         Copyright (c) 2022 Janne Lappalainen
         Copyright (c) 2018 Mason McGill
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
 Description-Content-Type: text/markdown
-Requires-Dist: pandas
-Requires-Dist: toolz
 Requires-Dist: numpy
+Requires-Dist: pandas
 Requires-Dist: typing_extensions
 Requires-Dist: h5py>=3.6.0
-Requires-Dist: ipython<8.5
-Requires-Dist: notebook
-Requires-Dist: ipywidgets
-Requires-Dist: tqdm
-Requires-Dist: matplotlib
 Requires-Dist: ruamel.yaml
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: jupyter; extra == "dev"
 Requires-Dist: setuptools_scm; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
+Provides-Extra: notebook
+Requires-Dist: ipython; extra == "notebook"
+Requires-Dist: notebook; extra == "notebook"
+Requires-Dist: ipywidgets; extra == "notebook"
+Requires-Dist: tqdm; extra == "notebook"
+Requires-Dist: matplotlib; extra == "notebook"
+Requires-Dist: toolz; extra == "notebook"
 
 # Datamate
 
 Datamate is a lightweight data and configuration management framework for structuring data in machine learning projects on a hierarchical filesystem.
 
 Datamate provides a simple framework to work with heterogenous data by automating
 input and output of arrays and configurations to disk.
```

### Comparing `datamate-0.2.1/README.md` & `datamate-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `datamate-0.2.1/datamate/directory.py` & `datamate-0.2.2/datamate/directory.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 Instances of the base Directory class have methods to simplify reading/writing
 collections of arrays.
 
 This module also exports `ArrayFile` a descriptor protocol intended to be used
 as attribute type annotations within `Directory` subclass definition.
 """
+
 import os
 import warnings
 import itertools
 from pathlib import Path
 import shutil
 import functools
 import threading
@@ -49,15 +50,16 @@
     Namespace,
     namespacify,
     is_disjoint,
     is_superset,
     to_dict,
 )
 
-__all__ = ["Directory", "ArrayFile"]
+__all__ = ["Directory", "DirectoryDiff", "ArrayFile"]
+__all__ = ["Directory", "DirectoryDiff", "ArrayFile"]
 
 # -- Custom Errors and Warnings ------------------------------------------------
 
 
 class ConfigWarning(Warning):
     pass
 
@@ -82,30 +84,29 @@
 
 
 class ArrayFile(Protocol):
     """
     A property that corresponds to a single-array HDF5 file
     """
 
-    def __get__(self, obj: object, type_: Optional[type]) -> h5.Dataset:
-        ...
+    def __get__(self, obj: object, type_: Optional[type]) -> h5.Dataset: ...
 
-    def __set__(self, obj: object, val: object) -> None:
-        ...
+    def __set__(self, obj: object, val: object) -> None: ...
 
 
 NoneType = type(None)
 
 
 # -- Root Directory directory management ----------------------------------------
 
 context = threading.local()
 context.enforce_config_match = True
 context.check_size_on_init = False
 context.verbosity_level = 2
+context.delete_if_exists = False
 # context.in_memory = False
 
 
 def set_root_dir(root_dir: Optional[Path]) -> None:
     """
     Set the directory in which to search for Directorys.
     """
@@ -210,14 +211,32 @@
     try:
         yield
     finally:
         set_root_dir(_root_dir)
         context.within_root_context = False
 
 
+@contextmanager
+def delete_if_exists(enable: bool = True):
+    """Delete directory if it exists within a context and revert after.
+
+    Example:
+        with delete_if_exists():
+            Directory(config)
+
+    Note, takes precendecence over all other methods to control the root
+        directory.
+    """
+    context.delete_if_exists = enable
+    try:
+        yield
+    finally:
+        context.delete_if_exists = False
+
+
 # @contextmanager
 # def in_memory():
 #     """Set in_memory mode within a context and revert after to debug a Directory.
 #     """
 #     _in_memory = getattr(context, "in_memory", False)
 #     context.in_memory = True
 #     try:
@@ -388,14 +407,31 @@
         pass
 
     path: Path
     config: Config
 
     def __new__(_type, *args: object, **kwargs: object) -> Any:
         path, config = _parse_directory_args(args, kwargs)
+
+        if path is not None and isinstance(path, Path) and path.exists():
+            # case 1: path exists and global context is deleting if exists
+            if context.delete_if_exists:
+                shutil.rmtree(path)
+            # case 2: path exists and local kwargs are deleting if exists
+            if (
+                config is not None
+                and "delete_if_exists" in config
+                and config["delete_if_exists"]
+            ):
+                shutil.rmtree(path)
+
+            if config is not None and "delete_if_exists" in config:
+                # always remove the deletion flag from the config
+                config.pop("delete_if_exists")
+
         cls = _directory(_type)
         _check_implementation(cls)
 
         defaults = get_defaults(cls)
 
         if config is None and defaults:  # and _implements_init(cls):
             # to initialize from defaults if no config or path is provided
@@ -540,16 +576,18 @@
 
         try:
             # to catch cases where key is an index to a reference to an h5 file.
             # this will yield a TypeError because Path / slice does not work.
             path = self.path / key
         except TypeError as e:
             if not self.path.exists():
+                # we wanted to index an H5Dataset but we tried to index a Directory
+                # because the H5Dataset does not exist
                 raise (
-                    AssertionError(
+                    FileNotFoundError(
                         f"Indexing {self.path.name} at {key} not possible for"
                         f" Directory at {self.path.parent}. File "
                         f"{self.path.name}.h5 does not exist."
                     )
                 )
             raise e
 
@@ -595,15 +633,15 @@
             elif os.path.isdir(val):
                 _copy_dir(path, val)
 
         # Write a subDirectory.
         elif isinstance(val, (Mapping, Directory)):
             assert path.suffix == ""
             MutableMapping.update(Directory(path), val)  # type: ignore
-        
+
         # Write a dataframe.
         elif isinstance(val, DataFrame):
             assert path.suffix == ""
             val.to_csv(path.with_suffix(".csv"), index=False)
 
         # Write an array.
         else:
@@ -639,27 +677,58 @@
         #     object.__delitem__(self, key)
         #     return
         path = self.path / key
 
         # Delete an array file.
         if path.with_suffix(".h5").is_file():
             path.with_suffix(".h5").unlink()
-            
+
         # Delete a csv file.
         if path.with_suffix(".csv").is_file():
             path.with_suffix(".csv").unlink()
 
         # Delete a non-array file.
         elif path.is_file():
             path.unlink()
 
         # Delete a Directory.
         else:
             shutil.rmtree(path, ignore_errors=True)
 
+    def __eq__(self, other: object) -> bool:
+        """
+        Returns True if `self` and `other` are equal, False otherwise.
+
+        Two Directorys are equal if they have the same keys and the same
+        values for each key.
+        """
+        if not isinstance(other, Directory):
+            raise ValueError(f"Cannot compare Directory to {type(other)}")
+
+        if self.path == other.path:
+            return True
+
+        if self.path != other.path:
+            diff = DirectoryDiff(self, other)
+            return diff.equal(fail=False)
+
+    def __neq__(self, other: object) -> bool:
+        return not self.__eq__(other)
+
+    def diff(self, other: object) -> Dict[str, List[str]]:
+        """
+        Returns a dictionary of differences between `self` and `other`.
+
+        The dictionary has two keys, the name of `self` and the name of `other`.
+        The values are lists of strings, each string representing a difference
+        between the corresponding entries in `self` and `other`.
+        """
+        diff = DirectoryDiff(self, other)
+        return diff.diff()
+
     def extend(self, key: str, val: object) -> None:
         """
         Extends an `ArrayFile`, `Path`, or `Directory` at `self.path/key`
 
         Extending `ArrayFile`s performs concatenation along the first axis,
         extending `Path`s performs byte-level concatenation, and
         extending subDirectorys extends their fields.
@@ -678,15 +747,15 @@
             _extend_file(path, val)
 
         # Append a subDirectory.
         elif isinstance(val, (Mapping, Directory)):
             assert path.suffix == ""
             for k in val:
                 Directory(path).extend(k, val[k])
-        
+
         elif isinstance(val, pd.DataFrame):
             assert path.suffix == ""
             if path.with_suffix(".csv").is_file():
                 old_df = pd.read_csv(path.with_suffix(".csv"))
                 new_df = pd.concat([old_df, val], axis=0)
             else:
                 new_df = val
@@ -753,15 +822,15 @@
                 limit_to_directories=limit_to_directories,
             )
         )
 
     # -- Attribute-style element access --------------------
 
     def __getattr__(self, key: str) -> Any:
-        if key.startswith("__") and key.endswith("__"): # exclude dunder attributes
+        if key.startswith("__") and key.endswith("__"):  # exclude dunder attributes
             return None
         return self.__getitem__(key.replace("__", "."))
 
     def __setattr__(self, key: str, value: object) -> None:
         # Fix autoreload related effect.
         if key.startswith("__") and key.endswith("__"):
             object.__setattr__(self, key, value)
@@ -834,15 +903,17 @@
                 )
         write_meta(path=meta_path, config=self.config, status=status)
 
     def _modified_past_init(self, is_modified):
         meta_path = self.path / "_meta.yaml"
 
         if is_modified:
-            write_meta(path=meta_path, config=self.config, status=self.status, modified=True)
+            write_meta(
+                path=meta_path, config=self.config, status=self.status, modified=True
+            )
 
     def check_size(self, warning_at=20 * 1024**3, print_size=False) -> None:
         """Prints the size of the directory in bytes."""
         return check_size(self.path, warning_at, print_size)
 
     def to_df(self, dtypes: dict = None) -> DataFrame:
         """
@@ -895,14 +966,189 @@
         Delete files ending with suffix in the current directory path
         """
         for file in self.path.iterdir():
             if file.is_file() and file.suffix == suffix:
                 file.unlink()
 
 
+# -- Directory comparison ------------------------------------------------------
+
+
+class DirectoryDiff:
+    """Compare two directories for equality or differences."""
+
+    def __init__(
+        self,
+        directory1: Directory,
+        directory2: Directory,
+        name1: str = None,
+        name2: str = None,
+    ):
+        self.directory1 = directory1
+        self.directory2 = directory2
+        self.name1 = name1 or self.directory1.path.name
+        self.name2 = name2 or self.directory2.path.name
+
+    def equal(self, fail: bool = False) -> bool:
+        """Return True if the directories are equal, False otherwise.
+
+        If fail is True, raise the AssertionError if the directories are not equal."""
+        try:
+            assert_equal_directories(self.directory1, self.directory2)
+            return True
+        except AssertionError as e:
+            if fail:
+                raise AssertionError from e
+            return False
+
+    def diff(self, invert: bool = False) -> Dict[str, List[str]]:
+        """Return a dictionary of differences between the directories."""
+        if invert:
+            return self._diff_directories(self.directory2, self.directory1)
+        return self._diff_directories(self.directory1, self.directory2)
+
+    def config_diff(self) -> Dict[str, List[str]]:
+        """Return the differences between the configurations of the directories."""
+        return self.directory1.config.diff(
+            self.directory2.config, name1=self.name1, name2=self.name2
+        )
+
+    def _diff_directories(
+        self, dir1: Directory, dir2: Directory, parent=""
+    ) -> Dict[str, List[str]]:
+        diffs = {self.name1: [], self.name2: []}
+
+        keys1 = set(dir1.keys())
+        keys2 = set(dir2.keys())
+
+        # Check for keys only in dir1
+        for key in keys1 - keys2:
+            val = dir1[key]
+            if isinstance(val, H5Reader):
+                val = val[()]
+            diffs[self.name1].append(self._format_diff("+", key, val, parent))
+            diffs[self.name2].append(self._format_diff("-", key, val, parent))
+
+        # Check for keys only in dir2
+        for key in keys2 - keys1:
+            val = dir2[key]
+            if isinstance(val, H5Reader):
+                val = val[()]
+            diffs[self.name2].append(self._format_diff("+", key, val, parent))
+            diffs[self.name1].append(self._format_diff("-", key, val, parent))
+
+        # Check for keys present in both
+        for key in keys1 & keys2:
+            val1 = dir1[key]
+            val2 = dir2[key]
+            if isinstance(val1, Directory) and isinstance(val2, Directory):
+                child_diffs = self._diff_directories(
+                    val1, val2, f"{parent}.{key}" if parent else key
+                )
+                diffs[self.name1].extend(child_diffs[self.name1])
+                diffs[self.name2].extend(child_diffs[self.name2])
+
+            elif isinstance(val1, H5Reader) and isinstance(val2, H5Reader):
+                val1 = val1[()]
+                val2 = val2[()]
+                equal = np.array_equal(val1, val2)
+                equal = equal & (type(val1) == type(val2))
+                equal = equal & (val1.dtype == val2.dtype)
+                if not equal:
+                    diffs[self.name1].append(self._format_diff("≠", key, val1, parent))
+                    diffs[self.name2].append(self._format_diff("≠", key, val2, parent))
+
+            elif isinstance(val1, pd.DataFrame) and isinstance(val2, pd.DataFrame):
+                equal = val1.equals(val2)
+                if not equal:
+                    diffs[self.name1].append(self._format_diff("≠", key, val1, parent))
+                    diffs[self.name2].append(self._format_diff("≠", key, val2, parent))
+
+            elif val1 != val2:
+                diffs[self.name1].append(self._format_diff("≠", key, val1, parent))
+                diffs[self.name2].append(self._format_diff("≠", key, val2, parent))
+
+        return diffs
+
+    def _format_diff(self, symbol, key, value, parent):
+        full_key = f"{parent}.{key}" if parent else key
+        return f"{symbol}{full_key}: {value}"
+
+
+def assert_equal_attributes(directory: Directory, target: Directory) -> None:
+    """Assert that two directories have equal attributes."""
+    if directory.path == target.path:
+        return
+    assert type(directory) == type(target)
+    assert directory._config == target._config
+    assert directory.meta == target.meta
+    assert directory.__doc__ == target.__doc__
+    assert directory.path.exists() == target.path.exists()
+
+
+def assert_equal_directories(directory: Directory, target: Directory) -> None:
+    """Assert that two directories are equal."""
+    assert_equal_attributes(directory, target)
+
+    assert len(directory) == len(target)
+    assert len(list(directory)) == len(list(target))
+
+    keys1 = set(directory.keys())
+    keys2 = set(target.keys())
+    assert keys1 == keys2
+
+    for k in keys1 & keys2:
+        assert k in directory and k in target
+        assert k in list(directory) and k in list(target)
+        assert hasattr(directory, k) and hasattr(target, k)
+
+        v1 = directory[k]
+        v2 = target[k]
+
+        if isinstance(v1, Directory):
+            assert isinstance(v2, Directory)
+            assert isinstance(getattr(directory, k), Directory) and isinstance(
+                getattr(target, k), Directory
+            )
+            assert_equal_directories(v1, v2)
+            assert_equal_directories(getattr(directory, k), v1)
+            assert_equal_directories(getattr(target, k), v2)
+
+        elif isinstance(v1, Path):
+            assert isinstance(v2, Path)
+            assert isinstance(getattr(directory, k), Path) and isinstance(
+                getattr(target, k), Path
+            )
+            assert v1.read_bytes() == v2.read_bytes()
+            assert getattr(directory, k).read_bytes() == v1.read_bytes()
+            assert getattr(target, k).read_bytes() == v2.read_bytes()
+
+        elif isinstance(v1, pd.DataFrame):
+            assert isinstance(v2, pd.DataFrame)
+            assert isinstance(getattr(directory, k), pd.DataFrame) and isinstance(
+                getattr(target, k), pd.DataFrame
+            )
+            assert v1.equals(v2)
+            assert getattr(directory, k).equals(v1)
+            assert getattr(target, k).equals(v2)
+
+        else:
+            assert isinstance(v1, H5Reader)
+            assert isinstance(v2, H5Reader)
+            assert isinstance(getattr(directory, k), H5Reader) and isinstance(
+                getattr(target, k), H5Reader
+            )
+            assert np.array_equal(v1[()], v2[()])
+            assert np.array_equal(getattr(directory, k)[()], v1[()])
+            assert np.array_equal(getattr(target, k)[()], v2[()])
+            assert v1.dtype == v2.dtype
+            assert getattr(directory, k).dtype == v1.dtype
+            assert getattr(target, k).dtype == v2.dtype
+
+
 # -- Directory construction -----------------------------------------------------
 
 
 def merge(dict1, dict2):
     merged = {}
     if is_disjoint(dict1, dict2):
         merged.update(dict1)
@@ -972,14 +1218,18 @@
     if len(args) == 0 and len(kwargs) == 0:
         return None, None
 
     # (conf)
     elif len(args) == 1 and isinstance(args[0], Mapping) and len(kwargs) == 0:
         return None, dict(args[0])
 
+    # (config=conf)
+    elif len(args) == 0 and len(kwargs) == 1 and "config" in kwargs:
+        return None, kwargs["config"]
+
     # (**conf)
     elif len(args) == 0 and len(kwargs) > 0:
         return None, kwargs
 
     # (path)
     elif len(args) == 1 and isinstance(args[0], Path) and len(kwargs) == 0:
         return Path(args[0]), None
@@ -1008,18 +1258,39 @@
         and len(kwargs) == 0
     ):
         if args[0][0] in [".", "..", "~", "@"]:
             return Path(args[0]), dict(args[1])
         root_dir = get_root_dir()
         return root_dir / args[0], dict(args[1])
 
+    # (path, config=conf)
+    elif (
+        len(args) == 1
+        and isinstance(args[0], Path)
+        and len(kwargs) == 1
+        and "config" in kwargs
+    ):
+        return Path(args[0]), kwargs["config"]
+
     # (path, **conf)
     elif len(args) == 1 and isinstance(args[0], Path) and len(kwargs) > 0:
         return Path(args[0]), kwargs
 
+    # (str, config=conf)
+    elif (
+        len(args) == 1
+        and isinstance(args[0], str)
+        and len(kwargs) == 1
+        and "config" in kwargs
+    ):
+        if args[0][0] in [".", "..", "~", "@"]:
+            return Path(args[0]), kwargs["config"]
+        root_dir = get_root_dir()
+        return root_dir / args[0], kwargs["config"]
+
     # (str, **conf)
     elif len(args) == 1 and isinstance(args[0], str) and len(kwargs) > 0:
         if args[0][0] in [".", "..", "~", "@"]:
             return Path(args[0]), kwargs
         root_dir = get_root_dir()
         return root_dir / args[0], kwargs
 
@@ -1145,32 +1416,23 @@
 
         if meta.config == config:
             if getattr(meta, "modified", False):
                 with warnings.catch_warnings():
                     warnings.simplefilter("always")
                     warnings.warn(
                         (
-                            f"The Directory {path} has been modified after being build."
-                            + f"\nBuilding a new directory {new_dir_path} to prevent that the files you would get from the object"
-                            + " mismatch the files you would expect based on your __init__ and configuration."
-                            + "\nYou can circumvent this"
-                            + " by e.g. using the explicit path as constructor (see Directory docs)."
+                            f"Skipping Directory {path}, which has been modified after "
+                            " being build."
+                            + "\nYou can use the explicit path as constructor (see "
+                            " Directory docs)."
                         ),
                         ModifiedWarning,
                         stacklevel=2,
                     )
-                return _new_directory()
-            # raise ModifiedError(
-            #             f"The Directory {path} has been modified after being build."
-            #             + "\nThis could mean that the files you would get from the object"
-            #             + " mismatch the files you would expect based on your configuration."
-            #             + "\nYou can circumvent this error"
-            #             + " by e.g. using the path as constructor"
-            #             + " as explained in the Directory docs."
-            #         )
+                continue
 
             while meta.status == "running":
                 sleep(0.01)
                 meta = read_meta(path)
             if meta.status == "done":
                 object.__setattr__(directory, "path", path)
                 return directory
@@ -1252,23 +1514,31 @@
         if callable(getattr(type(directory), "__init__", None)):
             n_build_args = directory.__init__.__code__.co_argcount
             # case 1: __init__(self)
             if n_build_args <= 1:
                 build_args = []
                 build_kwargs = {}
             # case 2: __init__(self, config)
-            elif n_build_args == 2:
+            elif n_build_args == 2 and any(
+                [
+                    vn in ["config", "conf"]
+                    for vn in directory.__init__.__code__.co_varnames
+                ]
+            ):
                 build_args = [directory._config]
                 build_kwargs = {}
             # case 3: __init__(self, foo=1, bar=2) to specify defaults and config
             else:
                 kwargs = namespacify(get_defaults_from_init(directory))
                 assert kwargs
                 build_args = []
                 build_kwargs = {k: directory._config[k] for k in kwargs}
+
+            # import pdb; pdb.set_trace()
+
             directory.__init__(*build_args, **build_kwargs)
 
         write_meta(path=meta_path, config=config, status="done")
     except BaseException as e:
         write_meta(path=meta_path, config=config, status="stopped")
         raise e
 
@@ -1355,14 +1625,15 @@
     return path.expanduser().resolve()
 
 
 def _new_directory_path(type_: type) -> Path:
     """
     Generate an unused path in the Directory root directory.
     """
+    # import pdb;pdb.set_trace()
     root = Path(get_root_dir())
     type_name = _identify(type_)
     for i in itertools.count():
         dst = root / f"{type_name}_{i:04x}"
         if not dst.exists():
             return dst.absolute()
     assert False  # for MyPy
@@ -1462,16 +1733,17 @@
 
 
 # -- I/O -----------------------------------------------------------------------
 
 
 class H5Reader:
     """Wrapper around h5 read operations to prevent persistent file handles
-    by ensuring file handles are open only during each access operation. 
+    by ensuring file handles are open only during each access operation.
     """
+
     def __init__(self, path, assert_swmr=True, n_retries=10):
         self.path = path
         with h5.File(self.path, mode="r", libver="latest", swmr=True) as f:
             if assert_swmr:
                 assert f.swmr_mode, "File is not in SWMR mode."
             assert "data" in f
             self.shape = f["data"].shape
@@ -1504,19 +1776,21 @@
                 if retry_count == self.n_retries - 1:
                     raise e
                 sleep(0.1)
         if value is None:
             raise AttributeError(f"Attribute {key} not found.")
         # wrap callable attributes to open file before calling function
         if callable(value):
+
             def safe_wrapper(*args, **kwargs):
                 # not trying `n_retries` times here, just for simplicity
                 with h5.File(self.path, mode="r", libver="latest", swmr=True) as f:
                     output = getattr(f["data"], key)(*args, **kwargs)
                 return output
+
             return safe_wrapper
         # otherwise just return value
         else:
             return value
 
 
 def _read_h5(path: Path, assert_swmr=True) -> ArrayFile:
@@ -1618,14 +1892,15 @@
 
 
 def _copy_file(dst: Path, src: Path) -> None:
     # shutil.rmtree(dst, ignore_errors=True)
     dst.parent.mkdir(parents=True, exist_ok=True)
     shutil.copy(src, dst)
 
+
 def _copy_dir(dst: Path, src: Path) -> None:
     # shutil.rmtree(dst, ignore_errors=True)
     dst.parent.mkdir(parents=True, exist_ok=True)
     shutil.copytree(src, dst)
 
 
 def _copy_if_conflict(src):
@@ -1651,34 +1926,40 @@
             meta = yaml.load(f)
         meta = namespacify(meta)
         assert isinstance(meta, Namespace)
         if hasattr(meta, "config"):
             assert isinstance(meta.config, Namespace)
         elif hasattr(meta, "spec"):  # for backwards compatibility
             assert isinstance(meta.spec, Namespace)
-            warnings.warn(f"Directory {path} has legacy `spec` attribute instead of `meta`. Please update when possible.")
+            warnings.warn(
+                f"Directory {path} has legacy `spec` attribute instead of `meta`. Please update when possible."
+            )
             meta["config"] = meta.pop("spec")
             # resp = input("Would you like to overwrite the existing config with an updated version? (y/n): ")
             # if resp.strip().lower() == "y":
             #     write_meta(path / "_meta.yaml", **meta)
             assert isinstance(meta.status, str)
         return meta
     except:
         return Namespace(config=None, status="done")
 
 
 def write_meta(path: Path, **kwargs):
     yaml = YAML()
+
     # support dumping numpy objects
     def represent_numpy_float(self, value):
         return self.represent_float(float(value))
+
     def represent_numpy_int(self, value):
         return self.represent_int(int(value))
+
     def represent_numpy_array(self, value):
         return self.represent_sequence(value.tolist())
+
     yaml.Representer.add_multi_representer(np.ndarray, represent_numpy_array)
     yaml.Representer.add_multi_representer(np.floating, represent_numpy_float)
     yaml.Representer.add_multi_representer(np.integer, represent_numpy_int)
     # dump config to yaml
     with open(path, "w") as f:
         yaml.dump(_identify_elements(kwargs), f)
 
@@ -1834,8 +2115,8 @@
     if isinstance(obj, type):
         return _identify(obj)
     elif isinstance(obj, list):
         return [_identify_elements(elem) for elem in obj]
     elif isinstance(obj, dict):
         return {k: _identify_elements(obj[k]) for k in obj}
     else:
-        return obj
+        return obj
```

### Comparing `datamate-0.2.1/datamate/namespaces.py` & `datamate-0.2.2/datamate/namespaces.py`

 * *Files identical despite different names*

### Comparing `datamate-0.2.1/datamate.egg-info/PKG-INFO` & `datamate-0.2.2/datamate.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 Metadata-Version: 2.1
 Name: datamate
-Version: 0.2.1
+Version: 0.2.2
 Summary: A data organization and compilation system.
 Author: Janne K. Lappalainen, Mason McGill
 License: MIT License
         
         Copyright (c) 2022 Janne Lappalainen
         Copyright (c) 2018 Mason McGill
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
 Description-Content-Type: text/markdown
-Requires-Dist: pandas
-Requires-Dist: toolz
 Requires-Dist: numpy
+Requires-Dist: pandas
 Requires-Dist: typing_extensions
 Requires-Dist: h5py>=3.6.0
-Requires-Dist: ipython<8.5
-Requires-Dist: notebook
-Requires-Dist: ipywidgets
-Requires-Dist: tqdm
-Requires-Dist: matplotlib
 Requires-Dist: ruamel.yaml
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: jupyter; extra == "dev"
 Requires-Dist: setuptools_scm; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
+Provides-Extra: notebook
+Requires-Dist: ipython; extra == "notebook"
+Requires-Dist: notebook; extra == "notebook"
+Requires-Dist: ipywidgets; extra == "notebook"
+Requires-Dist: tqdm; extra == "notebook"
+Requires-Dist: matplotlib; extra == "notebook"
+Requires-Dist: toolz; extra == "notebook"
 
 # Datamate
 
 Datamate is a lightweight data and configuration management framework for structuring data in machine learning projects on a hierarchical filesystem.
 
 Datamate provides a simple framework to work with heterogenous data by automating
 input and output of arrays and configurations to disk.
```

### Comparing `datamate-0.2.1/examples/01. Introduction to Datamate.ipynb` & `datamate-0.2.2/examples/01. Introduction to Datamate.ipynb`

 * *Files identical despite different names*

### Comparing `datamate-0.2.1/examples/another thread.ipynb` & `datamate-0.2.2/examples/another thread.ipynb`

 * *Files identical despite different names*

### Comparing `datamate-0.2.1/license` & `datamate-0.2.2/license`

 * *Files identical despite different names*

### Comparing `datamate-0.2.1/pyproject.toml` & `datamate-0.2.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -12,35 +12,38 @@
 authors = [
     {name = "Janne K. Lappalainen"},
     {name = "Mason McGill"}
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
 dependencies = [
-    "pandas",
-    "toolz",
     "numpy",
+    "pandas",
     "typing_extensions",
     "h5py>=3.6.0",
-    "ipython<8.5",
-    "notebook",
-    "ipywidgets",
-    "tqdm",
-    "matplotlib",
     "ruamel.yaml"
 ]
 
+
 [project.optional-dependencies]
 dev = [
     "black",
     "pre-commit",
     "jupyter",
     "setuptools_scm",
     "pytest"
 ]
+notebook = [
+    "ipython",
+    "notebook",
+    "ipywidgets",
+    "tqdm",
+    "matplotlib",
+    "toolz"
+]
 
 [tool.setuptools.packages.find]
 include=["datamate"]
 
 [tool.black]
 line-length = 88
```

### Comparing `datamate-0.2.1/tests/test_directory.py` & `datamate-0.2.2/tests/test_directory.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,18 @@
     ModifiedError,
     ModifiedWarning,
     ConfigWarning,
     ImplementationWarning,
     ImplementationError,
     _auto_doc,
     H5Reader,
+    DirectoryDiff,
 )
+from datamate import directory
+from datamate.namespaces import namespacify
 
 # -- Helper functions ----------------------------------------------------------
 
 
 def data_file(path: Path) -> Path:
     path.parent.mkdir(parents=True, exist_ok=True)
     path.write_bytes(np.random.rand(3).tobytes())
@@ -78,15 +81,15 @@
             k_mod = k.replace(".", "__")
             assert (directory.path / k).is_file()
             assert isinstance(directory[k], Path)
             assert isinstance(getattr(directory, k), Path)
             assert directory[k].read_bytes() == v.read_bytes()
             assert getattr(directory, k).read_bytes() == v.read_bytes()
             assert getattr(directory, k_mod).read_bytes() == v.read_bytes()
-        
+
         elif isinstance(v, pd.DataFrame):
             assert (directory.path / k).with_suffix(".csv").is_file()
             assert isinstance(directory[k], pd.DataFrame)
             assert isinstance(getattr(directory, k), pd.DataFrame)
             assert np.array_equal(directory[k].to_numpy(), v.to_numpy())
             assert np.array_equal(getattr(directory, k).to_numpy(), v.to_numpy())
 
@@ -247,15 +250,15 @@
     a.extend("b", np.uint16([[11, 12]]))
     assert_directory_equals(a, {"b": np.uint16([[7, 8], [9, 10], [11, 12]])})
 
     b = Directory(tmp_path)
     b.b = np.uint16([[7, 8], [9, 10]])
     b.extend("b", np.uint16([[11, 12]]))
     assert_directory_equals(b, {"b": np.uint16([[7, 8], [9, 10], [11, 12]])})
-    
+
 
 def test_dataframe_extension(tmp_path: Path) -> None:
     a = Directory(tmp_path)
     a.extend("b", pd.DataFrame({"a": [7, 9], "b": [8, 10]}))
     a.extend("b", pd.DataFrame({"a": [11], "b": [12]}))
     assert_directory_equals(a, {"b": pd.DataFrame({"a": [7, 9, 11], "b": [8, 10, 12]})})
 
@@ -1095,14 +1098,20 @@
         sigma: float = 0.1
 
     def __init__(self, tau=200):
         pass
 
 
 def test_cross_configs(tmp_path):
+    """Test that default config and init kwargs are merged.
+
+    Raises error if default config and init kwargs are not compatible.
+    """
+    set_root_dir(tmp_path)
+
     dir = ConIni1()
     assert_directory_equals(
         dir,
         dict(
             __conf__=Namespace(type="ConIni1", tau=200.0, sigma=0.1),
             __exists__=False,
         ),
@@ -1113,7 +1122,156 @@
         class ConIni2(Directory):
             class Config:
                 tau: float = 200.0
                 sigma: float = 0.1
 
             def __init__(self, sigma=2):
                 pass
+
+
+# --- test delete_if_exists context manager
+
+
+def test_delete_if_exists(tmp_path):
+    set_root_dir(tmp_path)
+
+    name = "test"
+    dir = DefaultConfigDir(name, x=2)
+    assert_directory_equals(
+        dir,
+        dict(
+            __type__=DefaultConfigDir,
+            __path__=tmp_path / name,
+            __conf__=Namespace(type="DefaultConfigDir", x=2),
+            __meta__={"config": {"type": "DefaultConfigDir", "x": 2}, "status": "done"},
+            x=np.arange(2),
+        ),
+    )
+
+    with pytest.raises(FileExistsError):
+        dir2 = DefaultConfigDir(name, config=dict(x=3))
+
+    with directory.delete_if_exists():
+        dir2 = DefaultConfigDir(name, config=dict(x=3))
+        assert_directory_equals(
+            dir2,
+            dict(
+                __type__=DefaultConfigDir,
+                __path__=tmp_path / name,
+                __conf__=Namespace(type="DefaultConfigDir", x=3),
+                __meta__={
+                    "config": {"type": "DefaultConfigDir", "x": 3},
+                    "status": "done",
+                },
+                x=np.arange(3),
+            ),
+        )
+
+    with pytest.raises(FileExistsError):
+        dir = DefaultConfigDir(name, x=2)
+
+    dir = DefaultConfigDir(name, x=2, delete_if_exists=True)
+    assert_directory_equals(
+        dir,
+        dict(
+            __type__=DefaultConfigDir,
+            __path__=tmp_path / name,
+            __conf__=Namespace(type="DefaultConfigDir", x=2),
+            __meta__={"config": {"type": "DefaultConfigDir", "x": 2}, "status": "done"},
+            x=np.arange(2),
+        ),
+    )
+
+    dir = DefaultConfigDir(name, x=2, delete_if_exists=False)
+    assert_directory_equals(
+        dir,
+        dict(
+            __type__=DefaultConfigDir,
+            __path__=tmp_path / name,
+            __conf__=Namespace(type="DefaultConfigDir", x=2),
+            __meta__={"config": {"type": "DefaultConfigDir", "x": 2}, "status": "done"},
+            x=np.arange(2),
+        ),
+    )
+
+
+# --- test directory comparison
+
+
+class CompDir(Directory):
+    class Config:
+        x: int = 2
+
+    def __init__(self, x: int = 2):
+        self.x = x
+
+
+def test_comparison(tmp_path):
+    set_root_dir(tmp_path)
+
+    a = CompDir()
+    b = CompDir()
+    directory.assert_equal_directories(a, b)
+    assert a.path == b.path
+
+    a = CompDir("a")
+    b = CompDir("b")
+    directory.assert_equal_directories(a, b)
+    assert a.path != b.path
+
+    b = CompDir(x=3)
+    with pytest.raises(AssertionError):
+        directory.assert_equal_directories(a, b)
+
+    b.x = 2
+    with pytest.raises(AssertionError):
+        directory.assert_equal_attributes(a, b)
+
+
+def test_diff(tmp_path):
+    set_root_dir(tmp_path)
+
+    a = CompDir()
+    b = CompDir(x=3)
+    diff = DirectoryDiff(a, b)
+    assert not diff.equal()
+    assert a != b
+
+    a = CompDir("a")
+    b = CompDir("b")
+    np.savez(b.y.path, np.ones(10))
+    diff = DirectoryDiff(a, b)
+    assert not diff.equal()
+    assert a != b
+
+    a = CompDir("aa")
+    b = CompDir("bb")
+    np.savez(a.y.path, np.ones(10))
+    np.savez(b.y.path, np.ones(10))
+    diff = DirectoryDiff(a, b)
+    assert diff.equal()
+    assert a == b
+
+    df = pd.DataFrame(np.random.rand(10, 2), columns=["a", "b"])
+    a = CompDir("aaa")
+    b = CompDir("bbb")
+    a.df = df
+    b.df = df
+    diff = DirectoryDiff(a, b)
+    assert diff.equal()
+    assert a == b
+
+    df1 = pd.DataFrame(np.random.rand(10, 2), columns=["a", "b"])
+    df2 = pd.DataFrame(np.random.rand(10, 2), columns=["a", "b"])
+    a = CompDir("aaaa")
+    b = CompDir("bbbb")
+    a.df = df1
+    b.df = df2
+    diff = DirectoryDiff(a, b)
+    assert not diff.equal()
+    assert a != b
+
+    a = Directory("aaaaa")
+    a.x = 3
+    b = Directory("bbbbb")
+    b.x = 2
+    assert a.diff(b) == {"aaaaa": ["≠x: 3"], "bbbbb": ["≠x: 2"]}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `datamate-0.2.1/tests/test_namespaces.py` & `datamate-0.2.2/tests/test_namespaces.py`

 * *Files identical despite different names*

### Comparing `datamate-0.2.1/tests/test_swmr.py` & `datamate-0.2.2/tests/test_swmr.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 def test_swmr_single_thread(tmp_path):
     directory = Directory(tmp_path / "swmr_single")
 
     value = np.random.rand(5)
     directory.x = value
     time.sleep(0.1)
 
-    for _ in range(10000):
+    for _ in range(1000):
         operation = random.choice(["read", "read", "write", "extend"])
         if operation == "read":
             reader = directory.x
             read_value = reader[:]
         elif operation == "write":
             write_value = np.random.rand(5)
             directory.x = write_value
             value = write_value
         else:
             extend_value = [np.random.rand()]
-            directory.extend('x', extend_value)
+            directory.extend("x", extend_value)
             value = np.concatenate([value, np.array(extend_value)])
```

