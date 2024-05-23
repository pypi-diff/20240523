# Comparing `tmp/loe_simp_app_fw-1.4.0.tar.gz` & `tmp/loe_simp_app_fw-1.4.1.tar.gz`

## Comparing `loe_simp_app_fw-1.4.0.tar` & `loe_simp_app_fw-1.4.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.0/config-example.yaml
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.0/src/loe_simp_app_fw/__init__.py
--rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.0/src/loe_simp_app_fw/config.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.0/src/loe_simp_app_fw/helper.py
--rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.0/src/loe_simp_app_fw/logger.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.0/tests/test_import.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.0/LICENSE
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.0/README.md
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.1/config-example.yaml
+-rwxr-xr-x   0        0        0     2617 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.1/.github/workflows/workflow.yaml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.1/src/loe_simp_app_fw/__init__.py
+-rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.1/src/loe_simp_app_fw/config.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.1/src/loe_simp_app_fw/helper.py
+-rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.1/src/loe_simp_app_fw/logger.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.1/tests/test_import.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.1/LICENSE
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.1/README.md
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.4.1/PKG-INFO
```

### Comparing `loe_simp_app_fw-1.4.0/src/loe_simp_app_fw/config.py` & `loe_simp_app_fw-1.4.1/src/loe_simp_app_fw/config.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.4.0/src/loe_simp_app_fw/helper.py` & `loe_simp_app_fw-1.4.1/src/loe_simp_app_fw/helper.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.4.0/src/loe_simp_app_fw/logger.py` & `loe_simp_app_fw-1.4.1/src/loe_simp_app_fw/logger.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.4.0/tests/test_import.py` & `loe_simp_app_fw-1.4.1/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.4.0/.gitignore` & `loe_simp_app_fw-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.4.0/LICENSE` & `loe_simp_app_fw-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.4.0/README.md` & `loe_simp_app_fw-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.4.0/pyproject.toml` & `loe_simp_app_fw-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "loe_simp_app_fw"
-version = "1.4.0"
+version = "1.4.1"
 authors = [
   { name="loeeeee", email="95266635+loeeeee@users.noreply.github.com" },
 ]
 description = "A super simple python app framework that includes a logger and a config manager. Also usable in jupyter notebook."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `loe_simp_app_fw-1.4.0/PKG-INFO` & `loe_simp_app_fw-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: loe_simp_app_fw
-Version: 1.4.0
+Version: 1.4.1
 Summary: A super simple python app framework that includes a logger and a config manager. Also usable in jupyter notebook.
 Project-URL: Homepage, https://github.com/loeeeee/loe-simp-app-fw
 Project-URL: Issues, https://github.com/loeeeee/loe-simp-app-fw/issues
 Author-email: loeeeee <95266635+loeeeee@users.noreply.github.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

