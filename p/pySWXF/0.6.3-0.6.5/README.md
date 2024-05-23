# Comparing `tmp/pyswxf-0.6.3.tar.gz` & `tmp/pyswxf-0.6.5.tar.gz`

## Comparing `pyswxf-0.6.3.tar` & `pyswxf-0.6.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 pyswxf-0.6.3/PyPI-Recovery-Codes-luriol-2023-10-13T13_43_44.046510.txt
--rwxr-xr-x   0        0        0      498 2020-02-02 00:00:00.000000 pyswxf-0.6.3/cbwe.py
--rwxr-xr-x   0        0        0      609 2020-02-02 00:00:00.000000 pyswxf-0.6.3/dot_pypirc
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 pyswxf-0.6.3/instructions
--rwxr-xr-x   0        0        0      724 2020-02-02 00:00:00.000000 pyswxf-0.6.3/pyproject.bak
--rwxr-xr-x   0        0        0      592 2020-02-02 00:00:00.000000 pyswxf-0.6.3/pyproject.new
--rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 pyswxf-0.6.3/token
--rwxr-xr-x   0        0        0     5451 2020-02-02 00:00:00.000000 pyswxf-0.6.3/src/pySWXF/AuI_funs (DESKTOP-09M4OT9's conflicted copy 2024-05-15).py
--rwxr-xr-x   0        0        0     8297 2020-02-02 00:00:00.000000 pyswxf-0.6.3/src/pySWXF/AuI_funs.py
--rwxr-xr-x   0        0        0     3063 2020-02-02 00:00:00.000000 pyswxf-0.6.3/src/pySWXF/NM_clean_NIU_NOKW_Mar26_24_fit4.json
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.6.3/src/pySWXF/__init__.py
--rwxr-xr-x   0        0        0     8356 2020-02-02 00:00:00.000000 pyswxf-0.6.3/src/pySWXF/fluor_fit.py
--rwxr-xr-x   0        0        0     6752 2020-02-02 00:00:00.000000 pyswxf-0.6.3/src/pySWXF/niu_multilayer_fit_params_3_LBL.json
--rwxr-xr-x   0        0        0     6863 2020-02-02 00:00:00.000000 pyswxf-0.6.3/src/pySWXF/refl_funs.py
--rwxr-xr-x   0        0        0    23866 2020-02-02 00:00:00.000000 pyswxf-0.6.3/src/pySWXF/spec_utils.py
--rwxr-xr-x   0        0        0     2747 2020-02-02 00:00:00.000000 pyswxf-0.6.3/src/pySWXF/view_new_multilayer.ipynb
--rwxr-xr-x   0        0        0      952 2020-02-02 00:00:00.000000 pyswxf-0.6.3/src/pySWXF/xray_utils.py
--rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 pyswxf-0.6.3/LICENSE
--rwxr-xr-x   0        0        0     3321 2020-02-02 00:00:00.000000 pyswxf-0.6.3/README.md
--rwxr-xr-x   0        0        0      592 2020-02-02 00:00:00.000000 pyswxf-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     3856 2020-02-02 00:00:00.000000 pyswxf-0.6.3/PKG-INFO
+-rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 pyswxf-0.6.5/PyPI-Recovery-Codes-luriol-2023-10-13T13_43_44.046510.txt
+-rwxr-xr-x   0        0        0      498 2020-02-02 00:00:00.000000 pyswxf-0.6.5/cbwe.py
+-rwxr-xr-x   0        0        0      609 2020-02-02 00:00:00.000000 pyswxf-0.6.5/dot_pypirc
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 pyswxf-0.6.5/instructions
+-rwxr-xr-x   0        0        0      724 2020-02-02 00:00:00.000000 pyswxf-0.6.5/pyproject.bak
+-rwxr-xr-x   0        0        0      592 2020-02-02 00:00:00.000000 pyswxf-0.6.5/pyproject.new
+-rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 pyswxf-0.6.5/token
+-rwxr-xr-x   0        0        0     5451 2020-02-02 00:00:00.000000 pyswxf-0.6.5/src/pySWXF/AuI_funs (DESKTOP-09M4OT9's conflicted copy 2024-05-15).py
+-rwxr-xr-x   0        0        0    10605 2020-02-02 00:00:00.000000 pyswxf-0.6.5/src/pySWXF/AuI_funs.py
+-rwxr-xr-x   0        0        0     3063 2020-02-02 00:00:00.000000 pyswxf-0.6.5/src/pySWXF/NM_clean_NIU_NOKW_Mar26_24_fit4.json
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyswxf-0.6.5/src/pySWXF/__init__.py
+-rwxr-xr-x   0        0        0     8356 2020-02-02 00:00:00.000000 pyswxf-0.6.5/src/pySWXF/fluor_fit.py
+-rwxr-xr-x   0        0        0     6752 2020-02-02 00:00:00.000000 pyswxf-0.6.5/src/pySWXF/niu_multilayer_fit_params_3_LBL.json
+-rwxr-xr-x   0        0        0     6863 2020-02-02 00:00:00.000000 pyswxf-0.6.5/src/pySWXF/refl_funs.py
+-rwxr-xr-x   0        0        0    23866 2020-02-02 00:00:00.000000 pyswxf-0.6.5/src/pySWXF/spec_utils.py
+-rwxr-xr-x   0        0        0     2747 2020-02-02 00:00:00.000000 pyswxf-0.6.5/src/pySWXF/view_new_multilayer.ipynb
+-rwxr-xr-x   0        0        0      952 2020-02-02 00:00:00.000000 pyswxf-0.6.5/src/pySWXF/xray_utils.py
+-rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 pyswxf-0.6.5/LICENSE
+-rwxr-xr-x   0        0        0     3321 2020-02-02 00:00:00.000000 pyswxf-0.6.5/README.md
+-rwxr-xr-x   0        0        0      592 2020-02-02 00:00:00.000000 pyswxf-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0     3856 2020-02-02 00:00:00.000000 pyswxf-0.6.5/PKG-INFO
```

### Comparing `pyswxf-0.6.3/dot_pypirc` & `pyswxf-0.6.5/dot_pypirc`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.3/pyproject.bak` & `pyswxf-0.6.5/pyproject.bak`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.3/pyproject.new` & `pyswxf-0.6.5/pyproject.new`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.3/src/pySWXF/AuI_funs (DESKTOP-09M4OT9's conflicted copy 2024-05-15).py` & `pyswxf-0.6.5/src/pySWXF/AuI_funs (DESKTOP-09M4OT9's conflicted copy 2024-05-15).py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.3/src/pySWXF/AuI_funs.py` & `pyswxf-0.6.5/src/pySWXF/AuI_funs.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,14 +29,73 @@
     else:
         parfilename = MULTILAYER_FIT_OLD
     with importlib.resources.open_text('pySWXF', parfilename) as f:
         params = Parameters()
         params.load(f)
     return(params)
 
+def get_offset_fit_D(th,I,dI,Beam_Energy, fitflag, showfit = True, verbose=True):
+    if verbose:
+        print('varying D instead of angle offset')
+    params = get_params(fitflag)
+    if fitflag == 'NN':
+        if verbose: 
+            print(f'Using flag {fitflag:s} New cell, New multilayer')
+        th_refrac = water_refract(th,Beam_Energy)
+        fitfun = multilayer_ref_new_model
+    elif fitflag == 'OO':
+        if verbose: 
+            print(f'Using flag {fitflag:s} Old cell, Old multilayer')
+            fitfun = multilayer_model_Ti
+        if verbose: 
+            print(f'Side entry sample cell: No refraction correction.')
+        th_refrac = th
+    else: 
+        print(f'not configured for flag {fitflag:s}')
+        exit
+    for key, value in params.items():
+        value.vary = False
+
+    params['I0'].vary = True
+    params['I0'].max = 1e9
+    params['I0'].min = 100
+    params['I0'].value = np.max(I)*3.5
+    params['thoff'].vary = False
+    params['res'].value = .001
+    params['D'].vary = True
+    D0 = params['D'].value
+
+    if verbose: 
+        print('fitting amplitude and offset')
+
+    presim = fitfun.eval(params = params, theta = th_refrac, 
+            Energy = Beam_Energy, water = True, bilayer = True, new_cell = False)
+    cen_sim = np.sum(presim*th)/np.sum(presim)
+    cen_dat = np.sum(I*th)/np.sum(I)
+    params['thoff'].value = cen_dat-cen_sim
+
+    result = fitfun.fit(
+        I,theta = th_refrac, params = params, Energy = Beam_Energy,
+        water = True, bilayer = True, new_cell = False, weights = I*0+1)
+    
+    D = result.params['D'].value
+    
+    if showfit:    
+        ysim=result.eval(theta = th_refrac, 
+            Energy = Beam_Energy, water = True, bilayer = True, new_cell = False)
+        plt.plot(th,I,label='data')
+        plt.plot(th,ysim,'-k',label='fit')
+        plt.locator_params(axis='x', nbins=20)
+        plt.grid()
+        plt.xlabel('th (deg)')
+        plt.ylabel('Reflected Intensity')
+        plt.legend()
+        print(f'D-spacing {D:7.3f} vs. D0 {D0:7.3f}')
+    return(D, result)
+
 def get_offset_fit(th,I,dI,Beam_Energy, fitflag, showfit = True, verbose=True):
     params = get_params(fitflag)
     if fitflag == 'NN':
         if verbose: 
             print(f'Using flag {fitflag:s} New cell, New multilayer')
         th_refrac = water_refract(th,Beam_Energy)
         fitfun = multilayer_ref_new_model
@@ -187,27 +246,32 @@
     zmax : float, the maximum height to consider for plotting
     """
     # Constants
     ANGSTROM = scc.angstrom  # This assumes scc has been properly imported
 
     # Unpacking parameters
     A = [result.params[f'A{i}'].value for i in range(NUM_SLABS)]
+    dA = [result.params[f'A{i}'].stderr for i in range(NUM_SLABS)]
     _, edgelist = get_Zlist(NUM_SLABS, zmax)
 
     # Check that edgelist is sufficiently long
     if len(edgelist) < NUM_SLABS + 1:
         raise ValueError("edgelist does not contain enough entries.")
 
     # Plotting
-    for i, tA in enumerate(A):
+    for i, (tA,tdA) in enumerate(zip(A,dA)):
         edge1 = edgelist[i] / ANGSTROM
         edge2 = edgelist[i + 1] / ANGSTROM
+        CEN = (edge1+edge2)/2
         plt.plot([edge1, edge1], [0, tA], '-k')
         plt.plot([edge1, edge2], [tA, tA], '-k')
         plt.plot([edge2, edge2], [tA, 0], '-k')
+        plt.errorbar([CEN],[tA],[tdA],fmt='ks')
+
+    # now plot error bars
 
     plt.xlabel('height ($\\mathrm{\\AA}$)')
     plt.ylabel('fluorophore concentration')
     plt.title('Fluorophore Concentration Profile')
 
 # Model for three slabs
```

### Comparing `pyswxf-0.6.3/src/pySWXF/NM_clean_NIU_NOKW_Mar26_24_fit4.json` & `pyswxf-0.6.5/src/pySWXF/NM_clean_NIU_NOKW_Mar26_24_fit4.json`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.3/src/pySWXF/fluor_fit.py` & `pyswxf-0.6.5/src/pySWXF/fluor_fit.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.3/src/pySWXF/niu_multilayer_fit_params_3_LBL.json` & `pyswxf-0.6.5/src/pySWXF/niu_multilayer_fit_params_3_LBL.json`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.3/src/pySWXF/refl_funs.py` & `pyswxf-0.6.5/src/pySWXF/refl_funs.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.3/src/pySWXF/spec_utils.py` & `pyswxf-0.6.5/src/pySWXF/spec_utils.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.3/src/pySWXF/view_new_multilayer.ipynb` & `pyswxf-0.6.5/src/pySWXF/view_new_multilayer.ipynb`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.3/src/pySWXF/xray_utils.py` & `pyswxf-0.6.5/src/pySWXF/xray_utils.py`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.3/LICENSE` & `pyswxf-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.3/README.md` & `pyswxf-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `pyswxf-0.6.3/pyproject.toml` & `pyswxf-0.6.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling==1.17.1"]
 build-backend = "hatchling.build"
 [project]
 name = "pySWXF"
-version = "0.6.3"
+version = "0.6.5"
 authors = [
 	{name="Laurence Lurio", email="llurio@niu.edu" },
 ]
 description = "Routines for calculating standing wave x-ray fluorescence and x-ray reflectivity"
 readme = "README.md"
 requires-python = ">3.7"
 classifiers = [
```

### Comparing `pyswxf-0.6.3/PKG-INFO` & `pyswxf-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pySWXF
-Version: 0.6.3
+Version: 0.6.5
 Summary: Routines for calculating standing wave x-ray fluorescence and x-ray reflectivity
 Project-URL: Homepage, https://github.com/pypa/pySWXF
 Project-URL: Bug Tracker, https://github.com/pypa/pySWXF/issues
 Author-email: Laurence Lurio <llurio@niu.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

