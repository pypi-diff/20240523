# Comparing `tmp/GeKiM-0.1.0a1.tar.gz` & `tmp/gekim-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GeKiM-0.1.0a1.tar", last modified: Tue Jan  9 19:25:30 2024, max compression
+gzip compressed data, was "gekim-0.2.0.tar", last modified: Wed May 22 22:55:35 2024, max compression
```

## Comparing `GeKiM-0.1.0a1.tar` & `gekim-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,37 @@
-drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-01-09 19:25:30.271681 GeKiM-0.1.0a1/
-drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-01-09 19:25:30.267681 GeKiM-0.1.0a1/GeKiM.egg-info/
--rw-r--r--   0 kyle      (1006) kyle      (1006)     2614 2024-01-09 19:25:30.000000 GeKiM-0.1.0a1/GeKiM.egg-info/PKG-INFO
--rw-rw-r--   0 kyle      (1006) kyle      (1006)      432 2024-01-09 19:25:30.000000 GeKiM-0.1.0a1/GeKiM.egg-info/SOURCES.txt
--rw-rw-r--   0 kyle      (1006) kyle      (1006)        1 2024-01-09 19:25:30.000000 GeKiM-0.1.0a1/GeKiM.egg-info/dependency_links.txt
--rw-rw-r--   0 kyle      (1006) kyle      (1006)       28 2024-01-09 19:25:30.000000 GeKiM-0.1.0a1/GeKiM.egg-info/requires.txt
--rw-rw-r--   0 kyle      (1006) kyle      (1006)        6 2024-01-09 19:25:30.000000 GeKiM-0.1.0a1/GeKiM.egg-info/top_level.txt
--rw-rw-r--   0 kyle      (1006) kyle      (1006)    35149 2024-01-05 21:34:29.000000 GeKiM-0.1.0a1/LICENSE
--rw-r--r--   0 kyle      (1006) kyle      (1006)     2614 2024-01-09 19:25:30.267681 GeKiM-0.1.0a1/PKG-INFO
--rw-rw-r--   0 kyle      (1006) kyle      (1006)     1902 2024-01-09 19:16:17.000000 GeKiM-0.1.0a1/README.md
-drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-01-09 19:25:30.267681 GeKiM-0.1.0a1/gekim/
--rw-rw-r--   0 kyle      (1006) kyle      (1006)      133 2024-01-06 01:51:22.000000 GeKiM-0.1.0a1/gekim/__init__.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)     6537 2024-01-09 19:16:09.000000 GeKiM-0.1.0a1/gekim/n_state.py
-drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-01-09 19:25:30.267681 GeKiM-0.1.0a1/gekim/specialized/
--rw-rw-r--   0 kyle      (1006) kyle      (1006)      262 2024-01-06 01:58:48.000000 GeKiM-0.1.0a1/gekim/specialized/__init__.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)     2435 2024-01-05 21:38:32.000000 GeKiM-0.1.0a1/gekim/specialized/axd.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)     4229 2024-01-05 21:38:46.000000 GeKiM-0.1.0a1/gekim/specialized/four_state.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)     3569 2024-01-05 21:38:40.000000 GeKiM-0.1.0a1/gekim/specialized/four_state_reduced.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)     3050 2024-01-05 21:38:54.000000 GeKiM-0.1.0a1/gekim/specialized/three_state.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)     1780 2024-01-05 20:11:53.000000 GeKiM-0.1.0a1/gekim/specialized/two_state.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)     5981 2024-01-09 19:19:30.000000 GeKiM-0.1.0a1/gekim/utils.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)       38 2024-01-09 19:25:30.271681 GeKiM-0.1.0a1/setup.cfg
--rw-rw-r--   0 kyle      (1006) kyle      (1006)      958 2024-01-09 19:25:08.000000 GeKiM-0.1.0a1/setup.py
-drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-01-09 19:25:30.267681 GeKiM-0.1.0a1/tests/
--rw-rw-r--   0 kyle      (1006) kyle      (1006)     2766 2024-01-09 19:17:01.000000 GeKiM-0.1.0a1/tests/test_nstate.py
+drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-22 22:55:35.887734 gekim-0.2.0/
+drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-22 22:55:35.887734 gekim-0.2.0/GeKiM.egg-info/
+-rw-r--r--   0 kyle      (1006) kyle      (1006)     3068 2024-05-22 22:55:35.000000 gekim-0.2.0/GeKiM.egg-info/PKG-INFO
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)      644 2024-05-22 22:55:35.000000 gekim-0.2.0/GeKiM.egg-info/SOURCES.txt
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)        1 2024-05-22 22:55:35.000000 gekim-0.2.0/GeKiM.egg-info/dependency_links.txt
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)       77 2024-05-22 22:55:35.000000 gekim-0.2.0/GeKiM.egg-info/requires.txt
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)        6 2024-05-22 22:55:35.000000 gekim-0.2.0/GeKiM.egg-info/top_level.txt
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)    35149 2024-01-05 21:34:29.000000 gekim-0.2.0/LICENSE
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)       24 2024-05-22 22:55:03.000000 gekim-0.2.0/MANIFEST.in
+-rw-r--r--   0 kyle      (1006) kyle      (1006)     3068 2024-05-22 22:55:35.887734 gekim-0.2.0/PKG-INFO
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)     2318 2024-05-22 22:34:32.000000 gekim-0.2.0/README.md
+drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-22 22:55:35.887734 gekim-0.2.0/gekim/
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)      131 2024-05-14 23:48:49.000000 gekim-0.2.0/gekim/__init__.py
+drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-22 22:55:35.887734 gekim-0.2.0/gekim/analysis/
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)      136 2024-05-22 20:27:14.000000 gekim-0.2.0/gekim/analysis/__init__.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)     1593 2024-05-15 19:36:51.000000 gekim-0.2.0/gekim/analysis/binding.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)    18178 2024-05-17 22:38:48.000000 gekim-0.2.0/gekim/analysis/covalent_inhibition.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)     7479 2024-05-17 22:41:27.000000 gekim-0.2.0/gekim/analysis/fitting.py
+drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-22 22:55:35.887734 gekim-0.2.0/gekim/schemes/
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)      134 2024-05-22 22:16:32.000000 gekim-0.2.0/gekim/schemes/__init__.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)    20744 2024-05-22 22:22:06.000000 gekim-0.2.0/gekim/schemes/n_state.py
+drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-22 22:55:35.887734 gekim-0.2.0/gekim/simulators/
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)      191 2024-05-14 23:49:52.000000 gekim-0.2.0/gekim/simulators/__init__.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)     1867 2024-05-15 23:52:27.000000 gekim-0.2.0/gekim/simulators/base_simulator.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)     5217 2024-05-17 21:16:04.000000 gekim-0.2.0/gekim/simulators/gillespie.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)    19942 2024-05-17 19:41:44.000000 gekim-0.2.0/gekim/simulators/ode_solver.py
+drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-22 22:55:35.887734 gekim-0.2.0/gekim/utils/
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)      111 2024-05-14 18:10:03.000000 gekim-0.2.0/gekim/utils/__init__.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)     4177 2024-05-16 22:45:21.000000 gekim-0.2.0/gekim/utils/helpers.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)     1877 2024-05-17 22:44:28.000000 gekim-0.2.0/gekim/utils/logging.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)     3553 2024-05-14 18:10:03.000000 gekim-0.2.0/gekim/utils/plotting.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)       93 2024-05-22 21:49:09.000000 gekim-0.2.0/pyproject.toml
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)       77 2024-05-22 21:21:28.000000 gekim-0.2.0/requirements.txt
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)       38 2024-05-22 22:55:35.887734 gekim-0.2.0/setup.cfg
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)      904 2024-05-22 22:45:47.000000 gekim-0.2.0/setup.py
+drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-22 22:55:35.887734 gekim-0.2.0/tests/
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)    13184 2024-05-22 20:43:57.000000 gekim-0.2.0/tests/test_nstate_ode.py
```

### Comparing `GeKiM-0.1.0a1/LICENSE` & `gekim-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `GeKiM-0.1.0a1/README.md` & `gekim-0.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,69 @@
 # GeKiM (Generalized Kinetic Modeler)
 
 ## Description
-GeKiM (Generalized Kinetic Modeler) is a Python package designed for creating, interpreting, and modeling arbitrary kinetic schemes with a focus on covalent inhibition. Schemes are defined by the user in a dictionary of species and transitions. These are then used to create instances of the NState class, which include methods of simulating and analyzing itself. 
-
-The package also contains classes for common schemes, which come with scheme-specific analyses and metrics (e.g., ThreeState.KI, AXD.jacobian).
+GeKiM (Generalized Kinetic Modeler) is a Python package designed for creating, interpreting, and modeling arbitrary kinetic schemes. Schemes are defined by the user in a dictionary of species and transitions, which is used to initialize an instance of the NState class. Choose (or make) and initialize a simulator for the instance and run it. Included applications are focused on covalent inhibition.
 
 ## Installation
-For now, you can only install GeKiM directly from the source code:
+With pip:
+```bash
+pip install gekim
+```
+
+Or directly from the source code (recommended):
 ```bash
 git clone https://github.com/kghaby/GeKiM.git
 cd GeKiM
 pip install .
 ```
 
 ## Usage
-Here is a basic example of how to use GeKiM to create and simulate a kinetic model:
+Here is a basic example of how to use GeKiM to create and simulate a kinetic system:
 ```python
-import gekim
+import gekim as gk
+from gekim.analysis import covalent_inhibition as ci
 
 # Define your kinetic scheme in a configuration dictionary
-config = {
+concI0,concE0 = 100,1
+scheme = {
     'species': {
-        "I": {"conc": 100, "label": "$I$"},
-        "E": {"conc": 1, "label": "$E$"},
-        "EI": {"conc": 0, "label": "$EI$"},
+        "I": {"y0": concI0, "label": "I"},
+        "E": {"y0": concE0, "label": "E"},
+        "EI": {"y0": 0, "label": "EI"},
     },    
     'transitions': {
-        "kon": {"value": 0.01, "from": ["E","I"], "to": ["EI"]},
-        "koff": {"value": 0.1, "from": ["EI"], "to": ["E","I"]},
+        "kon": {"k": 0.01, "source": ["2E","I"], "target": ["EI"]},
+        "koff": {"k": 0.1, "source": ["EI"], "target": ["2E","I"]},
     }
 }
 
-# Create a model
-model = gekim.NState(config)
+# Initialize a system with your schematic dictionary
+system = gk.schemes.NState(scheme)
+
+# Choose a simulator and go. In this example we're doing a deterministic 
+# simulation of the concentrations of each species over time.
+# Note that `system.simulator() = gk.simulators.ODESolver(system)` may be more doc-hint friendly
+system.set_simulator(gk.simulators.ODESolver)
+system.simulator.simulate() 
+
+# Fit the data to experimental models to extract mock-experimental measurements
+final_state = system.species["EI"].simout["y"]
+all_bound = system.sum_species_simout(blacklist=["E","I"])
 
-# Define time points and simulate. In this example we're doing a deterministic simulation of the concentrations of each species. 
-t = np.linspace(0.0001, 1000, 1000)
-model = model.solve_ode(t)
+fit_output = ci.kobs_uplim_fit_to_occ_final_wrt_t(
+    t,final_state,nondefault_params={"Etot":{"fix":concE0}})
 
-# Solution will be columned data of concentrations
-print(model.ode_sol)
+print(f"Fit: {fit_output.fitted_params}\n")
 ```
 For more detailed examples, please refer to the examples directory.
 
 ## Documentation
-API Documentation with examples can be found at TODO.
+Documentation and example notebook(s) are pending.
 
 ## Contributing
 If you have suggestions or want to contribute code, please feel free to open an issue or a pull request.
 
 ## License
-GeKiM is licensed under the GPL-3.0 license.
+GeKiM is licensed under the GPL-3.0.
 
 ## Contact
-kyleghaby@gmail.com
+kyleghaby@gmail.com
```

### Comparing `GeKiM-0.1.0a1/setup.py` & `gekim-0.2.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='GeKiM', 
-    version='0.1.0a1', 
+    version='0.2.0', 
     author='Kyle Ghaby', 
     author_email='kyleghaby@gmail.com',  
     description='Generalized Kinetic Modeler: A Python package for modeling arbitrary kinetic schemes.',  
     long_description=open('README.md').read(),  
     long_description_content_type='text/markdown',
     url='https://github.com/kghaby/GeKiM', 
     packages=find_packages(), 
     include_package_data=True,
     install_requires=required,
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha', 
+        'Development Status :: 4 - Beta', 
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Chemistry',
         'License :: OSI Approved :: GNU General Public License (GPL)',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
     ],
-    python_requires='>=3.8', 
+    python_requires='>=3.9', 
 )
```

