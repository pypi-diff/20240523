# Comparing `tmp/Algebra_with_SymPy-1.0.1.dev1.tar.gz` & `tmp/algebra_with_sympy-1.0.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Algebra_with_SymPy-1.0.1.dev1.tar", last modified: Sun Jan  7 22:23:35 2024, max compression
+gzip compressed data, was "algebra_with_sympy-1.0.1rc0.tar", last modified: Wed May 22 19:49:11 2024, max compression
```

## Comparing `Algebra_with_SymPy-1.0.1.dev1.tar` & `algebra_with_sympy-1.0.1rc0.tar`

### file list

```diff
@@ -1,23 +1,21 @@
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2024-01-07 22:23:35.474583 Algebra_with_SymPy-1.0.1.dev1/
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2024-01-07 22:23:35.474583 Algebra_with_SymPy-1.0.1.dev1/Algebra_with_SymPy.egg-info/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       92 2021-02-12 03:15:32.000000 Algebra_with_SymPy-1.0.1.dev1/Algebra_with_SymPy.egg-info/.~lock.In process discussion comment.odt#
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    13120 2021-02-12 03:15:32.000000 Algebra_with_SymPy-1.0.1.dev1/Algebra_with_SymPy.egg-info/In process discussion comment.odt
--rw-r--r--   0 jonathan  (1001) jonathan  (1001)    13621 2024-01-07 22:23:35.000000 Algebra_with_SymPy-1.0.1.dev1/Algebra_with_SymPy.egg-info/PKG-INFO
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      624 2024-01-07 22:23:35.000000 Algebra_with_SymPy-1.0.1.dev1/Algebra_with_SymPy.egg-info/SOURCES.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)        1 2024-01-07 22:23:35.000000 Algebra_with_SymPy-1.0.1.dev1/Algebra_with_SymPy.egg-info/dependency_links.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       55 2024-01-07 22:23:35.000000 Algebra_with_SymPy-1.0.1.dev1/Algebra_with_SymPy.egg-info/requires.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       25 2024-01-07 22:23:35.000000 Algebra_with_SymPy-1.0.1.dev1/Algebra_with_SymPy.egg-info/top_level.txt
--rw-r--r--   0 jonathan  (1001) jonathan  (1001)    13621 2024-01-07 22:23:35.474583 Algebra_with_SymPy-1.0.1.dev1/PKG-INFO
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2024-01-07 22:23:35.474583 Algebra_with_SymPy-1.0.1.dev1/algebra_with_sympy/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      963 2023-12-27 21:13:39.000000 Algebra_with_SymPy-1.0.1.dev1/algebra_with_sympy/__init__.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    26765 2024-01-06 19:39:35.000000 Algebra_with_SymPy-1.0.1.dev1/algebra_with_sympy/algebraic_equation.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     3982 2024-01-02 21:50:47.000000 Algebra_with_SymPy-1.0.1.dev1/algebra_with_sympy/preparser.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       26 2024-01-07 22:23:35.000000 Algebra_with_SymPy-1.0.1.dev1/algebra_with_sympy/version.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       38 2024-01-07 22:23:35.474583 Algebra_with_SymPy-1.0.1.dev1/setup.cfg
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1364 2024-01-02 15:48:31.000000 Algebra_with_SymPy-1.0.1.dev1/setup.py
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2024-01-07 22:23:35.474583 Algebra_with_SymPy-1.0.1.dev1/tests/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)        0 2022-04-03 01:35:16.000000 Algebra_with_SymPy-1.0.1.dev1/tests/__init__.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    15372 2024-01-02 15:37:03.000000 Algebra_with_SymPy-1.0.1.dev1/tests/test_algebraic_equation.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     4637 2023-12-30 02:55:58.000000 Algebra_with_SymPy-1.0.1.dev1/tests/test_extension_of_sympy_functions.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1492 2023-07-12 20:13:36.000000 Algebra_with_SymPy-1.0.1.dev1/tests/test_numerics.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     2433 2024-01-02 22:01:52.000000 Algebra_with_SymPy-1.0.1.dev1/tests/test_preparser.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-05-22 19:49:11.396370 algebra_with_sympy-1.0.1rc0/
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-05-22 19:49:11.392370 algebra_with_sympy-1.0.1rc0/Algebra_with_SymPy.egg-info/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)    14733 2024-05-22 19:49:11.000000 algebra_with_sympy-1.0.1rc0/Algebra_with_SymPy.egg-info/PKG-INFO
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      492 2024-05-22 19:49:11.000000 algebra_with_sympy-1.0.1rc0/Algebra_with_SymPy.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        1 2024-05-22 19:49:11.000000 algebra_with_sympy-1.0.1rc0/Algebra_with_SymPy.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       55 2024-05-22 19:49:11.000000 algebra_with_sympy-1.0.1rc0/Algebra_with_SymPy.egg-info/requires.txt
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       25 2024-05-22 19:49:11.000000 algebra_with_sympy-1.0.1rc0/Algebra_with_SymPy.egg-info/top_level.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)    14733 2024-05-22 19:49:11.392370 algebra_with_sympy-1.0.1rc0/PKG-INFO
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-05-22 19:49:11.392370 algebra_with_sympy-1.0.1rc0/algebra_with_sympy/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      963 2023-12-27 21:13:39.000000 algebra_with_sympy-1.0.1rc0/algebra_with_sympy/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    27787 2024-05-22 17:57:26.000000 algebra_with_sympy-1.0.1rc0/algebra_with_sympy/algebraic_equation.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3982 2024-01-02 21:50:47.000000 algebra_with_sympy-1.0.1rc0/algebra_with_sympy/preparser.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       25 2024-05-22 19:49:11.000000 algebra_with_sympy-1.0.1rc0/algebra_with_sympy/version.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       38 2024-05-22 19:49:11.396370 algebra_with_sympy-1.0.1rc0/setup.cfg
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1364 2024-01-02 15:48:31.000000 algebra_with_sympy-1.0.1rc0/setup.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-05-22 19:49:11.392370 algebra_with_sympy-1.0.1rc0/tests/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        0 2022-04-03 01:35:16.000000 algebra_with_sympy-1.0.1rc0/tests/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    16194 2024-05-22 01:10:16.000000 algebra_with_sympy-1.0.1rc0/tests/test_algebraic_equation.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4637 2023-12-30 02:55:58.000000 algebra_with_sympy-1.0.1rc0/tests/test_extension_of_sympy_functions.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1492 2023-07-12 20:13:36.000000 algebra_with_sympy-1.0.1rc0/tests/test_numerics.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2433 2024-01-02 22:01:52.000000 algebra_with_sympy-1.0.1rc0/tests/test_preparser.py
```

### Comparing `Algebra_with_SymPy-1.0.1.dev1/Algebra_with_SymPy.egg-info/PKG-INFO` & `algebra_with_sympy-1.0.1rc0/Algebra_with_SymPy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Algebra_with_SymPy
-Version: 1.0.1.dev1
+Version: 1.0.1rc0
 Summary: Equations that can be algebraicly manipulated.
 Home-page: https://gutow.github.io/Algebra_with_Sympy/
 Author: Jonathan Gutow
 Author-email: gutow@uwosh.edu
 License: GPL-3.0+
 Keywords: symbolic algebra,computer algebra,CAS,calculations with units,sympy
 Classifier: Development Status :: 5 - Production/Stable
@@ -133,48 +133,70 @@
   this way will **not** be labeled with the internal name for the equation, 
   independent of the setting of `algwsym_config.output.label`.
 
 * By default **solutions output by `solve()`** are returned as a SymPy 
   `FiniteSet()` to force typesetting of the included solutions. To get Python 
   lists instead you can override this for the whole session by setting
   `algwsym_config.output.solve_to_list = True`. For a one-off, simply 
-  wrap the output of a solve in `list()` (e.g. `list(solve(...))`).
+  wrap the output of a solve in `list()` (e.g. `list(solve(...))`). One 
+  advantage of list mode is that lists can be ordered. When
+  `algwsym_config.output.solve_to_list = True` `solve()` maintains the 
+  solutions in the order the solve for variables were input.
 
 ## Setup/Installation
 
 1. Use pip to install in your python environment: 
 `pip install -U Algebra-with-SymPy`
 2. To use in a running python session issue
 the following command : `from algebra_with_sympy import *`. 
 This will also import the SymPy tools. 
 3. If you want to isolate this tool from the global namespace you are 
    working with change the import statement 
 to `import algebra_with_sympy as spa`, where 
 `spa` stands for "SymPy Algebra". Then all calls would be made to `
-spa.funcname()`.
+spa.funcname()`. WARNING: Doing this makes shorthand equation input and 
+   control of interactive output formats unavailable. To recover this 
+   functionality the following code must be run in the interactive session.
+```
+Equation = spa.Equation
+Eqn = Equation
+algwsym_config = spa.algwsym_config
+```
 
 ## Try in binder
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/gutow/Algebra_with_Sympy.git/master/?filepath=Demonstration%20of%20equation%20class.ipynb)
 
 ## Issues or Comments
 
 * Issues and bug reports should be [filed on 
 github](https://github.com/gutow/Algebra_with_Sympy/issues).
 * Comments, questions, show and tell, etc. should go in the [project 
   discussions](https://github.com/gutow/Algebra_with_Sympy/discussions).
 
 ## Change Log
 
-* 1.0.1.dev0 ()
+* 1.0.1 (May 22, 2024)
+  * BUG FIX: equation labels that include underscore characters "_" are now 
+    accepted.
   * BUG FIX: wrapping equations formatted as LaTex equation (ie. surrounded 
     by `\begin{equation}...\end{equation}`) in the `$..$` code used to 
     indicate markdown for MathJax was causing output errors in Quarto when 
     outputing to .tex or .pdf. This is now fixed without negatively 
     impacting MathJax rendering.
+  * BUG FIX: Singleton results of solve unnecessarily wrapped by extra list 
+    or finiteset. No longer double nested.
+  * BUG FIX: When returning lists make solve respect user order of solutions.
+  * BUG FIX: Equation output threw error when Algebra_with_Sympy was 
+    imported as a submodule. Equation labeling turned off for this type of 
+    import to avoid error.
+  * BUG FIX: Equation labels are now copyable even with the newer MathJax 
+    commonHTML rendering.
+  * Updates to requirements.txt.
+  * Documentation updates.
 * 1.0.0 (January 2, 2024)
   * Added convenience operation `units(...)` which takes a string of space 
     separated symbols to use as units. This simply declares the symbols 
     to be positive, making them behave as units. This does not create units 
     that know about conversions, prefixes or systems of units. This lack 
     is on purpose to provide units that require the user to worry about 
     conversions (ideal in a teaching situation). To get units with built-in
```

### Comparing `Algebra_with_SymPy-1.0.1.dev1/PKG-INFO` & `algebra_with_sympy-1.0.1rc0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Algebra_with_SymPy
-Version: 1.0.1.dev1
+Version: 1.0.1rc0
 Summary: Equations that can be algebraicly manipulated.
 Home-page: https://gutow.github.io/Algebra_with_Sympy/
 Author: Jonathan Gutow
 Author-email: gutow@uwosh.edu
 License: GPL-3.0+
 Keywords: symbolic algebra,computer algebra,CAS,calculations with units,sympy
 Classifier: Development Status :: 5 - Production/Stable
@@ -133,48 +133,70 @@
   this way will **not** be labeled with the internal name for the equation, 
   independent of the setting of `algwsym_config.output.label`.
 
 * By default **solutions output by `solve()`** are returned as a SymPy 
   `FiniteSet()` to force typesetting of the included solutions. To get Python 
   lists instead you can override this for the whole session by setting
   `algwsym_config.output.solve_to_list = True`. For a one-off, simply 
-  wrap the output of a solve in `list()` (e.g. `list(solve(...))`).
+  wrap the output of a solve in `list()` (e.g. `list(solve(...))`). One 
+  advantage of list mode is that lists can be ordered. When
+  `algwsym_config.output.solve_to_list = True` `solve()` maintains the 
+  solutions in the order the solve for variables were input.
 
 ## Setup/Installation
 
 1. Use pip to install in your python environment: 
 `pip install -U Algebra-with-SymPy`
 2. To use in a running python session issue
 the following command : `from algebra_with_sympy import *`. 
 This will also import the SymPy tools. 
 3. If you want to isolate this tool from the global namespace you are 
    working with change the import statement 
 to `import algebra_with_sympy as spa`, where 
 `spa` stands for "SymPy Algebra". Then all calls would be made to `
-spa.funcname()`.
+spa.funcname()`. WARNING: Doing this makes shorthand equation input and 
+   control of interactive output formats unavailable. To recover this 
+   functionality the following code must be run in the interactive session.
+```
+Equation = spa.Equation
+Eqn = Equation
+algwsym_config = spa.algwsym_config
+```
 
 ## Try in binder
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/gutow/Algebra_with_Sympy.git/master/?filepath=Demonstration%20of%20equation%20class.ipynb)
 
 ## Issues or Comments
 
 * Issues and bug reports should be [filed on 
 github](https://github.com/gutow/Algebra_with_Sympy/issues).
 * Comments, questions, show and tell, etc. should go in the [project 
   discussions](https://github.com/gutow/Algebra_with_Sympy/discussions).
 
 ## Change Log
 
-* 1.0.1.dev0 ()
+* 1.0.1 (May 22, 2024)
+  * BUG FIX: equation labels that include underscore characters "_" are now 
+    accepted.
   * BUG FIX: wrapping equations formatted as LaTex equation (ie. surrounded 
     by `\begin{equation}...\end{equation}`) in the `$..$` code used to 
     indicate markdown for MathJax was causing output errors in Quarto when 
     outputing to .tex or .pdf. This is now fixed without negatively 
     impacting MathJax rendering.
+  * BUG FIX: Singleton results of solve unnecessarily wrapped by extra list 
+    or finiteset. No longer double nested.
+  * BUG FIX: When returning lists make solve respect user order of solutions.
+  * BUG FIX: Equation output threw error when Algebra_with_Sympy was 
+    imported as a submodule. Equation labeling turned off for this type of 
+    import to avoid error.
+  * BUG FIX: Equation labels are now copyable even with the newer MathJax 
+    commonHTML rendering.
+  * Updates to requirements.txt.
+  * Documentation updates.
 * 1.0.0 (January 2, 2024)
   * Added convenience operation `units(...)` which takes a string of space 
     separated symbols to use as units. This simply declares the symbols 
     to be positive, making them behave as units. This does not create units 
     that know about conversions, prefixes or systems of units. This lack 
     is on purpose to provide units that require the user to worry about 
     conversions (ideal in a teaching situation). To get units with built-in
```

### Comparing `Algebra_with_SymPy-1.0.1.dev1/algebra_with_sympy/__init__.py` & `algebra_with_sympy-1.0.1rc0/algebra_with_sympy/__init__.py`

 * *Files identical despite different names*

### Comparing `Algebra_with_SymPy-1.0.1.dev1/algebra_with_sympy/algebraic_equation.py` & `algebra_with_sympy-1.0.1rc0/algebra_with_sympy/algebraic_equation.py`

 * *Files 3% similar despite different names*

```diff
@@ -353,17 +353,15 @@
             pretty-printing will be wrapped in the formal Latex for an
             equation. For example rather than
             ```
             $\\frac{a}{b}=c$
             ```
             the output will be
             ```
-            $$
             \\begin{equation}\\frac{a}{b}=c\\end{equation}
-            $$
             ```
             """
             return self.latex_as_equation
 
     class numerics():
 
         def __init__(self):
@@ -406,18 +404,20 @@
     if latex_as_equations:
         return r'\begin{equation}'+latex(expr)+'\end{equation}'
     else:
         tempstr = ''
         namestr = ''
         if isinstance(expr, Equation):
             namestr = expr._get_eqn_name()
-        if namestr != '' and algwsym_config.output.label:
-            tempstr += r'\,\,\,\,\,\,\,\,\,\,'
-            tempstr += r'(\text{' + namestr + '})'
-        return r'$'+latex(expr) + tempstr + '$'
+        if namestr != '' and algwsym_config and algwsym_config.output.label:
+            tempstr += r'$'+latex(expr)
+            tempstr += r'\,\,\,\,\,\,\,\,\,\,$(' + namestr + ')'
+            return tempstr
+        else:
+            return '$'+latex(expr) + '$'
 
 def __command_line_printing__(expr, *arg):
     # print('Entering __command_line_printing__')
     human_text = True
     show_code = False
     if algwsym_config:
         human_text = algwsym_config.output.human_text
@@ -514,18 +514,22 @@
 if ip and "text/latex" not in formatter.active_types:
     old = formatter.formatters['text/plain'].for_type(Eqn,
                                                 __command_line_printing__)
     # print("For type Equation overriding plain text formatter = " + str(old))
 
 def units(names):
     """
-    This operation declares the symbols to be positive values, so that sympy will handle them properly
-    when simplifying expressions containing units.
+    This operation declares the symbols to be positive values, so that sympy
+    will handle them properly when simplifying expressions containing units.
+    Units defined this way are just unit symbols. If you want units that are
+    aware of conversions see sympy.physics.units.
+
 
-    :param string names: a string containing a space separated list of symbols to be treated as units.
+    :param string names: a string containing a space separated list of
+    symbols to be treated as units.
 
     :return string list of defined units: calls `name = symbols(name,
     positive=True)` in the interactive namespace for each symbol name.
     """
     from sympy.core.symbol import symbols
     #import __main__ as shell
     from IPython import get_ipython
@@ -620,36 +624,53 @@
         if isinstance(f, Equation):
             newf.append(f.lhs - f.rhs)
             contains_eqn = True
         else:
             newf.append(f)
     flags['dict'] = True
     result = solve(newf, *symbols, **flags)
+    if len(symbols) == 1 and hasattr(symbols[0], "__iter__"):
+        symbols = symbols[0]
     if contains_eqn:
         if len(result[0]) == 1:
             for k in result:
                 for key in k.keys():
                     val = k[key]
                     tempeqn = Eqn(key, val)
                     solns.append(tempeqn)
+            if len(solns) == len(symbols):
+                # sort according to the user-provided symbols
+                solns = sorted(solns, key=lambda x: symbols.index(x.lhs))
         else:
             for k in result:
                 solnset = []
                 for key in k.keys():
                     val = k[key]
                     tempeqn = Eqn(key, val)
                     solnset.append(tempeqn)
                 if not algwsym_config.output.solve_to_list:
                     solnset = FiniteSet(*solnset)
+                else:
+                    if len(solnset) == len(symbols):
+                        # sort according to the user-provided symbols
+                        solnset = sorted(solnset, key=lambda x: symbols.index(x.lhs))
                 solns.append(solnset)
     else:
         solns = result
     if algwsym_config.output.solve_to_list:
-        return list(solns)
+        if len(solns) == 1 and hasattr(solns[0], "__iter__"):
+            # no need to wrap a list of a single element inside another list
+            return solns[0]
+        return solns
     else:
+        if len(solns) == 1:
+            # do not wrap a singleton in FiniteSet if it already is
+            for k in solns:
+                if isinstance(k, FiniteSet):
+                    return k
         return FiniteSet(*solns)
 
 def solveset(f, symbols, domain=sympy.Complexes):
     """
     Very experimental override of sympy solveset, which we hope will replace
     solve. Much is not working. It is not clear how to input a system of
     equations unless you directly select `linsolve`, etc...
```

### Comparing `Algebra_with_SymPy-1.0.1.dev1/algebra_with_sympy/preparser.py` & `algebra_with_sympy-1.0.1rc0/algebra_with_sympy/preparser.py`

 * *Files identical despite different names*

### Comparing `Algebra_with_SymPy-1.0.1.dev1/setup.py` & `algebra_with_sympy-1.0.1rc0/setup.py`

 * *Files identical despite different names*

### Comparing `Algebra_with_SymPy-1.0.1.dev1/tests/test_algebraic_equation.py` & `algebra_with_sympy-1.0.1rc0/tests/test_algebraic_equation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sympy import symbols, integrate, simplify, expand, factor, Integral, Add
 from sympy import diff, FiniteSet, Equation, Function, Matrix, S, Eq
-from sympy import sin, cos, log, exp, latex, Symbol, I
+from sympy import sin, cos, log, exp, latex, Symbol, I, pi
 from sympy.core.function import AppliedUndef
 from sympy.printing.latex import LatexPrinter
 from algebra_with_sympy.algebraic_equation import solve, collect
 from algebra_with_sympy.algebraic_equation import Equality, units
 from sympy import Eqn, sqrt, root, Heaviside
 from algebra_with_sympy.algebraic_equation import algwsym_config
 
@@ -114,15 +114,15 @@
     __command_line_printing__(tsteqn)
     captured = capsys.readouterr()
     assert captured.out == 'a = b/c          (tsteqn)\n'
     # make sure sys.displayhook does not point to __command_line_printing__()
     import sys
     sys.displayhook = sys.__displayhook__
     assert __latex_override__(tsteqn) == ('$a=\\frac{b}{c}\\,\\,\\,\\,\\,\\,'
-                                          '\\,\\,\\,\\,(\\text{tsteqn})$')
+                                          '\\,\\,\\,\\,$(tsteqn)')
     algwsym_config.output.label = False
     __command_line_printing__(tsteqn)
     captured = capsys.readouterr()
     assert captured.out == 'a = b/c\n'
     assert __latex_override__(tsteqn) == '$a=\\frac{b}{c}$'
     algwsym_config.output.label = True
 
@@ -272,14 +272,33 @@
                                    Equation(y, 1)), FiniteSet(Equation(x, 3),
                                    Equation(y, -3)))
     algwsym_config.output.solve_to_list = True
     assert solve([eq1,eq2], x, y) == [[Equation(x, -3), Equation(y, 3)],
                                       [Equation(x, -1), Equation(y, -1)],
                                       [Equation(x, 1), Equation(y, 1)],
                                       [Equation(x, 3), Equation(y, -3)]]
+    
+    xi, wn = symbols("xi omega_n", real=True, positive=True)
+    Tp, Ts = symbols("T_p, T_s", real=True, positive=True)
+    e1 = Eqn(Tp, pi / (wn*sqrt(1 - xi**2)))
+    e2 = Eqn(Ts, 4 / (wn*xi))
+    algwsym_config.output.solve_to_list = False
+    assert solve([e1, e2], [xi, wn]) == FiniteSet(
+        Eqn(xi, 4*Tp/sqrt(16*Tp**2 + pi**2*Ts**2)),
+        Eqn(wn, sqrt(16*Tp**2 + pi**2*Ts**2)/(Tp*Ts)))
+    algwsym_config.output.solve_to_list = True
+    assert solve([e1, e2], [xi, wn]) == [
+        Eqn(xi, 4*Tp/sqrt(16*Tp**2 + pi**2*Ts**2)),
+        Eqn(wn, sqrt(16*Tp**2 + pi**2*Ts**2)/(Tp*Ts))
+    ]
+    # order of symbols are swapped -> results are swapped as well
+    assert solve([e1, e2], [wn, xi]) == [
+        Eqn(wn, sqrt(16*Tp**2 + pi**2*Ts**2)/(Tp*Ts)),
+        Eqn(xi, 4*Tp/sqrt(16*Tp**2 + pi**2*Ts**2))
+    ]
 
 def test_Heaviside():
     a, b, c, x = symbols('a b c x')
     tsteqn = Equation(a, b / c)
     assert (Heaviside(tsteqn) ==
             Equation(Heaviside(tsteqn.lhs), Heaviside(tsteqn.rhs)))
     assert Heaviside(0) == S(1)/S(2)
```

### Comparing `Algebra_with_SymPy-1.0.1.dev1/tests/test_extension_of_sympy_functions.py` & `algebra_with_sympy-1.0.1rc0/tests/test_extension_of_sympy_functions.py`

 * *Files identical despite different names*

### Comparing `Algebra_with_SymPy-1.0.1.dev1/tests/test_numerics.py` & `algebra_with_sympy-1.0.1rc0/tests/test_numerics.py`

 * *Files identical despite different names*

### Comparing `Algebra_with_SymPy-1.0.1.dev1/tests/test_preparser.py` & `algebra_with_sympy-1.0.1rc0/tests/test_preparser.py`

 * *Files identical despite different names*

