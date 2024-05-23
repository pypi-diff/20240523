# Comparing `tmp/factorio_randovania_mod-0.1.1.tar.gz` & `tmp/factorio_randovania_mod-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "factorio_randovania_mod-0.1.1.tar", last modified: Mon May 20 22:01:34 2024, max compression
+gzip compressed data, was "factorio_randovania_mod-0.2.0.tar", last modified: Thu May 23 21:26:14 2024, max compression
```

## Comparing `factorio_randovania_mod-0.1.1.tar` & `factorio_randovania_mod-0.2.0.tar`

### file list

```diff
@@ -1,47 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:01:34.827902 factorio_randovania_mod-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:01:34.819902 factorio_randovania_mod-0.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-20 22:01:29.000000 factorio_randovania_mod-0.1.1/.github/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-20 22:01:29.000000 factorio_randovania_mod-0.1.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:01:34.819902 factorio_randovania_mod-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-20 22:01:29.000000 factorio_randovania_mod-0.1.1/.github/workflows/python.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-20 22:01:29.000000 factorio_randovania_mod-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-20 22:01:29.000000 factorio_randovania_mod-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-20 22:01:29.000000 factorio_randovania_mod-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-20 22:01:34.827902 factorio_randovania_mod-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-20 22:01:29.000000 factorio_randovania_mod-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 22:01:34.827902 factorio_randovania_mod-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:01:34.819902 factorio_randovania_mod-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:01:34.823902 factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-20 22:01:29.000000 factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-20 22:01:29.000000 factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-20 22:01:29.000000 factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-20 22:01:29.000000 factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/color_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-20 22:01:29.000000 factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/configuration.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6565 2024-05-20 22:01:29.000000 factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/creator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:01:34.823902 factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/files/
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-20 22:01:29.000000 factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/files/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:01:34.823902 factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/lua_src/
--rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-05-20 22:01:29.000000 factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/lua_src/control.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-20 22:01:29.000000 factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/lua_src/data-updates.lua
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-05-20 22:01:29.000000 factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/lua_src/data.lua
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:01:34.819902 factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/lua_src/graphics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:01:34.823902 factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/lua_src/graphics/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-20 22:01:29.000000 factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/lua_src/graphics/icons/nothing.png
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-20 22:01:29.000000 factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/lua_src/info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:01:34.819902 factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/lua_src/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:01:34.823902 factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/lua_src/locale/en/
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-20 22:01:29.000000 factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/lua_src/locale/en/strings.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:01:34.823902 factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/lua_src/prototypes/
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-20 22:01:29.000000 factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/lua_src/prototypes/burners.lua
--rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-05-20 22:01:29.000000 factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/lua_src/prototypes/tech.lua
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-20 22:01:29.000000 factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/lua_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-20 22:01:34.000000 factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:01:34.827902 factorio_randovania_mod-0.1.1/src/factorio_randovania_mod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-20 22:01:34.000000 factorio_randovania_mod-0.1.1/src/factorio_randovania_mod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-20 22:01:34.000000 factorio_randovania_mod-0.1.1/src/factorio_randovania_mod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 22:01:34.000000 factorio_randovania_mod-0.1.1/src/factorio_randovania_mod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-20 22:01:34.000000 factorio_randovania_mod-0.1.1/src/factorio_randovania_mod.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-20 22:01:34.000000 factorio_randovania_mod-0.1.1/src/factorio_randovania_mod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-20 22:01:34.000000 factorio_randovania_mod-0.1.1/src/factorio_randovania_mod.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:01:34.827902 factorio_randovania_mod-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-20 22:01:29.000000 factorio_randovania_mod-0.1.1/tests/test_color_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:26:14.470064 factorio_randovania_mod-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:26:14.462064 factorio_randovania_mod-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:26:14.462064 factorio_randovania_mod-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/.github/workflows/python.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-23 21:26:14.470064 factorio_randovania_mod-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 21:26:14.470064 factorio_randovania_mod-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:26:14.458064 factorio_randovania_mod-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:26:14.466064 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/color_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/configuration.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/creator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:26:14.466064 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/files/
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/files/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:26:14.466064 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/
+-rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/control.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/data-updates.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/data.lua
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:26:14.462064 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/graphics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:26:14.466064 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/graphics/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/graphics/icons/nothing.png
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:26:14.462064 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:26:14.466064 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/locale/en/
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/locale/en/strings.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:26:14.466064 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/prototypes/
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/prototypes/burners.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/prototypes/extra-tiers.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/prototypes/tech.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-23 21:26:14.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:26:14.466064 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-23 21:26:14.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-23 21:26:14.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 21:26:14.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-23 21:26:14.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-23 21:26:14.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-23 21:26:14.000000 factorio_randovania_mod-0.2.0/src/factorio_randovania_mod.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:26:14.466064 factorio_randovania_mod-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-23 21:26:08.000000 factorio_randovania_mod-0.2.0/tests/test_color_util.py
```

### Comparing `factorio_randovania_mod-0.1.1/.github/dependabot.yml` & `factorio_randovania_mod-0.2.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.1.1/.github/workflows/python.yml` & `factorio_randovania_mod-0.2.0/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.1.1/.gitignore` & `factorio_randovania_mod-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.1.1/.pre-commit-config.yaml` & `factorio_randovania_mod-0.2.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 
 repos:
 -   repo: https://github.com/astral-sh/ruff-pre-commit
     # Ruff version.
-    rev: v0.2.2
+    rev: v0.4.4
     hooks:
       - id: ruff
         args: [ --fix, --exit-non-zero-on-fix ]
       - id: ruff-format
 
 -   repo: https://github.com/henriquegemignani/jsonschema-to-typeddict
-    rev: v1.0.1
+    rev: v1.1
     hooks:
     -   id: jsonschema-to-typeddict
         files: src/factorio_randovania_mod/files/schema.json
         args: [ --output-path, src/factorio_randovania_mod/configuration.pyi, --root-name, Configuration ]
```

### Comparing `factorio_randovania_mod-0.1.1/LICENSE` & `factorio_randovania_mod-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.1.1/pyproject.toml` & `factorio_randovania_mod-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -36,18 +36,32 @@
 test = [
     "pytest",
     "pytest-cov",
     "pytest-mock",
     "pre-commit",
 ]
 
+typing = [
+    "mypy",
+    "types-Pillow",
+]
+
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [project.urls]
 Homepage = "https://github.com/randovania/factorio-randovania-mod"
 
 [tool.setuptools_scm]
 local_scheme = "no-local-version"
 write_to = "src/factorio_randovania_mod/version.py"
-git_describe_command = "git describe --dirty --tags --long --match v[0-9]*"
+git_describe_command = "git describe --dirty --tags --long --match v[0-9]*"
+
+
+[tool.mypy]
+files = [
+    "src/",
+]
+follow_imports = "silent"
+disallow_untyped_defs = true
+local_partial_types = true
```

### Comparing `factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/cli.py` & `factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/cli.py`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/color_util.py` & `factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/color_util.py`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/creator.py` & `factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/creator.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,15 +66,23 @@
                 return f"{get_localized_name(locale, front)} {number}"
         raise
 
 
 template_path = Path(__file__).parent.joinpath("lua_src")
 
 
-def create_burner_images(factorio_path: Path, output_path: Path) -> None:
+def hue_shift(input_path: Path, output_path: Path, rotation: float) -> None:
+    """Creates a new image, by shifting the hue of the input image."""
+    img = PIL.Image.open(input_path)
+    new_img = color_util.shift_hue(img, rotation / 360.0)
+    output_path.parent.mkdir(parents=True, exist_ok=True)
+    new_img.save(output_path)
+
+
+def create_hue_shifted_images(factorio_path: Path, output_path: Path) -> None:
     lab_angle = 120.0
     assembler_angle = 310.0
 
     base_graphics_path = factorio_path.joinpath("data/base/graphics")
 
     lab_images = [
         "entity/lab/lab.png",
@@ -106,19 +114,19 @@
                 path,
                 path.replace("assembling-machine-1", "burner-assembling-machine"),
                 assembler_angle / 360.0,
             )
         )
 
     for source_path, target_path, rotation in conversions:
-        img = PIL.Image.open(base_graphics_path.joinpath(source_path))
-        new_img = color_util.shift_hue(img, rotation / 360.0)
-        out_path = output_path.joinpath("graphics", target_path)
-        out_path.parent.mkdir(parents=True, exist_ok=True)
-        new_img.save(out_path)
+        hue_shift(
+            base_graphics_path.joinpath(source_path),
+            output_path.joinpath("graphics", target_path),
+            rotation,
+        )
 
 
 def create(factorio_path: Path, patch_data: Configuration, output_folder: Path) -> None:
     output_path = output_folder.joinpath("randovania-layout")
     shutil.rmtree(output_path, ignore_errors=True)
 
     original_locale = configparser.ConfigParser()
@@ -141,28 +149,27 @@
     local_unlocks = {}
 
     for tech in patch_data["technologies"]:
         tech_name = tech["tech_name"]
         locale["technology-name"][tech_name] = tech["locale_name"]
         locale["technology-description"][tech_name] = tech["description"]
 
-        new_tech = {
+        new_tech: dict = {
             "name": tech_name,
             "icon": tech["icon"],
             "costs": {
                 "count": tech["cost"]["count"],
                 "time": tech["cost"]["time"],
                 "ingredients": [[it, 1] for it in tech["cost"]["ingredients"]],
             },
             "prerequisites": tech["prerequisites"] if tech["prerequisites"] else None,
             # "fake_effects": tech["fake_effects"],
         }
-        for extra in ["icon_size"]:
-            if extra in tech:
-                new_tech[extra] = tech[extra]
+        if "icon_size" in tech:
+            new_tech["icon_size"] = tech["icon_size"]
         tech_tree_lua.append(new_tech)
 
         if len(tech["unlocks"]) == 1:
             new_tech["take_effects_from"] = tech["unlocks"][0]
             locale["technology-description"][tech_name] = get_from_locale(
                 original_locale, "technology-description", tech["unlocks"][0]
             )
@@ -194,11 +201,11 @@
 
     generate_file("tech-tree.lua", wrap_array_pretty(tech_tree_lua))
     generate_file("local-unlocks.lua", wrap(local_unlocks))
     generate_file("starting-tech.lua", wrap_array_pretty(patch_data["starting_tech"]))
     generate_file("existing-tree-repurpose.lua", wrap(existing_tree_repurpose))
     generate_file("custom-recipes.lua", wrap_array_pretty(patch_data["recipes"]))
 
-    create_burner_images(factorio_path, output_path)
+    create_hue_shifted_images(factorio_path, output_path)
 
     with output_path.joinpath("locale/en/strings.cfg").open("w") as f:
         locale.write(f, space_around_delimiters=False)
```

### Comparing `factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/files/schema.json` & `factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/files/schema.json`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/lua_src/control.lua` & `factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/control.lua`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/lua_src/data.lua` & `factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/data.lua`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     "electric-mining-drill",
     -- science
     "lab"
 }
 
 require("prototypes.burners")
 require("prototypes.tech")
+require("prototypes.extra-tiers")
 
 ---- Lock all initial recipes
 
 for _, name in ipairs(kRecipesWithNewTech) do
     set_recipe_field(data.raw["recipe"][name], "enabled", false)
 end
```

### Comparing `factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/lua_src/graphics/icons/nothing.png` & `factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/graphics/icons/nothing.png`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/lua_src/locale/en/strings.cfg` & `factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/locale/en/strings.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -5,31 +5,35 @@
 light-armor=Light armor
 long-handed-inserter=Long-handed inserter
 oil-cracking=Oil cracking
 solid-fuel=Solid fuel
 steam-power=Steam power
 regular-inserter-capacity-bonus=Regular inserter capacity bonus
 stack-inserter-capacity-bonus=Stack inserter capacity bonus
+research-productivity=Lab research Productivity
 
 [technology-description]
 regular-inserter-capacity-bonus=Allows non-stack inserters to move more items at once.
 stack-inserter-capacity-bonus=Allows stack inserters to move more items at once.
 steam-power=Source of electric energy by boiling water.
 oil-cracking=Refine the different oil products.
 big-electric-pole=Distribute electricity over long distances.
 gate=Wall sections that open up when needed. Can be controlled by the circuit network.
 long-handed-inserter=An electric inserter that picks up and places items two tiles from its location instead of the usual one.
 solid-fuel=A burnable fuel produced from the oil products.
+research-productivity=Improves the yield of your science packs, providing more research at no cost.
 
 [entity-name]
 burner-lab=Burner lab
 lab=Electric lab
 burner-assembling-machine=Burner assembling machine
+longer-handed-inserter=Longer-handed inserter
 
 [item-name]
 burner-lab=Burner lab
 lab=Electric lab
 burner-assembling-machine=Burner assembling machine
 impossible-science-pack=Unresearchable
+longer-handed-inserter=Longer-handed inserter
 
 [item-description]
 impossible-science-pack=This research is unlocked by researching something else.
```

### Comparing `factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/lua_src/prototypes/burners.lua` & `factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/prototypes/burners.lua`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/lua_src/prototypes/tech.lua` & `factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_src/prototypes/tech.lua`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,26 @@
             }
         },
         icon = "__base__/graphics/technology/fast-inserter.png",
         icon_mipmaps = 4,
         icon_size = 256
     },
     make_tech {
+        name = "longer-handed-inserter",
+        effects = {
+            {
+                recipe = "longer-handed-inserter",
+                type = "unlock-recipe"
+            }
+        },
+        icon = "__base__/graphics/technology/fast-inserter.png",
+        icon_mipmaps = 4,
+        icon_size = 256
+    },
+    make_tech {
         name = "oil-cracking",
         effects = {
             {
                 recipe = "chemical-plant",
                 type = "unlock-recipe"
             },
             {
@@ -167,8 +179,22 @@
         },
         icon = "__base__/graphics/technology/inserter-capacity.png",
         icon_mipmaps = 4,
         icon_size = 256,
         max_level = "infinite",
         upgrade = true
     },
+    make_tech {
+        name = "research-productivity",
+        effects = {
+            {
+                type = "laboratory-productivity",
+                modifier = 0.1
+            }
+        },
+        icons = util.technology_icon_constant_productivity("__base__/graphics/technology/research-speed.png"),
+        icon_mipmaps = 4,
+        icon_size = 256,
+        max_level = "infinite",
+        upgrade = true
+    },
 }
```

### Comparing `factorio_randovania_mod-0.1.1/src/factorio_randovania_mod/lua_util.py` & `factorio_randovania_mod-0.2.0/src/factorio_randovania_mod/lua_util.py`

 * *Files identical despite different names*

### Comparing `factorio_randovania_mod-0.1.1/src/factorio_randovania_mod.egg-info/SOURCES.txt` & `factorio_randovania_mod-0.2.0/src/factorio_randovania_mod.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+.gitattributes
 .gitignore
 .pre-commit-config.yaml
 LICENSE
+README.md
 pyproject.toml
 .github/codecov.yml
 .github/dependabot.yml
 .github/workflows/python.yml
 src/factorio_randovania_mod/__init__.py
 src/factorio_randovania_mod/__main__.py
 src/factorio_randovania_mod/cli.py
 src/factorio_randovania_mod/color_util.py
 src/factorio_randovania_mod/configuration.pyi
 src/factorio_randovania_mod/creator.py
 src/factorio_randovania_mod/lua_util.py
+src/factorio_randovania_mod/py.typed
 src/factorio_randovania_mod/version.py
 src/factorio_randovania_mod.egg-info/PKG-INFO
 src/factorio_randovania_mod.egg-info/SOURCES.txt
 src/factorio_randovania_mod.egg-info/dependency_links.txt
 src/factorio_randovania_mod.egg-info/entry_points.txt
 src/factorio_randovania_mod.egg-info/requires.txt
 src/factorio_randovania_mod.egg-info/top_level.txt
@@ -23,9 +26,10 @@
 src/factorio_randovania_mod/lua_src/control.lua
 src/factorio_randovania_mod/lua_src/data-updates.lua
 src/factorio_randovania_mod/lua_src/data.lua
 src/factorio_randovania_mod/lua_src/info.json
 src/factorio_randovania_mod/lua_src/graphics/icons/nothing.png
 src/factorio_randovania_mod/lua_src/locale/en/strings.cfg
 src/factorio_randovania_mod/lua_src/prototypes/burners.lua
+src/factorio_randovania_mod/lua_src/prototypes/extra-tiers.lua
 src/factorio_randovania_mod/lua_src/prototypes/tech.lua
 tests/test_color_util.py
```

