# Comparing `tmp/yt_xarray-0.2.0.tar.gz` & `tmp/yt_xarray-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt_xarray-0.2.0.tar", last modified: Tue Oct 10 17:28:49 2023, max compression
+gzip compressed data, was "yt_xarray-0.3.0.tar", last modified: Thu May 23 20:07:51 2024, max compression
```

## Comparing `yt_xarray-0.2.0.tar` & `yt_xarray-0.3.0.tar`

### file list

```diff
@@ -1,66 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 17:28:49.714284 yt_xarray-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      155 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)      418 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      435 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      160 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      448 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2023-10-10 17:28:49.714284 yt_xarray-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 17:28:49.706284 yt_xarray-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (127)     4887 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 17:28:49.706284 yt_xarray-0.2.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    88920 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/docs/examples/example_001_xr_to_yt.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    45686 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/docs/examples/example_002_coord_aliases.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   113809 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/docs/examples/example_003_two_dimensional_fields.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   290757 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/docs/examples/example_004_xr_yt_cartopy.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  4627430 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/docs/examples/example_005_chunked_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      601 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)      833 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      771 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/docs/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 17:28:49.710284 yt_xarray-0.2.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      374 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/docs/source/yt_xarray.accessor.rst
--rw-r--r--   0 runner    (1001) docker     (127)      559 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/docs/source/yt_xarray.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/docs/supported_grids.rst
--rw-r--r--   0 runner    (1001) docker     (127)      374 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/docs/yt_xarray.accessor.rst
--rw-r--r--   0 runner    (1001) docker     (127)      578 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/docs/yt_xarray.rst
--rw-r--r--   0 runner    (1001) docker     (127)      384 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/docs/yt_xarray.utilities.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-10 17:28:49.714284 yt_xarray-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 17:28:49.710284 yt_xarray-0.2.0/yt_xarray/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/yt_xarray/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 17:28:49.714284 yt_xarray-0.2.0/yt_xarray/accessor/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/yt_xarray/accessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/yt_xarray/accessor/_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17267 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/yt_xarray/accessor/_xr_to_yt.py
--rw-r--r--   0 runner    (1001) docker     (127)    14832 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/yt_xarray/accessor/accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/yt_xarray/sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 17:28:49.714284 yt_xarray-0.2.0/yt_xarray/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/yt_xarray/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6172 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/yt_xarray/tests/test_accesor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/yt_xarray/tests/test_chunking.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/yt_xarray/tests/test_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/yt_xarray/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    16783 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/yt_xarray/tests/test_xr_to_yt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 17:28:49.714284 yt_xarray-0.2.0/yt_xarray/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/yt_xarray/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5020 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/yt_xarray/utilities/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/yt_xarray/utilities/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2023-10-10 17:28:32.000000 yt_xarray-0.2.0/yt_xarray/yt_xarray.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 17:28:49.710284 yt_xarray-0.2.0/yt_xarray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2023-10-10 17:28:49.000000 yt_xarray-0.2.0/yt_xarray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2023-10-10 17:28:49.000000 yt_xarray-0.2.0/yt_xarray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-10 17:28:49.000000 yt_xarray-0.2.0/yt_xarray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2023-10-10 17:28:49.000000 yt_xarray-0.2.0/yt_xarray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-10-10 17:28:49.000000 yt_xarray-0.2.0/yt_xarray.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:07:51.583273 yt_xarray-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-05-23 20:07:51.583273 yt_xarray-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:07:51.563272 yt_xarray-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5148 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:07:51.575273 yt_xarray-0.3.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    88920 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/docs/examples/example_001_xr_to_yt.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   207021 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/docs/examples/example_002_coord_aliases.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   113809 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/docs/examples/example_003_two_dimensional_fields.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   290757 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/docs/examples/example_004_xr_yt_cartopy.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  4627430 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/docs/examples/example_005_chunked_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   228739 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/docs/examples/example_006_yt_method_access.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1161728 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/docs/examples/example_007_interpolation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1337248 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/docs/examples/example_008_interpolation_with_refinement.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/docs/examples/example_009_custom_transformations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    88113 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/docs/examples/example_010_custom_interpolations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:07:51.575273 yt_xarray-0.3.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/docs/source/yt_xarray.YtAccessor.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/docs/source/yt_xarray.open_dataset.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/docs/source/yt_xarray.sample_data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/docs/source/yt_xarray.transformations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/docs/supported_grids.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 20:07:51.583273 yt_xarray-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:07:51.579273 yt_xarray-0.3.0/yt_xarray/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/yt_xarray/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:07:51.579273 yt_xarray-0.3.0/yt_xarray/accessor/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/yt_xarray/accessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/yt_xarray/accessor/_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19556 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/yt_xarray/accessor/_xr_to_yt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23232 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/yt_xarray/accessor/accessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/yt_xarray/sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:07:51.579273 yt_xarray-0.3.0/yt_xarray/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/yt_xarray/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/yt_xarray/tests/test_accesor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/yt_xarray/tests/test_chunking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/yt_xarray/tests/test_grid_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/yt_xarray/tests/test_optional_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/yt_xarray/tests/test_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/yt_xarray/tests/test_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/yt_xarray/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18502 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/yt_xarray/tests/test_xr_to_yt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/yt_xarray/tests/test_yt_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22914 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/yt_xarray/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:07:51.583273 yt_xarray-0.3.0/yt_xarray/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/yt_xarray/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13324 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/yt_xarray/utilities/_grid_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/yt_xarray/utilities/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/yt_xarray/utilities/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-23 20:07:39.000000 yt_xarray-0.3.0/yt_xarray/yt_xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:07:51.583273 yt_xarray-0.3.0/yt_xarray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-05-23 20:07:51.000000 yt_xarray-0.3.0/yt_xarray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-23 20:07:51.000000 yt_xarray-0.3.0/yt_xarray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 20:07:51.000000 yt_xarray-0.3.0/yt_xarray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-23 20:07:51.000000 yt_xarray-0.3.0/yt_xarray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 20:07:51.000000 yt_xarray-0.3.0/yt_xarray.egg-info/top_level.txt
```

### Comparing `yt_xarray-0.2.0/HISTORY.md` & `yt_xarray-0.3.0/HISTORY.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # History
 
+## 0.3.0
+
+### New Features
+* yt wrapper methods
+
 ## 0.2.0 (2023-10-10)
 
 Maintenance release. Minimum python version is now 3.9.
 
 ### Changes
 * improve error messaging for load_grid
 * fix deprecation warning from yt.load_amr_grids
```

### Comparing `yt_xarray-0.2.0/LICENSE` & `yt_xarray-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yt_xarray-0.2.0/Makefile` & `yt_xarray-0.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `yt_xarray-0.2.0/PKG-INFO` & `yt_xarray-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt_xarray
-Version: 0.2.0
+Version: 0.3.0
 Summary: interface between yt and xarray
 Author-email: Chris Havlin <chris.havlin@gmail.com>
 Project-URL: Homepage, https://github.com/data-exp-lab/yt_xarray
 Project-URL: Bug Tracker, https://github.com/data-exp-lab/yt_xarray/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -21,31 +21,34 @@
 Requires-Dist: h5py>=3.4.0
 Requires-Dist: pooch>=1.5.1
 Requires-Dist: xarray
 Provides-Extra: full
 Requires-Dist: netCDF4; extra == "full"
 Requires-Dist: scipy; extra == "full"
 Requires-Dist: dask[complete]; extra == "full"
+Requires-Dist: cf_xarray; extra == "full"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: cartopy; extra == "test"
 Provides-Extra: docs
-Requires-Dist: Sphinx==1.8.5; extra == "docs"
-Requires-Dist: jinja2<3.1.0; extra == "docs"
-Requires-Dist: nbsphinx; extra == "docs"
+Requires-Dist: Sphinx==7.2.6; extra == "docs"
+Requires-Dist: jinja2==3.1.2; extra == "docs"
+Requires-Dist: nbsphinx==0.9.3; extra == "docs"
 
 # yt_xarray
 
-
 [![PyPI version](https://badge.fury.io/py/yt_xarray.svg)](https://badge.fury.io/py/yt_xarray)
+[![Python Version](https://img.shields.io/pypi/pyversions/yt_xarray.svg?color=green)](https://python.org)
+[![Tests](https://github.com/data-exp-lab/yt_xarray/actions/workflows/run-pytest-tests.yml/badge.svg)](https://github.com/data-exp-lab/yt_xarray/actions/workflows/run-pytest-tests.yml)
+[![codecov](https://codecov.io/gh/data-exp-lab/yt_xarray/branch/main/graph/badge.svg)](https://codecov.io/gh/data-exp-lab/yt_xarray)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/data-exp-lab/yt_xarray/main.svg)](https://results.pre-commit.ci/latest/github/data-exp-lab/yt_xarray/main)
 
 An interface between yt and xarray
 
-
 ## Overview
 
 yt_xarray streamlines communication between
 [xarray](https://docs.xarray.dev/en/stable/#) and [yt](https://yt-project.org),
 making it easier use yt's visualization and analysis methods with data loaded
 via xarray.
```

### Comparing `yt_xarray-0.2.0/README.md` & `yt_xarray-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # yt_xarray
 
-
 [![PyPI version](https://badge.fury.io/py/yt_xarray.svg)](https://badge.fury.io/py/yt_xarray)
+[![Python Version](https://img.shields.io/pypi/pyversions/yt_xarray.svg?color=green)](https://python.org)
+[![Tests](https://github.com/data-exp-lab/yt_xarray/actions/workflows/run-pytest-tests.yml/badge.svg)](https://github.com/data-exp-lab/yt_xarray/actions/workflows/run-pytest-tests.yml)
+[![codecov](https://codecov.io/gh/data-exp-lab/yt_xarray/branch/main/graph/badge.svg)](https://codecov.io/gh/data-exp-lab/yt_xarray)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/data-exp-lab/yt_xarray/main.svg)](https://results.pre-commit.ci/latest/github/data-exp-lab/yt_xarray/main)
 
 An interface between yt and xarray
 
-
 ## Overview
 
 yt_xarray streamlines communication between
 [xarray](https://docs.xarray.dev/en/stable/#) and [yt](https://yt-project.org),
 making it easier use yt's visualization and analysis methods with data loaded
 via xarray.
```

### Comparing `yt_xarray-0.2.0/docs/Makefile` & `yt_xarray-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `yt_xarray-0.2.0/docs/conf.py` & `yt_xarray-0.3.0/docs/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,30 +34,30 @@
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.viewcode",
     "sphinx.ext.autosectionlabel",
     "nbsphinx",
 ]
-
+suppress_warnings = ["autosectionlabel.*"]
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 # source_suffix = ['.rst', '.md']
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "yt_xarray"
-copyright = "2022, Chris Havlin"
+copyright = "2024, Chris Havlin"
 author = "Chris Havlin"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
@@ -66,15 +66,17 @@
 release = yt_xarray.__version__
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
+
+toc_object_entries_show_parents = "hide"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # The name of the Pygments (syntax highlighting) style to use.
@@ -91,15 +93,22 @@
 #
 html_theme = "alabaster"
 
 # Theme options are theme-specific and customize the look and feel of a
 # theme further.  For a list of options available for each theme, see the
 # documentation.
 #
-# html_theme_options = {}
+html_theme_options = {
+    "fixed_sidebar": True,
+    "github_button": True,
+    "github_user": "data-exp-lab",
+    "github_repo": "yt_xarray",
+    "github_count": False,
+    "github_type": "no-text",
+}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
```

### Comparing `yt_xarray-0.2.0/docs/contributing.rst` & `yt_xarray-0.3.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `yt_xarray-0.2.0/docs/examples/example_001_xr_to_yt.ipynb` & `yt_xarray-0.3.0/docs/examples/example_001_xr_to_yt.ipynb`

 * *Files identical despite different names*

### Comparing `yt_xarray-0.2.0/docs/examples/example_003_two_dimensional_fields.ipynb` & `yt_xarray-0.3.0/docs/examples/example_003_two_dimensional_fields.ipynb`

 * *Files identical despite different names*

### Comparing `yt_xarray-0.2.0/docs/examples/example_004_xr_yt_cartopy.ipynb` & `yt_xarray-0.3.0/docs/examples/example_004_xr_yt_cartopy.ipynb`

 * *Files identical despite different names*

### Comparing `yt_xarray-0.2.0/docs/examples/example_005_chunked_data.ipynb` & `yt_xarray-0.3.0/docs/examples/example_005_chunked_data.ipynb`

 * *Files identical despite different names*

### Comparing `yt_xarray-0.2.0/docs/faq.rst` & `yt_xarray-0.3.0/docs/faq.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-Some common problems (and how to solve them)
-============================================
+FAQ
+===
 
 yt and xarray have many similarities in how they handle their Datasets, but
 there are also many aspects that differ to varying degree. This page describes
 some of the difficulties you may encounter while using yt_xarray to communicate
-between the two.
+between the two and how to solve those issues.
 
 xarray datasets with a mix of dimensionality
 ********************************************
 
 It is common for xarray datasets to have variables that have a mix of dimensionality.
 Some variables may be 3D in space ``(x, y, z)``, 2D ``(x, y)``, 3D in space and time ``(x, y, t)``, etc.
 But with the present implementation,  the fields that are loaded into yt must have the
@@ -22,15 +22,17 @@
 unknown coordinate names
 ************************
 
 yt datasets have a fixed expectation for coordinate names. In cartesian, these
 coordinate names are ``'x'``, ``'y'``, ``'z'`` while for geographic coordinate systems
 the coordinate names are ``'latitude'``, ``'longtiude'`` and then either ``'altitude'``
 or ``'depth'``. To work with xarray variables defined with coordinate names that
-differ from these, yt_xarray provides some coordinate aliasing.
+differ from these, yt_xarray provides some coordinate aliasing, which in part relies
+on `cf_xarray <https://cf-xarray.readthedocs.io>`_ (if it is installed) for
+additional conversion to standard names.
 
 See :doc:`examples/example_002_coord_aliases` for an example.
 
 unknown coordinate systems
 **************************
 
 yt is designed for volumetric data: 3D (or 2D) data defined in a
```

### Comparing `yt_xarray-0.2.0/docs/index.rst` & `yt_xarray-0.3.0/docs/index.rst`

 * *Files 18% similar despite different names*

```diff
@@ -14,16 +14,15 @@
 After installing, the easiest way to get started is to peruse the
 :ref:`Example Notebooks`.
 If you come across any issues or have feature requests, please reach out at the
 `yt_xarray github repository <https://github.com/data-exp-lab/yt_xarray/>`_!
 
 .. toctree::
    :hidden:
-   :maxdepth: 2
 
    installation
    supported_grids
    examples
    faq
-   API <modules>
+   API <source/modules>
    contributing
```

### Comparing `yt_xarray-0.2.0/docs/installation.rst` & `yt_xarray-0.3.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `yt_xarray-0.2.0/docs/make.bat` & `yt_xarray-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `yt_xarray-0.2.0/docs/supported_grids.rst` & `yt_xarray-0.3.0/docs/supported_grids.rst`

 * *Files identical despite different names*

### Comparing `yt_xarray-0.2.0/pyproject.toml` & `yt_xarray-0.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yt_xarray"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
   { name="Chris Havlin", email="chris.havlin@gmail.com" },
 ]
 description="interface between yt and xarray"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -24,17 +24,17 @@
 dependencies=['yt>=4.2.0', 'h5py>=3.4.0', 'pooch>=1.5.1', 'xarray']
 
 [project.urls]
 "Homepage" = "https://github.com/data-exp-lab/yt_xarray"
 "Bug Tracker" = "https://github.com/data-exp-lab/yt_xarray/issues"
 
 [project.optional-dependencies]
-full = ["netCDF4", "scipy", "dask[complete]"]
-test = ["pytest", "pytest-cov"]
-docs = ["Sphinx==1.8.5", "jinja2<3.1.0", "nbsphinx"]
+full = ["netCDF4", "scipy", "dask[complete]", "cf_xarray"]
+test = ["pytest", "pytest-cov", "cartopy"]
+docs = ["Sphinx==7.2.6", "jinja2==3.1.2", "nbsphinx==0.9.3"]
 
 [tool.black]
 line-length = 88
 target-version = ['py310']
 
 [tool.isort]
 profile = "black"
```

### Comparing `yt_xarray-0.2.0/yt_xarray/accessor/_readers.py` & `yt_xarray-0.3.0/yt_xarray/accessor/_readers.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 from yt_xarray.accessor import _xr_to_yt
 
 
 def _get_xarray_reader(
     handle, sel_info: _xr_to_yt.Selection, interp_required: Optional[bool] = True
 ):
-
     # the callable generator for an open xarray handle.
     # handle: an open xarray handle
     # sel_info: a Selection object for the handle
     # reader_type: specifies what type of reader (only "node_to_cell" exists now)
 
     def _reader(grid, field_name):
         # grid: a yt grid object
@@ -29,16 +28,16 @@
 
         # step 1 (if axis has been reversed, node ordering is also reversed)
         for idim in range(sel_info.ndims):
             if sel_info.reverse_axis[idim]:
                 # note that the si, ei are exchanged!
                 si0 = si.copy()
                 ei0 = ei.copy()
-                si[idim] = sel_info.global_dims[idim] - ei0[idim]
-                ei[idim] = sel_info.global_dims[idim] - si0[idim]
+                si[idim] = sel_info.global_dims_no_time[idim] - ei0[idim]
+                ei[idim] = sel_info.global_dims_no_time[idim] - si0[idim]
 
         # step 2: this global start index accounts for indexing after any
         # subselections on the xarray DataArray are made. might
         # be a way to properly set this with yt grid objects.
         gsi = sel_info.starting_indices
         if sel_info.ndims == 2:
             gsi = np.append(gsi, 0)
```

### Comparing `yt_xarray-0.2.0/yt_xarray/accessor/_xr_to_yt.py` & `yt_xarray-0.3.0/yt_xarray/accessor/_xr_to_yt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import collections.abc
 import enum
+from collections import defaultdict
 from typing import List, Optional, Tuple
 
 import numpy as np
 import unyt
 import xarray as xr
 
 from yt_xarray.utilities.logging import ytxr_log
@@ -28,15 +29,14 @@
     def __init__(
         self,
         xr_ds,
         fields: List[str] = None,
         sel_dict: Optional[dict] = None,
         sel_dict_type: Optional[str] = "isel",
     ):
-
         self.fields = self._validate_fields(xr_ds, fields)
         self.units: dict = self._find_units(xr_ds)
         self.full_shape = xr_ds.data_vars[self.fields[0]].shape
         self.sel_dict = sel_dict or {}
         if sel_dict_type not in ["sel", "isel"]:
             raise RuntimeError(
                 f"sel_dict_type must be 'sel' or 'isel', got {sel_dict_type}"
@@ -51,30 +51,32 @@
         self.selected_coords: Tuple[str] = None
         self.starting_indices: np.ndarray = None
         self.selected_time = None
         self.ndims: int = None
         self.grid_type = None  # one of _GridType members
         self.cell_widths: list = None
         self.global_dims: list = None
+        self.time_index_number: int = None
         self._process_selection(xr_ds)
 
-        self.yt_coord_names = _convert_to_yt_internal_coords(self.selected_coords)
+        xr_field = xr_ds.data_vars[fields[0]]
+        self.yt_coord_names = _convert_to_yt_internal_coords(
+            self.selected_coords, xr_field
+        )
 
     def _find_units(self, xr_ds) -> dict:
-
         units = {}
         for field in self.fields:
             unit = getattr(xr_ds[field], "units", "")
             if unit != "" and hasattr(unyt.unit_symbols, unit) is False:
                 unit = ""
             units[field] = unit
         return units
 
     def _find_starting_index(self, coordname, coord_da, coord_select) -> int:
-
         si = 0
         selector = coord_select[coordname]
         if self.sel_dict_type == "isel":
             if isinstance(selector, slice):
                 si = selector.start
             elif isinstance(selector, int):
                 si = selector
@@ -112,15 +114,14 @@
                     f"Could not find selected value: {coordname}:{search_for}"
                 )
             si = the_index[0]
 
         return si
 
     def _process_selection(self, xr_ds):
-
         # the full list of coordinates (in order)
         full_coords = list(xr_ds.data_vars[self.fields[0]].dims)
         time = 0.0
         # for each coordinate, apply any selector and then store min/max of the
         # coordinate. If the selector results in <= 1 in one of the dimensions,
         # that dimensions is dropped from the selection
         n_edges = []  # number of edges after selection
@@ -130,15 +131,16 @@
         coord_list = []  # the coord list after selection
         starting_indices = []  # global starting index
         cell_widths = []  # cell widths after selection
         grid_type = _GridType.UNIFORM  # start with uniform assumption
         reverse_axis = []  # axes must be positive-monitonic for yt
         reverse_axis_names = []
         global_dims = []  # the global shape
-        for c in full_coords:
+        time_index_number = None
+        for icoord, c in enumerate(full_coords):
             coord_da = getattr(xr_ds, c)  # the full coordinate data array
 
             # check if coordinate values are increasing
             if coord_da.size > 1:
                 rev_ax = coord_da[1] <= coord_da[0]
                 reverse_axis.append(bool(rev_ax.values))
                 if rev_ax:
@@ -156,17 +158,18 @@
                 coord_select[c] = self.sel_dict[c]
                 si = self._find_starting_index(c, coord_da, coord_select)
 
             # apply any selections and extract coordinates
             sel_or_isel = getattr(coord_da, self.sel_dict_type)
             coord_vals = sel_or_isel(coord_select).values.astype(np.float64)
             is_time_dim = _check_for_time(c, coord_vals)
+            if is_time_dim:
+                time_index_number = icoord
 
             if coord_vals.size > 1:
-
                 # not positive-monotonic? reverse it for cell width calculations
                 # changes to indexing are accounted for when extracting data.
                 if reverse_axis[-1]:
                     coord_vals = coord_vals[::-1]
 
                 cell_widths.append(coord_vals[1:] - coord_vals[:-1])
                 dimranges.append([coord_vals.min(), coord_vals.max()])
@@ -194,49 +197,55 @@
             raise ValueError(
                 f"ndim is {len(n_edges)}, please provide a sel_dict to"
                 f" reduce dimensionality to 3."
             )
         self.ndims = len(n_edges)
         self.selected_shape = tuple(n_edges)
         self.select_shape_cells = tuple(n_cells)
+        if time_index_number is not None:
+            _ = full_dimranges.pop(time_index_number)
         self.full_bbox = np.array(full_dimranges).astype(np.float64)
         self.selected_bbox = np.array(dimranges).astype(np.float64)
         self.full_coords = tuple(full_coords)
         self.selected_coords = tuple(coord_list)
         self.starting_indices = np.array(starting_indices)
         self.selected_time = time
         self.grid_type = grid_type
         self.cell_widths = cell_widths
-        self.reverse_axis = reverse_axis
         self.reverse_axis_names = reverse_axis_names
         self.global_dims = np.array(global_dims)
+        if time_index_number is not None:
+            _ = global_dims.pop(time_index_number)
+            _ = reverse_axis.pop(time_index_number)
+        self.reverse_axis = reverse_axis
+        self.time_index_number = time_index_number
+        self.global_dims_no_time = np.array(global_dims)
+
         # self.coord_selected_arrays = coord_selected_arrays
 
         # set the yt grid dictionary
         self.grid_dict = {
             "left_edge": self.selected_bbox[:, 0],
             "right_edge": self.selected_bbox[:, 1],
             "dimensions": self.select_shape_cells,
             "level": 0,
         }
 
     def _validate_fields(self, xr_ds, fields: List[str]) -> List[str]:
-
         if fields is None:
             raise ValueError("Please provide a list of fields")
 
         # ensure that all fields have the same coordinates and the same shape
         shape = xr_ds.data_vars[fields[0]].shape
         coords = xr_ds.data_vars[fields[0]].dims
 
         if len(fields) > 1:
             msg = "Provided fields must have the same "
 
             for f in fields[1:]:
-
                 if xr_ds.data_vars[f].shape != shape:
                     rmsg = msg + f"shape : {f} does not match {fields[0]}"
                     raise RuntimeError(rmsg)
 
                 if tuple(xr_ds.data_vars[f].dims) != coords:
                     rmsg = msg + f"coordinates : {f} does not match {fields[0]}"
                     raise RuntimeError(rmsg)
@@ -323,18 +332,34 @@
 _coord_aliases = {
     "altitude": ["altitude", "height", "level", "lev"],
     "latitude": ["latitude", "lat"],
     "longitude": ["longitude", "lon"],
 }
 
 
-known_coord_aliases = {}
+_default_known_coord_aliases = {}
 for ky, vals in _coord_aliases.items():
     for val in vals:
-        known_coord_aliases[val] = ky
+        _default_known_coord_aliases[val] = ky
+
+known_coord_aliases = _default_known_coord_aliases.copy()
+
+
+def reset_coordinate_aliases():
+    kys_to_pop = [
+        ky
+        for ky in known_coord_aliases.keys()
+        if ky not in _default_known_coord_aliases
+    ]
+    for ky in kys_to_pop:
+        known_coord_aliases.pop(ky)
+
+    for ky, val in _default_known_coord_aliases.items():
+        known_coord_aliases[ky] = val
+
 
 _expected_yt_axes = {
     "cartesian": set(["x", "y", "z"]),
     "spherical": set(["r", "phi", "theta"]),
     "geographic": set(["altitude", "latitude", "longitude"]),
     "internal_geographic": set(["depth", "latitude", "longitude"]),
 }
@@ -342,28 +367,63 @@
 valid_geometries = tuple(_expected_yt_axes.keys()) + ("geodetic",)
 
 _yt_coord_names = []
 for vals in _expected_yt_axes.values():
     _yt_coord_names += list(vals)
 
 
-def _convert_to_yt_internal_coords(coord_list):
+def _invert_cf_standard_names(standard_names: dict):
+    inverted_mapping = defaultdict(lambda: set())
+    for ky, vals in standard_names.items():
+        for val in vals:
+            inverted_mapping[val].add(ky)
+    return inverted_mapping
+
+
+def _cf_xr_coord_disamb(
+    cname: str, xr_field: xr.DataArray
+) -> Tuple[Optional[str], bool]:
+    # returns a tuple of (validated name, cf_xarray_is_installed)
+    try:
+        import cf_xarray as cfx  # noqa: F401
+    except ImportError:
+        return None, False
+
+    nm_to_standard = _invert_cf_standard_names(xr_field.cf.standard_names)
+    if cname in nm_to_standard:
+        cf_standard_name = nm_to_standard[cname]
+        if len(cf_standard_name):
+            cf_standard_name = list(cf_standard_name)[0]
+            if cf_standard_name in known_coord_aliases:
+                return cf_standard_name, True
+    return None, True
+
+
+def _convert_to_yt_internal_coords(coord_list: List[str], xr_field: xr.DataArray):
     yt_coords = []
     for c in coord_list:
         cname = c.lower()
+        cf_xarray_exists = None
         if cname in known_coord_aliases:
-            yt_coords.append(known_coord_aliases[cname])
+            valid_coord_name = known_coord_aliases[cname]
         elif cname in _yt_coord_names:
-            yt_coords.append(cname)
+            valid_coord_name = cname
         else:
-            raise ValueError(
+            valid_coord_name, cf_xarray_exists = _cf_xr_coord_disamb(cname, xr_field)
+        if valid_coord_name is None:
+            msg = (
                 f"{c} is not a known coordinate. To load in yt, you "
-                f"must supply an alias via the yt_xarray.known_coord_aliases"
-                f" dictionary."
+                "must supply an alias via the yt_xarray.known_coord_aliases"
+                " dictionary"
             )
+            if cf_xarray_exists is False:
+                msg += " or install cf_xarray to check for additional aliases."
+            raise ValueError(msg)
+
+        yt_coords.append(valid_coord_name)
 
     return yt_coords
 
 
 def _determine_yt_geomtype(coord_type: str, coord_list: List[str]) -> Optional[str]:
     # mainly for expanding geodetic into internal_geographic or geographic as used
     # by yt
@@ -396,15 +456,14 @@
             missing[0],
         ]
 
     raise RuntimeError("Could not determine missing coordinate.")
 
 
 def _size_of_array_like(v):
-
     if isinstance(v, (np.ndarray, xr.DataArray)):
         return v.size
 
     return len(v)
 
 
 def _validate_geometry(possible_geom: str) -> str:
```

### Comparing `yt_xarray-0.2.0/yt_xarray/sample_data.py` & `yt_xarray-0.3.0/yt_xarray/sample_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     """
     available_coords = {}
     for dim_name, dim_range in dims.items():
         available_coords[dim_name] = np.linspace(*dim_range)
 
     data = {}
     for field, field_dims in fields.items():
-
         coords = {}
         sz = []
         for dim_name in field_dims:
             if dim_name not in available_coords:
                 raise KeyError(
                     f"{dim_name} is specified as a dimension for "
                     f"{field} but does not exist in the dims argument!"
```

### Comparing `yt_xarray-0.2.0/yt_xarray/tests/test_accesor.py` & `yt_xarray-0.3.0/yt_xarray/tests/test_accesor.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,14 @@
         z_name="depth",
         coord_order=["z", "y", "x"],
     )
     return ds
 
 
 def test_accessor():
-
     tfield = "a_new_field"
     n_x = 3
     n_y = 4
     n_z = 5
     ds = construct_minimal_ds(
         field_name=tfield, n_x=n_x, n_y=n_y, n_z=n_z, coord_order=["x", "y", "z"]
     )
@@ -78,15 +77,14 @@
 
     bbox = ds.yt.get_bbox("test_field_1")
     assert np.all(expected == bbox)
 
 
 @pytest.mark.parametrize("use_callable", (True, False))
 def test_load_grid(ds_xr, use_callable):
-
     flds = ["a_new_field_0", "a_new_field_1"]
     ds_yt = ds_xr.yt.load_grid(flds, use_callable=use_callable)
     assert ds_yt.coordinates.name == "internal_geographic"
     expected_field_list = [("stream", f) for f in flds]
     assert all([f in expected_field_list] for f in ds_yt.field_list)
 
     ds_yt = ds_xr.yt.load_grid(use_callable=use_callable)
@@ -187,30 +185,51 @@
 
 def test_geom_kwarg(ds_xr):
     # make sure we can specify the geometry
     flds = ["a_new_field_0", "a_new_field_1"]
     _ = ds_xr.yt.load_grid(fields=flds, geometry="cartesian")
 
 
-def test_stretched_grid():
+@pytest.mark.parametrize("use_callable", [True, False])
+def test_stretched_grid(use_callable):
     ds = construct_minimal_ds(
         x_stretched=False,
         x_name="x",
         y_stretched=True,
         y_name="y",
         z_stretched=True,
         z_name="z",
     )
 
-    with pytest.raises(NotImplementedError, match="Detected a stretched grid"):
-        _ = ds.yt.load_grid(
-            fields=[
-                "test_field",
-            ]
-        )
-
-    _ = ds.yt.load_grid(
+    ds_yt = ds.yt.load_grid(
         fields=[
             "test_field",
         ],
-        use_callable=False,
+        use_callable=use_callable,
     )
+
+    # stretched grid will interpolate using raw values as nodal values, so
+    # end up with n - 1 cells in each dimension
+    expected_n = np.prod([n - 1 for n in ds.test_field.shape])
+    ad = ds_yt.all_data()
+
+    tst_fld = ad[("stream", "test_field")]
+    assert tst_fld.size == expected_n
+
+    # check that the grid vals match
+    for dim in "xyz":
+        dims = ds.coords[dim].values
+        cell_centers = (dims[:-1] + dims[1:]) / 2
+        dimvals = np.unique(ad[("index", dim)].d)
+        assert np.all(dimvals == cell_centers)
+
+
+def test_load_single_field(ds_xr):
+    flds = "a_new_field_0"
+    ds_yt = ds_xr.yt.load_grid(flds)
+    _ = ds_yt.all_data()[("stream", flds)]
+
+
+def test_last_yt_cache(ds_xr):
+    flds = "a_new_field_0"
+    _ = ds_xr.yt.load_grid(flds)
+    assert ds_xr.yt._yt_ds is not None
```

### Comparing `yt_xarray-0.2.0/yt_xarray/tests/test_chunking.py` & `yt_xarray-0.3.0/yt_xarray/tests/test_chunking.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 import yt_xarray  # noqa: F401
 from yt_xarray import sample_data
 from yt_xarray.utilities._utilities import construct_minimal_ds
 
 
 def test_partial_chunks_uni_cartesian():
-
     # uniform grid, cartesian
     fields = {
         "field0": ("x", "y", "z"),
         "field1": ("x", "y", "z"),
     }
     dims = {"x": (0, 1, 30), "y": (0, 2, 62), "z": (-1, 0.5, 25)}
     ds = sample_data.load_random_xr_data(fields, dims)
@@ -25,15 +24,14 @@
     # uniform grid cartesian will wrap it, so number of cells should match
     # the number of grid points initially
     expected_size = np.prod([dim[2] for dim in dims.values()])
     assert fld_vals.size == expected_size
 
 
 def test_cartesian():
-
     # builds yt grids with and without chunking (and callables), compares the
     # frb ImageArrays for equivalent SlicePlots
     ds = construct_minimal_ds(x_name="x", y_name="y", z_name="z", n_fields=2)
 
     ds_yt_nochunk = ds.yt.load_grid(length_unit="km")
     ds_ch_no_call = ds.yt.load_grid(length_unit="km", chunksizes=2, use_callable=False)
     ds_ch_call = ds.yt.load_grid(length_unit="km", chunksizes=2)
@@ -45,15 +43,14 @@
         slices.append(slc.frb[("stream", "test_field_0")])
 
     assert np.all(slices[0] == slices[1])
     assert np.all(slices[0] == slices[2])
 
 
 def test_geographic_interp():
-
     # this case will require interpolation
     ds = construct_minimal_ds(n_fields=2)
     ds_yt_nochunk = ds.yt.load_grid()
     ds_ch_no_call = ds.yt.load_grid(chunksizes=2, use_callable=False)
     ds_ch_call = ds.yt.load_grid(chunksizes=2)
 
     initial_shape = np.asarray(ds.data_vars["test_field_0"].shape)
@@ -62,15 +59,14 @@
     for dsyt in [ds_yt_nochunk, ds_ch_no_call, ds_ch_call]:
         ad = dsyt.all_data()
         fld = ad[("stream", "test_field_0")]
         assert fld.size == expected_size
 
 
 def test_geographic_no_interp():
-
     # this case will not require interpolation
     ds = construct_minimal_ds(
         n_fields=2, min_x=30.0, max_x=35.0, min_y=40.0, max_y=42.0
     )
     ds_yt_nochunk = ds.yt.load_grid()
     ds_ch_no_call = ds.yt.load_grid(chunksizes=2, use_callable=False)
     ds_ch_call = ds.yt.load_grid(chunksizes=2)
@@ -102,15 +98,14 @@
 def test_chunks_stretched_not_implemented():
     ds = construct_minimal_ds(x_name="x", y_name="y", z_name="z", x_stretched=True)
     with pytest.raises(NotImplementedError, match="Stretched grids cannot set"):
         _ = ds.yt.load_grid(length_unit="km", chunksizes=10, use_callable=False)
 
 
 def test_dask_array():
-
     # checks that we can handle a field that is a dask array
     shp = (10, 12, 5)
     f1 = da.random.random(shp, chunks=5)
     coords = {
         "x": np.linspace(0, 1, shp[0]),
         "y": np.linspace(0, 1, shp[1]),
         "z": np.linspace(0, 1, shp[2]),
```

### Comparing `yt_xarray-0.2.0/yt_xarray/tests/test_sample_data.py` & `yt_xarray-0.3.0/yt_xarray/tests/test_sample_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import pytest
 import xarray as xr
 
 from yt_xarray.sample_data import load_random_xr_data
 
 
 def test_load_random_xr_data():
-
     fields = {
         "field0": ("x", "y"),
         "field1": ("x", "y", "z"),
         "field2": ("x", "t"),
         "field3": ("x", "y", "t"),
     }
     dims = {"x": (0, 1, 4), "y": (0, 2, 6), "z": (-1, 0.5, 5), "t": (1, 200, 7)}
@@ -19,13 +18,12 @@
         assert hasattr(ds, field)
 
     ds = load_random_xr_data(fields, dims, length_unit="km")
     assert ds.attrs["geospatial_vertical_units"] == "km"
 
 
 def test_load_random_xr_data_bad():
-
     fields = {"field0": ("x", "y")}
     dims = {"x": (0, 1, 4)}
 
     with pytest.raises(KeyError, match="is specified as a dimension for"):
         _ = load_random_xr_data(fields, dims)
```

### Comparing `yt_xarray-0.2.0/yt_xarray/tests/test_utilities.py` & `yt_xarray-0.3.0/yt_xarray/tests/test_utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     # float32 must be upcast for grid positions. This only manifested when
     # using a stretched grid (as the cell_widths were in float32).
     ds = construct_minimal_ds(dtype="float32", x_stretched=True)
     assert ds.test_field.dtype == np.float32
 
 
 def test_file_validation(tmp_path):
-
     tdir = tmp_path / "test_data"
     tdir.mkdir()
     b = tdir / "test_file.txt"
     b.write_text("test test test")
 
     yt.config.ytcfg.set("yt", "test_data_dir", str(tdir))
```

### Comparing `yt_xarray-0.2.0/yt_xarray/tests/test_xr_to_yt.py` & `yt_xarray-0.3.0/yt_xarray/tests/test_xr_to_yt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import builtins
+
 import numpy as np
 import pytest
 import xarray as xr
 import yt
 
 import yt_xarray.accessor._xr_to_yt as xr2yt
 from yt_xarray.utilities._utilities import (
@@ -31,17 +33,15 @@
 
 
 c_m_ds_kwargs = {"latitude": "y_name", "longitude": "x_name", "altitude": "z_name"}
 
 
 @pytest.mark.parametrize("coord", ("latitude", "longitude", "altitude"))
 def test_selection_aliases(coord):
-
     for othername in xr2yt._coord_aliases[coord]:
-
         kwargs = {c_m_ds_kwargs[coord]: othername}
         ds = construct_minimal_ds(**kwargs)
         fields = list(ds.data_vars)
         sel = xr2yt.Selection(ds, fields)
         assert np.all(sel.starting_indices == np.array((0, 0, 0)))
 
         n_edges = ds.data_vars[fields[0]].shape
@@ -70,15 +70,14 @@
         if idim != dim_id:
             assert sel.full_bbox[idim][0] == sel.selected_bbox[idim][0]
             assert sel.full_shape[idim] == sel.selected_shape[idim]
 
 
 @pytest.mark.parametrize("coord", ("latitude", "longitude", "depth"))
 def test_selection_isel(ds_xr, coord):
-
     fields = list(ds_xr.data_vars)
 
     sel_dict = {coord: slice(1, len(ds_xr.coords[coord]))}
     sel_dict_type = "isel"
     sel = xr2yt.Selection(ds_xr, fields, sel_dict=sel_dict, sel_dict_type=sel_dict_type)
     _isel_tester(ds_xr, sel, fields, coord, 1)
 
@@ -125,15 +124,14 @@
         finfo = ds_yt.field_info[("stream", fld)]
         assert finfo.units == ds.data_vars[fld].units
 
     assert ds_yt.field_info[("stream", "flips")].units == ""
 
 
 def test_selection_errors(ds_xr):
-
     coord = "latitude"
     sel_dict = {coord: slice(1, len(ds_xr.coords[coord]))}
     sel_dict_type = "isel"
     with pytest.raises(ValueError, match="Please provide a list of fields"):
         _ = xr2yt.Selection(ds_xr, None, sel_dict=sel_dict, sel_dict_type=sel_dict_type)
 
     x = np.linspace(0, 1, 5)
@@ -348,15 +346,14 @@
 }
 
 
 @pytest.mark.parametrize(
     "geometry", ["cartesian", "spherical", "geographic", "internal_geographic"]
 )
 def test_finding_3rd_dim(geometry):
-
     expected = _expected_geoms[geometry]
     # select any 2, make sure we add the 3rd back. repeat for every permutation
     choices = list(expected)
     for axis_pairs in ((0, 1), (0, 2), (1, 2)):
         axes = [choices[axis_pairs[0]], choices[axis_pairs[1]]]
         new_axes = xr2yt._add_3rd_axis_name(geometry, axes)
         assert len(set(new_axes).difference(set(expected))) == 0
@@ -428,15 +425,14 @@
         ("cartesian", True, True),
         ("geographic", False, True),
         ("internal_geographic", False, True),
         ("not_a_geometry", False, True),
     ],
 )
 def test_selection_interp_validation(geometry, stretched, interp_required):
-
     if geometry == "cartesian":
         dim_names = ("x", "y", "z")
     elif geometry == "geographic":
         dim_names = ("longitude", "latitude", "altitude")
     elif geometry == "internal_geographic":
         dim_names = ("longitude", "latitude", "depth")
     else:
@@ -463,15 +459,14 @@
     assert interp_reqd_actual == interp_required
 
 
 @pytest.mark.parametrize(
     "yt_geom", ("cartesian", "spherical", "geographic", "internal_geographic")
 )
 def test_add_3rd_axis_name(yt_geom):
-
     # get full list, remove on and make sure we get it back
     expected = list(xr2yt._expected_yt_axes[yt_geom])
     actual = xr2yt._add_3rd_axis_name(yt_geom, expected[:-1])
     for dim in expected:
         assert dim in actual
 
     with pytest.raises(RuntimeError, match="This function should only"):
@@ -536,7 +531,66 @@
         assert np.all(grid_obj.cell_widths[ax_id] > 0)
 
     slc, vals = _get_pixelized_slice(yt_ds)
 
     pdy_lats = slc._generate_container_field("pdy")
     assert np.all(pdy_lats > 0)
     assert np.all(np.isfinite(vals))
+
+
+def test_cf_xarray_disambiguation():
+    from cf_xarray.datasets import airds
+
+    # run the whole selection (will internally run coord disambiguation)
+    sel = xr2yt.Selection(
+        airds, fields=["air"], sel_dict={"time": 0}, sel_dict_type="isel"
+    )
+    xr_da = airds.air
+    selected_names = []
+    for c in sel.selected_coords:
+        selected_names.append(xr2yt._cf_xr_coord_disamb(c, xr_da)[0])
+
+    assert "latitude" in selected_names
+    assert "longitude" in selected_names
+
+
+def test_missing_cfxarray(monkeypatch):
+    from cf_xarray.datasets import airds
+
+    def _bad_import(name, globals=None, locals=None, fromlist=(), level=0):
+        raise ImportError
+
+    xr_da = airds.air
+    clist = list(xr_da.dims)
+    with monkeypatch.context() as m:
+        m.setattr(builtins, "__import__", _bad_import)
+        with pytest.raises(ValueError, match=f"{clist[0]} is not"):
+
+            _ = xr2yt._convert_to_yt_internal_coords(clist, xr_da)
+
+
+def test_coord_alias_reset():
+    xr2yt.known_coord_aliases["blah"] = "lwkerj"
+    xr2yt.reset_coordinate_aliases()
+    assert "blah" not in xr2yt.known_coord_aliases
+
+
+def test_reader_with_2d_space_time_and_reverse_axis():
+
+    # test for https://github.com/data-exp-lab/yt_xarray/issues/86
+
+    # a base xarray ds to be used in various places.
+    ds = construct_ds_with_extra_dim(
+        3,
+        ncoords=5,
+        nd_space=2,
+        reverse_indices=[
+            1,
+        ],
+    )
+
+    field = ("stream", "test_case_3")
+    ds_yt = ds.yt.load_grid(
+        "test_case_3", sel_dict={"time": 0}, geometry="geographic", use_callable=True
+    )
+    slc = yt.SlicePlot(ds_yt, "altitude", field)
+    assert np.all(np.isfinite(slc.frb[field]))
```

### Comparing `yt_xarray-0.2.0/yt_xarray/utilities/_utilities.py` & `yt_xarray-0.3.0/yt_xarray/utilities/_utilities.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+import importlib
 import os.path
-from typing import Optional, Tuple
+from typing import List, Optional, Tuple
 
 import numpy as np
 import xarray as xr
 import yt.config
 
 from yt_xarray.accessor._xr_to_yt import known_coord_aliases
 
@@ -27,15 +28,14 @@
     z_stretched: bool = False,
     field_name: str = "test_field",
     n_fields: int = 1,
     coord_order: Optional[Tuple[str, str, str]] = None,
     dtype: str = "float64",
     npseed: bool = False,
 ) -> xr.Dataset:
-
     if coord_order is None:
         coord_order = ("z", "y", "x")
 
     dtype_to_use = getattr(np, dtype)
 
     # contruct and return a minimal xarray dataset to use in tests as needed
 
@@ -108,16 +108,15 @@
     for _ in range(nt):
         tvals.append(tvals[-1] + dt)
     return np.array(tvals)
 
 
 def _get_test_coord(
     cname, n, minv: Optional[float] = None, maxv: Optional[float] = None
-):
-
+) -> np.ndarray:
     if cname in known_coord_aliases:
         cname = known_coord_aliases[cname]
 
     if cname == "time":
         return _test_time_coord(nt=n)
 
     if cname == "latitude":
@@ -138,30 +137,46 @@
         minv = 0.0
     if maxv is None:
         maxv = 1.0
 
     return np.linspace(minv, maxv, n)
 
 
-def construct_ds_with_extra_dim(icoord: int, dim_name: str = "time"):
-
+def construct_ds_with_extra_dim(
+    icoord: int,
+    dim_name: str = "time",
+    ncoords: Optional[int] = None,
+    nd_space: int = 3,
+    reverse_indices: Optional[List[int]] = None,
+):
     coord_configs = {
         0: (dim_name, "x", "y", "z"),
         1: (dim_name, "z", "y", "x"),
         2: (dim_name, "lon", "lat", "lev"),
         3: (dim_name, "longitude", "latitude", "altitude"),
         4: (dim_name, "depth", "longitude", "lat"),
     }
 
     data_vars = {}
-    coords = {c: _get_test_coord(c, icoord + 4) for c in coord_configs[icoord]}
+    if ncoords is None:
+        ncoords = icoord + 4
+
+    full_dims = coord_configs[icoord]
+    dim_order = [full_dims[idim] for idim in range(nd_space + 1)]
+    coords = {c: _get_test_coord(c, ncoords) for c in dim_order}
+
+    if reverse_indices is not None:
+        for indx in reverse_indices:
+            dim = dim_order[indx]
+            coords[dim] = coords[dim][::-1]
+
     var_shape = tuple([len(c) for c in coords.values()])
     vals = np.random.random(var_shape)
     fname = f"test_case_{icoord}"
-    da = xr.DataArray(vals, coords=coords, dims=coord_configs[icoord])
+    da = xr.DataArray(vals, coords=coords, dims=dim_order)
     data_vars[fname] = da
 
     return xr.Dataset(data_vars=data_vars)
 
 
 def _find_file(file):
     if os.path.isfile(file):
@@ -181,7 +196,23 @@
 
 def _validate_file(function):
     def validate_then_call(file, *args, **kwargs):
         goodfile = _find_file(file)
         return function(goodfile, *args, **kwargs)
 
     return validate_then_call
+
+
+def _import_optional_dep(
+    name: str, package: Optional[str] = None, custom_message: Optional[str] = None
+):
+    # wrapper of importlib.import_module
+    # name, package get sent to importlib.import_module
+    # custom_message will overwrite the ImportError message if the package is not
+    # found.
+    try:
+        return importlib.import_module(name, package=package)
+    except ImportError:
+        msg = custom_message
+        if msg is None:
+            msg = f"This functionality requires {name}. Install it and try again."
+        raise ImportError(msg)
```

### Comparing `yt_xarray-0.2.0/yt_xarray.egg-info/PKG-INFO` & `yt_xarray-0.3.0/yt_xarray.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: yt-xarray
-Version: 0.2.0
+Name: yt_xarray
+Version: 0.3.0
 Summary: interface between yt and xarray
 Author-email: Chris Havlin <chris.havlin@gmail.com>
 Project-URL: Homepage, https://github.com/data-exp-lab/yt_xarray
 Project-URL: Bug Tracker, https://github.com/data-exp-lab/yt_xarray/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -21,31 +21,34 @@
 Requires-Dist: h5py>=3.4.0
 Requires-Dist: pooch>=1.5.1
 Requires-Dist: xarray
 Provides-Extra: full
 Requires-Dist: netCDF4; extra == "full"
 Requires-Dist: scipy; extra == "full"
 Requires-Dist: dask[complete]; extra == "full"
+Requires-Dist: cf_xarray; extra == "full"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: cartopy; extra == "test"
 Provides-Extra: docs
-Requires-Dist: Sphinx==1.8.5; extra == "docs"
-Requires-Dist: jinja2<3.1.0; extra == "docs"
-Requires-Dist: nbsphinx; extra == "docs"
+Requires-Dist: Sphinx==7.2.6; extra == "docs"
+Requires-Dist: jinja2==3.1.2; extra == "docs"
+Requires-Dist: nbsphinx==0.9.3; extra == "docs"
 
 # yt_xarray
 
-
 [![PyPI version](https://badge.fury.io/py/yt_xarray.svg)](https://badge.fury.io/py/yt_xarray)
+[![Python Version](https://img.shields.io/pypi/pyversions/yt_xarray.svg?color=green)](https://python.org)
+[![Tests](https://github.com/data-exp-lab/yt_xarray/actions/workflows/run-pytest-tests.yml/badge.svg)](https://github.com/data-exp-lab/yt_xarray/actions/workflows/run-pytest-tests.yml)
+[![codecov](https://codecov.io/gh/data-exp-lab/yt_xarray/branch/main/graph/badge.svg)](https://codecov.io/gh/data-exp-lab/yt_xarray)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/data-exp-lab/yt_xarray/main.svg)](https://results.pre-commit.ci/latest/github/data-exp-lab/yt_xarray/main)
 
 An interface between yt and xarray
 
-
 ## Overview
 
 yt_xarray streamlines communication between
 [xarray](https://docs.xarray.dev/en/stable/#) and [yt](https://yt-project.org),
 making it easier use yt's visualization and analysis methods with data loaded
 via xarray.
```

### Comparing `yt_xarray-0.2.0/yt_xarray.egg-info/SOURCES.txt` & `yt_xarray-0.3.0/yt_xarray.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -6,50 +6,58 @@
 CONTRIBUTING.md
 HISTORY.md
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 pyproject.toml
-requirements_docs.txt
 docs/Makefile
 docs/conf.py
 docs/contributing.rst
 docs/examples.rst
 docs/faq.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
-docs/modules.rst
 docs/supported_grids.rst
-docs/yt_xarray.accessor.rst
-docs/yt_xarray.rst
-docs/yt_xarray.utilities.rst
 docs/examples/example_001_xr_to_yt.ipynb
 docs/examples/example_002_coord_aliases.ipynb
 docs/examples/example_003_two_dimensional_fields.ipynb
 docs/examples/example_004_xr_yt_cartopy.ipynb
 docs/examples/example_005_chunked_data.ipynb
+docs/examples/example_006_yt_method_access.ipynb
+docs/examples/example_007_interpolation.ipynb
+docs/examples/example_008_interpolation_with_refinement.ipynb
+docs/examples/example_009_custom_transformations.ipynb
+docs/examples/example_010_custom_interpolations.ipynb
 docs/source/modules.rst
-docs/source/yt_xarray.accessor.rst
-docs/source/yt_xarray.rst
+docs/source/yt_xarray.YtAccessor.rst
+docs/source/yt_xarray.open_dataset.rst
+docs/source/yt_xarray.sample_data.rst
+docs/source/yt_xarray.transformations.rst
 yt_xarray/__init__.py
 yt_xarray/sample_data.py
+yt_xarray/transformations.py
 yt_xarray/yt_xarray.py
 yt_xarray.egg-info/PKG-INFO
 yt_xarray.egg-info/SOURCES.txt
 yt_xarray.egg-info/dependency_links.txt
 yt_xarray.egg-info/requires.txt
 yt_xarray.egg-info/top_level.txt
 yt_xarray/accessor/__init__.py
 yt_xarray/accessor/_readers.py
 yt_xarray/accessor/_xr_to_yt.py
 yt_xarray/accessor/accessor.py
 yt_xarray/tests/__init__.py
 yt_xarray/tests/test_accesor.py
 yt_xarray/tests/test_chunking.py
+yt_xarray/tests/test_grid_decomposition.py
+yt_xarray/tests/test_optional_imports.py
 yt_xarray/tests/test_sample_data.py
+yt_xarray/tests/test_transformations.py
 yt_xarray/tests/test_utilities.py
 yt_xarray/tests/test_xr_to_yt.py
+yt_xarray/tests/test_yt_wrappers.py
 yt_xarray/utilities/__init__.py
+yt_xarray/utilities/_grid_decomposition.py
 yt_xarray/utilities/_utilities.py
 yt_xarray/utilities/logging.py
```

