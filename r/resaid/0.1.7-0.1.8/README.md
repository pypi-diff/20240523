# Comparing `tmp/resaid-0.1.7.tar.gz` & `tmp/resaid-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resaid-0.1.7.tar", last modified: Thu Apr 18 16:39:12 2024, max compression
+gzip compressed data, was "resaid-0.1.8.tar", last modified: Thu May 23 15:25:31 2024, max compression
```

## Comparing `resaid-0.1.7.tar` & `resaid-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 16:39:12.113599 resaid-0.1.7/
--rw-rw-rw-   0        0        0     1067 2023-10-05 19:55:40.000000 resaid-0.1.7/LICENSE
--rw-rw-rw-   0        0        0      704 2024-04-18 16:39:12.109607 resaid-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0       70 2022-02-28 19:33:00.000000 resaid-0.1.7/README.md
--rw-rw-rw-   0        0        0      103 2023-10-09 21:04:28.000000 resaid-0.1.7/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-18 16:39:12.062637 resaid-0.1.7/resaid/
--rw-rw-rw-   0        0        0        0 2021-10-06 19:02:31.000000 resaid-0.1.7/resaid/__init__.py
--rw-rw-rw-   0        0        0    42266 2023-12-01 16:38:17.000000 resaid-0.1.7/resaid/dca.py
--rw-rw-rw-   0        0        0    23130 2024-04-18 13:52:40.000000 resaid-0.1.7/resaid/econ.py
-drwxrwxrwx   0        0        0        0 2024-04-18 16:39:12.102592 resaid-0.1.7/resaid.egg-info/
--rw-rw-rw-   0        0        0      704 2024-04-18 16:39:11.000000 resaid-0.1.7/resaid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-04-18 16:39:11.000000 resaid-0.1.7/resaid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 16:39:11.000000 resaid-0.1.7/resaid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-04-18 16:39:11.000000 resaid-0.1.7/resaid.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-18 16:39:11.000000 resaid-0.1.7/resaid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 16:39:12.115600 resaid-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1177 2024-04-17 20:59:08.000000 resaid-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 15:25:31.476505 resaid-0.1.8/
+-rw-rw-rw-   0        0        0     1067 2023-10-05 19:55:40.000000 resaid-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0      704 2024-05-23 15:25:31.466506 resaid-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0       70 2022-02-28 19:33:00.000000 resaid-0.1.8/README.md
+-rw-rw-rw-   0        0        0      103 2023-10-09 21:04:28.000000 resaid-0.1.8/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-23 15:25:31.379646 resaid-0.1.8/resaid/
+-rw-rw-rw-   0        0        0        0 2021-10-06 19:02:31.000000 resaid-0.1.8/resaid/__init__.py
+-rw-rw-rw-   0        0        0    42266 2023-12-01 16:38:17.000000 resaid-0.1.8/resaid/dca.py
+-rw-rw-rw-   0        0        0    23548 2024-05-23 15:22:40.000000 resaid-0.1.8/resaid/econ.py
+drwxrwxrwx   0        0        0        0 2024-05-23 15:25:31.453505 resaid-0.1.8/resaid.egg-info/
+-rw-rw-rw-   0        0        0      704 2024-05-23 15:25:30.000000 resaid-0.1.8/resaid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-23 15:25:31.000000 resaid-0.1.8/resaid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 15:25:30.000000 resaid-0.1.8/resaid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-05-23 15:25:30.000000 resaid-0.1.8/resaid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-23 15:25:30.000000 resaid-0.1.8/resaid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 15:25:31.479507 resaid-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1177 2024-05-23 15:24:48.000000 resaid-0.1.8/setup.py
```

### Comparing `resaid-0.1.7/LICENSE` & `resaid-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `resaid-0.1.7/PKG-INFO` & `resaid-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resaid
-Version: 0.1.7
+Version: 0.1.8
 Summary: Reservoir engineering tools
 Home-page: https://github.com/gregeasley/resaid
 Author: Greg Easley
 Author-email: greg@easley.dev
 Project-URL: Bug Tracker, https://github.com/gregeasley/resaid/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `resaid-0.1.7/resaid/dca.py` & `resaid-0.1.8/resaid/dca.py`

 * *Files identical despite different names*

### Comparing `resaid-0.1.7/resaid/econ.py` & `resaid-0.1.8/resaid/econ.py`

 * *Files 2% similar despite different names*

```diff
@@ -573,14 +573,19 @@
             l_nri = 1-l_royalty
         else:
             l_royalty = self._royalty
             l_flow['royalty'] = l_flow['revenue']*self._royalty
             l_wi = 1
             l_nri = 1-l_royalty
 
+        l_flow['fixed_expense'] = self._opc_t
+        l_flow['oil_variable_expense'] = self._opc_oil*l_flow[self.OIL_COL]
+        l_flow['gas_variable_expense'] = self._opc_gas*l_flow['gas_sold']
+        l_flow['water_variable_expense'] = self._opc_water*l_flow[self.WATER_COL]
+
         l_flow['expense'] = (
             self._opc_t
             + self._opc_gas*l_flow['gas_sold']
             + self._opc_oil*l_flow[self.OIL_COL]
             + self._opc_water*l_flow[self.WATER_COL]
         )
 
@@ -634,14 +639,18 @@
             self.WATER_COL,
             'ngl_volume',
             'oil_revenue',
             'gas_revenue',
             'ngl_revenue',
             'revenue',
             'royalty',
+            'fixed_expense',
+            'oil_variable_expense',
+            'gas_variable_expense',
+            'water_variable_expense',
             'expense',
             'severance_tax',
             'ad_val_tax',
             'taxes',
             'capex',
             'cf',
             'dcf'
```

### Comparing `resaid-0.1.7/resaid.egg-info/PKG-INFO` & `resaid-0.1.8/resaid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resaid
-Version: 0.1.7
+Version: 0.1.8
 Summary: Reservoir engineering tools
 Home-page: https://github.com/gregeasley/resaid
 Author: Greg Easley
 Author-email: greg@easley.dev
 Project-URL: Bug Tracker, https://github.com/gregeasley/resaid/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `resaid-0.1.7/setup.py` & `resaid-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="resaid",
-    version="0.1.7",
+    version="0.1.8",
     author="Greg Easley",
     author_email="greg@easley.dev",
     description="Reservoir engineering tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gregeasley/resaid",
     project_urls={
```

