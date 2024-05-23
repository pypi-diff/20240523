# Comparing `tmp/pywdpa-0.1.5.tar.gz` & `tmp/pywdpa-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywdpa-0.1.5.tar", last modified: Fri Mar 12 16:59:11 2021, max compression
+gzip compressed data, was "pywdpa-0.1.6.tar", last modified: Thu May 23 07:30:21 2024, max compression
```

## Comparing `pywdpa-0.1.5.tar` & `pywdpa-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-12 16:59:11.970529 pywdpa-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (116)      837 2021-03-12 16:59:08.000000 pywdpa-0.1.5/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (116)    35149 2021-03-12 16:59:08.000000 pywdpa-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       56 2021-03-12 16:59:08.000000 pywdpa-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     6195 2021-03-12 16:59:11.970529 pywdpa-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4268 2021-03-12 16:59:08.000000 pywdpa-0.1.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-12 16:59:11.970529 pywdpa-0.1.5/pywdpa/
--rw-r--r--   0 runner    (1001) docker     (116)      563 2021-03-12 16:59:08.000000 pywdpa-0.1.5/pywdpa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      550 2021-03-12 16:59:08.000000 pywdpa-0.1.5/pywdpa/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2374 2021-03-12 16:59:08.000000 pywdpa-0.1.5/pywdpa/get_token.py
--rw-r--r--   0 runner    (1001) docker     (116)     5285 2021-03-12 16:59:08.000000 pywdpa-0.1.5/pywdpa/get_wdpa.py
--rwxr-xr-x   0 runner    (1001) docker     (116)      650 2021-03-12 16:59:08.000000 pywdpa-0.1.5/pywdpa/pywdpa-runner.py
--rw-r--r--   0 runner    (1001) docker     (116)      754 2021-03-12 16:59:08.000000 pywdpa-0.1.5/pywdpa/pywdpa.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-12 16:59:11.970529 pywdpa-0.1.5/pywdpa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     6195 2021-03-12 16:59:11.000000 pywdpa-0.1.5/pywdpa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      437 2021-03-12 16:59:11.000000 pywdpa-0.1.5/pywdpa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-03-12 16:59:11.000000 pywdpa-0.1.5/pywdpa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       47 2021-03-12 16:59:11.000000 pywdpa-0.1.5/pywdpa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-03-12 16:59:11.000000 pywdpa-0.1.5/pywdpa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       84 2021-03-12 16:59:11.000000 pywdpa-0.1.5/pywdpa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2021-03-12 16:59:11.000000 pywdpa-0.1.5/pywdpa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       67 2021-03-12 16:59:11.974529 pywdpa-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2211 2021-03-12 16:59:08.000000 pywdpa-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-12 16:59:11.970529 pywdpa-0.1.5/test/
--rw-r--r--   0 runner    (1001) docker     (116)      871 2021-03-12 16:59:08.000000 pywdpa-0.1.5/test/test_get_token.py
--rw-r--r--   0 runner    (1001) docker     (116)      576 2021-03-12 16:59:08.000000 pywdpa-0.1.5/test/test_get_wdpa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:30:21.551177 pywdpa-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-23 07:30:19.000000 pywdpa-0.1.6/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-23 07:30:19.000000 pywdpa-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-23 07:30:19.000000 pywdpa-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-05-23 07:30:21.551177 pywdpa-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-05-23 07:30:19.000000 pywdpa-0.1.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:30:21.547177 pywdpa-0.1.6/pywdpa/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-23 07:30:19.000000 pywdpa-0.1.6/pywdpa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-23 07:30:19.000000 pywdpa-0.1.6/pywdpa/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-23 07:30:19.000000 pywdpa-0.1.6/pywdpa/get_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-05-23 07:30:19.000000 pywdpa-0.1.6/pywdpa/get_wdpa.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      650 2024-05-23 07:30:19.000000 pywdpa-0.1.6/pywdpa/pywdpa-runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-23 07:30:19.000000 pywdpa-0.1.6/pywdpa/pywdpa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:30:21.551177 pywdpa-0.1.6/pywdpa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-05-23 07:30:21.000000 pywdpa-0.1.6/pywdpa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-23 07:30:21.000000 pywdpa-0.1.6/pywdpa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 07:30:21.000000 pywdpa-0.1.6/pywdpa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 07:30:21.000000 pywdpa-0.1.6/pywdpa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 07:30:21.000000 pywdpa-0.1.6/pywdpa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-23 07:30:21.000000 pywdpa-0.1.6/pywdpa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 07:30:21.000000 pywdpa-0.1.6/pywdpa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-23 07:30:21.551177 pywdpa-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-23 07:30:19.000000 pywdpa-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:30:21.551177 pywdpa-0.1.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-23 07:30:19.000000 pywdpa-0.1.6/test/test_get_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-23 07:30:19.000000 pywdpa-0.1.6/test/test_get_wdpa.py
```

### Comparing `pywdpa-0.1.5/CHANGELOG.rst` & `pywdpa-0.1.6/CHANGELOG.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 Changelog
 *********
 
+pywdpa 0.1.6
+============
+
+* Adding workflow for GitHub pages.
+* Website update.
+
 pywdpa 0.1.5
 ============
 
 * Including more attributes (in particular status and date).
 
 pywdpa 0.1.4
 ============
 
-* Correcting a bug to include multipolygons
-* Get started notebook
-* Web-site update
+* Correcting a bug to include multipolygons.
+* Get started notebook.
+* Website update.
 
 pywdpa 0.1.2 to 0.1.3
 =====================
 
 * Minor changes.
 * New logo.
 * New website using Sphinx.
```

### Comparing `pywdpa-0.1.5/LICENSE` & `pywdpa-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pywdpa-0.1.5/PKG-INFO` & `pywdpa-0.1.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,148 +1,199 @@
 Metadata-Version: 2.1
 Name: pywdpa
-Version: 0.1.5
+Version: 0.1.6
 Summary: Easy access to world's protected areas
 Home-page: https://ecology.ghislainv.fr/pywdpa
 Author: Ghislain Vieilledent
 Author-email: ghislain.vieilledent@cirad.fr
 License: GPLv3
 Project-URL: Documentation, https://ecology.ghislainv.fr/pywdpa
 Project-URL: Source, https://github.com/ghislainv/pywdpa/
 Project-URL: Traker, https://github.com/ghislainv/pywdpa/issues
-Description: ..
-           # ==============================================================================
-           # author          :Ghislain Vieilledent
-           # email           :ghislain.vieilledent@cirad.fr, ghislainv@gmail.com
-           # web             :https://ecology.ghislainv.fr
-           # license         :GPLv3
-           # ==============================================================================
-        
-        .. image:: https://ecology.ghislainv.fr/pywdpa/_static/logo-pywdpa.svg
-           :align: right
-           :target: https://ecology.ghislainv.fr/pywdpa
-           :alt: Logo pywdpa
-           :width: 140px
-        	   
-        ``pywdpa`` Python package
-        *************************
-        
-        
-        |Python version| |PyPI version| |GitHub Actions| |License| |Zenodo|
-        
-        
-        Overview
-        ========
-        
-        The ``pywdpa`` Python package is an interface to the World Database on
-        Protected Areas (WDPA) hosted on the Protected Planet website at
-        `<https://www.protectedplanet.net>`_. The ``pywdpa`` package provides
-        functions to download shapefiles of protected areas (PA) for any
-        countries with an iso3 code using the Protected Planet API at
-        `<https://api.protectedplanet.net>`_. The ``pywdpa`` package
-        translates some functions of the R package ``worldpa``
-        (`<https://github.com/FRBCesab/worldpa>`_) in the Python language.
-        
-        .. image:: https://ecology.ghislainv.fr/pywdpa/_static/protected-planet.jpg
-           :align: center
-           :target: https://ecology.ghislainv.fr/pywdpa
-           :alt: protected-planet
-        
-        Terms and conditions
-        ====================
-        
-        You must ensure that the following citation is always clearly
-        reproduced in any publication or analysis involving the Protected
-        Planet Materials in any derived form or format:
-        
-        ..
-           
-            UNEP-WCMC and IUCN (\ ``YEAR``\ ) Protected Planet: The World
-            Database on Protected Areas (WDPA). Cambridge, UK: UNEP-WCMC and
-            IUCN. Available at: www.protectedplanet.net (dataset downloaded the
-            ``YEAR/MONTH``\ ).
-        
-        
-        For further details on terms and conditions of the WDPA usage, please
-        visit the page:
-        `<https://www.protectedplanet.net/c/terms-and-conditions>`_.
-        
-        Prerequisites
-        =============
-        
-        This package uses the Protected Planet API to access data on world
-        protected areas. You must first have obtained a Personal API Token by
-        filling in the form available at
-        `<https://api.protectedplanet.net/request>`_. Then you need to set an
-        environment variable (we recommend using the name ``WDPA_KEY``\ )
-        using either the command ``os.environ["WDPA_KEY"]="your_token"`` or
-        `python-dotenv <https://github.com/theskumar/python-dotenv>`_.
-        
-        Installation
-        ============
-        
-        The easiest way to install the ``pywdpa`` Python package is via `pip <https://pip.pypa.io/en/stable/>`_:
-        
-        .. code-block:: bash
-        
-           $ # For version on PyPI
-           $ python -m pip install pywdpa
-        
-        or 
-        
-        .. code-block:: bash
-        
-           $ # For development version on GitHub
-           $ python -m pip install https://github.com/ghislainv/pywdpa/archive/master.zip
-        
-        but you can also install ``pywdpa`` executing the ``setup.py`` file:
-        
-        .. code-block:: bash
-        
-           $ git clone https://github.com/ghislainv/pywdpa
-           $ cd pywdpa
-           $ python setup.py install
-        
-        Contributing
-        ============
-        
-        The ``pywdpa`` Python package is Open Source and released under
-        the `GNU GPL version 3 license
-        <https://ecology.ghislainv.fr/pywdpa/license.html>`__. Anybody
-        who is interested can contribute to the package development following
-        our `Community guidelines
-        <https://ecology.ghislainv.fr/pywdpa/contributing.html>`__. Every
-        contributor must agree to follow the project's `Code of conduct
-        <https://ecology.ghislainv.fr/pywdpa/code_of_conduct.html>`__.
-           
-        .. |Python version| image:: https://img.shields.io/pypi/pyversions/pywdpa?logo=python&logoColor=ffd43b&color=306998
-           :target: https://pypi.org/project/pywdpa
-           :alt: Python version
-        
-        .. |PyPI version| image:: https://img.shields.io/pypi/v/pywdpa
-           :target: https://pypi.org/project/pywdpa
-           :alt: PyPI version
-        
-        .. |GitHub Actions| image:: https://github.com/ghislainv/pywdpa/workflows/PyPkg/badge.svg
-           :target: https://github.com/ghislainv/pywdpa/actions
-           :alt: GitHub Actions
-        	 
-        .. |License| image:: https://img.shields.io/badge/licence-GPLv3-8f10cb.svg
-           :target: https://www.gnu.org/licenses/gpl-3.0.html
-           :alt: License GPLv3
-        
-        .. |Zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4275513.svg
-           :target: https://doi.org/10.5281/zenodo.4275513
-           :alt: Zenodo
-        
-        
 Keywords: protected areas wdpa world database protected areas
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=2.7
+Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: gdal
+Requires-Dist: requests
 Provides-Extra: interactive
+Requires-Dist: jupyter; extra == "interactive"
+Requires-Dist: python-dotenv; extra == "interactive"
+Requires-Dist: geopandas; extra == "interactive"
+Requires-Dist: descartes; extra == "interactive"
+Requires-Dist: folium; extra == "interactive"
+
+..
+   # ==============================================================================
+   # author          :Ghislain Vieilledent
+   # email           :ghislain.vieilledent@cirad.fr, ghislainv@gmail.com
+   # web             :https://ecology.ghislainv.fr
+   # license         :GPLv3
+   # ==============================================================================
+
+.. image:: https://ecology.ghislainv.fr/pywdpa/_static/logo-pywdpa.svg
+   :align: right
+   :target: https://ecology.ghislainv.fr/pywdpa
+   :alt: Logo pywdpa
+   :width: 140px
+	   
+``pywdpa`` Python package
+*************************
+
+
+|Python version| |PyPI version| |GitHub Actions| |License| |Zenodo|
+
+
+Overview
+========
+
+The ``pywdpa`` Python package is an interface to the World Database on
+Protected Areas (WDPA) hosted on the Protected Planet website at
+`<https://www.protectedplanet.net>`_. The ``pywdpa`` package provides
+functions to download shapefiles of protected areas (PA) for any
+countries with an iso3 code using the Protected Planet API at
+`<https://api.protectedplanet.net>`_. The ``pywdpa`` package
+translates some functions of the R package ``worldpa``
+(`<https://github.com/FRBCesab/worldpa>`_) in the Python language.
+
+.. image:: https://ecology.ghislainv.fr/pywdpa/_static/banner_pywdpa.png
+   :align: center
+   :target: https://ecology.ghislainv.fr/pywdpa
+   :alt: protected-planet
+
+Terms and conditions
+====================
+
+You must ensure that the following citation is always clearly
+reproduced in any publication or analysis involving the Protected
+Planet Materials in any derived form or format:
+
+..
+   
+    UNEP-WCMC and IUCN (\ ``YEAR``\ ) Protected Planet: The World
+    Database on Protected Areas (WDPA). Cambridge, UK: UNEP-WCMC and
+    IUCN. Available at: www.protectedplanet.net (dataset downloaded the
+    ``YEAR/MONTH``\ ).
+
+
+For further details on terms and conditions of the WDPA usage, please
+visit the page: `<https://www.protectedplanet.net/en/legal>`_.
+
+Prerequisites
+=============
+
+Access to Protected Planet API
+------------------------------
+
+This package uses the Protected Planet API to access data on world
+protected areas. You must first have obtained a Personal API Token by
+filling in the form available at
+`<https://api.protectedplanet.net/request>`_. Then you need to set an
+environment variable (we recommend using the name ``WDPA_KEY``\ )
+using either the command ``os.environ["WDPA_KEY"]="your_token"`` or
+`python-dotenv <https://github.com/theskumar/python-dotenv>`_.
+
+GDAL
+----
+
+GDAL must be installed on your system.
+
+To install GDAL on Windows, use the `OSGeo4W <https://trac.osgeo.org/osgeo4w/>`_ network installer. OSGeo4W is a binary distribution of a broad set of open source geospatial software for Windows environments (Windows 11 down to 7). Select *Express Install* and install GDAL. Several Gb of space will be needed on disk to install this programs. This will also install *OSGeo4W Shell* to execute command lines.
+
+To install GDAL on other systems, use your package manager, for example ``apt`` for Debian/Ubuntu Linux distributions.
+
+.. code:: shell
+
+    sudo apt update
+    sudo apt install gdal-bin libgdal-dev
+
+After installing GDAL, you can test the installation by running ``gdalinfo --version`` in the command prompt or terminal, which should display the installed GDAL version.
+
+
+Installation
+============
+
+The easiest way to install the ``pywdpa`` Python package is via `pip <https://pip.pypa.io/en/stable/>`_ in the *OSGeo4W Shell* for Windows or in a virtual environment for Linux.
+
+For Linux, create and activate a virtual environment before install ``pywdpa`` with ``pip``:
+
+.. code-block:: shell
+
+   cd ~
+   # Create a directory for virtual environments
+   mkdir venvs
+   # Create the virtual environment with venv
+   python3 -m venv ~/venvs/venv-pywdpa
+   # Activate (start) the virtual environment
+   source ~/venvs/venv-pywdpa/bin/activate
+
+Install Python dependencies and ``pywdpa`` in the *OSGeo4W Shell* or in the newly created virtual environment:
+   
+.. code-block:: shell
+   
+   # Upgrade pip, setuptools, and wheel
+   python3 -m pip install --upgrade pip setuptools wheel
+   # Install numpy
+   python3 -m numpy
+   # Install gdal Python bindings (the correct version)
+   python3 -m pip install gdal==$(gdal-config --version)
+   # Install pywdpa. This will install all other dependencies
+   python3 -m pip install pywdpa
+
+If you want to install the development version of ``pywdpa``, replace the last line with:
+
+.. code-block:: shell
+
+   python3 -m pip install https://github.com/ghislainv/pywdpa/archive/master.zip
+
+To deactivate and delete the virtual environment:
+
+.. code-block:: shell
+		
+   deactivate
+   rm -R ~/venvs/venv-pywdpa # Just remove the repository
+
+In case of problem while installing GDAL Python bindings, try the following command:
+
+.. code-block:: shell
+		
+   python3 -m pip install  --no-cache-dir --force-reinstall gdal==$(gdal-config --version)
+
+
+Contributing
+============
+
+The ``pywdpa`` Python package is Open Source and released under
+the `GNU GPL version 3 license
+<https://ecology.ghislainv.fr/pywdpa/license.html>`__. Anybody
+who is interested can contribute to the package development following
+our `Community guidelines
+<https://ecology.ghislainv.fr/pywdpa/contributing.html>`__. Every
+contributor must agree to follow the project's `Code of conduct
+<https://ecology.ghislainv.fr/pywdpa/code_of_conduct.html>`__.
+   
+.. |Python version| image:: https://img.shields.io/pypi/pyversions/pywdpa?logo=python&logoColor=ffd43b&color=306998
+   :target: https://pypi.org/project/pywdpa
+   :alt: Python version
+
+.. |PyPI version| image:: https://img.shields.io/pypi/v/pywdpa
+   :target: https://pypi.org/project/pywdpa
+   :alt: PyPI version
+
+.. |GitHub Actions| image:: https://github.com/ghislainv/pywdpa/workflows/PyPkg/badge.svg
+   :target: https://github.com/ghislainv/pywdpa/actions
+   :alt: GitHub Actions
+	 
+.. |License| image:: https://img.shields.io/badge/licence-GPLv3-8f10cb.svg
+   :target: https://www.gnu.org/licenses/gpl-3.0.html
+   :alt: License GPLv3
+
+.. |Zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4275513.svg
+   :target: https://doi.org/10.5281/zenodo.4275513
+   :alt: Zenodo
+
```

### Comparing `pywdpa-0.1.5/pywdpa/__main__.py` & `pywdpa-0.1.6/pywdpa/__main__.py`

 * *Files identical despite different names*

### Comparing `pywdpa-0.1.5/pywdpa/get_token.py` & `pywdpa-0.1.6/pywdpa/get_token.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,20 @@
 # email           :ghislain.vieilledent@cirad.fr, ghislainv@gmail.com
 # web             :https://ecology.ghislainv.fr
 # python_version  :>=2.7
 # license         :GPLv3
 # ==============================================================================
 
 # Import
-from __future__ import division, print_function  # Python 3 compatibility
 import os
 import requests
 
 
 # get_token()
 def get_token(key="WDPA_KEY"):
-
     r"""Check Protected Planet API token.
 
     This function checks if the user has stored a valid Protected
     Planet API token as an environment variable file under the
     key ``"WDPA_KEY"``\ .
 
     Before using this package for the first time, the user must follow
@@ -45,15 +43,16 @@
         msg = ("Missing WDPA API token. Please ensure that:{sep}"
                "1) You completed this form [https://api.protectedplanet.net/request] "
                "to get the token.{sep}"
                "2) You stored the value as an environment variable with the "
                "recommended name WDPA_KEY.").format(sep="\n")
         return msg
 
-    response = requests.get("https://api.protectedplanet.net/test?token=" + wdpa_key)
+    response = requests.get("https://api.protectedplanet.net/"
+                            f"test?token={wdpa_key}", timeout=None)
 
     if response.status_code == 401:
         msg = ("Invalid WDPA API token. Please ensure that:{sep}"
                "1) You completed this form [https://api.protectedplanet.net/request] "
                "to get the token.{sep}"
                "2) You stored the value as an environment variable with the "
                "recommended name WDPA_KEY.").format(sep="\n")
```

### Comparing `pywdpa-0.1.5/pywdpa/get_wdpa.py` & `pywdpa-0.1.6/pywdpa/get_wdpa.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,29 +6,28 @@
 # email           :ghislain.vieilledent@cirad.fr, ghislainv@gmail.com
 # web             :https://ecology.ghislainv.fr
 # python_version  :>=2.7
 # license         :GPLv3
 # ==============================================================================
 
 # Import
-from __future__ import division, print_function  # Python 3 compatibility
 import os
 
 import json
 import numpy as np
 from osgeo import ogr
 import requests
 
 from .get_token import get_token
 
-# get_wdpa()
-
 
 def get_wdpa(iso3, output_dir="."):
-    """This function downloads protected areas for one country using the
+    """Get protected areas for a country from WDPA.
+
+    This function downloads protected areas for one country using the
     WDPA API. Protected areas defined by a point are not
     considered. The shapefile is written on the hard drive (in the
     current directory).
 
     :param iso3: The ISO-3 code of the country.
 
     :param output_dir: Directory used for download.
@@ -36,15 +35,15 @@
     """
 
     os.environ["SHAPE_ENCODING"] = "utf-8"
     base_url = "https://api.protectedplanet.net/"
     category = "v3/countries/"
     wdpa_token = get_token()
     request = base_url + category + iso3 + "?token=" + wdpa_token
-    response = requests.get(request)
+    response = requests.get(request, timeout=None)
 
     if response.status_code == 404:
         return "Invalid ISO-3 code"
 
     response = json.loads(response.text)  # Equivalent to response.json()
 
     pas_count = response["country"]["pas_count"]
@@ -81,15 +80,15 @@
         for p in pages:
             request = "".join(
                 [base_url, category, "?token=", wdpa_token,
                  "&with_geometry=", "true", "&country=",
                  iso3, "&per_page=", str(50), "&page=", str(p+1)]
             )
 
-            response = requests.get(request)
+            response = requests.get(request, timeout=None)
             response = response.json()
             response = response["protected_areas"]
 
             # Number of protected areas
             npa = len(response)
 
             # Loop on protected areas
@@ -106,16 +105,16 @@
                 #     area = np.float(pa["reported_area"])
                 #     buffer_size = int(round(np.sqrt(area/np.pi)*1000))
                 #     g = g.Buffer(buffer_size)
 
                 # If polygon, add feature
                 if g.GetGeometryName() in ["POLYGON", "MULTIPOLYGON"]:
                     # Create feature with geometry and attributes
-                    featureDefn = layer.GetLayerDefn()
-                    feature = ogr.Feature(featureDefn)
+                    feature_defn = layer.GetLayerDefn()
+                    feature = ogr.Feature(feature_defn)
                     feature.SetGeometry(g)
                     feature.SetField("wdpa_id", pa["wdpa_id"])
                     feature.SetField("pa_name", pa["name"])
                     feature.SetField(
                         "orig_name", pa["original_name"])
                     feature.SetField("ctry_iso3", iso3)
                     feature.SetField("owner_type", pa["owner_type"])
```

### Comparing `pywdpa-0.1.5/pywdpa/pywdpa-runner.py` & `pywdpa-0.1.6/pywdpa/pywdpa-runner.py`

 * *Files identical despite different names*

### Comparing `pywdpa-0.1.5/pywdpa/pywdpa.py` & `pywdpa-0.1.6/pywdpa/pywdpa.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 # web             :https://ecology.ghislainv.fr
 # python_version  :>=2.7
 # license         :GPLv3
 # ==============================================================================
 
 import sys
 
+import pywdpa
 from .get_wdpa import get_wdpa
 
-__version__ = "0.1.5"
-
 
 def main():
     """
     pywdpa.pywdpa: provides entry point main().
     """
     isocode = sys.argv[1]
-    print("Executing pywdpa version {}.".format(__version__))
-    print("For country with isocode: {}.".format(isocode))
+    print(pywdpa.__doc__)
+    print(f"version {pywdpa.__version__}.")
+    print(f"Country isocode: {isocode}.")
     get_wdpa(isocode)
-    return None
+
 
 # End
```

### Comparing `pywdpa-0.1.5/pywdpa.egg-info/PKG-INFO` & `pywdpa-0.1.6/pywdpa.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,148 +1,199 @@
 Metadata-Version: 2.1
 Name: pywdpa
-Version: 0.1.5
+Version: 0.1.6
 Summary: Easy access to world's protected areas
 Home-page: https://ecology.ghislainv.fr/pywdpa
 Author: Ghislain Vieilledent
 Author-email: ghislain.vieilledent@cirad.fr
 License: GPLv3
 Project-URL: Documentation, https://ecology.ghislainv.fr/pywdpa
 Project-URL: Source, https://github.com/ghislainv/pywdpa/
 Project-URL: Traker, https://github.com/ghislainv/pywdpa/issues
-Description: ..
-           # ==============================================================================
-           # author          :Ghislain Vieilledent
-           # email           :ghislain.vieilledent@cirad.fr, ghislainv@gmail.com
-           # web             :https://ecology.ghislainv.fr
-           # license         :GPLv3
-           # ==============================================================================
-        
-        .. image:: https://ecology.ghislainv.fr/pywdpa/_static/logo-pywdpa.svg
-           :align: right
-           :target: https://ecology.ghislainv.fr/pywdpa
-           :alt: Logo pywdpa
-           :width: 140px
-        	   
-        ``pywdpa`` Python package
-        *************************
-        
-        
-        |Python version| |PyPI version| |GitHub Actions| |License| |Zenodo|
-        
-        
-        Overview
-        ========
-        
-        The ``pywdpa`` Python package is an interface to the World Database on
-        Protected Areas (WDPA) hosted on the Protected Planet website at
-        `<https://www.protectedplanet.net>`_. The ``pywdpa`` package provides
-        functions to download shapefiles of protected areas (PA) for any
-        countries with an iso3 code using the Protected Planet API at
-        `<https://api.protectedplanet.net>`_. The ``pywdpa`` package
-        translates some functions of the R package ``worldpa``
-        (`<https://github.com/FRBCesab/worldpa>`_) in the Python language.
-        
-        .. image:: https://ecology.ghislainv.fr/pywdpa/_static/protected-planet.jpg
-           :align: center
-           :target: https://ecology.ghislainv.fr/pywdpa
-           :alt: protected-planet
-        
-        Terms and conditions
-        ====================
-        
-        You must ensure that the following citation is always clearly
-        reproduced in any publication or analysis involving the Protected
-        Planet Materials in any derived form or format:
-        
-        ..
-           
-            UNEP-WCMC and IUCN (\ ``YEAR``\ ) Protected Planet: The World
-            Database on Protected Areas (WDPA). Cambridge, UK: UNEP-WCMC and
-            IUCN. Available at: www.protectedplanet.net (dataset downloaded the
-            ``YEAR/MONTH``\ ).
-        
-        
-        For further details on terms and conditions of the WDPA usage, please
-        visit the page:
-        `<https://www.protectedplanet.net/c/terms-and-conditions>`_.
-        
-        Prerequisites
-        =============
-        
-        This package uses the Protected Planet API to access data on world
-        protected areas. You must first have obtained a Personal API Token by
-        filling in the form available at
-        `<https://api.protectedplanet.net/request>`_. Then you need to set an
-        environment variable (we recommend using the name ``WDPA_KEY``\ )
-        using either the command ``os.environ["WDPA_KEY"]="your_token"`` or
-        `python-dotenv <https://github.com/theskumar/python-dotenv>`_.
-        
-        Installation
-        ============
-        
-        The easiest way to install the ``pywdpa`` Python package is via `pip <https://pip.pypa.io/en/stable/>`_:
-        
-        .. code-block:: bash
-        
-           $ # For version on PyPI
-           $ python -m pip install pywdpa
-        
-        or 
-        
-        .. code-block:: bash
-        
-           $ # For development version on GitHub
-           $ python -m pip install https://github.com/ghislainv/pywdpa/archive/master.zip
-        
-        but you can also install ``pywdpa`` executing the ``setup.py`` file:
-        
-        .. code-block:: bash
-        
-           $ git clone https://github.com/ghislainv/pywdpa
-           $ cd pywdpa
-           $ python setup.py install
-        
-        Contributing
-        ============
-        
-        The ``pywdpa`` Python package is Open Source and released under
-        the `GNU GPL version 3 license
-        <https://ecology.ghislainv.fr/pywdpa/license.html>`__. Anybody
-        who is interested can contribute to the package development following
-        our `Community guidelines
-        <https://ecology.ghislainv.fr/pywdpa/contributing.html>`__. Every
-        contributor must agree to follow the project's `Code of conduct
-        <https://ecology.ghislainv.fr/pywdpa/code_of_conduct.html>`__.
-           
-        .. |Python version| image:: https://img.shields.io/pypi/pyversions/pywdpa?logo=python&logoColor=ffd43b&color=306998
-           :target: https://pypi.org/project/pywdpa
-           :alt: Python version
-        
-        .. |PyPI version| image:: https://img.shields.io/pypi/v/pywdpa
-           :target: https://pypi.org/project/pywdpa
-           :alt: PyPI version
-        
-        .. |GitHub Actions| image:: https://github.com/ghislainv/pywdpa/workflows/PyPkg/badge.svg
-           :target: https://github.com/ghislainv/pywdpa/actions
-           :alt: GitHub Actions
-        	 
-        .. |License| image:: https://img.shields.io/badge/licence-GPLv3-8f10cb.svg
-           :target: https://www.gnu.org/licenses/gpl-3.0.html
-           :alt: License GPLv3
-        
-        .. |Zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4275513.svg
-           :target: https://doi.org/10.5281/zenodo.4275513
-           :alt: Zenodo
-        
-        
 Keywords: protected areas wdpa world database protected areas
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=2.7
+Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: gdal
+Requires-Dist: requests
 Provides-Extra: interactive
+Requires-Dist: jupyter; extra == "interactive"
+Requires-Dist: python-dotenv; extra == "interactive"
+Requires-Dist: geopandas; extra == "interactive"
+Requires-Dist: descartes; extra == "interactive"
+Requires-Dist: folium; extra == "interactive"
+
+..
+   # ==============================================================================
+   # author          :Ghislain Vieilledent
+   # email           :ghislain.vieilledent@cirad.fr, ghislainv@gmail.com
+   # web             :https://ecology.ghislainv.fr
+   # license         :GPLv3
+   # ==============================================================================
+
+.. image:: https://ecology.ghislainv.fr/pywdpa/_static/logo-pywdpa.svg
+   :align: right
+   :target: https://ecology.ghislainv.fr/pywdpa
+   :alt: Logo pywdpa
+   :width: 140px
+	   
+``pywdpa`` Python package
+*************************
+
+
+|Python version| |PyPI version| |GitHub Actions| |License| |Zenodo|
+
+
+Overview
+========
+
+The ``pywdpa`` Python package is an interface to the World Database on
+Protected Areas (WDPA) hosted on the Protected Planet website at
+`<https://www.protectedplanet.net>`_. The ``pywdpa`` package provides
+functions to download shapefiles of protected areas (PA) for any
+countries with an iso3 code using the Protected Planet API at
+`<https://api.protectedplanet.net>`_. The ``pywdpa`` package
+translates some functions of the R package ``worldpa``
+(`<https://github.com/FRBCesab/worldpa>`_) in the Python language.
+
+.. image:: https://ecology.ghislainv.fr/pywdpa/_static/banner_pywdpa.png
+   :align: center
+   :target: https://ecology.ghislainv.fr/pywdpa
+   :alt: protected-planet
+
+Terms and conditions
+====================
+
+You must ensure that the following citation is always clearly
+reproduced in any publication or analysis involving the Protected
+Planet Materials in any derived form or format:
+
+..
+   
+    UNEP-WCMC and IUCN (\ ``YEAR``\ ) Protected Planet: The World
+    Database on Protected Areas (WDPA). Cambridge, UK: UNEP-WCMC and
+    IUCN. Available at: www.protectedplanet.net (dataset downloaded the
+    ``YEAR/MONTH``\ ).
+
+
+For further details on terms and conditions of the WDPA usage, please
+visit the page: `<https://www.protectedplanet.net/en/legal>`_.
+
+Prerequisites
+=============
+
+Access to Protected Planet API
+------------------------------
+
+This package uses the Protected Planet API to access data on world
+protected areas. You must first have obtained a Personal API Token by
+filling in the form available at
+`<https://api.protectedplanet.net/request>`_. Then you need to set an
+environment variable (we recommend using the name ``WDPA_KEY``\ )
+using either the command ``os.environ["WDPA_KEY"]="your_token"`` or
+`python-dotenv <https://github.com/theskumar/python-dotenv>`_.
+
+GDAL
+----
+
+GDAL must be installed on your system.
+
+To install GDAL on Windows, use the `OSGeo4W <https://trac.osgeo.org/osgeo4w/>`_ network installer. OSGeo4W is a binary distribution of a broad set of open source geospatial software for Windows environments (Windows 11 down to 7). Select *Express Install* and install GDAL. Several Gb of space will be needed on disk to install this programs. This will also install *OSGeo4W Shell* to execute command lines.
+
+To install GDAL on other systems, use your package manager, for example ``apt`` for Debian/Ubuntu Linux distributions.
+
+.. code:: shell
+
+    sudo apt update
+    sudo apt install gdal-bin libgdal-dev
+
+After installing GDAL, you can test the installation by running ``gdalinfo --version`` in the command prompt or terminal, which should display the installed GDAL version.
+
+
+Installation
+============
+
+The easiest way to install the ``pywdpa`` Python package is via `pip <https://pip.pypa.io/en/stable/>`_ in the *OSGeo4W Shell* for Windows or in a virtual environment for Linux.
+
+For Linux, create and activate a virtual environment before install ``pywdpa`` with ``pip``:
+
+.. code-block:: shell
+
+   cd ~
+   # Create a directory for virtual environments
+   mkdir venvs
+   # Create the virtual environment with venv
+   python3 -m venv ~/venvs/venv-pywdpa
+   # Activate (start) the virtual environment
+   source ~/venvs/venv-pywdpa/bin/activate
+
+Install Python dependencies and ``pywdpa`` in the *OSGeo4W Shell* or in the newly created virtual environment:
+   
+.. code-block:: shell
+   
+   # Upgrade pip, setuptools, and wheel
+   python3 -m pip install --upgrade pip setuptools wheel
+   # Install numpy
+   python3 -m numpy
+   # Install gdal Python bindings (the correct version)
+   python3 -m pip install gdal==$(gdal-config --version)
+   # Install pywdpa. This will install all other dependencies
+   python3 -m pip install pywdpa
+
+If you want to install the development version of ``pywdpa``, replace the last line with:
+
+.. code-block:: shell
+
+   python3 -m pip install https://github.com/ghislainv/pywdpa/archive/master.zip
+
+To deactivate and delete the virtual environment:
+
+.. code-block:: shell
+		
+   deactivate
+   rm -R ~/venvs/venv-pywdpa # Just remove the repository
+
+In case of problem while installing GDAL Python bindings, try the following command:
+
+.. code-block:: shell
+		
+   python3 -m pip install  --no-cache-dir --force-reinstall gdal==$(gdal-config --version)
+
+
+Contributing
+============
+
+The ``pywdpa`` Python package is Open Source and released under
+the `GNU GPL version 3 license
+<https://ecology.ghislainv.fr/pywdpa/license.html>`__. Anybody
+who is interested can contribute to the package development following
+our `Community guidelines
+<https://ecology.ghislainv.fr/pywdpa/contributing.html>`__. Every
+contributor must agree to follow the project's `Code of conduct
+<https://ecology.ghislainv.fr/pywdpa/code_of_conduct.html>`__.
+   
+.. |Python version| image:: https://img.shields.io/pypi/pyversions/pywdpa?logo=python&logoColor=ffd43b&color=306998
+   :target: https://pypi.org/project/pywdpa
+   :alt: Python version
+
+.. |PyPI version| image:: https://img.shields.io/pypi/v/pywdpa
+   :target: https://pypi.org/project/pywdpa
+   :alt: PyPI version
+
+.. |GitHub Actions| image:: https://github.com/ghislainv/pywdpa/workflows/PyPkg/badge.svg
+   :target: https://github.com/ghislainv/pywdpa/actions
+   :alt: GitHub Actions
+	 
+.. |License| image:: https://img.shields.io/badge/licence-GPLv3-8f10cb.svg
+   :target: https://www.gnu.org/licenses/gpl-3.0.html
+   :alt: License GPLv3
+
+.. |Zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4275513.svg
+   :target: https://doi.org/10.5281/zenodo.4275513
+   :alt: Zenodo
+
```

### Comparing `pywdpa-0.1.5/setup.py` & `pywdpa-0.1.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
+"""Installation setup."""
 
-# ==============================================================================
+# ================================================================
 # author          :Ghislain Vieilledent
-# email           :ghislain.vieilledent@cirad.fr, ghislainv@gmail.com
+# email           :ghislain.vieilledent@cirad.fr
 # web             :https://ecology.ghislainv.fr
-# python_version  :>=2.7
+# python_version  :>=3.6
 # license         :GPLv3
-# ==============================================================================
+# ================================================================
 
 # Import
+import io
 import re  # Regular expression
 from setuptools import setup
 
-# Version
-version = re.search(
-    '^__version__\s*=\s*"(.*)"',
-    open('pywdpa/pywdpa.py').read(),
-    re.M
-    ).group(1)
+
+# find_version
+def find_version():
+    """Finding package version."""
+    with open("pywdpa/__init__.py", encoding="utf-8") as init_file:
+        init_text = init_file.read()
+    _version = (re.search('^__version__\\s*=\\s*"(.*)"',
+                          init_text, re.M)
+                .group(1))
+    return _version
+
+
+version = find_version()
 
 # reStructuredText README file
-with open("README.rst", "rb") as f:
-    long_description = f.read().decode("utf-8")
+with io.open("README.rst", encoding="utf-8") as f:
+    long_description = f.read()
 
 # Project URLs
 project_urls = {
     'Documentation': 'https://ecology.ghislainv.fr/pywdpa',
     'Source': 'https://github.com/ghislainv/pywdpa/',
     'Traker': 'https://github.com/ghislainv/pywdpa/issues',
 }
@@ -41,20 +50,19 @@
       license="GPLv3",
       description="Easy access to world's protected areas",
       long_description=long_description,
       long_description_content_type="text/x-rst",
       classifiers=["Development Status :: 4 - Beta",
                    "License :: OSI Approved :: GNU General Public License v3 "
                    "(GPLv3)",
-                   "Programming Language :: Python :: 2",
                    "Programming Language :: Python :: 3",
                    "Operating System :: OS Independent",
                    "Topic :: Scientific/Engineering :: Bio-Informatics"],
       keywords="protected areas wdpa world database protected areas",
-      python_requires=">=2.7",
+      python_requires=">=3.6",
       packages=["pywdpa"],
       package_dir={"pywdpa": "pywdpa"},
       entry_points={"console_scripts": ["pywdpa = pywdpa.pywdpa:main"]},
       install_requires=["numpy", "gdal", "requests"],
       extras_require={
           "interactive": ["jupyter", "python-dotenv", "geopandas",
                           "descartes", "folium"]},
```

### Comparing `pywdpa-0.1.5/test/test_get_token.py` & `pywdpa-0.1.6/test/test_get_token.py`

 * *Files identical despite different names*

### Comparing `pywdpa-0.1.5/test/test_get_wdpa.py` & `pywdpa-0.1.6/test/test_get_wdpa.py`

 * *Files identical despite different names*

