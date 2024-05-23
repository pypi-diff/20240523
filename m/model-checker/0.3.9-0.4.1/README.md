# Comparing `tmp/model_checker-0.3.9.tar.gz` & `tmp/model_checker-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_checker-0.3.9.tar", last modified: Mon May 20 21:36:04 2024, max compression
+gzip compressed data, was "model_checker-0.4.1.tar", last modified: Thu May 23 21:05:54 2024, max compression
```

## Comparing `model_checker-0.3.9.tar` & `model_checker-0.4.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 21:36:04.365435 model_checker-0.3.9/
--rw-r--r--   0 benjamin  (1000) users      (100)     1064 2024-05-08 20:11:06.000000 model_checker-0.3.9/LICENCE
--rw-r--r--   0 benjamin  (1000) users      (100)     6168 2024-05-20 21:36:04.365435 model_checker-0.3.9/PKG-INFO
--rw-r--r--   0 benjamin  (1000) users      (100)     5437 2024-05-20 20:33:25.000000 model_checker-0.3.9/README.md
--rw-r--r--   0 benjamin  (1000) users      (100)      947 2024-05-20 21:33:49.000000 model_checker-0.3.9/pyproject.toml
--rw-r--r--   0 benjamin  (1000) users      (100)       38 2024-05-20 21:36:04.365435 model_checker-0.3.9/setup.cfg
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 21:36:04.364435 model_checker-0.3.9/src/
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 21:36:04.365435 model_checker-0.3.9/src/model_checker/
--rw-r--r--   0 benjamin  (1000) users      (100)       84 2024-05-20 21:24:07.000000 model_checker-0.3.9/src/model_checker/__init__.py
--rw-r--r--   0 benjamin  (1000) users      (100)    10264 2024-05-20 21:33:49.000000 model_checker-0.3.9/src/model_checker/__main__.py
--rw-r--r--   0 benjamin  (1000) users      (100)    19988 2024-05-20 20:33:25.000000 model_checker-0.3.9/src/model_checker/model_definitions.py
--rw-r--r--   0 benjamin  (1000) users      (100)    23981 2024-05-20 21:34:33.000000 model_checker-0.3.9/src/model_checker/model_structure.py
--rw-r--r--   0 benjamin  (1000) users      (100)    18152 2024-05-13 15:43:10.000000 model_checker-0.3.9/src/model_checker/semantics.py
--rw-r--r--   0 benjamin  (1000) users      (100)     7686 2024-05-17 23:03:51.000000 model_checker-0.3.9/src/model_checker/syntax.py
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 21:36:04.365435 model_checker-0.3.9/src/model_checker.egg-info/
--rw-r--r--   0 benjamin  (1000) users      (100)     6168 2024-05-20 21:36:04.000000 model_checker-0.3.9/src/model_checker.egg-info/PKG-INFO
--rw-r--r--   0 benjamin  (1000) users      (100)      510 2024-05-20 21:36:04.000000 model_checker-0.3.9/src/model_checker.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin  (1000) users      (100)        1 2024-05-20 21:36:04.000000 model_checker-0.3.9/src/model_checker.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       62 2024-05-20 21:36:04.000000 model_checker-0.3.9/src/model_checker.egg-info/entry_points.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       10 2024-05-20 21:36:04.000000 model_checker-0.3.9/src/model_checker.egg-info/requires.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       14 2024-05-20 21:36:04.000000 model_checker-0.3.9/src/model_checker.egg-info/top_level.txt
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-20 21:36:04.365435 model_checker-0.3.9/test/
--rw-r--r--   0 benjamin  (1000) users      (100)     2985 2024-05-16 20:27:14.000000 model_checker-0.3.9/test/test.py
--rw-r--r--   0 benjamin  (1000) users      (100)      330 2024-05-13 22:46:42.000000 model_checker-0.3.9/test/test_examples.py
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-23 21:05:54.821076 model_checker-0.4.1/
+-rw-r--r--   0 benjamin  (1000) users      (100)     1064 2024-05-08 20:11:06.000000 model_checker-0.4.1/LICENCE
+-rw-r--r--   0 benjamin  (1000) users      (100)     9074 2024-05-23 21:05:54.821076 model_checker-0.4.1/PKG-INFO
+-rw-r--r--   0 benjamin  (1000) users      (100)     8289 2024-05-23 21:03:42.000000 model_checker-0.4.1/README.md
+-rw-r--r--   0 benjamin  (1000) users      (100)     1007 2024-05-23 21:05:51.000000 model_checker-0.4.1/pyproject.toml
+-rw-r--r--   0 benjamin  (1000) users      (100)       38 2024-05-23 21:05:54.821076 model_checker-0.4.1/setup.cfg
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-23 21:05:54.820076 model_checker-0.4.1/src/
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-23 21:05:54.820076 model_checker-0.4.1/src/model_checker/
+-rw-r--r--   0 benjamin  (1000) users      (100)      124 2024-05-23 21:05:51.000000 model_checker-0.4.1/src/model_checker/__init__.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    13625 2024-05-23 17:20:26.000000 model_checker-0.4.1/src/model_checker/__main__.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    21385 2024-05-23 19:00:33.000000 model_checker-0.4.1/src/model_checker/model_definitions.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    26177 2024-05-23 17:40:02.000000 model_checker-0.4.1/src/model_checker/model_structure.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    27951 2024-05-23 18:56:17.000000 model_checker-0.4.1/src/model_checker/semantics.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     7836 2024-05-23 18:38:27.000000 model_checker-0.4.1/src/model_checker/syntax.py
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-23 21:05:54.821076 model_checker-0.4.1/src/model_checker.egg-info/
+-rw-r--r--   0 benjamin  (1000) users      (100)     9074 2024-05-23 21:05:54.000000 model_checker-0.4.1/src/model_checker.egg-info/PKG-INFO
+-rw-r--r--   0 benjamin  (1000) users      (100)      510 2024-05-23 21:05:54.000000 model_checker-0.4.1/src/model_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)        1 2024-05-23 21:05:54.000000 model_checker-0.4.1/src/model_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       62 2024-05-23 21:05:54.000000 model_checker-0.4.1/src/model_checker.egg-info/entry_points.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       10 2024-05-23 21:05:54.000000 model_checker-0.4.1/src/model_checker.egg-info/requires.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       14 2024-05-23 21:05:54.000000 model_checker-0.4.1/src/model_checker.egg-info/top_level.txt
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-23 21:05:54.821076 model_checker-0.4.1/test/
+-rw-r--r--   0 benjamin  (1000) users      (100)     2985 2024-05-23 04:07:12.000000 model_checker-0.4.1/test/test.py
+-rw-r--r--   0 benjamin  (1000) users      (100)      330 2024-05-23 04:07:12.000000 model_checker-0.4.1/test/test_examples.py
```

### Comparing `model_checker-0.3.9/LICENCE` & `model_checker-0.4.1/LICENCE`

 * *Files identical despite different names*

### Comparing `model_checker-0.3.9/PKG-INFO` & `model_checker-0.4.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,84 +1,97 @@
-Metadata-Version: 2.1
-Name: model-checker
-Version: 0.3.9
-Summary: A hyperintensional theorem prover for counterfactual conditionals and modal operators.
-Author-email: Benjamin Brast-McKie <benbrastmckie@gmail.com>, Miguel Buitrago <mbuit82@gmail.com>
-License: MIT
-Project-URL: Homepage, https://github.com/benbrastmckie/ModelChecker
-Project-URL: Issues, https://github.com/benbrastmckie/ModelChecker/issues
-Keywords: semantics,Z3,counterfactuals,model checker,theorem prover,hyperintensionality
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENCE
-Requires-Dist: z3-solver
-
 # Model Checker
 
-This project draws on the [Z3](https://github.com/Z3Prover/z3) theorem prover to provide tooling for proving theorems and finding countermodels for counterfactual conditional and modal claims.
+This project draws on the [Z3](https://github.com/Z3Prover/z3) theorem prover to provide tooling for finding countermodels for claims which include modal, counterfactual conditional, constitutive explanatory, and extensional operators.
+The language currently includes the following operators:
+
+  - `neg` for _negation_
+  - `not` for _exclusion_
+  - `wedge` for _conjunction_
+  - `vee` for _disjunction_
+  - `rightarrow` for _material conditional_
+  - `leftrightarrow` for _material biconditional_
+  - `Box` for _necessity_
+  - `Diamond` for _possibility_
+  - `boxright` for the _must counterfactual conditional_
+  - `circleright` for the _might counterfactual conditional_
+  - `leq` for _ground_
+  - `sqsubseteq` for _essence_
+  - `equiv` for _propositional identity_
 
 Accessible [installation instructions](https://github.com/benbrastmckie/ModelChecker?tab=readme-ov-file#installation) are provided in the GitHub repository.
 
 ## Instructions
 
-To generate a test file run `model-checker` without arguments.
-
+To generate a test file run `model-checker` in the terminal without arguments.
 Alternatively, run `model-checker path/to/test_file.py` if the `test_file.py` already exists.
-
 A number of [examples](https://github.com/benbrastmckie/ModelChecker/blob/master/Examples/examples.py) are provided in the GitHub repository.
 
-Each file must specify a set of `premises` which are treated conjunctively, `conclusions` which are treated disjunctively, and the number `N` of atomic states to include in each model.
-
-Optionally, the user can specify the following settings in each file: 
+Each file may specify a set of `premises` which are treated conjunctively, `conclusions` which are treated disjunctively, and the number `N` of atomic states to include in each model.
+If unspecified, `premises = []`, `conclusions = []`, and `N = 3` will be set by default.
+Optionally, the user can specify whether to print the Z3 constraints when a model is found, or the unsatisfiable core when no model exists, as well as an option to save or append the output.
+These settings are specified with the Boolean values `True` and `False`:
 
 - Print all Z3 constraints if a model is found: `print_cons_bool`
 - Print the Z3 unsatisfiable core constraints if no model exists: `print_unsat_core_bool`
 - Print all states including impossible states: `print_impossibe_states_bool`
 - Prompt the user to append the output to the current file in a new file: `save_bool`
 
 Users can override these settings by including the following flags:
 
-- Include `-s` to prompt the user to save the output in a new file.
 - Include `-c` to include Z3 constraints.
 - Include `-i` to print impossible states.
-- Include `-h` to print help information about the programs usage.
+- Include `-s` to prompt the user to save the output in a new file.
 
-## Syntax
+Users can print help information, the current version, and upgrade to the latest version with the following flags:
 
-The language currently includes operators for the counterfactual conditional `boxright`, modal operators for necessity `Box` and possibility `Diamond`, and the extensional operators for conjunction `wedge`, disjunction `vee`, material conditional `rightarrow`, material biconditional `leftrightarrow`, and negation `neg`.
+- Include `-h` to print help information about the programs usage.
+- Include `-v` to print the installed version number.
+- Include `-u` to upgrade to the latest version.
 
-## Semantics
+## Hyperintensional Semantics
 
-The semantics included is hyperintensional insofar as sentences are evaluated at _states_ which may be partial rather than total as in intensional semantic theories.
+The semantics is hyperintensional insofar as sentences are evaluated at _states_ which may be partial rather than total as in intensional semantic theories.
 States are modeled by bitvectors of a specified length (e.g., `#b00101` has length `5`), where _state fusion_ is modeled by the bitwise OR operator `|`.
 For instance, `#b00101 | #b11001 = #b11101`.
 The _atomic states_ have exactly one occurrence of `1` and the _null state_ has no occurrences of `1`.
 The space of states is finite and closed under fusion.
 
-States are named by lowercase letters for the sake of printing readable countermodels.
-Fusions are printed using `.` so that `a.b` is the fusion of the states `a` and `b`.
+States are named by lowercase letters in order to print readable countermodels.
+Fusions are printed using `.` where `a.b` is the fusion of the states `a` and `b`.
 A state `a` is _part_ of a state `b` just in case `a.b = b`.
 States may be either _possible_ or _impossible_ where the null state is required to be possible and every part of a possible state is possible.
 The states `a` and `b` are _compatible_ just in case `a.b` is possible.
 A _world state_ is any state that is both possible and includes every compatible state as a part.
 
 Sentences are assigned _verifier states_ and _falsifier states_ where both the verifiers and falsifiers are required to be closed under fusion.
 A sentence is _true at_ a world state `w` just in case `w` includes a verifier for that sentence as a part and _false at_ `w` just in case `w` includes a falsifier for that sentence as a part.
 In order to ensure that sentence letters have at most one truth-value at each world state, a fusion `a.b` is required to be impossible whenever `a` is verifier for a sentence letter `A` and `b` is a falsifier for `A`.
-Additionally, sentence letters have at least one truth-value at each world state by requiring every possible state to be compatible with either a verifier or falsifier for any sentence letter.
+Additionally, sentence letters are guaranteed to have at least one truth-value at each world state by requiring every possible state to be compatible with either a verifier or falsifier for any sentence letter.
 
-Negated sentences are verified by the falsifiers for the sentence negated and falsified by the verifiers for the sentence negated.
-Conjunctions are verified by the pairwise fusions of verifiers for the conjuncts and falsified by falsifiers for either of the conjuncts or fusions thereof.
-Conjunction and disjunction are dual operators obeying the standard idempotent and De Morgan laws.
+A _negated sentence_ is verified by the falsifiers for the sentence negated and falsified by the verifiers for the sentence negated.
+A _conjunctive sentence_ is verified by the pairwise fusions of verifiers for the conjuncts and falsified by falsifiers for either of the conjuncts or fusions thereof.
+A _disjunctive sentence_ is verified by the verifiers for either disjunct or fusions thereof and falsified by pairwise fusions of falsifiers for the disjuncts.
+Conjunction and disjunction are dual operators obeying the standard idempotence and De Morgan laws.
 The absorption laws do not hold, nor does conjunction distribute over disjunction, nor _vice versa_.
 For a defense of the background theory of hyperintensional propositions, see this [paper](https://link.springer.com/article/10.1007/s10992-021-09612-w).
 
-A modal sentence `Box A` is true at a world just in case every world state includes a part that verifies `A`, where `Diamond A` is true at a world just in case some world state includes a part that verifies `A`.
-Given a world state `w` and state `s`, an `s`_-alternative_ to `w` is any world state to include `s` along with a maximal part of `w` that is compatible with `s` as parts.
-A counterfactual conditional sentences `A boxright B` is true at a world state `w` just in case its consequent is true at any `s`-alternative to `w` for any verifier `s` for the antecedent of the counterfactual.
-
+A _necessity sentence_ `Box A` is true at a world just in case every world state includes a part that verifies `A` and a _possibility sentence_ `Diamond A` is true at a world just in case some world state includes a part that verifies `A`.
+Given a world state `w` and state `s`, an `s`_-alternative_ to `w` is any world state to include as parts both `s` and a maximal part of `w` that is compatible with `s`.
+A _must counterfactual conditional sentences_ `A boxright B` is true at a world state `w` just in case its consequent is true at any `s`-alternative to `w` for any verifier `s` for the antecedent of the counterfactual.
+A _might counterfactual conditional sentences_ `A boxright B` is true at a world state `w` just in case its consequent is true at some `s`-alternative to `w` for some verifier `s` for the antecedent of the counterfactual.
 The semantic theory for counterfactual conditionals is motivated and further elaborated in this [draft](https://github.com/benbrastmckie/ModelChecker/blob/master/Counterfactuals.pdf).
-This account builds on [Fine 2012](https://www.pdcnet.org/jphil/content/jphil_2012_0109_0003_0221_0246) and [Fine 2017](https://link.springer.com/article/10.1007/s10992-016-9413-y).
-More information can be found in the GitHub [repository](https://github.com/benbrastmckie/ModelChecker). 
+This account builds on [Fine 2012](https://www.pdcnet.org/jphil/content/jphil_2012_0109_0003_0221_0246) and [Fine2012a](https://link.springer.com/article/10.1007/s11229-012-0094-y?error=cookies_not_supported&code=5166a4da-1834-438c-9f93-75b61f58b6db).
 
+A _grounding sentence_ `A leq B` may be read '`A` is _sufficient for_ `B`' and an _essence sentence_ `A sqsubseteq B` may be read '`A` is _necessary for_ `B`'.
+A _propositional identity sentence_ `A equiv B` may be read '`A` _just is for_ `B`'.
+The semantics for ground requires every verifier for the antecedent to be a verifier for the consequent, any fusion of a falsifier for the antecedent and consequent to be a falsifier for the consequent, and any falsifier for the consequent to have a part that falsifies the antecedent.
+The semantics for essence requires every fusion of a verifier for the antecedent and consequent to be a verifier for the consequent, any verifier for the consequent must have a part that verifies the antecedent, and every falsifier for the antecedent to be a falsifier for the consequent.
+The semantics for propositional identity requires the two arguments to have the same verifiers and falsifiers.
+All three constitutive operators are interdefinable as indicated below: 
+
+- `A leq B` _iff_ `neg A sqsubseteq neg B` _iff_ `(A vee B) equiv B`.
+- `A sqsubseteq B` _iff_ `neg A leq neg B` _iff_ `(A wedge B) equiv B`
+- `A equiv B` _iff_ `(A leq B) wedge (B leq A)` _iff_ `(A sqsubseteq B) wedge (B sqsubseteq A)`.
+
+Instead of a Boolean lattice as in extensional and intensional semantics theories, the space of hyperintensional propositions forms a non-interlaced bilattice as described in this [paper](https://link.springer.com/article/10.1007/s10992-021-09612-w), building on [Fine 2017](https://link.springer.com/article/10.1007/s10992-016-9413-y).
+
+More information can be found in the GitHub [repository](https://github.com/benbrastmckie/ModelChecker).
```

### Comparing `model_checker-0.3.9/pyproject.toml` & `model_checker-0.4.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "model-checker"
-version = "0.3.9"
-description = "A hyperintensional theorem prover for counterfactual conditionals and modal operators."
+version = "0.4.1"
+description = "A hyperintensional theorem prover for modal, counterfactual conditional, constitutive explanatory, and extensional operators."
 authors = [
     { name = "Benjamin Brast-McKie", email = "benbrastmckie@gmail.com" },
     { name = "Miguel Buitrago", email = "mbuit82@gmail.com" },
 ]
 license = { text = "MIT" }
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-keywords = ["semantics", "Z3", "counterfactuals", "model checker", "theorem prover", "hyperintensionality"]
+keywords = ["semantics", "Z3", "logic", "counterfactuals", "modality", "model checker", "theorem prover", "hyperintensionality"]
 dependencies = [
     "z3-solver",
 ]
 
 [project.urls]
 Homepage = "https://github.com/benbrastmckie/ModelChecker"
 Issues = "https://github.com/benbrastmckie/ModelChecker/issues"
```

### Comparing `model_checker-0.3.9/src/model_checker/__main__.py` & `model_checker-0.4.1/src/model_checker/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 '''
 file specifies premises, conclusions, and settings.
 running the file finds a model and prints the result.
 '''
 
 import sys
 import os
+import subprocess
 from string import Template
 import argparse
 import importlib.util
+# import warnings
 # import cProfile
 # import pstats
 
 # Get the directory path of the current file
 current_dir = os.path.dirname(__file__)
 # Construct the full path to your project root
 project_root = os.path.abspath(os.path.join(current_dir, ".."))
 # Add the project root to the Python path
 sys.path.append(project_root)
 
-# from model_structure import (
+from model_checker.__init__ import __version__
 from model_checker.model_structure import ( # for packaging
     StateSpace,
     make_model_for,
     )
 
 script_template = Template("""
 '''
@@ -102,51 +104,55 @@
 """)
 
 class LoadModule:
     """load module and store values as a class"""
     def __init__(self, module_name, module_path):
         self.module_name = module_name
         self.module_path = module_path
+        self.default_values = {
+            "N": 3,
+            "premises": [],
+            "conclusions": [],
+        }
         self.module = self.load_module()
-        self.validate_attributes()
         self.initialize_attributes()
+        self.validate_attributes()
 
     def load_module(self):
         try:
             spec = importlib.util.spec_from_file_location(self.module_name, self.module_path)
             if spec is None or spec.loader is None:
                 raise ImportError("Module spec could not be loaded.")
             module = importlib.util.module_from_spec(spec)
             spec.loader.exec_module(module)
             return module
         except Exception as e:
             raise ImportError(f"Failed to load the module '{self.module_name}': {e}") from e
 
-    def validate_attributes(self):
-        required_attrs = ["N", "premises", "conclusions"]
-        for attr in required_attrs:
-            if not hasattr(self.module, attr):
-                raise ImportError(f"The value of '{attr}' is absent")
-
     def initialize_attributes(self):
         self.parent_file = getattr(self.module, "file_name", True)
         self.parent_directory = getattr(self.module, "parent_directory", True)
-        self.N = getattr(self.module, "N")
-        self.premises = getattr(self.module, "premises")
-        self.conclusions = getattr(self.module, "conclusions")
+        self.N = getattr(self.module, "N", self.default_values["N"])
+        self.premises = getattr(self.module, "premises", self.default_values["premises"])
+        self.conclusions = getattr(self.module, "conclusions", self.default_values["conclusions"])
         self.print_cons_bool = getattr(self.module, "print_cons_bool", False)
         self.print_unsat_core_bool = getattr(self.module, "print_unsat_core_bool", True)
         self.print_impossible_states_bool = getattr(
             self.module,
             "print_impossible_states_bool",
             False
         )
         self.save_bool = getattr(self.module, "save_bool", True)
-        # self.use_constraints_bool = getattr(self.module, "use_constraints", False)
-        self.all_constraints = getattr(self.module, "all_constraints", [])
+        # self.all_constraints = getattr(self.module, "all_constraints", [])
+
+    def validate_attributes(self):
+        for attr, default_value in self.default_values.items():
+            if not hasattr(self.module, attr):
+                print(f"The value of '{attr}' is absent and has been set to {default_value}.")
+                # raise ImportError(f"The value of '{attr}' is absent")
 
 def parse_file_and_flags():
     """returns the name and path for the current script"""
     # create an ArgumentParser object
     parser = argparse.ArgumentParser(
         prog='model-checker',
         usage='%(prog)s [options] input',
@@ -156,14 +162,16 @@
         the path to that file as the input.""",
         epilog="""
         More information can be found at:
         https://github.com/benbrastmckie/ModelChecker/""",
     )
     parser.add_argument(
         "file_path",
+        nargs='?',
+        default=None,
         type=str,
         help="Specifies the path to a Python.",
     )
     parser.add_argument(
         '--constraints',
         '-c',
         action='store_true',
@@ -177,22 +185,78 @@
     )
     parser.add_argument(
         '--impossible',
         '-i',
         action='store_true',
         help='Overrides to print impossible states.'
     )
+    parser.add_argument(
+        '--version',
+        '-v',
+        action='version',
+        version=f"%(prog)s:  {__version__}",
+        help='Prints the version number.'
+    )
+    # parser.add_argument(
+    #     '--latest',
+    #     '-l',
+    #     action='store_true',
+    #     help='Checks the version number of the latest release.'
+    # )
+    parser.add_argument(
+        '--upgrade',
+        '-u',
+        action='store_true',
+        help='Upgrade the package.'
+    )
     # parse the command-line argument to get the module path
     args = parser.parse_args()
-    module_path = args.file_path
-    module_name = os.path.splitext(os.path.basename(module_path))[0]
-    cons_bool = args.constraints
-    save_bool = args.save
-    imposs_bool = args.impossible
-    return module_name, module_path, cons_bool, save_bool, imposs_bool
+    package_name = parser.prog  # Get the package name from the parser
+    return args, package_name
+
+# NOTE: the below was in attempt to check for the most recent version before upgrade
+# having trouble getting the most recent version from PyPI
+# everything else seems to work
+
+# def get_installed_version(package_name):
+#     """returns the current version of the package"""
+#     try:
+#         installed_version = __version__
+#         # installed_version = subprocess.check_output(['pip', 'show', package_name]).decode().split('\n')[1].split(': ')[1]
+#         return installed_version
+#     except ValueError as e:
+#         print(f"Error getting installed version: {e}")
+#         return False
+
+# def get_latest_version(package_name):
+#     """returns the latest version of the package"""
+#     try:
+#         output = subprocess.check_output(['pip', 'show', package_name, '--no-cache-dir']).decode()
+#         version_line = [
+#             line for line in output.split('\n')
+#             if line.lower().startswith('version:')
+#         ][0]
+#         latest_version = version_line.split(': ')[1].strip()
+#         return latest_version
+#     except ValueError as e:
+#         print(f"Error getting latest version: {e}")
+#         return None
+
+# def check_update(package_name):
+#     """finds and compares the latest version to the installed version."""
+#     # Get the installed version of the package
+#     installed_version = get_installed_version(package_name)
+#     # Get the latest version of the package from PyPI
+#     latest_version = get_latest_version(package_name)
+#     # Compare the installed version with the latest version
+#     if installed_version == latest_version:
+#         print(f"{package_name} is already up to date (version {installed_version})")
+#         return True
+#     print(f"{package_name} is not up to date (installed version: {installed_version}, latest version: {latest_version})")
+#     return False
 
 def generate_test(name):
     """check if a script name was provided"""
     template_data = {
         'name': name
     }
     script_content = script_template.substitute(template_data)
@@ -223,47 +287,71 @@
     file_name = input(
         "\nEnter the file name in snake_case without an extension.\n"
         "Leave the file name blank to append the output to the project file.\n"
         "\nFile name:\n"
     )
     return file_name, print_cons
 
-def no_model_save_or_append(module, model_structure, file_name, print_cons, print_imposs):
+def no_model_save_or_append(module, model_structure, file_name, print_cons):
+    """option to save or append if no model is found"""
     if len(file_name) == 0:
         with open(f"{module.module_path}", 'a', encoding="utf-8") as f:
             print('\n"""', file=f)
             model_structure.no_model_print(print_cons, f)
             print('"""', file=f)
         return
     with open(f"{module.parent_directory}/{file_name}.py", 'w', encoding="utf-8") as n:
         print(f'# TITLE: {file_name}.py generated from {module.parent_file}\n"""', file=n)
         model_structure.no_model_save(print_cons, n)
     print()
 
 
 def save_or_append(module, structure, file_name, print_cons, print_imposs):
+    """option to save or append if a model is found"""
     if len(file_name) == 0:
         with open(f"{module.module_path}", 'a', encoding="utf-8") as f:
             print('\n"""', file=f)
             structure.print_to(print_cons, print_imposs, f)
             print('"""', file=f)
         return
     with open(f"{module.parent_directory}/{file_name}.py", 'w', encoding="utf-8") as n:
         print(f'# TITLE: {file_name}.py generated from {module.parent_file}\n"""', file=n)
         structure.save_to(print_cons, print_imposs, n)
     print()
 
 def main():
     """load a test or generate a test when run without input"""
+    # TODO: can module_name and module_path be extracted from the sys.argv?
+    # this would reduce the number of arguments returned by parse_file_and_flags()
+    args, package_name = parse_file_and_flags()
+    cons_flag = args.constraints
+    save_flag = args.save
+    imposs_flag = args.impossible
+    upgrade_flag = args.upgrade
+    # latest_flag = args.latest
+    # NOTE: the checker is not working
+    # if latest_flag:
+    #     latest_version = get_latest_version(package_name)
+    #     print(f"Latest version on PyPI: {latest_version}")
+    #     return
+    if upgrade_flag:
+        # # NOTE: the checker is not working
+        # if check_update(package_name):
+        #     return
+        # Upgrade the package if it is not up to date
+        try:
+            subprocess.run(['pip', 'install', '--upgrade', package_name], check=True)
+        except subprocess.CalledProcessError as e:
+            print(f"Failed to upgrade {package_name}: {e}")
+        return
     if len(sys.argv) < 2:
         ask_generate_test()
         return
-    # TODO: can module_name and module_path be extracted from the sys.argv?
-    # this would reduce the number of arguments returned by parse_file_and_flags()
-    module_name, module_path, cons_flag, save_flag, imposs_flag = parse_file_and_flags()
+    module_path = args.file_path
+    module_name = os.path.splitext(os.path.basename(module_path))[0]
     module = LoadModule(module_name, module_path)
     print_imposs = module.print_impossible_states_bool or imposs_flag
     print_cons = module.print_cons_bool or cons_flag
     save_model = module.save_bool or save_flag
     model_setup, model_structure = make_model_for(module.N, module.premises, module.conclusions)
     if model_structure.model_status:
         states_print = StateSpace(model_setup, model_structure)
@@ -272,15 +360,15 @@
             file_name, print_cons = ask_save()
             save_or_append(module, states_print, file_name, print_cons, print_imposs)
         return
     print_unsat = module.print_unsat_core_bool or cons_flag
     model_structure.no_model_print(print_unsat)
     if save_model:
         file_name, print_cons = ask_save()
-        no_model_save_or_append(module, model_structure, file_name, print_unsat, print_imposs)
+        no_model_save_or_append(module, model_structure, file_name, print_unsat)
 
 
 if __name__ == "__main__":
     main()
     # cProfile.run('main()')
     # cProfile.run('main()', 'profile_results')
```

### Comparing `model_checker-0.3.9/src/model_checker/model_definitions.py` & `model_checker-0.4.1/src/model_checker/model_definitions.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,27 +156,25 @@
         fal_bits = relate_sents_and_states(all_bits, letter, z3_model, falsify)
         atomic_VFs_dict[letter] = (ver_bits, fal_bits)
     return atomic_VFs_dict
 
 def bit_fusion(bit_s, bit_t):
     """the result of taking the maximum for each index in _s and _t"""
     return simplify(bit_s | bit_t)
-    # NOTE: this does seem to make a difference, otherwise no comp_parts
+    # NOTE: 'simplify' does seem to make a difference, otherwise no comp_parts
 
 def bit_part(bit_s, bit_t):
     """the fusion of _s and _t is identical to bit_t"""
     return bool(simplify(bit_fusion(bit_s, bit_t) == bit_t))
-    # NOTE: this does seem to make a difference, otherwise no comp_parts
+    # NOTE: 'bool' does seem to make a difference, otherwise no comp_parts
 
 def bit_proper_part(bit_s, bit_t):
     """bit_s is a part of bit_t and bit_t is not a part of bit_s"""
     return bool(bit_part(bit_s, bit_t)) and not bit_s == bit_t
     # NOTE: this does not seem to make a difference and so has been turned off
-    # in the interest of discovering if it is required or not
-    # return bool(bit_part(bit_s, bit_t)) and not bit_s == bit_t
 
 def index_to_substate(index):
     '''
     test cases should make evident what's going on
     >>> index_to_substate(0)
     'a'
     >>> index_to_substate(26)
@@ -223,41 +221,41 @@
                 return "□"  #  null state
             return state_repr[0 : len(state_repr) - 1]
         if char == "1":
             state_repr += index_to_substate(i)
             state_repr += "."
     raise ValueError("should have run into 'b' at the end but didn't")
 
-def infix_combine(premises, conclusions):
-    '''combines the premises with the negation of the conclusion(s).
-    premises are infix sentences, and so are the conclusions
-    imported by model_structure, in __init__ method of ModelStructure'''
-    input_sentences = premises[:]
-    for sent in conclusions:
-        neg_sent = '\\neg ' + sent
-        input_sentences.append(neg_sent)
-    return input_sentences
-
-def disjoin_prefix(sentences):
-    """disjoins the list of sentences in prefix form
-    helper for prefix_combine (immediately below)"""
-    if len(sentences) > 2:
-        copy_sentences = sentences[:]
-        first_sent = copy_sentences.pop(0)
-        return ['\\vee ', first_sent, disjoin_prefix(copy_sentences)]
-    # if len(sentences) == 1:
-    #     return sentences[0]
-    return sentences
-
-def prefix_combine(prefix_premises, prefix_conclusions):
-    '''negates and disjoins the prefix conclusions, combining the result with
-    prefix premises to form a new list'''
-    neg_conclusions = [['\\neg ', con] for con in prefix_conclusions]
-    disjoin_neg_conclusions = disjoin_prefix(neg_conclusions)
-    return prefix_premises + disjoin_neg_conclusions
+# def infix_combine(premises, conclusions):
+#     '''combines the premises with the negation of the conclusion(s).
+#     premises are infix sentences, and so are the conclusions
+#     imported by model_structure, in __init__ method of ModelStructure'''
+#     input_sentences = premises[:]
+#     for sent in conclusions:
+#         neg_sent = '\\neg ' + sent
+#         input_sentences.append(neg_sent)
+#     return input_sentences
+
+# def disjoin_prefix(sentences):
+#     """disjoins the list of sentences in prefix form
+#     helper for prefix_combine (immediately below)"""
+#     if len(sentences) > 2:
+#         copy_sentences = sentences[:]
+#         first_sent = copy_sentences.pop(0)
+#         return ['\\vee ', first_sent, disjoin_prefix(copy_sentences)]
+#     # if len(sentences) == 1:
+#     #     return sentences[0]
+#     return sentences
+
+# def prefix_combine(prefix_premises, prefix_conclusions):
+#     '''negates and disjoins the prefix conclusions, combining the result with
+#     prefix premises to form a new list'''
+#     neg_conclusions = [['\\neg ', con] for con in prefix_conclusions]
+#     disjoin_neg_conclusions = disjoin_prefix(neg_conclusions)
+#     return prefix_premises + disjoin_neg_conclusions
 
 # def is_counterfactual(prefix_sentence):
 #     '''returns a boolean to say whether a given sentence is a counterfactual
 #     used in find_extensional_subsentences'''
 #     if len(prefix_sentence) == 1:
 #         return False
 #     if len(prefix_sentence) == 2:
@@ -316,14 +314,23 @@
 #     if kind == 'all':
 #         counterfactual = rr([sent for sent in all_subsentences if is_counterfactual(sent)])
 #         modal = rr([sent for sent in all_subsentences if is_modal(sent)])
 #         extensional = rr([sent for sent in all_subsentences if sent not in counterfactual and sent not in modal])
 #         return (extensional, modal, counterfactual, all_subsentences)
 #     return rr(return_list)
 
+def repeats_removed(sentences):
+    '''takes a list and removes the repeats in it.
+    used in find_all_constraints'''
+    seen = []
+    for obj in sentences:
+        if obj not in seen:
+            seen.append(obj)
+    return seen
+
 def subsentences_of(prefix_sentence):
     '''finds all the subsentence of a prefix sentence
     returns these as a set
     used in find_extensional_subsentences'''
     progress = []
     progress.append(prefix_sentence)
     if len(prefix_sentence) == 2:
@@ -340,56 +347,68 @@
     """take a set of prefix sentences and returns a set of all subsentences"""
     all_subsentences = []
     for prefix_sent in prefix_sentences:
         all_prefix_subs = subsentences_of(prefix_sent)
         all_subsentences.extend(all_prefix_subs)
     return repeats_removed(all_subsentences)
 
-def repeats_removed(sentences):
-    '''takes a list and removes the repeats in it.
-    used in find_all_constraints'''
-    seen = []
-    for obj in sentences:
-        if obj not in seen:
-            seen.append(obj)
-    return seen
-
-
 def evaluate_modal_expr(model_structure, prefix_modal, eval_world):
     '''evaluates whether a counterfatual in prefix form is true at a world (BitVecVal).
     used to initialize Counterfactuals
     returns a bool representing whether the counterfactual is true at the world or not'''
-    op, argument = prefix_modal[0], prefix_modal[1]
+    operator, argument = prefix_modal[0], prefix_modal[1]
+    # TODO: is this necessary?
     # if is_modal(argument):
     #     if model_structure.evaluate_modal_expr(prefix_modal) is True: # ie, verifiers is null state
     #         return True # both Box and Diamond will return true, since verifiers is not empty
     #     return False
-    if 'Diamond' in op:
+    if 'Diamond' in operator:
         for poss in model_structure.poss_bits:
             if poss in find_complex_proposition(model_structure, argument, eval_world)[0]:
                 return True
         return False
-    if 'Box' in op:
+    if 'Box' in operator:
         for poss in model_structure.poss_bits:
             if poss in find_complex_proposition(model_structure, argument, eval_world)[1]:
                 return False
         return True
+    raise ValueError(
+        prefix_modal,
+        "Something has gone wrong in evaluate_cf_counterfactual. "
+        f"The operator {operator} in {prefix_modal} is not a modal."
+    )
 
 def evaluate_cf_expr(state_space, prefix_cf, eval_world):
     """evaluates whether a counterfatual in prefix form is true at a world (BitVecVal).
     used to initialize Counterfactuals
     returns a bool representing whether the counterfactual is true at the world or not
     """
-    antecedent, consequent = prefix_cf[1], prefix_cf[2]
-    ant_verifiers = find_complex_proposition(state_space, antecedent, eval_world)[0]
-    con_falsifiers = find_complex_proposition(state_space, consequent, eval_world)[1]
-    antecedent_alts = state_space.find_alt_bits(ant_verifiers, eval_world)
-    if any(bit_part(con_fal, u) for u in antecedent_alts for con_fal in con_falsifiers):
+    operator, antecedent, consequent = prefix_cf[0], prefix_cf[1], prefix_cf[2]
+    antecedent_vers = find_complex_proposition(state_space, antecedent, eval_world)[0]
+    consequent_vers = find_complex_proposition(state_space, consequent, eval_world)[0]
+    consequent_fals = find_complex_proposition(state_space, consequent, eval_world)[1]
+    antecedent_alts = state_space.find_alt_bits(antecedent_vers, eval_world)
+    if 'boxright' in operator:
+        for alt_world in antecedent_alts:
+            for falsifier in consequent_fals:
+                if bit_part(falsifier, alt_world):
+                    return False
+        return True
+    if 'circleright' in operator:
+        for alt_world in antecedent_alts:
+            for verifier in consequent_vers:
+                if bit_part(verifier, alt_world):
+                    return True
         return False
-    return True
+    raise ValueError(
+        prefix_cf,
+        "Something has gone wrong in evaluate_cf_counterfactual. "
+        f"The operator {operator} in {prefix_cf} is not a counterfatual."
+    )
+
 
 # def evaluate_mainclause_cf_expr(model_structure, prefix_cf, eval_world):
 #     """evaluates whether a counterfatual in prefix form is true at a world (BitVecVal).
 #     used to initialize Counterfactuals
 #     returns a bool representing whether the counterfactual is true at the world or not
 #     """
 #     op = prefix_cf[0]
@@ -403,41 +422,40 @@
 #         if is_counterfactual(consequent_expr):
 #             if not find_complex_proposition(model_structure, consequent_expr, u)[0]:
 #                 return False
 #         elif str(consequent_expr) not in str(find_true_and_false_in_alt(u, model_structure)[0]):
 #             return False
 #     return True
 
-def true_and_false_worlds_for_cf(model_structure, complex_cf_sent):
+def true_and_false_worlds_for_cf(model_structure, cf_sentence):
     '''used in find_complex_proposition'''
     worlds_true_at, worlds_false_at = set(), set()
     for world in model_structure.world_bits:
-        if find_complex_proposition(model_structure, complex_cf_sent, world)[0]:
+        if find_complex_proposition(model_structure, cf_sentence, world)[0]:
             worlds_true_at.add(world)
             continue
         worlds_false_at.add(world)
     return (worlds_true_at, worlds_false_at)
 
 def find_complex_proposition(model_structure, complex_sentence, eval_world):
     """sentence is a sentence in prefix notation
     For a given complex proposition, returns the verifiers and falsifiers of that proposition
     given a solved model
     for a counterfactual, it'll just give the worlds it's true at and worlds it's not true at
     """
     if not model_structure.atomic_props_dict:
         raise ValueError(
-            "There is nothing in atomic_props_dict yet. Have you actually run the model?"
+            "There is nothing in atomic_props_dict yet. Has a model been found?"
         )
     if len(complex_sentence) == 1:
         sent = complex_sentence[0]
-        # TODO: linter error: expected 0 arguments
         return model_structure.atomic_props_dict[sent]
     op = complex_sentence[0]
     Y = complex_sentence[1]
-    if "neg" in op:
+    if "neg" in op or "not" in op:
         Y_V, Y_F = find_complex_proposition(model_structure, Y, eval_world)
         return (Y_F, Y_V)
     null_state = {BitVecVal(0,model_structure.N)}
     if 'Box' in op or 'Diamond' in op:
         if evaluate_modal_expr(model_structure, complex_sentence, eval_world):
             return (null_state, set())
         return (set(), null_state)
@@ -452,12 +470,29 @@
         return (
             product(coproduct(Y_F, Z_V), coproduct(Y_V, Z_F)),
             coproduct(product(Y_V, Z_F), product(Y_F, Z_V)),
         )
     if "rightarrow" in op:
         return (coproduct(Y_F, Z_V), product(Y_V, Z_F))
     if "boxright" in op:
-        # if evaluate_mainclause_cf_expr(model_structure, complex_sentence, eval_world):
         if evaluate_cf_expr(model_structure, complex_sentence, eval_world):
+            # val = evaluate_cf_expr(model_structure, complex_sentence, eval_world)
+            # print(f"TEST: truth_vf of cf = {val}")
+            return (null_state, set())
+        return (set(), null_state)
+    if "circleright" in op:
+        if evaluate_cf_expr(model_structure, complex_sentence, eval_world):
+            return (null_state, set())
+        return (set(), null_state)
+    if "leq" in op:
+        if Y_V <= Z_V and product(Y_F, Z_F) == Z_F:
+            return (null_state, set())
+        return (set(), null_state)
+    if "sqsubseteq" in op:
+        if product(Y_V, Z_V) == Z_V and Y_F <= Z_F:
+            return (null_state, set())
+        return (set(), null_state)
+    if "equiv" in op:
+        if Y_V == Z_V and Y_F == Z_F:
             return (null_state, set())
         return (set(), null_state)
     raise ValueError(f"Don't know how to handle {op} operator")
```

### Comparing `model_checker-0.3.9/src/model_checker/model_structure.py` & `model_checker-0.4.1/src/model_checker/model_structure.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,38 +9,35 @@
     Function,
     BitVecSort,
     BoolSort,
     BitVec,
     BitVecVal
 )
 
-from model_checker.semantics import ( # for packaging
-# from semantics import (
+from model_checker.semantics import (
     make_constraints,
     solve_constraints,
+    all_sentence_letters,
 )
-from model_checker.model_definitions import ( # for packaging
-# from model_definitions import (
+from model_checker.model_definitions import (
     find_compatible_parts,
     atomic_propositions_dict_maker,
     find_all_bits,
     find_max_comp_ver_parts,
     find_poss_bits,
     find_subsentences,
     find_world_bits,
-    prefix_combine,
     pretty_set_print,
     bit_part,
     bitvec_to_substates,
     int_to_binary,
     true_and_false_worlds_for_cf,
     find_complex_proposition,
 )
-from model_checker.syntax import ( # for packaging
-# from syntax import (
+from model_checker.syntax import (
     AtomSort,
     infix,
     prefix,
     add_backslashes_to_infix,
 )
 
 inputs_template = Template(
@@ -103,27 +100,32 @@
         self.verify = Function("verify", BitVecSort(N), AtomSort, BoolSort())
         self.falsify = Function("falsify", BitVecSort(N), AtomSort, BoolSort())
         self.assign = Function("assign", BitVecSort(N), AtomSort, BitVecSort(N))
         self.w = BitVec("w", N) # what will be the main world
         self.prefix_premises = [prefix(prem) for prem in infix_premises]
         # M: I think below is a problem
         self.prefix_conclusions = [prefix(con) for con in infix_conclusions]
-        self.prefix_sentences = prefix_combine(self.prefix_premises, self.prefix_conclusions)
         find_constraints_func = make_constraints(
             self.verify,
             self.falsify,
             self.possible,
             self.assign,
             self.N,
             self.w
         )
-        constraints, sentence_letters = find_constraints_func(self.prefix_sentences)
-        self.sentence_letters = sentence_letters
-        self.constraints = constraints
-        self.all_subsentences = find_subsentences(self.prefix_sentences)
+        frame_cons, prop_cons, premise_cons, conclusion_cons = find_constraints_func(
+            self.prefix_premises,
+            self.prefix_conclusions
+        )
+        self.frame_constraints = frame_cons
+        self.prop_constraints = prop_cons
+        self.premise_constraints = premise_cons
+        self.conclusion_constraints = conclusion_cons
+        prefix_sentences = self.prefix_premises + self.prefix_conclusions
+        self.all_subsentences = find_subsentences(prefix_sentences)
 
     # def constraints_func(self):
     #     """returns constraints_func"""
     #     return self.find_constraints_func
 
     def solve(self):
         """solves for the model, returns None
@@ -132,15 +134,16 @@
         self.all_bits is a list of all bits (each of sort BitVecVal)
         self.poss_bits is a list of all possible bits
         self.world_bits is a lsit of all world bits
         self.main_world is the eval world (as a BitVecVal)
         self.atomic_props_dict is a dictionary with keys AtomSorts and keys (V,F)
         """
         model_start = time.time()  # start benchmark timer
-        z3_model_status, z3_model = solve_constraints(self.constraints)
+        constraints = self.frame_constraints + self.prop_constraints + self.premise_constraints + self.conclusion_constraints
+        z3_model_status, z3_model = solve_constraints(constraints)
         model_end = time.time()
         model_runtime = round(model_end - model_start, 4)
         return (z3_model_status, z3_model, model_runtime)
 
 
 class ModelStructure:
     """self.premises is a list of prefix sentences
@@ -194,32 +197,32 @@
     def no_model_print(self, print_unsat_core_bool, output=sys.__stdout__):
         """prints the argument when there is no model with the option to
         include Z3 constraints."""
         print(f"There are no {self.N}-models of:\n", file=output)
         self.print_enumerate(output)
         print(file=output)
         if print_unsat_core_bool:
-            self.print_constraints(self.z3_model, output)
+            self.print_constraints(self.z3_model, '', output)
         print(f"Run time: {self.model_runtime} seconds\n", file=output)
 
     def no_model_save(self, print_unsat_core_bool, output):
         """saves the arguments to a new file when there is no model with the
         option to include Z3 constraints."""
         constraints = self.model_setup.constraints
         print(f"There are no {self.N}-models of:\n", file=output)
         self.print_enumerate(output)
         self.build_test_file(output)
         if print_unsat_core_bool:
             print("# Unsatisfiable constraints", file=output)
             print(f"all_constraints = {constraints}", file=output)
 
-    def print_constraints(self, consts, output=sys.__stdout__):
+    def print_constraints(self, consts, name, output=sys.__stdout__):
         """prints constraints in an numbered list"""
         if self.model_status:
-            print("Satisfiable constraints:\n", file=output)
+            print(f"Satisfiable {name} constraints:\n", file=output)
         else:
             print("Unsatisfiable core constraints:\n", file=output)
         for index, con in enumerate(consts, start=1):
             print(f"{index}. {con}\n", file=output)
             # print(f"Constraints time: {time}\n")
 
 
@@ -234,18 +237,19 @@
         self.model_status = model_structure.model_status
         self.N = model_setup.N
         self.main_world = model_setup.w
         self.all_bits = find_all_bits(self.N)
         self.poss_bits = find_poss_bits(self.z3_model, self.all_bits, model_setup.possible)
         self.world_bits = find_world_bits(self.poss_bits)
         self.main_world = self.z3_model[self.main_world]
-        self.sentence_letters = model_setup.sentence_letters
         self.verify = model_setup.verify
         self.falsify = model_setup.falsify
         self.all_subsentences = model_setup.all_subsentences
+        prefix_sentences = model_setup.prefix_premises + model_setup.prefix_conclusions
+        self.sentence_letters = all_sentence_letters(prefix_sentences)
         self.atomic_props_dict = atomic_propositions_dict_maker(self)
         self.all_propositions = [
             Proposition(sent, self, self.main_world) for sent in model_setup.all_subsentences
         ]
         self.premise_propositions = [
             Proposition(sent, self, self.main_world) for sent in model_setup.prefix_premises
         ]
@@ -273,23 +277,23 @@
                 for max_ver in max_comp_ver_parts:
                     if bit_part(max_ver, world):
                         alt_bits.add(world)
                         break  # to return to the second for loop over world_bits
         return alt_bits
 
     # Useful to user now that can search an infix expression
-    def find_proposition_object(self, expression, prefix_search=False):
+    def find_proposition_object(self, expression):
         """given a sentence, finds the Proposition object in the model that corresponds
         to it. Can optionally search through only the extensional sentences
         Also defaults to searching an infix sentence, though internally it always searches
         prefix.
         If search infix, make sure you put double backslashes always!!
         returns a Proposition object"""
         # search_list = self.all_propositions
-        # if prefix_search:
+        # if infix_search:
         #     for prop_object in search_list:
         #         if prop_object["prefix expression"] == expression:
         #             return prop_object
         # else:
         #     for prop_object in search_list:
         #         if str(prop_object) == add_backslashes_to_infix(expression):
         #             return prop_object
@@ -312,47 +316,56 @@
     def print_evaluation(self, output=sys.__stdout__):
         """print the evaluation world and all sentences letters that true/false
         in that world"""
         N = self.model_setup.N
         sentence_letters = self.sentence_letters
         main_world = self.main_world
         print(
-            f"\nThe evaluation world is {bitvec_to_substates(main_world, N)}:",
+            f"\nThe evaluation world is: {bitvec_to_substates(main_world, N)}",
             file=output,
         )
         true_in_eval = set()
         for sent in sentence_letters:
             for bit in self.all_bits:
                 ver_bool = self.model_setup.verify(bit, self.z3_model[sent])
                 part_bool = bit_part(bit, main_world)
                 if bool(self.z3_model.evaluate(ver_bool) and part_bool):
                     true_in_eval.add(sent)
                     break  # exits the first for loop
         false_in_eval = {R for R in sentence_letters if not R in true_in_eval}
+        GREEN = '\033[32m'
+        RED = '\033[31m'
+        # YELLOW = '\033[33m'
+        RESET = '\033[0m'
         if true_in_eval:
             true_eval_list = sorted([str(sent) for sent in true_in_eval])
             true_eval_string = ", ".join(true_eval_list)
             print(
-                f"  {true_eval_string}  (True in {bitvec_to_substates(main_world, N)})",
+                f"  {GREEN}{true_eval_string}  (True in {bitvec_to_substates(main_world, N)}){RESET}",
                 file=output,
             )
         if false_in_eval:
             false_eval_list = sorted([str(sent) for sent in false_in_eval])
             false_eval_string = ", ".join(false_eval_list)
             print(
-                f"  {false_eval_string}  (False in {bitvec_to_substates(main_world, N)})",
+                f"  {RED}{false_eval_string}  (False in {bitvec_to_substates(main_world, N)}){RESET}",
                 file=output,
             )
         print(file=output)
 
     def print_to(self, print_cons_bool, print_impossible, output=sys.__stdout__):
         """append all elements of the model to the file provided"""
         self.print_all(print_impossible, output)
+        structure = self.model_structure
+        setup = self.model_setup
         if print_cons_bool:
-            self.z3_model.print_constraints(self.model_setup.constraints, output)
+            structure.print_constraints(setup.frame_constraints, 'FRAME', output)
+            structure.print_constraints(setup.prop_constraints, 'PROPOSTION', output)
+            structure.print_constraints(setup.premise_constraints, 'PREMISE', output)
+            structure.print_constraints(setup.conclusion_constraints, 'CONCLUSION', output)
         print(f"Run time: {self.model_runtime} seconds\n", file=output)
 
     def save_to(self, cons_include, print_impossible, output):
         """append all elements of the model to the file provided"""
         constraints = self.model_setup.constraints
         self.print_all(print_impossible, output)
         self.model_structure.build_test_file(output)
@@ -361,61 +374,72 @@
             # TODO: print constraint objects, not constraint strings
             print(f"all_constraints = {constraints}", file=output)
 
     def print_states(self, print_impossible, output=sys.__stdout__):
         """print all fusions of atomic states in the model
         first print function in print.py"""
         N = self.model_setup.N
-        print("\nPossible states:", file=output)  # Print states
+        print("\nState Space:", file=output)  # Print states
+        YELLOW = '\033[33m'
+        BLUE = '\033[34m'
+        MAGENTA = '\033[35m'
+        CYAN = '\033[36m'
+        WHITE = '\033[37m'
+        RESET = '\033[0m'
         for bit in self.all_bits:
             state = bitvec_to_substates(bit, N)
             bin_rep = (
                 bit.sexpr()
                 if N % 4 != 0
                 else int_to_binary(int(bit.sexpr()[2:], 16), N)
             )
+            if bit == 0:
+                print(f"  {WHITE}{bin_rep} = {YELLOW}{state}{RESET}", file=output)
+                continue
             if bit in self.world_bits:
-                print(f"  {bin_rep} = {state} (world)", file=output)
+                print(f"  {WHITE}{bin_rep} = {BLUE}{state} (world){RESET}", file=output)
                 continue
             if bit in self.poss_bits:
-                print(f"  {bin_rep} = {state}", file=output)
+                print(f"  {WHITE}{bin_rep} = {CYAN}{state}{RESET}", file=output)
                 continue
             if print_impossible:
-                print(f"  {bin_rep} = {state} (impossible)", file=output)
+                print(f"  {WHITE}{bin_rep} = {MAGENTA}{state} (impossible){RESET}", file=output)
 
     def rec_print(self, prop_obj, world_bit, print_impossible, output, indent=0):
         """recursive print function (previously print_sort)
         returns None"""
         N = self.model_setup.N
         sentence_letters = self.sentence_letters
         prop_obj.print_verifiers_and_falsifiers(world_bit, print_impossible, indent, output)
         if str(prop_obj) in [str(atom) for atom in sentence_letters]:
             return
         prefix_expr = prop_obj["prefix expression"]
         op = prefix_expr[0]
-        first_subprop = self.find_proposition_object(prefix_expr[1], prefix_search=True)
+        first_subprop = self.find_proposition_object(prefix_expr[1])
         indent += 1 # begin subcases, so indent
-        if "neg" in op:
+        if "neg" in op or "not" in op:
             self.rec_print(first_subprop, world_bit, print_impossible, output, indent)
             return
         if 'Diamond' in op or 'Box' in op:
             for u in self.world_bits:
                 self.rec_print(first_subprop, u, print_impossible, output, indent)
             return
         left_subprop = first_subprop
-        right_subprop = self.find_proposition_object(prefix_expr[2], prefix_search=True)
+        right_subprop = self.find_proposition_object(prefix_expr[2])
         if "boxright" in op:
+            CYAN = '\033[36m'
+            RESET = '\033[0m'
             left_subprop_vers = left_subprop['verifiers']
             phi_alt_worlds_to_world_bit = self.find_alt_bits(left_subprop_vers, world_bit)
             alt_worlds_as_strings = {bitvec_to_substates(u,N) for u in phi_alt_worlds_to_world_bit}
             self.rec_print(left_subprop, world_bit, print_impossible, output, indent)
             print(
                 f'{"  " * indent}'
-                f'{left_subprop}-alternatives to {bitvec_to_substates(world_bit, N)} = '
-                f'{pretty_set_print(alt_worlds_as_strings)}',
+                f'{CYAN}({left_subprop})-alternatives to {bitvec_to_substates(world_bit, N)} = '
+                f'{pretty_set_print(alt_worlds_as_strings)}{RESET}',
                 file=output
             )
             indent += 1
             for u in phi_alt_worlds_to_world_bit:
                 self.rec_print(right_subprop, u, print_impossible, output, indent)
             return
         self.rec_print(left_subprop, world_bit, print_impossible, output, indent)
@@ -426,36 +450,36 @@
         returns None"""
         initial_eval_world = self.main_world
         infix_premises = self.model_setup.infix_premises
         infix_conclusions = self.model_setup.infix_conclusions
         start_con_num = len(infix_premises) + 1
         if self.premise_propositions:
             if len(infix_premises) < 2:
-                print("Interpreted premise:\n", file=output)
+                print("INTERPRETED PREMISE:\n", file=output)
             else:
-                print("Interpreted premises:\n", file=output)
+                print("INTERPRETED PREMISES:\n", file=output)
             for index, input_prop in enumerate(self.premise_propositions, start=1):
                 print(f"{index}.", end="", file=output)
                 self.rec_print(input_prop, initial_eval_world, print_impossible, output, 1)
                 print(file=output)
         if self.conclusion_propositions:
             if len(infix_conclusions) < 2:
-                print("Interpreted conclusion:\n", file=output)
+                print("INTERPRETED CONCLUSION:\n", file=output)
             else:
-                print("Interpreted conclusions:\n", file=output)
+                print("INTERPRETED CONCLUSIONS:\n", file=output)
             for index, input_prop in enumerate(self.conclusion_propositions, start=start_con_num):
                 print(f"{index}.", end="", file=output)
                 self.rec_print(input_prop, initial_eval_world, print_impossible, output, 1)
                 print(file=output)
 
     def print_all(self, print_impossible, output):
         """prints states, sentence letters evaluated at the designated world and
         recursively prints each sentence and its parts"""
         N = self.model_setup.N
-        print(f"There is a {N}-model of:\n", file=output)
+        print(f"\nThere is a {N}-model of:\n", file=output)
         self.model_structure.print_enumerate(output)
         self.print_states(print_impossible, output)
         self.print_evaluation(output)
         self.print_inputs_recursively(print_impossible, output)
 
 class Proposition:
     """class for propositions to store their verifiers, falsifiers, alt worlds, etc
@@ -467,53 +491,75 @@
         are only the null state and falsifiers are nothing; if they're false the opposite"""
         self.prop_dict = {}
         self.prop_dict["prefix expression"] = prefix_expr
         self.model_structure = model_structure
         verifiers, falsifiers = find_complex_proposition(model_structure, prefix_expr, eval_world)
         self.prop_dict["verifiers"] = verifiers
         self.prop_dict["falsifiers"] = falsifiers
-        # if is_counterfactual(prefix_expr):
+        # TODO: can cf_sentences be treated in a more uniform way, avoiding the if clause below?
         if 'boxright' in str(prefix_expr[0]):
-            self.current_eval_world = eval_world
+            # print(f"TEST: check condition")
+            self.cf_world = eval_world
             true_worlds, false_worlds = true_and_false_worlds_for_cf(model_structure, prefix_expr)
+            # print(f"TEST WORLDS: true {true_worlds}; false {false_worlds}")
             self['worlds cf true at'] = true_worlds
             self['worlds cf false at'] = false_worlds
 
     def __setitem__(self, key, value):
         self.prop_dict[key] = value
 
     def __getitem__(self, key):
         '''NOTE: If a user wants to access a modal or counterfactual Proposition's verifiers, 
         THEY SHOULD NOT. They should instead use the truth_value_at() method'''
         return self.prop_dict[key]
 
     def __str__(self):
         return infix(self["prefix expression"])
 
-    def update_verifiers(self, eval_world):
+    def update_proposition(self, eval_world):
         """updates the evaluation world for counterfactuals"""
         # if not is_counterfactual(self['prefix expression']):
         #     raise AttributeError(f'You can only update verifiers for CFs, and {self} is not a CF.')
         N = self.model_structure.N
-        if eval_world == self.current_eval_world:
+        if eval_world == self.cf_world:
             return
         if eval_world in self['worlds cf true at']:
             self['verifiers'], self['falsifiers'] = {BitVecVal(0,N)}, set()
             return
         self['verifiers'], self['falsifiers'] = set(), {BitVecVal(0,N)}
         return
 
+    def truth_value_at(self, eval_world):
+        '''Given a world, returns the truth value of the Proposition at that world.
+        Used in print_verifiers_and_falsifiers.'''
+        for verifier in self["verifiers"]:
+            if bit_part(verifier, eval_world):
+                return True
+        for falsifier in self["falsifiers"]:
+            # test = self["falsifiers"]
+            # print(f"TEST: {test}")
+            if bit_part(falsifier, eval_world):
+                # N = self.model_structure.N
+                # print(f"TEST: falsifier = {bitvec_to_substates(falsifier, N)}")
+                return False
+        raise ValueError(
+            "Something has gone wrong.\n"
+            f'No verifier or falsifier for {self["prefix expression"]} at world {eval_world}'
+        )
+
     def print_verifiers_and_falsifiers(self, eval_world, print_impossible=False, indent=0, output=sys.__stdout__):
         """prints the possible verifiers and falsifier states for a sentence.
         used in: rec_print() 
         ensures eval_world is in fact the eval_world for CFs"""
         N = self.model_structure.N
         truth_value = self.truth_value_at(eval_world)
+        # TODO: is this necessary?
         # prefix_expr_op = self.prop_dict["prefix expression"][0]
         # if 'boxright' in str(prefix_expr_op):
+        #     # print('TEST: CONFIRM')
         #     self.update_verifiers(eval_world)
         indent_num = indent
         possible = self.model_structure.model_setup.possible
         z3_model = self.model_structure.z3_model
         ver_prints = '∅'
         ver_states = {
             bitvec_to_substates(bit, N)
@@ -529,29 +575,33 @@
             for bit in self["falsifiers"]
             if z3_model.evaluate(possible(bit))
             or print_impossible
         }
         if fal_states:
             fal_prints = pretty_set_print(fal_states)
         world_state = bitvec_to_substates(eval_world, N)
+        RED = '\033[31m'
+        GREEN = '\033[32m'
+        RESET = '\033[0m'
+        if indent_num == 1:
+            if truth_value:
+                FULL = GREEN
+                PART = GREEN
+            else:
+                FULL = RED
+                PART = RED
+        else:
+            FULL = '\033[37m'
+            PART = '\033[33m'
         print(
-            f"{'  ' * indent_num}|{self}| = < {ver_prints}, {fal_prints} >"
-            f"  ({truth_value} in {world_state})",
+            f"{'  ' * indent_num}{FULL}|{self}| = < {ver_prints}, {fal_prints} >{RESET}"
+            f"  {PART}({truth_value} in {world_state}){RESET}",
             file=output,
         )
 
-    def truth_value_at(self, eval_world):
-        '''Given a world, returns the truth value of the Proposition at that world.
-        Used in print_verifiers_and_falsifiers.'''
-        for verifier in self["verifiers"]:
-            if bit_part(verifier, eval_world):
-                return True
-        return False
-
-
 def make_model_for(N, premises, conclusions):
     """
     input: N (int of number of atomic states you want in the model)
     returns a function that will solve the premises and conclusions"""
     backslash_premises = [add_backslashes_to_infix(prem) for prem in premises]
     backslash_conclusions = [add_backslashes_to_infix(concl) for concl in conclusions]
     model_setup = ModelSetup(N, backslash_premises, backslash_conclusions)
```

### Comparing `model_checker-0.3.9/src/model_checker/syntax.py` & `model_checker-0.4.1/src/model_checker/syntax.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,17 +8,31 @@
 """
 from z3 import Const, DeclareSort
 
 
 AtomSort = DeclareSort("AtomSort")
 capital_alphabet = {"A", "B", "C", "D", "E", "F", "G", "H", "I", "J", "K", "L", "M",
                     "N", "O", "P", "Q", "R", "S", "T", "U", "V", "W", "X", "Y", "Z",}
-unary_operators = {"\\neg", "neg", "Box", "\\Box", "Diamond", "\\Diamond"}
-binary_operators = {"\\wedge", 'wedge', '\\vee', 'vee', '\\rightarrow', 'rightarrow',
-                    '\\leftrightarrow', 'leftrightarrow', '\\boxright', 'boxright'}
+unary_operators = {
+    "\\neg", "neg",
+    "\\not", "not",
+    "Box", "\\Box",
+    "Diamond", "\\Diamond"
+}
+binary_operators = {
+    "\\wedge", "wedge",
+    "\\vee", "vee",
+    "\\rightarrow", "rightarrow",
+    "\\leftrightarrow", "leftrightarrow",
+    "\\boxright", "boxright",
+    "\\circleright", "circleright",
+    "\\leq", "leq",
+    "\\sqsubseteq", "sqsubseteq",
+    "\\equiv", "equiv"
+}
 all_operators = unary_operators.union(binary_operators)
 
 
 def add_double_backslashes(tokens):
     """adds a double backslash to tokens in the output of tokenize that meet these 3 conditions:
     1. are not capital letters,
     2. do not already have a double backslash in them, AND
```

### Comparing `model_checker-0.3.9/src/model_checker.egg-info/PKG-INFO` & `model_checker-0.4.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,84 +1,113 @@
 Metadata-Version: 2.1
 Name: model-checker
-Version: 0.3.9
-Summary: A hyperintensional theorem prover for counterfactual conditionals and modal operators.
+Version: 0.4.1
+Summary: A hyperintensional theorem prover for modal, counterfactual conditional, constitutive explanatory, and extensional operators.
 Author-email: Benjamin Brast-McKie <benbrastmckie@gmail.com>, Miguel Buitrago <mbuit82@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/benbrastmckie/ModelChecker
 Project-URL: Issues, https://github.com/benbrastmckie/ModelChecker/issues
-Keywords: semantics,Z3,counterfactuals,model checker,theorem prover,hyperintensionality
+Keywords: semantics,Z3,logic,counterfactuals,modality,model checker,theorem prover,hyperintensionality
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: z3-solver
 
 # Model Checker
 
-This project draws on the [Z3](https://github.com/Z3Prover/z3) theorem prover to provide tooling for proving theorems and finding countermodels for counterfactual conditional and modal claims.
+This project draws on the [Z3](https://github.com/Z3Prover/z3) theorem prover to provide tooling for finding countermodels for claims which include modal, counterfactual conditional, constitutive explanatory, and extensional operators.
+The language currently includes the following operators:
+
+  - `neg` for _negation_
+  - `not` for _exclusion_
+  - `wedge` for _conjunction_
+  - `vee` for _disjunction_
+  - `rightarrow` for _material conditional_
+  - `leftrightarrow` for _material biconditional_
+  - `Box` for _necessity_
+  - `Diamond` for _possibility_
+  - `boxright` for the _must counterfactual conditional_
+  - `circleright` for the _might counterfactual conditional_
+  - `leq` for _ground_
+  - `sqsubseteq` for _essence_
+  - `equiv` for _propositional identity_
 
 Accessible [installation instructions](https://github.com/benbrastmckie/ModelChecker?tab=readme-ov-file#installation) are provided in the GitHub repository.
 
 ## Instructions
 
-To generate a test file run `model-checker` without arguments.
-
+To generate a test file run `model-checker` in the terminal without arguments.
 Alternatively, run `model-checker path/to/test_file.py` if the `test_file.py` already exists.
-
 A number of [examples](https://github.com/benbrastmckie/ModelChecker/blob/master/Examples/examples.py) are provided in the GitHub repository.
 
-Each file must specify a set of `premises` which are treated conjunctively, `conclusions` which are treated disjunctively, and the number `N` of atomic states to include in each model.
-
-Optionally, the user can specify the following settings in each file: 
+Each file may specify a set of `premises` which are treated conjunctively, `conclusions` which are treated disjunctively, and the number `N` of atomic states to include in each model.
+If unspecified, `premises = []`, `conclusions = []`, and `N = 3` will be set by default.
+Optionally, the user can specify whether to print the Z3 constraints when a model is found, or the unsatisfiable core when no model exists, as well as an option to save or append the output.
+These settings are specified with the Boolean values `True` and `False`:
 
 - Print all Z3 constraints if a model is found: `print_cons_bool`
 - Print the Z3 unsatisfiable core constraints if no model exists: `print_unsat_core_bool`
 - Print all states including impossible states: `print_impossibe_states_bool`
 - Prompt the user to append the output to the current file in a new file: `save_bool`
 
 Users can override these settings by including the following flags:
 
-- Include `-s` to prompt the user to save the output in a new file.
 - Include `-c` to include Z3 constraints.
 - Include `-i` to print impossible states.
-- Include `-h` to print help information about the programs usage.
+- Include `-s` to prompt the user to save the output in a new file.
 
-## Syntax
+Users can print help information, the current version, and upgrade to the latest version with the following flags:
 
-The language currently includes operators for the counterfactual conditional `boxright`, modal operators for necessity `Box` and possibility `Diamond`, and the extensional operators for conjunction `wedge`, disjunction `vee`, material conditional `rightarrow`, material biconditional `leftrightarrow`, and negation `neg`.
+- Include `-h` to print help information about the programs usage.
+- Include `-v` to print the installed version number.
+- Include `-u` to upgrade to the latest version.
 
-## Semantics
+## Hyperintensional Semantics
 
-The semantics included is hyperintensional insofar as sentences are evaluated at _states_ which may be partial rather than total as in intensional semantic theories.
+The semantics is hyperintensional insofar as sentences are evaluated at _states_ which may be partial rather than total as in intensional semantic theories.
 States are modeled by bitvectors of a specified length (e.g., `#b00101` has length `5`), where _state fusion_ is modeled by the bitwise OR operator `|`.
 For instance, `#b00101 | #b11001 = #b11101`.
 The _atomic states_ have exactly one occurrence of `1` and the _null state_ has no occurrences of `1`.
 The space of states is finite and closed under fusion.
 
-States are named by lowercase letters for the sake of printing readable countermodels.
-Fusions are printed using `.` so that `a.b` is the fusion of the states `a` and `b`.
+States are named by lowercase letters in order to print readable countermodels.
+Fusions are printed using `.` where `a.b` is the fusion of the states `a` and `b`.
 A state `a` is _part_ of a state `b` just in case `a.b = b`.
 States may be either _possible_ or _impossible_ where the null state is required to be possible and every part of a possible state is possible.
 The states `a` and `b` are _compatible_ just in case `a.b` is possible.
 A _world state_ is any state that is both possible and includes every compatible state as a part.
 
 Sentences are assigned _verifier states_ and _falsifier states_ where both the verifiers and falsifiers are required to be closed under fusion.
 A sentence is _true at_ a world state `w` just in case `w` includes a verifier for that sentence as a part and _false at_ `w` just in case `w` includes a falsifier for that sentence as a part.
 In order to ensure that sentence letters have at most one truth-value at each world state, a fusion `a.b` is required to be impossible whenever `a` is verifier for a sentence letter `A` and `b` is a falsifier for `A`.
-Additionally, sentence letters have at least one truth-value at each world state by requiring every possible state to be compatible with either a verifier or falsifier for any sentence letter.
+Additionally, sentence letters are guaranteed to have at least one truth-value at each world state by requiring every possible state to be compatible with either a verifier or falsifier for any sentence letter.
 
-Negated sentences are verified by the falsifiers for the sentence negated and falsified by the verifiers for the sentence negated.
-Conjunctions are verified by the pairwise fusions of verifiers for the conjuncts and falsified by falsifiers for either of the conjuncts or fusions thereof.
-Conjunction and disjunction are dual operators obeying the standard idempotent and De Morgan laws.
+A _negated sentence_ is verified by the falsifiers for the sentence negated and falsified by the verifiers for the sentence negated.
+A _conjunctive sentence_ is verified by the pairwise fusions of verifiers for the conjuncts and falsified by falsifiers for either of the conjuncts or fusions thereof.
+A _disjunctive sentence_ is verified by the verifiers for either disjunct or fusions thereof and falsified by pairwise fusions of falsifiers for the disjuncts.
+Conjunction and disjunction are dual operators obeying the standard idempotence and De Morgan laws.
 The absorption laws do not hold, nor does conjunction distribute over disjunction, nor _vice versa_.
 For a defense of the background theory of hyperintensional propositions, see this [paper](https://link.springer.com/article/10.1007/s10992-021-09612-w).
 
-A modal sentence `Box A` is true at a world just in case every world state includes a part that verifies `A`, where `Diamond A` is true at a world just in case some world state includes a part that verifies `A`.
-Given a world state `w` and state `s`, an `s`_-alternative_ to `w` is any world state to include `s` along with a maximal part of `w` that is compatible with `s` as parts.
-A counterfactual conditional sentences `A boxright B` is true at a world state `w` just in case its consequent is true at any `s`-alternative to `w` for any verifier `s` for the antecedent of the counterfactual.
-
+A _necessity sentence_ `Box A` is true at a world just in case every world state includes a part that verifies `A` and a _possibility sentence_ `Diamond A` is true at a world just in case some world state includes a part that verifies `A`.
+Given a world state `w` and state `s`, an `s`_-alternative_ to `w` is any world state to include as parts both `s` and a maximal part of `w` that is compatible with `s`.
+A _must counterfactual conditional sentences_ `A boxright B` is true at a world state `w` just in case its consequent is true at any `s`-alternative to `w` for any verifier `s` for the antecedent of the counterfactual.
+A _might counterfactual conditional sentences_ `A boxright B` is true at a world state `w` just in case its consequent is true at some `s`-alternative to `w` for some verifier `s` for the antecedent of the counterfactual.
 The semantic theory for counterfactual conditionals is motivated and further elaborated in this [draft](https://github.com/benbrastmckie/ModelChecker/blob/master/Counterfactuals.pdf).
-This account builds on [Fine 2012](https://www.pdcnet.org/jphil/content/jphil_2012_0109_0003_0221_0246) and [Fine 2017](https://link.springer.com/article/10.1007/s10992-016-9413-y).
-More information can be found in the GitHub [repository](https://github.com/benbrastmckie/ModelChecker). 
+This account builds on [Fine 2012](https://www.pdcnet.org/jphil/content/jphil_2012_0109_0003_0221_0246) and [Fine2012a](https://link.springer.com/article/10.1007/s11229-012-0094-y?error=cookies_not_supported&code=5166a4da-1834-438c-9f93-75b61f58b6db).
 
+A _grounding sentence_ `A leq B` may be read '`A` is _sufficient for_ `B`' and an _essence sentence_ `A sqsubseteq B` may be read '`A` is _necessary for_ `B`'.
+A _propositional identity sentence_ `A equiv B` may be read '`A` _just is for_ `B`'.
+The semantics for ground requires every verifier for the antecedent to be a verifier for the consequent, any fusion of a falsifier for the antecedent and consequent to be a falsifier for the consequent, and any falsifier for the consequent to have a part that falsifies the antecedent.
+The semantics for essence requires every fusion of a verifier for the antecedent and consequent to be a verifier for the consequent, any verifier for the consequent must have a part that verifies the antecedent, and every falsifier for the antecedent to be a falsifier for the consequent.
+The semantics for propositional identity requires the two arguments to have the same verifiers and falsifiers.
+All three constitutive operators are interdefinable as indicated below: 
+
+- `A leq B` _iff_ `neg A sqsubseteq neg B` _iff_ `(A vee B) equiv B`.
+- `A sqsubseteq B` _iff_ `neg A leq neg B` _iff_ `(A wedge B) equiv B`
+- `A equiv B` _iff_ `(A leq B) wedge (B leq A)` _iff_ `(A sqsubseteq B) wedge (B sqsubseteq A)`.
+
+Instead of a Boolean lattice as in extensional and intensional semantics theories, the space of hyperintensional propositions forms a non-interlaced bilattice as described in this [paper](https://link.springer.com/article/10.1007/s10992-021-09612-w), building on [Fine 2017](https://link.springer.com/article/10.1007/s10992-016-9413-y).
+
+More information can be found in the GitHub [repository](https://github.com/benbrastmckie/ModelChecker).
```

### Comparing `model_checker-0.3.9/test/test.py` & `model_checker-0.4.1/test/test.py`

 * *Files identical despite different names*

