# Comparing `tmp/edwh_auth_rbac-0.2.0.tar.gz` & `tmp/edwh_auth_rbac-0.2.1.tar.gz`

## Comparing `edwh_auth_rbac-0.2.0.tar` & `edwh_auth_rbac-0.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/htmlcov/.gitignore
--rw-r--r--   0        0        0    10830 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/htmlcov/class_index.html
--rw-r--r--   0        0        0    24699 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/htmlcov/coverage_html_cb_da166b87.js
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/htmlcov/favicon_32_cb_58284776.png
--rw-r--r--   0        0        0    36695 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/htmlcov/function_index.html
--rw-r--r--   0        0        0     6425 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/htmlcov/keybd_closed_cb_ce680311.png
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/htmlcov/status.json
--rw-r--r--   0        0        0    14077 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/htmlcov/style_cb_8e611ae1.css
--rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/htmlcov/z_438b44bce6437be6___init___py.html
--rw-r--r--   0        0        0     7068 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/htmlcov/z_438b44bce6437be6_helpers_py.html
--rw-r--r--   0        0        0    15181 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/htmlcov/z_438b44bce6437be6_migrations_py.html
--rw-r--r--   0        0        0   123833 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/htmlcov/z_438b44bce6437be6_model_py.html
--rw-r--r--   0        0        0    61606 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/htmlcov/z_438b44bce6437be6_rbac_py.html
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/htmlcov/z_a44f0ac069e85531___init___py.html
--rw-r--r--   0        0        0    60186 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/htmlcov/z_a44f0ac069e85531_test_rbac_py.html
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/src/edwh_auth_rbac/__init__.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/src/edwh_auth_rbac/helpers.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/src/edwh_auth_rbac/migrations.py
--rw-r--r--   0        0        0    13060 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/src/edwh_auth_rbac/model.py
--rw-r--r--   0        0        0     7658 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/src/edwh_auth_rbac/rbac.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/tests/test_rbac.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/.gitignore
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/README.md
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.1/htmlcov/.gitignore
+-rw-r--r--   0        0        0    10830 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.1/htmlcov/class_index.html
+-rw-r--r--   0        0        0    24699 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.1/htmlcov/coverage_html_cb_da166b87.js
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.1/htmlcov/favicon_32_cb_58284776.png
+-rw-r--r--   0        0        0    36695 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.1/htmlcov/function_index.html
+-rw-r--r--   0        0        0     6425 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.1/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.1/htmlcov/keybd_closed_cb_ce680311.png
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.1/htmlcov/status.json
+-rw-r--r--   0        0        0    14077 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.1/htmlcov/style_cb_8e611ae1.css
+-rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.1/htmlcov/z_438b44bce6437be6___init___py.html
+-rw-r--r--   0        0        0     7068 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.1/htmlcov/z_438b44bce6437be6_helpers_py.html
+-rw-r--r--   0        0        0    15181 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.1/htmlcov/z_438b44bce6437be6_migrations_py.html
+-rw-r--r--   0        0        0   123833 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.1/htmlcov/z_438b44bce6437be6_model_py.html
+-rw-r--r--   0        0        0    61606 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.1/htmlcov/z_438b44bce6437be6_rbac_py.html
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.1/htmlcov/z_a44f0ac069e85531___init___py.html
+-rw-r--r--   0        0        0    60186 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.1/htmlcov/z_a44f0ac069e85531_test_rbac_py.html
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.1/src/edwh_auth_rbac/__init__.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.1/src/edwh_auth_rbac/helpers.py
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.1/src/edwh_auth_rbac/migrations.py
+-rw-r--r--   0        0        0    13060 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.1/src/edwh_auth_rbac/model.py
+-rw-r--r--   0        0        0     7658 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.1/src/edwh_auth_rbac/rbac.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.1/tests/test_rbac.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.1/.gitignore
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.1/README.md
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.1/PKG-INFO
```

### Comparing `edwh_auth_rbac-0.2.0/CHANGELOG.md` & `edwh_auth_rbac-0.2.1/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.2.1 (2024-05-22)
+
+### Fix
+
+* Those views are not tables ([`f2d8496`](https://github.com/educationwarehouse/edwh-auth-rbac/commit/f2d84962bd3aa5bf87901d999f180ac1e9ffd815))
+
 ## v0.2.0 (2024-05-22)
 
 ### Feature
 
 * Publish (postgres) migrations for rbac ([`5d00057`](https://github.com/educationwarehouse/edwh-auth-rbac/commit/5d00057d16e58c87369be0658fa1c62032ea045b))
 
 ### Fix
```

### Comparing `edwh_auth_rbac-0.2.0/htmlcov/class_index.html` & `edwh_auth_rbac-0.2.1/htmlcov/class_index.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.0/htmlcov/coverage_html_cb_da166b87.js` & `edwh_auth_rbac-0.2.1/htmlcov/coverage_html_cb_da166b87.js`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.0/htmlcov/favicon_32_cb_58284776.png` & `edwh_auth_rbac-0.2.1/htmlcov/favicon_32_cb_58284776.png`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.0/htmlcov/function_index.html` & `edwh_auth_rbac-0.2.1/htmlcov/function_index.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.0/htmlcov/index.html` & `edwh_auth_rbac-0.2.1/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.0/htmlcov/keybd_closed_cb_ce680311.png` & `edwh_auth_rbac-0.2.1/htmlcov/keybd_closed_cb_ce680311.png`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.0/htmlcov/status.json` & `edwh_auth_rbac-0.2.1/htmlcov/status.json`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.0/htmlcov/style_cb_8e611ae1.css` & `edwh_auth_rbac-0.2.1/htmlcov/style_cb_8e611ae1.css`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.0/htmlcov/z_438b44bce6437be6___init___py.html` & `edwh_auth_rbac-0.2.1/htmlcov/z_438b44bce6437be6___init___py.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.0/htmlcov/z_438b44bce6437be6_helpers_py.html` & `edwh_auth_rbac-0.2.1/htmlcov/z_438b44bce6437be6_helpers_py.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.0/htmlcov/z_438b44bce6437be6_migrations_py.html` & `edwh_auth_rbac-0.2.1/htmlcov/z_438b44bce6437be6_migrations_py.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.0/htmlcov/z_438b44bce6437be6_model_py.html` & `edwh_auth_rbac-0.2.1/htmlcov/z_438b44bce6437be6_model_py.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.0/htmlcov/z_438b44bce6437be6_rbac_py.html` & `edwh_auth_rbac-0.2.1/htmlcov/z_438b44bce6437be6_rbac_py.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.0/htmlcov/z_a44f0ac069e85531___init___py.html` & `edwh_auth_rbac-0.2.1/htmlcov/z_a44f0ac069e85531___init___py.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.0/htmlcov/z_a44f0ac069e85531_test_rbac_py.html` & `edwh_auth_rbac-0.2.1/htmlcov/z_a44f0ac069e85531_test_rbac_py.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.0/src/edwh_auth_rbac/model.py` & `edwh_auth_rbac-0.2.1/src/edwh_auth_rbac/model.py`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.0/src/edwh_auth_rbac/rbac.py` & `edwh_auth_rbac-0.2.1/src/edwh_auth_rbac/rbac.py`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.0/tests/test_rbac.py` & `edwh_auth_rbac-0.2.1/tests/test_rbac.py`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.0/pyproject.toml` & `edwh_auth_rbac-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.2.0/PKG-INFO` & `edwh_auth_rbac-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: edwh-auth-rbac
-Version: 0.2.0
+Version: 0.2.1
 Summary: Recursive Memberships and Permissions for the Education Warehouse Authentication System
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-auth-rbac#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-auth-rbac/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-auth-rbac
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>
 License-Expression: MIT
 Keywords: edwh,omgeving,whitelabel
```

