# Comparing `tmp/better_hydroponics-0.1.0.tar.gz` & `tmp/better_hydroponics-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better_hydroponics-0.1.0.tar", last modified: Wed May 22 11:00:51 2024, max compression
+gzip compressed data, was "better_hydroponics-0.1.1.tar", last modified: Thu May 23 14:16:46 2024, max compression
```

## Comparing `better_hydroponics-0.1.0.tar` & `better_hydroponics-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 11:00:51.071353 better_hydroponics-0.1.0/
--rw-rw-rw-   0        0        0     1114 2024-05-19 15:56:16.000000 better_hydroponics-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     8302 2024-05-22 11:00:51.071353 better_hydroponics-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5398 2024-05-22 10:43:34.000000 better_hydroponics-0.1.0/README.md
--rw-rw-rw-   0        0        0     1780 2024-05-22 11:00:40.000000 better_hydroponics-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-22 11:00:51.071353 better_hydroponics-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-22 11:00:51.023899 better_hydroponics-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-22 11:00:51.071353 better_hydroponics-0.1.0/src/better_hydroponics.egg-info/
--rw-rw-rw-   0        0        0     8302 2024-05-22 11:00:50.000000 better_hydroponics-0.1.0/src/better_hydroponics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      562 2024-05-22 11:00:51.000000 better_hydroponics-0.1.0/src/better_hydroponics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 11:00:50.000000 better_hydroponics-0.1.0/src/better_hydroponics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      169 2024-05-22 11:00:50.000000 better_hydroponics-0.1.0/src/better_hydroponics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-22 11:00:50.000000 better_hydroponics-0.1.0/src/better_hydroponics.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-22 11:00:51.055644 better_hydroponics-0.1.0/src/hydroponics/
--rw-rw-rw-   0        0        0    19816 2024-05-22 09:59:14.000000 better_hydroponics-0.1.0/src/hydroponics/Basic_functions.py
--rw-rw-rw-   0        0        0    10398 2024-05-21 13:35:22.000000 better_hydroponics-0.1.0/src/hydroponics/Generate_Report.py
--rw-rw-rw-   0        0        0    16029 2024-05-22 09:59:14.000000 better_hydroponics-0.1.0/src/hydroponics/PH_Approximation_0.py
--rw-rw-rw-   0        0        0     2132 2024-05-22 09:59:14.000000 better_hydroponics-0.1.0/src/hydroponics/Refill_0.py
--rw-rw-rw-   0        0        0    11885 2024-05-21 13:35:22.000000 better_hydroponics-0.1.0/src/hydroponics/Solutions_Solubility.py
--rw-rw-rw-   0        0        0      229 2024-05-22 09:59:14.000000 better_hydroponics-0.1.0/src/hydroponics/__init__.py
--rw-rw-rw-   0        0        0     5643 2024-05-22 09:59:14.000000 better_hydroponics-0.1.0/src/hydroponics/pH_graph_0.py
-drwxrwxrwx   0        0        0        0 2024-05-22 11:00:51.055644 better_hydroponics-0.1.0/tests/
--rw-rw-rw-   0        0        0     6771 2024-05-22 09:59:14.000000 better_hydroponics-0.1.0/tests/test_Basic_functions_pH.py
--rw-rw-rw-   0        0        0     4794 2024-05-22 09:59:14.000000 better_hydroponics-0.1.0/tests/test_Solution_Solubility.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:16:46.747772 better_hydroponics-0.1.1/
+-rw-rw-rw-   0        0        0     1114 2024-05-19 15:56:16.000000 better_hydroponics-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0       49 2024-05-23 13:33:00.000000 better_hydroponics-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     8306 2024-05-23 14:16:46.747772 better_hydroponics-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5402 2024-05-23 14:15:41.000000 better_hydroponics-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 14:16:46.731961 better_hydroponics-0.1.1/data/
+-rw-rw-rw-   0        0        0       38 2024-05-19 15:56:16.000000 better_hydroponics-0.1.1/data/README.md
+-rw-rw-rw-   0        0        0    22994 2024-05-20 12:58:13.000000 better_hydroponics-0.1.1/data/Solubility_data.csv
+-rw-rw-rw-   0        0        0    16854 2024-05-20 13:36:18.000000 better_hydroponics-0.1.1/data/UserData.xlsx
+-rw-rw-rw-   0        0        0     1304 2024-05-20 12:58:13.000000 better_hydroponics-0.1.1/data/molar_mass.csv
+-rw-rw-rw-   0        0        0     1888 2024-05-23 14:14:32.000000 better_hydroponics-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-23 14:16:46.747772 better_hydroponics-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-23 14:16:46.700658 better_hydroponics-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-23 14:16:46.747772 better_hydroponics-0.1.1/src/better_hydroponics.egg-info/
+-rw-rw-rw-   0        0        0     8306 2024-05-23 14:16:46.000000 better_hydroponics-0.1.1/src/better_hydroponics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      741 2024-05-23 14:16:46.000000 better_hydroponics-0.1.1/src/better_hydroponics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 14:16:46.000000 better_hydroponics-0.1.1/src/better_hydroponics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      169 2024-05-23 14:16:46.000000 better_hydroponics-0.1.1/src/better_hydroponics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-23 14:16:46.000000 better_hydroponics-0.1.1/src/better_hydroponics.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 14:16:46.731961 better_hydroponics-0.1.1/src/hydroponics/
+-rw-rw-rw-   0        0        0    19816 2024-05-22 09:59:14.000000 better_hydroponics-0.1.1/src/hydroponics/Basic_functions.py
+-rw-rw-rw-   0        0        0    10398 2024-05-21 13:35:22.000000 better_hydroponics-0.1.1/src/hydroponics/Generate_Report.py
+-rw-rw-rw-   0        0        0    15980 2024-05-23 13:39:06.000000 better_hydroponics-0.1.1/src/hydroponics/PH_Approximation_0.py
+-rw-rw-rw-   0        0        0     2132 2024-05-22 09:59:14.000000 better_hydroponics-0.1.1/src/hydroponics/Refill_0.py
+-rw-rw-rw-   0        0        0    11885 2024-05-21 13:35:22.000000 better_hydroponics-0.1.1/src/hydroponics/Solutions_Solubility.py
+-rw-rw-rw-   0        0        0      229 2024-05-22 09:59:14.000000 better_hydroponics-0.1.1/src/hydroponics/__init__.py
+-rw-rw-rw-   0        0        0     5643 2024-05-22 09:59:14.000000 better_hydroponics-0.1.1/src/hydroponics/pH_graph_0.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:16:46.731961 better_hydroponics-0.1.1/tests/
+-rw-rw-rw-   0        0        0     6771 2024-05-22 09:59:14.000000 better_hydroponics-0.1.1/tests/test_Basic_functions_pH.py
+-rw-rw-rw-   0        0        0     4794 2024-05-22 09:59:14.000000 better_hydroponics-0.1.1/tests/test_Solution_Solubility.py
```

### Comparing `better_hydroponics-0.1.0/LICENSE` & `better_hydroponics-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `better_hydroponics-0.1.0/PKG-INFO` & `better_hydroponics-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: better_hydroponics
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simulation of hydroponic farming
 Author-email: Nils Theeten <nils.theeten@epfl.ch>, Mathieu Penn <mathieu.penn@epfl.ch>
 License: MIT License
         
         Copyright (c) 2024 by Nils Theeten <nils.theeten@epfl.ch>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -108,15 +108,15 @@
 ## 1. Installation 👩‍💻
 
  > Everything is just one pip install away - philippe schwaller
 <br>
 
 The following *pip command* can be used to install the python package. The package was made with python 3.10
 ```
-pip -m install better_hydroponics
+pip install better-hydroponics==0.1.1
 ```
   
 Be aware, the package uses the following dependencies:
  * Numpy (1.26.4)
  * Pandas (2.2.2)
  * matplotlib (3.8.4)
  * sympy (1.12)
```

### Comparing `better_hydroponics-0.1.0/README.md` & `better_hydroponics-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 ## 1. Installation 👩‍💻
 
  > Everything is just one pip install away - philippe schwaller
 <br>
 
 The following *pip command* can be used to install the python package. The package was made with python 3.10
 ```
-pip -m install better_hydroponics
+pip install better-hydroponics==0.1.1
 ```
   
 Be aware, the package uses the following dependencies:
  * Numpy (1.26.4)
  * Pandas (2.2.2)
  * matplotlib (3.8.4)
  * sympy (1.12)
```

### Comparing `better_hydroponics-0.1.0/pyproject.toml` & `better_hydroponics-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system] 
-requires = ["setuptools>=42", "wheel"]
+requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
-version = "0.1.0"
+version = "0.1.1"
 name = "better_hydroponics"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 description = "Simulation of hydroponic farming"
 dependencies = [
     "numpy","sympy","reportlab","pandas","matplotlib","openpyxl","ipython"
@@ -34,14 +34,21 @@
         "pH calculation",
         "solution solubility",
         "plant simulation",
         "solution maker"
 
 ]
 
+[tools.setuptools.packages.find]
+
+
+[tool.setuptools.package-data]
+hydroponics = ["../../data/*"]
+
+
 
 [project.urls]
 source = "https://github.com/NilsTheeten/hydroponics"
 tracker = "https://github.com/NilsTheeten/hydroponics/issues"
 
 [project.optional-dependencies]
 test = [
```

### Comparing `better_hydroponics-0.1.0/src/better_hydroponics.egg-info/PKG-INFO` & `better_hydroponics-0.1.1/src/better_hydroponics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: better_hydroponics
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simulation of hydroponic farming
 Author-email: Nils Theeten <nils.theeten@epfl.ch>, Mathieu Penn <mathieu.penn@epfl.ch>
 License: MIT License
         
         Copyright (c) 2024 by Nils Theeten <nils.theeten@epfl.ch>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -108,15 +108,15 @@
 ## 1. Installation 👩‍💻
 
  > Everything is just one pip install away - philippe schwaller
 <br>
 
 The following *pip command* can be used to install the python package. The package was made with python 3.10
 ```
-pip -m install better_hydroponics
+pip install better-hydroponics==0.1.1
 ```
   
 Be aware, the package uses the following dependencies:
  * Numpy (1.26.4)
  * Pandas (2.2.2)
  * matplotlib (3.8.4)
  * sympy (1.12)
```

### Comparing `better_hydroponics-0.1.0/src/better_hydroponics.egg-info/SOURCES.txt` & `better_hydroponics-0.1.1/src/better_hydroponics.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 src/better_hydroponics.egg-info/PKG-INFO
 src/better_hydroponics.egg-info/SOURCES.txt
 src/better_hydroponics.egg-info/dependency_links.txt
 src/better_hydroponics.egg-info/requires.txt
 src/better_hydroponics.egg-info/top_level.txt
 src/hydroponics/Basic_functions.py
 src/hydroponics/Generate_Report.py
 src/hydroponics/PH_Approximation_0.py
 src/hydroponics/Refill_0.py
 src/hydroponics/Solutions_Solubility.py
 src/hydroponics/__init__.py
 src/hydroponics/pH_graph_0.py
+src/hydroponics/../../data/README.md
+src/hydroponics/../../data/Solubility_data.csv
+src/hydroponics/../../data/UserData.xlsx
+src/hydroponics/../../data/molar_mass.csv
 tests/test_Basic_functions_pH.py
 tests/test_Solution_Solubility.py
```

### Comparing `better_hydroponics-0.1.0/src/hydroponics/Basic_functions.py` & `better_hydroponics-0.1.1/src/hydroponics/Basic_functions.py`

 * *Files identical despite different names*

### Comparing `better_hydroponics-0.1.0/src/hydroponics/Generate_Report.py` & `better_hydroponics-0.1.1/src/hydroponics/Generate_Report.py`

 * *Files identical despite different names*

### Comparing `better_hydroponics-0.1.0/src/hydroponics/PH_Approximation_0.py` & `better_hydroponics-0.1.1/src/hydroponics/PH_Approximation_0.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             The Ksp constant has an impact on the concentration of OH^-1 which in itself impact the pH of the solution.
             """
             if compound in Ksp_values:
                 #Defines variables for the concentrations of the metal in a dissociated state or not, i.e, Ca(OH)^2- or Ca^2+
                 exec(f"dissociated_metal_{l}_concentration]=symbols(dissociated_metal_{l}_concentration)")
                 exec(f"undissociated_metal_compound_{l}_concentration=symbols(undissociated_metal_compound_{l}_concentration)")
                 #Equation of dissociation equilibrium
-                exec(f"equation_Ksp = Eq((dissociated_metal_compound_{l}_concentration*OH_minus_concentration**(compound_charge[compound]))/(undissociated_metal_compound_{l}_concentration), Ksp_values[compound])")
+                exec(f"equation_Ksp = Eq((dissociated_metal_compound_{l}_concentration*OH_minus_concentration**(compound_charge[compound])), Ksp_values[compound])")
                 equations.append(equation_Ksp)
                 # Accumulating variables for charge balance. 
                 accumulated_variables_for_charge_balance.append(compound_charge[compound]*f'dissociated_metal_{l}_concentration')
                 #Mass equation of metal/metal compound
                 exec(f"mass_balance_metal = Eq(dissociated_metal_{l}_concentration + undissociated_metal_{l}_concentration, compound_concentration)")
                 equations.append(mass_balance_metal)
                 exec(f"accumulated_variables_for_final_OH_concentration.append(-compound_charge[compound]*undissociated_metal_compound_{l}_concentration)")
```

### Comparing `better_hydroponics-0.1.0/src/hydroponics/Refill_0.py` & `better_hydroponics-0.1.1/src/hydroponics/Refill_0.py`

 * *Files identical despite different names*

### Comparing `better_hydroponics-0.1.0/src/hydroponics/Solutions_Solubility.py` & `better_hydroponics-0.1.1/src/hydroponics/Solutions_Solubility.py`

 * *Files identical despite different names*

### Comparing `better_hydroponics-0.1.0/src/hydroponics/pH_graph_0.py` & `better_hydroponics-0.1.1/src/hydroponics/pH_graph_0.py`

 * *Files identical despite different names*

### Comparing `better_hydroponics-0.1.0/tests/test_Basic_functions_pH.py` & `better_hydroponics-0.1.1/tests/test_Basic_functions_pH.py`

 * *Files identical despite different names*

### Comparing `better_hydroponics-0.1.0/tests/test_Solution_Solubility.py` & `better_hydroponics-0.1.1/tests/test_Solution_Solubility.py`

 * *Files identical despite different names*

