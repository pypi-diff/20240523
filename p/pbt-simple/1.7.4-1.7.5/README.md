# Comparing `tmp/pbt_simple-1.7.4.tar.gz` & `tmp/pbt_simple-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbt_simple-1.7.4.tar", max compression
+gzip compressed data, was "pbt_simple-1.7.5.tar", max compression
```

## Comparing `pbt_simple-1.7.4.tar` & `pbt_simple-1.7.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1064 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/LICENSE
--rw-r--r--   0        0        0      178 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/README.md
--rw-r--r--   0        0        0      952 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/__init__.py
--rw-r--r--   0        0        0     1224 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/__main__.py
--rw-r--r--   0        0        0        0 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/commands/__init__.py
--rw-r--r--   0        0        0     2693 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/commands/build.py
--rw-r--r--   0        0        0     1550 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/commands/git.py
--rw-r--r--   0        0        0    16253 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/commands/install.py
--rw-r--r--   0        0        0     1209 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/commands/list.py
--rw-r--r--   0        0        0     6874 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/config.py
--rw-r--r--   0        0        0     5611 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/misc.py
--rw-r--r--   0        0        0        0 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/package/__init__.py
--rw-r--r--   0        0        0    12169 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/package/discovery.py
--rw-r--r--   0        0        0     3452 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/package/graph.py
--rw-r--r--   0        0        0     7100 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/package/package.py
--rw-r--r--   0        0        0        0 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/registry/__init__.py
--rw-r--r--   0        0        0     2834 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/registry/pypi.py
--rw-r--r--   0        0        0      434 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/registry/registry.py
--rw-r--r--   0        0        0        0 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/vcs/__init__.py
--rw-r--r--   0        0        0    10514 2024-05-11 02:15:52.649557 pbt_simple-1.7.4/sbt/vcs/git.py
--rw-r--r--   0        0        0     1365 1970-01-01 00:00:00.000000 pbt_simple-1.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-23 04:22:55.065991 pbt_simple-1.7.5/LICENSE
+-rw-r--r--   0        0        0      178 2024-05-23 04:22:55.065991 pbt_simple-1.7.5/README.md
+-rw-r--r--   0        0        0      952 2024-05-23 04:22:55.065991 pbt_simple-1.7.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-23 04:22:55.065991 pbt_simple-1.7.5/sbt/__init__.py
+-rw-r--r--   0        0        0     1224 2024-05-23 04:22:55.065991 pbt_simple-1.7.5/sbt/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-23 04:22:55.065991 pbt_simple-1.7.5/sbt/commands/__init__.py
+-rw-r--r--   0        0        0     2693 2024-05-23 04:22:55.065991 pbt_simple-1.7.5/sbt/commands/build.py
+-rw-r--r--   0        0        0     1550 2024-05-23 04:22:55.065991 pbt_simple-1.7.5/sbt/commands/git.py
+-rw-r--r--   0        0        0    16300 2024-05-23 04:22:55.065991 pbt_simple-1.7.5/sbt/commands/install.py
+-rw-r--r--   0        0        0     1209 2024-05-23 04:22:55.065991 pbt_simple-1.7.5/sbt/commands/list.py
+-rw-r--r--   0        0        0     6874 2024-05-23 04:22:55.065991 pbt_simple-1.7.5/sbt/config.py
+-rw-r--r--   0        0        0     5611 2024-05-23 04:22:55.065991 pbt_simple-1.7.5/sbt/misc.py
+-rw-r--r--   0        0        0        0 2024-05-23 04:22:55.065991 pbt_simple-1.7.5/sbt/package/__init__.py
+-rw-r--r--   0        0        0    12169 2024-05-23 04:22:55.065991 pbt_simple-1.7.5/sbt/package/discovery.py
+-rw-r--r--   0        0        0     3452 2024-05-23 04:22:55.065991 pbt_simple-1.7.5/sbt/package/graph.py
+-rw-r--r--   0        0        0     7100 2024-05-23 04:22:55.065991 pbt_simple-1.7.5/sbt/package/package.py
+-rw-r--r--   0        0        0        0 2024-05-23 04:22:55.065991 pbt_simple-1.7.5/sbt/registry/__init__.py
+-rw-r--r--   0        0        0     2834 2024-05-23 04:22:55.065991 pbt_simple-1.7.5/sbt/registry/pypi.py
+-rw-r--r--   0        0        0      434 2024-05-23 04:22:55.065991 pbt_simple-1.7.5/sbt/registry/registry.py
+-rw-r--r--   0        0        0        0 2024-05-23 04:22:55.065991 pbt_simple-1.7.5/sbt/vcs/__init__.py
+-rw-r--r--   0        0        0    10514 2024-05-23 04:22:55.065991 pbt_simple-1.7.5/sbt/vcs/git.py
+-rw-r--r--   0        0        0     1365 1970-01-01 00:00:00.000000 pbt_simple-1.7.5/PKG-INFO
```

### Comparing `pbt_simple-1.7.4/LICENSE` & `pbt_simple-1.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.4/pyproject.toml` & `pbt_simple-1.7.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pbt-simple"
-version = "1.7.4"
+version = "1.7.5"
 description = "A simpler version of [PBT](https://github.com/binh-vu/pbt) for installing a package (and its local dependencies in editable mode) and build extension modules written in PYO3."
 authors = ["Binh Vu <binh@toan2.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "sbt" }]
 homepage = "https://github.com/binh-vu/pbt-simple"
 repository = "https://github.com/binh-vu/pbt-simple"
```

### Comparing `pbt_simple-1.7.4/sbt/__main__.py` & `pbt_simple-1.7.5/sbt/__main__.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.4/sbt/commands/build.py` & `pbt_simple-1.7.5/sbt/commands/build.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.4/sbt/commands/git.py` & `pbt_simple-1.7.5/sbt/commands/git.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.4/sbt/commands/install.py` & `pbt_simple-1.7.5/sbt/commands/install.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,16 @@
         packages[deppkg.name] = deppkg
     else:
         deppkg = packages[dependency]
 
     # step 2: update the list of manually installed
     pkg_cache_dir = cfg.pkg_cache_dir(packages[package])
     manual_deps = packages[package].find_manually_installed_dependencies(pkg_cache_dir)
-    manual_deps.append(deppkg.location)
+    if deppkg.location not in manual_deps:
+        manual_deps.append(deppkg.location)
     packages[package].save_manually_installed_dependencies(
         pkg_cache_dir, sorted(set(manual_deps))
     )
 
     # step 3: gather dependencies of the package -- include the one from manually installed packages
     if no_dep_dep:
         pkg_venv_path = venv_path(
```

### Comparing `pbt_simple-1.7.4/sbt/commands/list.py` & `pbt_simple-1.7.5/sbt/commands/list.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.4/sbt/config.py` & `pbt_simple-1.7.5/sbt/config.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.4/sbt/misc.py` & `pbt_simple-1.7.5/sbt/misc.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.4/sbt/package/discovery.py` & `pbt_simple-1.7.5/sbt/package/discovery.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.4/sbt/package/graph.py` & `pbt_simple-1.7.5/sbt/package/graph.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.4/sbt/package/package.py` & `pbt_simple-1.7.5/sbt/package/package.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.4/sbt/registry/pypi.py` & `pbt_simple-1.7.5/sbt/registry/pypi.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.4/sbt/vcs/git.py` & `pbt_simple-1.7.5/sbt/vcs/git.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.4/PKG-INFO` & `pbt_simple-1.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbt-simple
-Version: 1.7.4
+Version: 1.7.5
 Summary: A simpler version of [PBT](https://github.com/binh-vu/pbt) for installing a package (and its local dependencies in editable mode) and build extension modules written in PYO3.
 Home-page: https://github.com/binh-vu/pbt-simple
 License: MIT
 Author: Binh Vu
 Author-email: binh@toan2.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

