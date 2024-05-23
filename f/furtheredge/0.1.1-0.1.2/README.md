# Comparing `tmp/furtheredge-0.1.1.tar.gz` & `tmp/furtheredge-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furtheredge-0.1.1.tar", last modified: Sat Apr 13 15:49:57 2024, max compression
+gzip compressed data, was "furtheredge-0.1.2.tar", last modified: Thu May 23 11:12:27 2024, max compression
```

## Comparing `furtheredge-0.1.1.tar` & `furtheredge-0.1.2.tar`

### file list

```diff
@@ -1,43 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:49:57.807524 furtheredge-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-13 15:49:48.000000 furtheredge-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-13 15:49:57.807524 furtheredge-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-13 15:49:48.000000 furtheredge-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:49:57.799524 furtheredge-0.1.1/furtheredge/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:49:48.000000 furtheredge-0.1.1/furtheredge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:49:57.807524 furtheredge-0.1.1/furtheredge/inputs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:49:48.000000 furtheredge-0.1.1/furtheredge/inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1958711 2024-04-13 15:49:48.000000 furtheredge-0.1.1/furtheredge/inputs/model_points2.csv
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-13 15:49:48.000000 furtheredge-0.1.1/furtheredge/inputs/product.csv
--rw-r--r--   0 runner    (1001) docker     (127)    23785 2024-04-13 15:49:48.000000 furtheredge-0.1.1/furtheredge/inputs/ri_rates.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-13 15:49:48.000000 furtheredge-0.1.1/furtheredge/inputs/tech_assumptions.csv
--rw-r--r--   0 runner    (1001) docker     (127)    42155 2024-04-13 15:49:48.000000 furtheredge-0.1.1/furtheredge/inputs/wop_rates.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:49:57.807524 furtheredge-0.1.1/furtheredge/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:49:48.000000 furtheredge-0.1.1/furtheredge/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:49:57.807524 furtheredge-0.1.1/furtheredge/modules/universal_life/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:49:48.000000 furtheredge-0.1.1/furtheredge/modules/universal_life/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-13 15:49:48.000000 furtheredge-0.1.1/furtheredge/modules/universal_life/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:49:57.807524 furtheredge-0.1.1/furtheredge/modules/universal_life/sub_modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:49:48.000000 furtheredge-0.1.1/furtheredge/modules/universal_life/sub_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10012 2024-04-13 15:49:48.000000 furtheredge-0.1.1/furtheredge/modules/universal_life/sub_modules/duration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-13 15:49:48.000000 furtheredge-0.1.1/furtheredge/modules/universal_life/sub_modules/proba.py
--rw-r--r--   0 runner    (1001) docker     (127)     9663 2024-04-13 15:49:48.000000 furtheredge-0.1.1/furtheredge/modules/universal_life/sub_modules/prospective.py
--rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-04-13 15:49:48.000000 furtheredge-0.1.1/furtheredge/modules/universal_life/sub_modules/reserve.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-13 15:49:48.000000 furtheredge-0.1.1/furtheredge/modules/universal_life/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-13 15:49:48.000000 furtheredge-0.1.1/furtheredge/universal_life_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:49:57.807524 furtheredge-0.1.1/furtheredge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-13 15:49:57.000000 furtheredge-0.1.1/furtheredge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-13 15:49:57.000000 furtheredge-0.1.1/furtheredge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:49:57.000000 furtheredge-0.1.1/furtheredge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-13 15:49:57.000000 furtheredge-0.1.1/furtheredge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-13 15:49:57.000000 furtheredge-0.1.1/furtheredge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-13 15:49:48.000000 furtheredge-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 15:49:57.807524 furtheredge-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-13 15:49:48.000000 furtheredge-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:49:57.807524 furtheredge-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:49:48.000000 furtheredge-0.1.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:49:57.807524 furtheredge-0.1.1/tests/universal_life/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:49:48.000000 furtheredge-0.1.1/tests/universal_life/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:49:57.807524 furtheredge-0.1.1/tests/universal_life/sub_modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:49:48.000000 furtheredge-0.1.1/tests/universal_life/sub_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-13 15:49:48.000000 furtheredge-0.1.1/tests/universal_life/sub_modules/duration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-13 15:49:48.000000 furtheredge-0.1.1/tests/universal_life/universal_life_module_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:12:27.748610 furtheredge-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-23 11:12:17.000000 furtheredge-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-23 11:12:27.748610 furtheredge-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-23 11:12:17.000000 furtheredge-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:12:27.740610 furtheredge-0.1.2/furtheredge/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 11:12:17.000000 furtheredge-0.1.2/furtheredge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-23 11:12:17.000000 furtheredge-0.1.2/furtheredge/abstracted_packages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:12:27.744609 furtheredge-0.1.2/furtheredge/inputs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:12:17.000000 furtheredge-0.1.2/furtheredge/inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1958711 2024-05-23 11:12:17.000000 furtheredge-0.1.2/furtheredge/inputs/model_points2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-23 11:12:17.000000 furtheredge-0.1.2/furtheredge/inputs/product.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    23786 2024-05-23 11:12:17.000000 furtheredge-0.1.2/furtheredge/inputs/ri_rates.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-05-23 11:12:17.000000 furtheredge-0.1.2/furtheredge/inputs/tech_assumptions.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    42155 2024-05-23 11:12:17.000000 furtheredge-0.1.2/furtheredge/inputs/wop_rates.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:12:27.744609 furtheredge-0.1.2/furtheredge/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 11:12:17.000000 furtheredge-0.1.2/furtheredge/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:12:27.744609 furtheredge-0.1.2/furtheredge/modules/model_point_generator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:12:17.000000 furtheredge-0.1.2/furtheredge/modules/model_point_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-23 11:12:17.000000 furtheredge-0.1.2/furtheredge/modules/model_point_generator/model_point_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-23 11:12:17.000000 furtheredge-0.1.2/furtheredge/modules/model_point_generator/policies_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-23 11:12:17.000000 furtheredge-0.1.2/furtheredge/modules/model_point_generator/policy_refinement.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:12:27.748610 furtheredge-0.1.2/furtheredge/modules/universal_life/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:12:17.000000 furtheredge-0.1.2/furtheredge/modules/universal_life/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-05-23 11:12:17.000000 furtheredge-0.1.2/furtheredge/modules/universal_life/merge_all_df.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-23 11:12:17.000000 furtheredge-0.1.2/furtheredge/modules/universal_life/required_data_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-23 11:12:17.000000 furtheredge-0.1.2/furtheredge/modules/universal_life/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:12:27.748610 furtheredge-0.1.2/furtheredge/modules/universal_life/sub_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:12:17.000000 furtheredge-0.1.2/furtheredge/modules/universal_life/sub_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9567 2024-05-23 11:12:17.000000 furtheredge-0.1.2/furtheredge/modules/universal_life/sub_modules/duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-23 11:12:17.000000 furtheredge-0.1.2/furtheredge/modules/universal_life/sub_modules/proba.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14336 2024-05-23 11:12:17.000000 furtheredge-0.1.2/furtheredge/modules/universal_life/sub_modules/prospective.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-05-23 11:12:17.000000 furtheredge-0.1.2/furtheredge/modules/universal_life/sub_modules/reserve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:12:27.748610 furtheredge-0.1.2/furtheredge/modules/universal_life/sub_modules_engines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:12:17.000000 furtheredge-0.1.2/furtheredge/modules/universal_life/sub_modules_engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:12:17.000000 furtheredge-0.1.2/furtheredge/modules/universal_life/sub_modules_engines/duration_calculated_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:12:17.000000 furtheredge-0.1.2/furtheredge/modules/universal_life/sub_modules_engines/proba_calculated_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:12:17.000000 furtheredge-0.1.2/furtheredge/modules/universal_life/sub_modules_engines/prospective_calculated_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:12:17.000000 furtheredge-0.1.2/furtheredge/modules/universal_life/sub_modules_engines/reserve_calculated_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-23 11:12:17.000000 furtheredge-0.1.2/furtheredge/modules/universal_life/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-23 11:12:17.000000 furtheredge-0.1.2/furtheredge/modules/validator_dfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-23 11:12:17.000000 furtheredge-0.1.2/furtheredge/universal_life_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:12:27.748610 furtheredge-0.1.2/furtheredge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-23 11:12:27.000000 furtheredge-0.1.2/furtheredge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-23 11:12:27.000000 furtheredge-0.1.2/furtheredge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 11:12:27.000000 furtheredge-0.1.2/furtheredge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-23 11:12:27.000000 furtheredge-0.1.2/furtheredge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-23 11:12:27.000000 furtheredge-0.1.2/furtheredge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-23 11:12:17.000000 furtheredge-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 11:12:27.748610 furtheredge-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-23 11:12:17.000000 furtheredge-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:12:27.748610 furtheredge-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:12:17.000000 furtheredge-0.1.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:12:27.748610 furtheredge-0.1.2/tests/universal_life/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:12:17.000000 furtheredge-0.1.2/tests/universal_life/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:12:27.748610 furtheredge-0.1.2/tests/universal_life/sub_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:12:17.000000 furtheredge-0.1.2/tests/universal_life/sub_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-23 11:12:17.000000 furtheredge-0.1.2/tests/universal_life/sub_modules/duration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-23 11:12:17.000000 furtheredge-0.1.2/tests/universal_life/universal_life_module_test.py
```

### Comparing `furtheredge-0.1.1/furtheredge/inputs/model_points2.csv` & `furtheredge-0.1.2/furtheredge/inputs/model_points2.csv`

 * *Files identical despite different names*

### Comparing `furtheredge-0.1.1/furtheredge/inputs/ri_rates.csv` & `furtheredge-0.1.2/furtheredge/inputs/ri_rates.csv`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿RI_RATE_ID;AGE;COVER;RATE
+﻿RI_RATES_ID;AGE;COVER;RATE
 1;0;Death;0,21
 1;1;Death;0,21
 1;2;Death;0,21
 1;3;Death;0,21
 1;4;Death;0,21
 1;5;Death;0,21
 1;6;Death;0,21
```

### Comparing `furtheredge-0.1.1/furtheredge/inputs/tech_assumptions.csv` & `furtheredge-0.1.2/furtheredge/inputs/tech_assumptions.csv`

 * *Files identical despite different names*

### Comparing `furtheredge-0.1.1/furtheredge/inputs/wop_rates.csv` & `furtheredge-0.1.2/furtheredge/inputs/wop_rates.csv`

 * *Files identical despite different names*

### Comparing `furtheredge-0.1.1/furtheredge/universal_life_module.py` & `furtheredge-0.1.2/tests/universal_life/universal_life_module_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-import pandas as pd
-from furtheredge.modules.universal_life.run import universal_life_module
-import pkg_resources
+# from furtheredge.abstracted_packages import furtheredge_pandas as pd
+# from pandas.testing import assert_frame_equal
+# from furtheredge.modules.universal_life.run import universal_life_module
+
+
+# def should_return_universal_life_product():
+#     # Given
+#     model_points = pd.read_csv("furtheredge/inputs/model_points2.csv")
+#     ri_rates = pd.read_csv(
+#         "furtheredge/inputs/ri_rates.csv", sep=";", decimal=","
+#     )
+#     wop_rates = pd.read_csv(
+#         "furtheredge/inputs/wop_rates.csv", sep=";", decimal=","
+#     )
+#     tech_assumptions = pd.read_csv(
+#         "furtheredge/inputs/tech_assumptions.csv", sep=";", decimal=","
+#     )
+#     product = pd.read_csv(
+#         "furtheredge/inputs/product.csv", sep=";", decimal=","
+#     )
+
+#     # expected = pd.read_csv("furtheredge/outputs/universal_life_output.csv")
+#     # expected["fin_mois"] = pd.to_datetime(expected["fin_mois"])
+
+#     # When
+#     result_universal_life = universal_life_module(
+#         model_points,
+#         {"time_horizon": 50, "projection_date": "2023-10-01"},
+#         tech_assumptions,
+#         ri_rates,
+#         wop_rates,
+#         product,
+#     )
 
-
-def universal_life():
-    package_dir = pkg_resources.resource_filename("furtheredge", "")
-
-    model_points_path = package_dir + "/inputs/model_points2.csv"
-    ri_rates_path = package_dir + "/inputs/ri_rates.csv"
-    wop_rates_path = package_dir + "/inputs/wop_rates.csv"
-    tech_assumptions_path = package_dir + "/inputs/tech_assumptions.csv"
-    product_path = package_dir + "/inputs/product.csv"
-
-    model_points = pd.read_csv(model_points_path)
-    ri_rates = pd.read_csv(ri_rates_path, sep=";", decimal=",")
-    wop_rates = pd.read_csv(wop_rates_path, sep=";", decimal=",")
-    tech_assumptions = pd.read_csv(tech_assumptions_path, sep=";", decimal=",")
-    product = pd.read_csv(product_path, sep=";", decimal=",")
-
-    # print(f"Model points length: {len(model_points)}")
-    result_universal_life = universal_life_module(
-        model_points,
-        {"time_horizon": 50, "projection_date": "2023-10-31"},
-        tech_assumptions,
-        ri_rates,
-        wop_rates,
-        product,
-    )
-    # print(result_universal_life[result_universal_life["MP_ID"] == 169])
-    return result_universal_life
-
-
-# result_universal_life = universal_life()
-# result_universal_life.to_csv(
-#     "furtheredge/outputs/universal_life_output.csv", index=False
-# )
+#     # Then
+#     # assert_frame_equal(result_universal_life, expected)
```

### Comparing `furtheredge-0.1.1/furtheredge.egg-info/SOURCES.txt` & `furtheredge-0.1.2/furtheredge.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,44 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 furtheredge/__init__.py
+furtheredge/abstracted_packages.py
 furtheredge/universal_life_module.py
 furtheredge.egg-info/PKG-INFO
 furtheredge.egg-info/SOURCES.txt
 furtheredge.egg-info/dependency_links.txt
 furtheredge.egg-info/requires.txt
 furtheredge.egg-info/top_level.txt
 furtheredge/inputs/__init__.py
 furtheredge/inputs/model_points2.csv
 furtheredge/inputs/product.csv
 furtheredge/inputs/ri_rates.csv
 furtheredge/inputs/tech_assumptions.csv
 furtheredge/inputs/wop_rates.csv
 furtheredge/modules/__init__.py
+furtheredge/modules/validator_dfs.py
+furtheredge/modules/model_point_generator/__init__.py
+furtheredge/modules/model_point_generator/model_point_generator.py
+furtheredge/modules/model_point_generator/policies_refinement.py
+furtheredge/modules/model_point_generator/policy_refinement.py
 furtheredge/modules/universal_life/__init__.py
+furtheredge/modules/universal_life/merge_all_df.py
+furtheredge/modules/universal_life/required_data_calculation.py
 furtheredge/modules/universal_life/run.py
 furtheredge/modules/universal_life/tools.py
 furtheredge/modules/universal_life/sub_modules/__init__.py
 furtheredge/modules/universal_life/sub_modules/duration.py
 furtheredge/modules/universal_life/sub_modules/proba.py
 furtheredge/modules/universal_life/sub_modules/prospective.py
 furtheredge/modules/universal_life/sub_modules/reserve.py
+furtheredge/modules/universal_life/sub_modules_engines/__init__.py
+furtheredge/modules/universal_life/sub_modules_engines/duration_calculated_variables.py
+furtheredge/modules/universal_life/sub_modules_engines/proba_calculated_variables.py
+furtheredge/modules/universal_life/sub_modules_engines/prospective_calculated_variables.py
+furtheredge/modules/universal_life/sub_modules_engines/reserve_calculated_variables.py
 tests/__init__.py
 tests/universal_life/__init__.py
 tests/universal_life/universal_life_module_test.py
 tests/universal_life/sub_modules/__init__.py
 tests/universal_life/sub_modules/duration_test.py
```

### Comparing `furtheredge-0.1.1/setup.py` & `furtheredge-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setup(
     name="furtheredge",
-    version="0.1.1",
+    version="0.1.2",
     description="""furtheredge-modules""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Novacture",
     author_email="amine.zemni@novacture.com",
     packages=find_packages(),
     classifiers=[
```

### Comparing `furtheredge-0.1.1/tests/universal_life/sub_modules/duration_test.py` & `furtheredge-0.1.2/tests/universal_life/sub_modules/duration_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-import pandas as pd
-from pandas.testing import assert_frame_equal
+# from furtheredge.abstracted_packages import furtheredge_pandas as pd
+# from pandas.testing import assert_frame_equal
 
-from furtheredge.modules.universal_life.run import initialize_output_dataframe
-from furtheredge.modules.universal_life.sub_modules.duration import (
-    duration_calculation,
-)
-
-
-def should_return_duration_calculation():
-    # Given
-    model_points = pd.read_csv("furtheredge/inputs/model_points2.csv")
-    ri_rates = pd.read_csv(
-        "furtheredge/inputs/ri_rates.csv", sep=";", decimal=","
-    )
-    wop_rates = pd.read_csv(
-        "furtheredge/inputs/wop_rates.csv", sep=";", decimal=","
-    )
-    tech_assumptions = pd.read_csv(
-        "furtheredge/inputs/tech_assumptions.csv", sep=";", decimal=","
-    )
-    product = pd.read_csv(
-        "furtheredge/inputs/product.csv", sep=";", decimal=","
-    )
-
-    expected = pd.read_csv(
-        "furtheredge/outputs/universal_life_duration_output.csv"
-    )
-    expected["fin_mois"] = pd.to_datetime(expected["fin_mois"])
-
-    run_settings = {"time_horizon": 50, "projection_date": "2023-10-01"}
-    output = initialize_output_dataframe(
-        len(model_points),
-        run_settings["time_horizon"],
-        run_settings["projection_date"],
-    )
-
-    # When
-    duration_result = duration_calculation(
-        model_points, output, tech_assumptions, ri_rates, wop_rates, product
-    )
+# from furtheredge.modules.universal_life.run import initialize_output_dataframe
+# from furtheredge.modules.universal_life.sub_modules.duration import (
+#     duration_calculation,
+# )
+
+
+# def should_return_duration_calculation():
+#     # Given
+#     model_points = pd.read_csv("furtheredge/inputs/model_points2.csv")
+#     ri_rates = pd.read_csv(
+#         "furtheredge/inputs/ri_rates.csv", sep=";", decimal=","
+#     )
+#     wop_rates = pd.read_csv(
+#         "furtheredge/inputs/wop_rates.csv", sep=";", decimal=","
+#     )
+#     tech_assumptions = pd.read_csv(
+#         "furtheredge/inputs/tech_assumptions.csv", sep=";", decimal=","
+#     )
+#     product = pd.read_csv(
+#         "furtheredge/inputs/product.csv", sep=";", decimal=","
+#     )
+
+#     expected = pd.read_csv(
+#         "furtheredge/outputs/universal_life_duration_output.csv"
+#     )
+#     expected["fin_mois"] = pd.to_datetime(expected["fin_mois"])
+
+#     run_settings = {"time_horizon": 50, "projection_date": "2023-10-01"}
+#     output = initialize_output_dataframe(
+#         len(model_points),
+#         run_settings["time_horizon"],
+#         run_settings["projection_date"],
+#     )
+
+#     # When
+#     duration_result = duration_calculation(
+#         model_points, output, tech_assumptions, ri_rates, wop_rates, product
+#     )
 
-    # Then
-    # assert_frame_equal(duration_result, expected)
+#     # Then
+#     # assert_frame_equal(duration_result, expected)
```

