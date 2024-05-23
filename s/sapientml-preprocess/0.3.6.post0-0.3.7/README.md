# Comparing `tmp/sapientml_preprocess-0.3.6.post0.tar.gz` & `tmp/sapientml_preprocess-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sapientml_preprocess-0.3.6.post0.tar", max compression
+gzip compressed data, was "sapientml_preprocess-0.3.7.tar", max compression
```

## Comparing `sapientml_preprocess-0.3.6.post0.tar` & `sapientml_preprocess-0.3.7.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0    11356 2024-03-18 15:28:15.774729 sapientml_preprocess-0.3.6.post0/LICENSE
--rw-r--r--   0        0        0     1269 2024-03-18 15:28:30.974648 sapientml_preprocess-0.3.6.post0/pyproject.toml
--rw-r--r--   0        0        0      703 2024-03-18 15:28:15.778729 sapientml_preprocess-0.3.6.post0/sapientml_preprocess/__init__.py
--rw-r--r--   0        0        0    13596 2024-03-18 15:28:15.778729 sapientml_preprocess-0.3.6.post0/sapientml_preprocess/generator.py
--rw-r--r--   0        0        0      760 2024-03-18 15:28:15.778729 sapientml_preprocess-0.3.6.post0/sapientml_preprocess/params.py
--rw-r--r--   0        0        0      301 2024-03-18 15:28:15.778729 sapientml_preprocess-0.3.6.post0/sapientml_preprocess/templates/drop_one_value_columns.py.jinja
--rw-r--r--   0        0        0      332 2024-03-18 15:28:15.778729 sapientml_preprocess-0.3.6.post0/sapientml_preprocess/templates/handle_inf_columns.py.jinja
--rw-r--r--   0        0        0      310 2024-03-18 15:28:15.778729 sapientml_preprocess-0.3.6.post0/sapientml_preprocess/templates/handle_iterable_values.py.jinja
--rw-r--r--   0        0        0     1244 2024-03-18 15:28:15.778729 sapientml_preprocess-0.3.6.post0/sapientml_preprocess/templates/handle_japanese_text.py.jinja
--rw-r--r--   0        0        0     1107 2024-03-18 15:28:15.778729 sapientml_preprocess-0.3.6.post0/sapientml_preprocess/templates/handle_mixed_typed_columns.py.jinja
--rw-r--r--   0        0        0      509 2024-03-18 15:28:15.778729 sapientml_preprocess-0.3.6.post0/sapientml_preprocess/templates/rename_columns.py.jinja
--rw-r--r--   0        0        0      824 1970-01-01 00:00:00.000000 sapientml_preprocess-0.3.6.post0/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-05-23 06:24:00.146649 sapientml_preprocess-0.3.7/LICENSE
+-rw-r--r--   0        0        0     1251 2024-05-23 06:24:23.122633 sapientml_preprocess-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0      703 2024-05-23 06:24:00.150649 sapientml_preprocess-0.3.7/sapientml_preprocess/__init__.py
+-rw-r--r--   0        0        0    14154 2024-05-23 06:24:00.150649 sapientml_preprocess-0.3.7/sapientml_preprocess/generator.py
+-rw-r--r--   0        0        0      760 2024-05-23 06:24:00.150649 sapientml_preprocess-0.3.7/sapientml_preprocess/params.py
+-rw-r--r--   0        0        0      301 2024-05-23 06:24:00.150649 sapientml_preprocess-0.3.7/sapientml_preprocess/templates/drop_one_value_columns.py.jinja
+-rw-r--r--   0        0        0      332 2024-05-23 06:24:00.150649 sapientml_preprocess-0.3.7/sapientml_preprocess/templates/handle_inf_columns.py.jinja
+-rw-r--r--   0        0        0      310 2024-05-23 06:24:00.150649 sapientml_preprocess-0.3.7/sapientml_preprocess/templates/handle_iterable_values.py.jinja
+-rw-r--r--   0        0        0     1244 2024-05-23 06:24:00.150649 sapientml_preprocess-0.3.7/sapientml_preprocess/templates/handle_japanese_text.py.jinja
+-rw-r--r--   0        0        0     1107 2024-05-23 06:24:00.150649 sapientml_preprocess-0.3.7/sapientml_preprocess/templates/handle_mixed_typed_columns.py.jinja
+-rw-r--r--   0        0        0      180 2024-05-23 06:24:00.150649 sapientml_preprocess-0.3.7/sapientml_preprocess/templates/none_has_columns.py.jinja
+-rw-r--r--   0        0        0      509 2024-05-23 06:24:00.150649 sapientml_preprocess-0.3.7/sapientml_preprocess/templates/rename_columns.py.jinja
+-rw-r--r--   0        0        0      818 1970-01-01 00:00:00.000000 sapientml_preprocess-0.3.7/PKG-INFO
```

### Comparing `sapientml_preprocess-0.3.6.post0/LICENSE` & `sapientml_preprocess-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sapientml_preprocess-0.3.6.post0/pyproject.toml` & `sapientml_preprocess-0.3.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sapientml-preprocess"
-version = "0.3.6.post0"
+version = "0.3.7"
 description = "A SapientML plugin of preprocess CodeBlockGenerator"
 authors = ["The SapientML Authors"]
 maintainers = [
     "Kosaku Kimura <kimura.kosaku@fujitsu.com>",
     "Akira Ura <ura.akira@fujitsu.com>",
 ]
 license = "Apache-2.0"
@@ -33,26 +33,26 @@
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."sapientml.code_block_generator"]
 preprocess = "sapientml_preprocess:Preprocess"
 
 [tool.pysen]
-version = "0.3.6.post0"
+version = "0.3.7"
 
 [tool.pysen-cli]
 settings_dir = ".pysen"
 
 [tool.pysen.lint]
 enable_black = true
 enable_flake8 = true
 enable_isort = true
 enable_mypy = false
 line_length = 120
-py_version = "0.3.6.post0"
+py_version = "0.3.7"
 
 [tool.pysen.lint.source]
 includes = ["sapientml_preprocess/", "tests/"]
 
 [tool.pytest.ini_options]
 addopts = "-n auto"
 testpaths = ["tests"]
```

### Comparing `sapientml_preprocess-0.3.6.post0/sapientml_preprocess/__init__.py` & `sapientml_preprocess-0.3.7/sapientml_preprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `sapientml_preprocess-0.3.6.post0/sapientml_preprocess/generator.py` & `sapientml_preprocess-0.3.7/sapientml_preprocess/generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -235,14 +235,23 @@
             ]
             tpl = template_env.get_template("rename_columns.py.jinja")
             code.validation += _render(tpl, training=True, test=True, cols_has_symbols=cols_has_symbols)
             code.test += _render(tpl, training=True, test=True, cols_has_symbols=cols_has_symbols)
             code.train += _render(tpl, training=True, test=False, cols_has_symbols=cols_has_symbols)
             code.predict += _render(tpl, training=False, test=True, cols_has_symbols=cols_has_symbols)
 
+        # If None is intentionally inserted in the data, an error occurs, so we have added an action to change None to "np.nan."
+        if df.isin([None]).any(axis=None):
+            df = df.replace([None], np.nan)
+            tpl = template_env.get_template("none_has_columns.py.jinja")
+            code.validation += _render(tpl, training=True, test=True)
+            code.test += _render(tpl, training=True, test=True)
+            code.train += _render(tpl, training=True, test=False)
+            code.predict += _render(tpl, training=False, test=True)
+
         # handle list(tuple, dict) value in dataframe.
         # in generated scripts, visualisation will be executed before pre-processing such as handle mixed-type.
         # so, need to check before mixed-type column names are added to suppress errors during visualisation.
         cols_iterable_values = []
         for col in df.columns:
             exist_list_values = [x for x in df[col] if type(x) in [list, tuple, dict]]
             if len(exist_list_values) > 0:
```

### Comparing `sapientml_preprocess-0.3.6.post0/sapientml_preprocess/params.py` & `sapientml_preprocess-0.3.7/sapientml_preprocess/params.py`

 * *Files identical despite different names*

### Comparing `sapientml_preprocess-0.3.6.post0/sapientml_preprocess/templates/handle_japanese_text.py.jinja` & `sapientml_preprocess-0.3.7/sapientml_preprocess/templates/handle_japanese_text.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_preprocess-0.3.6.post0/sapientml_preprocess/templates/handle_mixed_typed_columns.py.jinja` & `sapientml_preprocess-0.3.7/sapientml_preprocess/templates/handle_mixed_typed_columns.py.jinja`

 * *Files identical despite different names*

### Comparing `sapientml_preprocess-0.3.6.post0/PKG-INFO` & `sapientml_preprocess-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapientml-preprocess
-Version: 0.3.6.post0
+Version: 0.3.7
 Summary: A SapientML plugin of preprocess CodeBlockGenerator
 License: Apache-2.0
 Author: The SapientML Authors
 Maintainer: Kosaku Kimura
 Maintainer-email: kimura.kosaku@fujitsu.com
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
```

