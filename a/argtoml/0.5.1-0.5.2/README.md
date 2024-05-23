# Comparing `tmp/argtoml-0.5.1.tar.gz` & `tmp/argtoml-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argtoml-0.5.1.tar", last modified: Sun May  5 16:25:20 2024, max compression
+gzip compressed data, was "argtoml-0.5.2.tar", last modified: Thu May 23 12:24:41 2024, max compression
```

## Comparing `argtoml-0.5.1.tar` & `argtoml-0.5.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jo3       (1000) jo3       (1000)        0 2024-05-05 16:25:20.986922 argtoml-0.5.1/
--rw-r--r--   0 jo3       (1000) jo3       (1000)     1069 2023-07-23 14:09:52.000000 argtoml-0.5.1/LICENSE
--rw-r--r--   0 jo3       (1000) jo3       (1000)     3731 2024-05-05 16:25:20.986922 argtoml-0.5.1/PKG-INFO
--rw-r--r--   0 jo3       (1000) jo3       (1000)     3218 2024-01-02 10:21:38.000000 argtoml-0.5.1/README.md
-drwxr-xr-x   0 jo3       (1000) jo3       (1000)        0 2024-05-05 16:25:20.986922 argtoml-0.5.1/argtoml/
--rw-r--r--   0 jo3       (1000) jo3       (1000)       57 2024-02-13 08:37:22.000000 argtoml-0.5.1/argtoml/__init__.py
--rw-r--r--   0 jo3       (1000) jo3       (1000)     2802 2024-02-18 11:11:25.000000 argtoml-0.5.1/argtoml/__main__.py
--rw-r--r--   0 jo3       (1000) jo3       (1000)     3076 2024-02-13 08:37:22.000000 argtoml-0.5.1/argtoml/locate.py
--rw-r--r--   0 jo3       (1000) jo3       (1000)    10953 2024-02-13 08:37:22.000000 argtoml-0.5.1/argtoml/main.py
--rw-r--r--   0 jo3       (1000) jo3       (1000)     4948 2024-05-05 15:53:40.000000 argtoml-0.5.1/argtoml/opt.py
-drwxr-xr-x   0 jo3       (1000) jo3       (1000)        0 2024-05-05 16:25:20.986922 argtoml-0.5.1/argtoml.egg-info/
--rw-r--r--   0 jo3       (1000) jo3       (1000)     3731 2024-05-05 16:25:20.000000 argtoml-0.5.1/argtoml.egg-info/PKG-INFO
--rw-r--r--   0 jo3       (1000) jo3       (1000)      273 2024-05-05 16:25:20.000000 argtoml-0.5.1/argtoml.egg-info/SOURCES.txt
--rw-r--r--   0 jo3       (1000) jo3       (1000)        1 2024-05-05 16:25:20.000000 argtoml-0.5.1/argtoml.egg-info/dependency_links.txt
--rw-r--r--   0 jo3       (1000) jo3       (1000)        8 2024-05-05 16:25:20.000000 argtoml-0.5.1/argtoml.egg-info/top_level.txt
--rw-r--r--   0 jo3       (1000) jo3       (1000)      951 2024-05-05 16:23:36.000000 argtoml-0.5.1/pyproject.toml
--rw-r--r--   0 jo3       (1000) jo3       (1000)       38 2024-05-05 16:25:20.986922 argtoml-0.5.1/setup.cfg
--rw-r--r--   0 jo3       (1000) jo3       (1000)       61 2023-07-23 14:09:52.000000 argtoml-0.5.1/setup.py
-drwxr-xr-x   0 jo3       (1000) jo3       (1000)        0 2024-05-05 16:25:20.986922 argtoml-0.5.1/tests/
--rw-r--r--   0 jo3       (1000) jo3       (1000)      218 2023-07-23 14:09:52.000000 argtoml-0.5.1/tests/test_main.py
+drwxr-xr-x   0 jo3       (1000) jo3       (1000)        0 2024-05-23 12:24:41.750219 argtoml-0.5.2/
+-rw-r--r--   0 jo3       (1000) jo3       (1000)     1069 2023-07-23 14:09:52.000000 argtoml-0.5.2/LICENSE
+-rw-r--r--   0 jo3       (1000) jo3       (1000)     3731 2024-05-23 12:24:41.750219 argtoml-0.5.2/PKG-INFO
+-rw-r--r--   0 jo3       (1000) jo3       (1000)     3218 2024-01-02 10:21:38.000000 argtoml-0.5.2/README.md
+drwxr-xr-x   0 jo3       (1000) jo3       (1000)        0 2024-05-23 12:24:41.746886 argtoml-0.5.2/argtoml/
+-rw-r--r--   0 jo3       (1000) jo3       (1000)       57 2024-02-13 08:37:22.000000 argtoml-0.5.2/argtoml/__init__.py
+-rw-r--r--   0 jo3       (1000) jo3       (1000)     3240 2024-05-07 09:23:38.000000 argtoml-0.5.2/argtoml/__main__.py
+-rw-r--r--   0 jo3       (1000) jo3       (1000)     3121 2024-05-07 11:35:09.000000 argtoml-0.5.2/argtoml/locate.py
+-rw-r--r--   0 jo3       (1000) jo3       (1000)    10953 2024-02-13 08:37:22.000000 argtoml-0.5.2/argtoml/main.py
+-rw-r--r--   0 jo3       (1000) jo3       (1000)     5073 2024-05-23 12:22:48.000000 argtoml-0.5.2/argtoml/opt.py
+drwxr-xr-x   0 jo3       (1000) jo3       (1000)        0 2024-05-23 12:24:41.750219 argtoml-0.5.2/argtoml.egg-info/
+-rw-r--r--   0 jo3       (1000) jo3       (1000)     3731 2024-05-23 12:24:41.000000 argtoml-0.5.2/argtoml.egg-info/PKG-INFO
+-rw-r--r--   0 jo3       (1000) jo3       (1000)      273 2024-05-23 12:24:41.000000 argtoml-0.5.2/argtoml.egg-info/SOURCES.txt
+-rw-r--r--   0 jo3       (1000) jo3       (1000)        1 2024-05-23 12:24:41.000000 argtoml-0.5.2/argtoml.egg-info/dependency_links.txt
+-rw-r--r--   0 jo3       (1000) jo3       (1000)        8 2024-05-23 12:24:41.000000 argtoml-0.5.2/argtoml.egg-info/top_level.txt
+-rw-r--r--   0 jo3       (1000) jo3       (1000)      951 2024-05-23 12:23:14.000000 argtoml-0.5.2/pyproject.toml
+-rw-r--r--   0 jo3       (1000) jo3       (1000)       38 2024-05-23 12:24:41.750219 argtoml-0.5.2/setup.cfg
+-rw-r--r--   0 jo3       (1000) jo3       (1000)       61 2023-07-23 14:09:52.000000 argtoml-0.5.2/setup.py
+drwxr-xr-x   0 jo3       (1000) jo3       (1000)        0 2024-05-23 12:24:41.750219 argtoml-0.5.2/tests/
+-rw-r--r--   0 jo3       (1000) jo3       (1000)      218 2023-07-23 14:09:52.000000 argtoml-0.5.2/tests/test_main.py
```

### Comparing `argtoml-0.5.1/LICENSE` & `argtoml-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `argtoml-0.5.1/PKG-INFO` & `argtoml-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argtoml
-Version: 0.5.1
+Version: 0.5.2
 Summary: Add the keys from a .toml file to your CLI as arguments. Their values default to the values in the .toml file.
 Author-email: Jochem Hölscher <a.fake@e.mail>
 Project-URL: homepage, https://github.com/JJJHolscher/argtoml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `argtoml-0.5.1/README.md` & `argtoml-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `argtoml-0.5.1/argtoml/__main__.py` & `argtoml-0.5.2/argtoml/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,77 +1,91 @@
 #! /usr/bin/env python3
 # vim:fenc=utf-8
 
 from argparse import ArgumentParser
 from pathlib import Path
-import tomllib
 from typing import Optional, Union, List
 
 from .locate import TPath, locate_toml_path
-from .opt import toml_to_opt, opt_to_argument_parser, cli_arguments_to_opt
+from .opt import toml_to_opt, opt_to_argument_parser, cli_arguments_to_opt, merge_opts
+
+
+StrPath = Union[Path, str]
 
 
 def parse_args(
-    toml_path: Union[List[Path], Path] = [Path("config.toml")],
+    toml_path: Union[List[StrPath], StrPath] = [Path("config.toml")],
     parser: Optional[ArgumentParser] = None,
     description: str = "",
     toml_dir: Optional[TPath] = None,
     strings_to_paths: bool = True,
     grandparent: Optional[bool] = None,
+    overwrite: dict = {}
 ) -> dict:
-    """ THIS DOCSTRING IS OUTDATED.
+    """
     Add the content of a toml file as argument with default values
     to an ArgumentParser object.
+    You can specify additional toml files with the -c cli argument.
+    You can overwrite any values by providing an overwrite argument.
+
+    This function does not look for cli arguments in an ipython context.
 
     Args:
-        parser: ArgumentParser object that can be pre-filled.
-        description: an description if the ArgumentParser is not given.
         toml_path: a relative or absolute path to the toml file.
+        parser: ArgumentParser object that can be pre-filled.
+        description: a cli description for if the ArgumentParser is not given.
         toml_dir: the absolute path to the parent directory of the toml file.
-        base_path: the prefix to prepend to relative paths from the toml file.
-            if False: never interpret toml file string values as paths.
-            if True: use the toml_dir as prefix.
+        strings_to_paths: whether to convert path-like strings to 
+            pathlib.Path objects.
         grandparent: use grandparent directory of the file calling argtoml
             instead of parent directory. Defaults to True if argtoml is not
             called from ipython.
+        overwrite: values with the highest presedence.
     Out:
         A (nested) SimpleNamespace object filled with cli argument values that
         defaults to values from the toml file.
     """
     # Create toml paths depending on the context in which this is called.
     locations = []
     for path in toml_path if isinstance(toml_path, list) else [toml_path]:
         location = locate_toml_path(
-            path, toml_dir, grandparent
+            Path(path), toml_dir, grandparent
         )
         locations.append(location)
 
     # Merge all the toml files into a single dictionary.
-    options = {}
+    options: dict = {}
     for location in locations:
         options = toml_to_opt(location, options, strings_to_paths)
 
+    # Jupyter Lab crashes if argparse looks for command line arguments.
+    try:
+        get_ipython()  #type:ignore
+        options = merge_opts(options, overwrite, None)  #type:ignore
+        return options
+    except NameError:
+        pass
+
     # Translate that dictionary into command line arguments.
     if parser is None:
-        parser = ArgumentParser()
+        parser = ArgumentParser(description=description)
     parser.add_argument("-c", required=False, help="path to an optional extra \
                         toml file for loading configuration from.")
     parser = opt_to_argument_parser(options, parser)
+    args = parser.parse_args()
 
-    # Jupyter Lab crashes if argparse looks for command line arguments.
-    try:
-        get_ipython()
-        args = parser.parse_args(args=[])
-    except NameError:
-        args = parser.parse_args()
-
-    # Merge the user-supplied command line arguments with the toml options.
+    # Merge any cli-supplied toml file.
     if args.c:
         options = toml_to_opt(Path(args.c), options, strings_to_paths)
         args.c = None
+
+    # Merge the cli-supplied values.
     options = cli_arguments_to_opt(args, options)
 
+    # Apply any options provided during the function call.
+    options = merge_opts(options, overwrite, None)  #type:ignore
+
     return options
 
 
 if __name__ == "__main__":
     print(parse_args())
```

### Comparing `argtoml-0.5.1/argtoml/locate.py` & `argtoml-0.5.2/argtoml/locate.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     2. the directory of the main file
     3. the directory of the ipynb file
 
     Args:
         toml_path: a relative or absolute path to the toml file.
         toml_dir: an absolute path in which to look for the toml file.
         parent: whether to look for the toml file in the parent directory of
-            the directory containing the toml file.
+            the directory containing the toml file instead.
 
     Returns:
         The path to the toml file.
 
     Errors:
         NotImplementedError: The context in which this function was called does
             not lend itself for the automatic location of toml files. Supply
@@ -66,15 +66,15 @@
             return Path(toml_dir) / toml_path
 
     # Return the toml_path if it is absolute.
     elif toml_path.is_absolute():
         return Path(toml_path)
 
     # Have toml_dir be the package dir if argtoml is called from a package.
-    if __main__.__package__:
+    if hasattr(__main__, "__package__") and __main__.__package__:
         toml_dir = files(__main__.__package__)
         if parent:
             toml_dir = toml_dir.joinpath(Path(".."))
         return toml_dir.joinpath(toml_path)
 
     # Use the folder of the main file as toml_dir.
     elif "__file__" in dir(__main__):
```

### Comparing `argtoml-0.5.1/argtoml/main.py` & `argtoml-0.5.2/argtoml/main.py`

 * *Files identical despite different names*

### Comparing `argtoml-0.5.1/argtoml/opt.py` & `argtoml-0.5.2/argtoml/opt.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,26 +50,26 @@
     return string
 
 
 def merge_opts(old: Opt, add: Opt, path: Optional[Path]):
     new = copy.deepcopy(old)
 
     for k, v in iter_opt(add):
-        t = type(v)
-        if t is str and path is not None:
+        if type(v) is str and path is not None:
             v = string_to_path(v, path)
 
         if k in old:
-            assert type(old[k]) is t
+            # Check whether identical keys have values of the same type.
+            assert type(old[k]) is type(v)
             old_v = old[k]
         else:
             old_v = {}
 
         if isinstance(v, get_args(Opt)):
-            new[k] = merge_opts(old_v, v, path)
+            new[k] = merge_opts(old_v, v, path)  #type:ignore
         else:
             new[k] = v
 
     return new
 
 
 def opt_to_argument_parser(
@@ -137,15 +137,15 @@
             return opt[key]
     else:
         if key not in reference and value is not None:
             raise KeyError(f"{key} is being edited twice.")
         return travel_opt(keys[1:], opt[key], reference[key], value)
 
 
-def cli_arguments_to_opt(cli_args, opt: Opt) -> dict:
+def cli_arguments_to_opt(cli_args, opt: dict) -> dict:
     """ Merge options from arguments with existing options."""
     args = sorted(list(vars(cli_args).items()), key=lambda x: len(x[0]))
     reference = copy.deepcopy(opt)
     for k, v in args:
         if v is None:
             continue
 
@@ -161,15 +161,18 @@
                 travel_opt(k, opt, reference, value=v)
             except IndexError:
                 k[-1] = k[-1][3:]
                 travel_opt(k, opt, reference, value=v)
 
         else:
             travel_opt(k, opt, reference, value=v)
+
     return opt
 
 
-def toml_to_opt(toml_path: Path, opt: Opt, strings_to_paths: bool) -> Opt:
+def toml_to_opt(toml_path: Path, opt: Opt, strings_to_paths: bool) -> dict:
     with open(toml_path, 'rb') as toml_file:
         toml_options = tomllib.load(toml_file)
     base_path = Path(toml_path).parent if strings_to_paths else None
-    return merge_opts(opt, toml_options, base_path)
+    out = merge_opts(opt, toml_options, base_path)
+    assert type(out) is dict
+    return out
```

### Comparing `argtoml-0.5.1/argtoml.egg-info/PKG-INFO` & `argtoml-0.5.2/argtoml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argtoml
-Version: 0.5.1
+Version: 0.5.2
 Summary: Add the keys from a .toml file to your CLI as arguments. Their values default to the values in the .toml file.
 Author-email: Jochem Hölscher <a.fake@e.mail>
 Project-URL: homepage, https://github.com/JJJHolscher/argtoml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `argtoml-0.5.1/pyproject.toml` & `argtoml-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "argtoml"
-version = "0.5.1"
+version = "0.5.2"
 description = "Add the keys from a .toml file to your CLI as arguments. Their values default to the values in the .toml file."
 dynamic = ["readme"]
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

