# Comparing `tmp/python_linters-0.1.2.tar.gz` & `tmp/python_linters-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_linters-0.1.2.tar", max compression
+gzip compressed data, was "python_linters-0.1.3.tar", max compression
```

## Comparing `python_linters-0.1.2.tar` & `python_linters-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1073 2024-05-21 06:39:18.689597 python_linters-0.1.2/LICENSE
--rw-r--r--   0        0        0     8928 2024-05-21 06:39:18.689597 python_linters-0.1.2/README.md
--rw-r--r--   0        0        0      963 2024-05-21 06:39:30.665487 python_linters-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2960 2024-05-21 06:39:18.689597 python_linters-0.1.2/python_linters/.flake8
--rw-r--r--   0        0        0        0 2024-05-21 06:39:18.689597 python_linters-0.1.2/python_linters/__init__.py
--rw-r--r--   0        0        0      859 2024-05-21 06:39:18.689597 python_linters-0.1.2/python_linters/add_noqa.py
--rw-r--r--   0        0        0      758 2024-05-21 06:39:18.689597 python_linters-0.1.2/python_linters/fix_code.py
--rw-r--r--   0        0        0      531 2024-05-21 06:39:18.689597 python_linters-0.1.2/python_linters/parse_rules.py
--rw-r--r--   0        0        0     7364 2024-05-21 06:39:18.689597 python_linters-0.1.2/python_linters/ruff.toml
--rw-r--r--   0        0        0     1647 2024-05-21 06:39:18.689597 python_linters-0.1.2/python_linters/ruff_rule_categories.py
--rw-r--r--   0        0        0    75528 2024-05-21 06:39:18.689597 python_linters-0.1.2/python_linters/ruff_rules.txt
--rw-r--r--   0        0        0     3466 2024-05-21 06:39:18.689597 python_linters-0.1.2/python_linters/run_linters.py
--rw-r--r--   0        0        0     9763 1970-01-01 00:00:00.000000 python_linters-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-23 07:59:33.566660 python_linters-0.1.3/LICENSE
+-rw-r--r--   0        0        0     8928 2024-05-23 07:59:33.566660 python_linters-0.1.3/README.md
+-rw-r--r--   0        0        0      963 2024-05-23 07:59:43.818793 python_linters-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2960 2024-05-23 07:59:33.566660 python_linters-0.1.3/python_linters/.flake8
+-rw-r--r--   0        0        0        0 2024-05-23 07:59:33.566660 python_linters-0.1.3/python_linters/__init__.py
+-rw-r--r--   0        0        0      859 2024-05-23 07:59:33.566660 python_linters-0.1.3/python_linters/add_noqa.py
+-rw-r--r--   0        0        0      758 2024-05-23 07:59:33.566660 python_linters-0.1.3/python_linters/fix_code.py
+-rw-r--r--   0        0        0      531 2024-05-23 07:59:33.566660 python_linters-0.1.3/python_linters/parse_rules.py
+-rw-r--r--   0        0        0     7333 2024-05-23 07:59:33.566660 python_linters-0.1.3/python_linters/ruff.toml
+-rw-r--r--   0        0        0     1647 2024-05-23 07:59:33.566660 python_linters-0.1.3/python_linters/ruff_rule_categories.py
+-rw-r--r--   0        0        0    75528 2024-05-23 07:59:33.566660 python_linters-0.1.3/python_linters/ruff_rules.txt
+-rw-r--r--   0        0        0     3466 2024-05-23 07:59:33.566660 python_linters-0.1.3/python_linters/run_linters.py
+-rw-r--r--   0        0        0     9763 1970-01-01 00:00:00.000000 python_linters-0.1.3/PKG-INFO
```

### Comparing `python_linters-0.1.2/LICENSE` & `python_linters-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_linters-0.1.2/README.md` & `python_linters-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `python_linters-0.1.2/pyproject.toml` & `python_linters-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-linters"
-version = "0.1.2"
+version = "0.1.3"
 description = "bundling config files for linters like ruff and flake8"
 authors = ["Tilo Himmelsbach <dertilo@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/dertilo/python-linters"
 packages = [{ include = "python_linters" }]
 
 include=["python_linters/.flake8","python_linters/ruff.toml"]
```

### Comparing `python_linters-0.1.2/python_linters/.flake8` & `python_linters-0.1.3/python_linters/.flake8`

 * *Files identical despite different names*

### Comparing `python_linters-0.1.2/python_linters/add_noqa.py` & `python_linters-0.1.3/python_linters/add_noqa.py`

 * *Files identical despite different names*

### Comparing `python_linters-0.1.2/python_linters/fix_code.py` & `python_linters-0.1.3/python_linters/fix_code.py`

 * *Files identical despite different names*

### Comparing `python_linters-0.1.2/python_linters/parse_rules.py` & `python_linters-0.1.3/python_linters/parse_rules.py`

 * *Files identical despite different names*

### Comparing `python_linters-0.1.2/python_linters/ruff.toml` & `python_linters-0.1.3/python_linters/ruff.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 target-version = "py310"
-[lint.isort]
-profile = "black"
 # Exclude a variety of commonly ignored directories. see https://beta.ruff.rs/docs/configuration/#using-pyprojecttoml
 [lint]
 exclude = [
     ".bzr",
     ".direnv",
     ".eggs",
     ".git",
```

### Comparing `python_linters-0.1.2/python_linters/ruff_rule_categories.py` & `python_linters-0.1.3/python_linters/ruff_rule_categories.py`

 * *Files identical despite different names*

### Comparing `python_linters-0.1.2/python_linters/ruff_rules.txt` & `python_linters-0.1.3/python_linters/ruff_rules.txt`

 * *Files identical despite different names*

### Comparing `python_linters-0.1.2/python_linters/run_linters.py` & `python_linters-0.1.3/python_linters/run_linters.py`

 * *Files identical despite different names*

### Comparing `python_linters-0.1.2/PKG-INFO` & `python_linters-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-linters
-Version: 0.1.2
+Version: 0.1.3
 Summary: bundling config files for linters like ruff and flake8
 Home-page: https://github.com/dertilo/python-linters
 Author: Tilo Himmelsbach
 Author-email: dertilo@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

