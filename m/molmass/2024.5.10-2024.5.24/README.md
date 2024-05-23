# Comparing `tmp/molmass-2024.5.10.tar.gz` & `tmp/molmass-2024.5.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molmass-2024.5.10.tar", last modified: Fri May 10 15:16:35 2024, max compression
+gzip compressed data, was "molmass-2024.5.24.tar", last modified: Thu May 23 19:51:33 2024, max compression
```

## Comparing `molmass-2024.5.10.tar` & `molmass-2024.5.24.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 15:16:35.642995 molmass-2024.5.10/
--rw-rw-rw-   0        0        0     1559 2024-05-10 15:16:34.000000 molmass-2024.5.10/LICENSE
--rw-rw-rw-   0        0        0      305 2023-08-11 03:03:18.000000 molmass-2024.5.10/MANIFEST.in
--rw-rw-rw-   0        0        0     6986 2024-05-10 15:16:35.641995 molmass-2024.5.10/PKG-INFO
--rw-rw-rw-   0        0        0     5877 2024-05-10 15:16:34.000000 molmass-2024.5.10/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-10 15:16:35.638996 molmass-2024.5.10/molmass/
--rw-rw-rw-   0        0        0      206 2022-10-18 17:06:47.000000 molmass-2024.5.10/molmass/__init__.py
--rw-rw-rw-   0        0        0      132 2020-01-01 02:11:19.000000 molmass-2024.5.10/molmass/__main__.py
--rw-rw-rw-   0        0        0    81350 2024-05-10 15:02:07.000000 molmass-2024.5.10/molmass/elements.py
--rw-rw-rw-   0        0        0    44874 2023-03-08 23:01:23.000000 molmass-2024.5.10/molmass/elements_descriptions.py
--rw-rw-rw-   0        0        0    39129 2024-05-10 14:59:59.000000 molmass-2024.5.10/molmass/elements_gui.py
--rw-rw-rw-   0        0        0      355 2010-03-08 22:00:45.000000 molmass-2024.5.10/molmass/icon.png
--rw-rw-rw-   0        0        0    76646 2024-05-10 15:16:29.000000 molmass-2024.5.10/molmass/molmass.py
--rw-rw-rw-   0        0        0        0 2023-08-11 00:10:50.000000 molmass-2024.5.10/molmass/py.typed
--rw-rw-rw-   0        0        0    19551 2024-01-06 17:38:30.000000 molmass-2024.5.10/molmass/web.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:16:35.641995 molmass-2024.5.10/molmass.egg-info/
--rw-rw-rw-   0        0        0     6986 2024-05-10 15:16:35.000000 molmass-2024.5.10/molmass.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      412 2024-05-10 15:16:35.000000 molmass-2024.5.10/molmass.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 15:16:35.000000 molmass-2024.5.10/molmass.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      136 2024-05-10 15:16:35.000000 molmass-2024.5.10/molmass.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       41 2024-05-10 15:16:35.000000 molmass-2024.5.10/molmass.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-10 15:16:35.000000 molmass-2024.5.10/molmass.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 15:16:35.642995 molmass-2024.5.10/setup.cfg
--rw-rw-rw-   0        0        0     2714 2023-08-30 03:54:38.000000 molmass-2024.5.10/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:51:33.635412 molmass-2024.5.24/
+-rw-rw-rw-   0        0        0     1559 2024-05-23 19:51:32.000000 molmass-2024.5.24/LICENSE
+-rw-rw-rw-   0        0        0      305 2023-08-11 03:03:18.000000 molmass-2024.5.24/MANIFEST.in
+-rw-rw-rw-   0        0        0     7061 2024-05-23 19:51:33.635412 molmass-2024.5.24/PKG-INFO
+-rw-rw-rw-   0        0        0     6342 2024-05-23 19:51:32.000000 molmass-2024.5.24/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-23 19:51:33.619265 molmass-2024.5.24/molmass/
+-rw-rw-rw-   0        0        0      206 2022-10-18 17:06:47.000000 molmass-2024.5.24/molmass/__init__.py
+-rw-rw-rw-   0        0        0      132 2020-01-01 02:11:19.000000 molmass-2024.5.24/molmass/__main__.py
+-rw-rw-rw-   0        0        0    81349 2024-05-10 15:21:12.000000 molmass-2024.5.24/molmass/elements.py
+-rw-rw-rw-   0        0        0    44874 2023-03-08 23:01:23.000000 molmass-2024.5.24/molmass/elements_descriptions.py
+-rw-rw-rw-   0        0        0    39129 2024-05-10 14:59:59.000000 molmass-2024.5.24/molmass/elements_gui.py
+-rw-rw-rw-   0        0        0      355 2010-03-08 22:00:45.000000 molmass-2024.5.24/molmass/icon.png
+-rw-rw-rw-   0        0        0    76721 2024-05-23 19:49:49.000000 molmass-2024.5.24/molmass/molmass.py
+-rw-rw-rw-   0        0        0        0 2023-08-11 00:10:50.000000 molmass-2024.5.24/molmass/py.typed
+-rw-rw-rw-   0        0        0    19551 2024-01-06 17:38:30.000000 molmass-2024.5.24/molmass/web.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:51:33.635412 molmass-2024.5.24/molmass.egg-info/
+-rw-rw-rw-   0        0        0     7061 2024-05-23 19:51:33.000000 molmass-2024.5.24/molmass.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      412 2024-05-23 19:51:33.000000 molmass-2024.5.24/molmass.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 19:51:33.000000 molmass-2024.5.24/molmass.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      136 2024-05-23 19:51:33.000000 molmass-2024.5.24/molmass.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       41 2024-05-23 19:51:33.000000 molmass-2024.5.24/molmass.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-23 19:51:33.000000 molmass-2024.5.24/molmass.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 19:51:33.635412 molmass-2024.5.24/setup.cfg
+-rw-rw-rw-   0        0        0     3418 2024-05-20 17:03:50.000000 molmass-2024.5.24/setup.py
```

### Comparing `molmass-2024.5.10/LICENSE` & `molmass-2024.5.24/LICENSE`

 * *Files identical despite different names*

### Comparing `molmass-2024.5.10/PKG-INFO` & `molmass-2024.5.24/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molmass
-Version: 2024.5.10
+Version: 2024.5.24
 Summary: Molecular mass calculations
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/molmass/issues
 Project-URL: Source Code, https://github.com/cgohlke/molmass
@@ -40,24 +40,24 @@
 deficiency due to chemical bonding is not taken into account.
 
 The library includes a database of physicochemical and descriptive properties
 of the chemical elements.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.5.10
+:Version: 2024.5.24
 :DOI: `10.5281/zenodo.7135495 <https://doi.org/10.5281/zenodo.7135495>`_
 
 Quickstart
 ----------
 
 Install the molmass package and all dependencies from the
 `Python Package Index <https://pypi.org/project/molmass/>`_::
 
-    python -m pip install -U molmass[all]
+    python -m pip install -U "molmass[all]"
 
 Print the console script usage::
 
     python -m molmass --help
 
 Run the web application::
 
@@ -80,14 +80,18 @@
 - `Flask <https://pypi.org/project/Flask/>`_ 3.0.3 (optional)
 - `Pandas <https://pypi.org/project/pandas/>`_ 2.2.2 (optional)
 - `wxPython <https://pypi.org/project/wxPython/>`_ 4.2.1 (optional)
 
 Revisions
 ---------
 
+2024.5.24
+
+- Fix GitHub not correctly rendering docstring examples.
+
 2024.5.10
 
 - Add options to disable parsing groups, oligos, fractions, arithmetic (#14).
 - Add Formula.expanded property.
 
 2023.8.30
```

### Comparing `molmass-2024.5.10/README.rst` & `molmass-2024.5.24/molmass.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,37 @@
+Metadata-Version: 2.1
+Name: molmass
+Version: 2024.5.24
+Summary: Molecular mass calculations
+Home-page: https://www.cgohlke.com
+Author: Christoph Gohlke
+Author-email: cgohlke@cgohlke.com
+License: BSD
+Project-URL: Bug Tracker, https://github.com/cgohlke/molmass/issues
+Project-URL: Source Code, https://github.com/cgohlke/molmass
+Platform: any
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Provides-Extra: all
+Requires-Dist: Flask; extra == "all"
+Requires-Dist: pandas; extra == "all"
+Provides-Extra: gui
+Requires-Dist: wxPython>=4.0; extra == "gui"
+
 Molecular mass calculations
 ===========================
 
 Molmass is a Python library, console script, and web application to calculate
 the molecular mass (average, nominal, and isotopic pure), the elemental
 composition, and the mass distribution spectrum of a molecule given by its
 chemical formula, relative element weights, or sequence.
@@ -10,24 +40,24 @@
 deficiency due to chemical bonding is not taken into account.
 
 The library includes a database of physicochemical and descriptive properties
 of the chemical elements.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.5.10
+:Version: 2024.5.24
 :DOI: `10.5281/zenodo.7135495 <https://doi.org/10.5281/zenodo.7135495>`_
 
 Quickstart
 ----------
 
 Install the molmass package and all dependencies from the
 `Python Package Index <https://pypi.org/project/molmass/>`_::
 
-    python -m pip install -U molmass[all]
+    python -m pip install -U "molmass[all]"
 
 Print the console script usage::
 
     python -m molmass --help
 
 Run the web application::
 
@@ -50,14 +80,18 @@
 - `Flask <https://pypi.org/project/Flask/>`_ 3.0.3 (optional)
 - `Pandas <https://pypi.org/project/pandas/>`_ 2.2.2 (optional)
 - `wxPython <https://pypi.org/project/wxPython/>`_ 4.2.1 (optional)
 
 Revisions
 ---------
 
+2024.5.24
+
+- Fix GitHub not correctly rendering docstring examples.
+
 2024.5.10
 
 - Add options to disable parsing groups, oligos, fractions, arithmetic (#14).
 - Add Formula.expanded property.
 
 2023.8.30
```

### Comparing `molmass-2024.5.10/molmass/elements.py` & `molmass-2024.5.24/molmass/elements.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
    atomic-weights-and-isotopic-compositions-relative-atomic-masses
 2. https://en.wikipedia.org/wiki/{element.name}
 
 """
 
 from __future__ import annotations
 
-__version__ = '2024.5.10'
+__version__ = '2024.x.x'
 
 __all__ = [
     'Element',
     'Isotope',
     'Particle',
     'ELECTRON',
     'ELEMENTARY_CHARGE',
```

### Comparing `molmass-2024.5.10/molmass/elements_descriptions.py` & `molmass-2024.5.24/molmass/elements_descriptions.py`

 * *Files identical despite different names*

### Comparing `molmass-2024.5.10/molmass/elements_gui.py` & `molmass-2024.5.24/molmass/elements_gui.py`

 * *Files identical despite different names*

### Comparing `molmass-2024.5.10/molmass/molmass.py` & `molmass-2024.5.24/molmass/molmass.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,24 +40,24 @@
 deficiency due to chemical bonding is not taken into account.
 
 The library includes a database of physicochemical and descriptive properties
 of the chemical elements.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.5.10
+:Version: 2024.5.24
 :DOI: `10.5281/zenodo.7135495 <https://doi.org/10.5281/zenodo.7135495>`_
 
 Quickstart
 ----------
 
 Install the molmass package and all dependencies from the
 `Python Package Index <https://pypi.org/project/molmass/>`_::
 
-    python -m pip install -U molmass[all]
+    python -m pip install -U "molmass[all]"
 
 Print the console script usage::
 
     python -m molmass --help
 
 Run the web application::
 
@@ -80,14 +80,18 @@
 - `Flask <https://pypi.org/project/Flask/>`_ 3.0.3 (optional)
 - `Pandas <https://pypi.org/project/pandas/>`_ 2.2.2 (optional)
 - `wxPython <https://pypi.org/project/wxPython/>`_ 4.2.1 (optional)
 
 Revisions
 ---------
 
+2024.5.24
+
+- Fix GitHub not correctly rendering docstring examples.
+
 2024.5.10
 
 - Add options to disable parsing groups, oligos, fractions, arithmetic (#14).
 - Add Formula.expanded property.
 
 2023.8.30
 
@@ -246,15 +250,15 @@
 ...     e = eval(repr(e))
 ...
 
 """
 
 from __future__ import annotations
 
-__version__ = '2024.5.10'
+__version__ = '2024.5.24'
 
 __all__ = [
     'Composition',
     'CompositionItem',
     'Formula',
     'FormulaError',
     'Spectrum',
```

### Comparing `molmass-2024.5.10/molmass/web.py` & `molmass-2024.5.24/molmass/web.py`

 * *Files identical despite different names*

### Comparing `molmass-2024.5.10/molmass.egg-info/PKG-INFO` & `molmass-2024.5.24/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,9 @@
-Metadata-Version: 2.1
-Name: molmass
-Version: 2024.5.10
-Summary: Molecular mass calculations
-Home-page: https://www.cgohlke.com
-Author: Christoph Gohlke
-Author-email: cgohlke@cgohlke.com
-License: BSD
-Project-URL: Bug Tracker, https://github.com/cgohlke/molmass/issues
-Project-URL: Source Code, https://github.com/cgohlke/molmass
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-Provides-Extra: all
-Requires-Dist: Flask; extra == "all"
-Requires-Dist: pandas; extra == "all"
-Provides-Extra: gui
-Requires-Dist: wxPython>=4.0; extra == "gui"
+..
+  This file is generated by setup.py
 
 Molecular mass calculations
 ===========================
 
 Molmass is a Python library, console script, and web application to calculate
 the molecular mass (average, nominal, and isotopic pure), the elemental
 composition, and the mass distribution spectrum of a molecule given by its
@@ -40,24 +13,24 @@
 deficiency due to chemical bonding is not taken into account.
 
 The library includes a database of physicochemical and descriptive properties
 of the chemical elements.
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2024.5.10
+:Version: 2024.5.24
 :DOI: `10.5281/zenodo.7135495 <https://doi.org/10.5281/zenodo.7135495>`_
 
 Quickstart
 ----------
 
 Install the molmass package and all dependencies from the
 `Python Package Index <https://pypi.org/project/molmass/>`_::
 
-    python -m pip install -U molmass[all]
+    python -m pip install -U "molmass[all]"
 
 Print the console script usage::
 
     python -m molmass --help
 
 Run the web application::
 
@@ -80,14 +53,18 @@
 - `Flask <https://pypi.org/project/Flask/>`_ 3.0.3 (optional)
 - `Pandas <https://pypi.org/project/pandas/>`_ 2.2.2 (optional)
 - `wxPython <https://pypi.org/project/wxPython/>`_ 4.2.1 (optional)
 
 Revisions
 ---------
 
+2024.5.24
+
+- Fix GitHub not correctly rendering docstring examples.
+
 2024.5.10
 
 - Add options to disable parsing groups, oligos, fractions, arithmetic (#14).
 - Add Formula.expanded property.
 
 2023.8.30
 
@@ -164,84 +141,88 @@
 
 Examples
 --------
 
 Calculate the molecular mass, elemental composition, and mass distribution of
 a molecule from its chemical formula:
 
->>> from molmass import Formula
->>> f = Formula('C8H10N4O2')  # Caffeine
->>> f
-Formula('C8H10N4O2')
->>> f.formula  # hill notation
-'C8H10N4O2'
->>> f.empirical
-'C4H5N2O'
->>> f.mass  # average mass
-194.1909...
->>> f.nominal_mass  # == f.isotope.massnumber
-194
->>> f.monoisotopic_mass  # == f.isotope.mass
-194.0803...
->>> f.atoms
-24
->>> f.charge
-0
->>> f.composition().dataframe()
-         Count  Relative mass  Fraction
-Element...
-C            8      96.085920  0.494801
-H           10      10.079410  0.051905
-N            4      56.026812  0.288514
-O            2      31.998810  0.164780
->>> f.spectrum(min_intensity=0.01).dataframe()
-             Relative mass  Fraction  Intensity %         m/z
-Mass number...
-194             194.080376  0.898828   100.000000  194.080376
-195             195.082873  0.092625    10.305100  195.082873
-196             196.084968  0.008022     0.892492  196.084968
-197             197.087214  0.000500     0.055681  197.087214
+.. code-block:: python
+
+    >>> from molmass import Formula
+    >>> f = Formula('C8H10N4O2')  # Caffeine
+    >>> f
+    Formula('C8H10N4O2')
+    >>> f.formula  # hill notation
+    'C8H10N4O2'
+    >>> f.empirical
+    'C4H5N2O'
+    >>> f.mass  # average mass
+    194.1909...
+    >>> f.nominal_mass  # == f.isotope.massnumber
+    194
+    >>> f.monoisotopic_mass  # == f.isotope.mass
+    194.0803...
+    >>> f.atoms
+    24
+    >>> f.charge
+    0
+    >>> f.composition().dataframe()
+             Count  Relative mass  Fraction
+    Element...
+    C            8      96.085920  0.494801
+    H           10      10.079410  0.051905
+    N            4      56.026812  0.288514
+    O            2      31.998810  0.164780
+    >>> f.spectrum(min_intensity=0.01).dataframe()
+                 Relative mass  Fraction  Intensity %         m/z
+    Mass number...
+    194             194.080376  0.898828   100.000000  194.080376
+    195             195.082873  0.092625    10.305100  195.082873
+    196             196.084968  0.008022     0.892492  196.084968
+    197             197.087214  0.000500     0.055681  197.087214
 
 Access physicochemical and descriptive properties of the chemical elements:
 
->>> from molmass import ELEMENTS, Element
->>> e = ELEMENTS['C']
->>> e
-Element(
-    6, 'C', 'Carbon',
-    group=14, period=2, block='p', series=1,
-    mass=12.01074, eleneg=2.55, eleaffin=1.262118,
-    covrad=0.77, atmrad=0.91, vdwrad=1.7,
-    tboil=5100.0, tmelt=3825.0, density=3.51,
-    eleconfig='[He] 2s2 2p2',
-    oxistates='4*, 2, -4*',
-    ionenergy=(
-        11.2603, 24.383, 47.877, 64.492, 392.077,
-        489.981,
-    ),
-    isotopes={
-        12: Isotope(12.0, 0.9893, 12),
-        13: Isotope(13.00335483507, 0.0107, 13),
-    },
-)
->>> e.number
-6
->>> e.symbol
-'C'
->>> e.name
-'Carbon'
->>> e.description
-'Carbon is a member of group 14 of the periodic table...'
->>> e.eleconfig
-'[He] 2s2 2p2'
->>> e.eleconfig_dict
-{(1, 's'): 2, (2, 's'): 2, (2, 'p'): 2}
->>> str(ELEMENTS[6])
-'Carbon'
->>> len(ELEMENTS)
-109
->>> sum(e.mass for e in ELEMENTS)
-14693.181589001...
->>> for e in ELEMENTS:
-...     e.validate()
-...     e = eval(repr(e))
-...
+.. code-block:: python
+
+    >>> from molmass import ELEMENTS, Element
+    >>> e = ELEMENTS['C']
+    >>> e
+    Element(
+        6, 'C', 'Carbon',
+        group=14, period=2, block='p', series=1,
+        mass=12.01074, eleneg=2.55, eleaffin=1.262118,
+        covrad=0.77, atmrad=0.91, vdwrad=1.7,
+        tboil=5100.0, tmelt=3825.0, density=3.51,
+        eleconfig='[He] 2s2 2p2',
+        oxistates='4*, 2, -4*',
+        ionenergy=(
+            11.2603, 24.383, 47.877, 64.492, 392.077,
+            489.981,
+        ),
+        isotopes={
+            12: Isotope(12.0, 0.9893, 12),
+            13: Isotope(13.00335483507, 0.0107, 13),
+        },
+    )
+    >>> e.number
+    6
+    >>> e.symbol
+    'C'
+    >>> e.name
+    'Carbon'
+    >>> e.description
+    'Carbon is a member of group 14 of the periodic table...'
+    >>> e.eleconfig
+    '[He] 2s2 2p2'
+    >>> e.eleconfig_dict
+    {(1, 's'): 2, (2, 's'): 2, (2, 'p'): 2}
+    >>> str(ELEMENTS[6])
+    'Carbon'
+    >>> len(ELEMENTS)
+    109
+    >>> sum(e.mass for e in ELEMENTS)
+    14693.181589001...
+    >>> for e in ELEMENTS:
+    ...     e.validate()
+    ...     e = eval(repr(e))
+    ...
```

### Comparing `molmass-2024.5.10/setup.py` & `molmass-2024.5.24/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,53 +4,72 @@
 
 import re
 import sys
 
 from setuptools import setup
 
 
-def search(pattern, code, flags=0):
-    # return first match for pattern in code
-    match = re.search(pattern, code, flags)
+def search(pattern, string, flags=0):
+    """Return first match of pattern in string."""
+    match = re.search(pattern, string, flags)
     if match is None:
         raise ValueError(f'{pattern!r} not found')
     return match.groups()[0]
 
 
+def fix_docstring_examples(docstring):
+    """Return docstring with examples fixed for GitHub."""
+    start = True
+    indent = False
+    lines = ['..', '  This file is generated by setup.py', '']
+    for line in docstring.splitlines():
+        if not line.strip():
+            start = True
+            indent = False
+        if line.startswith('>>> '):
+            indent = True
+            if start:
+                lines.extend(['.. code-block:: python', ''])
+                start = False
+        lines.append(('    ' if indent else '') + line)
+    return '\n'.join(lines)
+
+
 with open('molmass/molmass.py', encoding='utf-8') as fh:
     code = fh.read()
 
 version = search(r"__version__ = '(.*?)'", code).replace('.x.x', '.dev0')
 
 description = search(r'"""(.*)\.(?:\r\n|\r|\n)', code)
 
 readme = search(
     r'(?:\r\n|\r|\n){2}"""(.*)"""(?:\r\n|\r|\n){2}from __future__',
     code,
     re.MULTILINE | re.DOTALL,
 )
-
 readme = '\n'.join(
     [description, '=' * len(description)] + readme.splitlines()[1:]
 )
 
-license = search(
-    r'(# Copyright.*?(?:\r\n|\r|\n))(?:\r\n|\r|\n)+""',
-    code,
-    re.MULTILINE | re.DOTALL,
-)
+if 'sdist' in sys.argv:
+    # update README, LICENSE, and CHANGES files
 
-license = license.replace('# ', '').replace('#', '')
+    with open('README.rst', 'w', encoding='utf-8') as fh:
+        fh.write(fix_docstring_examples(readme))
+
+    license = search(
+        r'(# Copyright.*?(?:\r\n|\r|\n))(?:\r\n|\r|\n)+""',
+        code,
+        re.MULTILINE | re.DOTALL,
+    )
+    license = license.replace('# ', '').replace('#', '')
 
-if 'sdist' in sys.argv:
     with open('LICENSE', 'w', encoding='utf-8') as fh:
         fh.write('BSD 3-Clause License\n\n')
         fh.write(license)
-    with open('README.rst', 'w', encoding='utf-8') as fh:
-        fh.write(readme)
 
 setup(
     name='molmass',
     version=version,
     license='BSD',
     description=description,
     long_description=readme,
```

