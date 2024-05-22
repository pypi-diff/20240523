# Comparing `tmp/metloom-0.4.2.tar.gz` & `tmp/metloom-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metloom-0.4.2.tar", last modified: Mon May  6 16:59:31 2024, max compression
+gzip compressed data, was "metloom-0.4.3.tar", last modified: Wed May 22 22:32:57 2024, max compression
```

## Comparing `metloom-0.4.2.tar` & `metloom-0.4.3.tar`

### file list

```diff
@@ -1,83 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:59:31.827835 metloom-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-06 16:59:24.000000 metloom-0.4.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-06 16:59:24.000000 metloom-0.4.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-06 16:59:24.000000 metloom-0.4.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-06 16:59:24.000000 metloom-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-06 16:59:24.000000 metloom-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-05-06 16:59:31.827835 metloom-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-05-06 16:59:24.000000 metloom-0.4.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:59:31.819835 metloom-0.4.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-06 16:59:24.000000 metloom-0.4.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-06 16:59:24.000000 metloom-0.4.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-06 16:59:24.000000 metloom-0.4.2/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     4999 2024-05-06 16:59:24.000000 metloom-0.4.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-06 16:59:24.000000 metloom-0.4.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-06 16:59:24.000000 metloom-0.4.2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-06 16:59:24.000000 metloom-0.4.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-06 16:59:24.000000 metloom-0.4.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-06 16:59:24.000000 metloom-0.4.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-06 16:59:24.000000 metloom-0.4.2/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-06 16:59:24.000000 metloom-0.4.2/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:59:31.819835 metloom-0.4.2/metloom/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-06 16:59:24.000000 metloom-0.4.2/metloom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-06 16:59:24.000000 metloom-0.4.2/metloom/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-06 16:59:24.000000 metloom-0.4.2/metloom/dataframe_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:59:31.819835 metloom-0.4.2/metloom/pointdata/
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-06 16:59:24.000000 metloom-0.4.2/metloom/pointdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9299 2024-05-06 16:59:24.000000 metloom-0.4.2/metloom/pointdata/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    16704 2024-05-06 16:59:24.000000 metloom-0.4.2/metloom/pointdata/cdec.py
--rw-r--r--   0 runner    (1001) docker     (127)    14252 2024-05-06 16:59:24.000000 metloom-0.4.2/metloom/pointdata/geosphere_austria.py
--rw-r--r--   0 runner    (1001) docker     (127)    13801 2024-05-06 16:59:24.000000 metloom-0.4.2/metloom/pointdata/mesowest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13870 2024-05-06 16:59:24.000000 metloom-0.4.2/metloom/pointdata/snotel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-05-06 16:59:24.000000 metloom-0.4.2/metloom/pointdata/snotel_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    17138 2024-05-06 16:59:24.000000 metloom-0.4.2/metloom/pointdata/usgs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-06 16:59:24.000000 metloom-0.4.2/metloom/request_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8682 2024-05-06 16:59:24.000000 metloom-0.4.2/metloom/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:59:31.827835 metloom-0.4.2/metloom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-05-06 16:59:31.000000 metloom-0.4.2/metloom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-06 16:59:31.000000 metloom-0.4.2/metloom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:59:31.000000 metloom-0.4.2/metloom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-06 16:59:31.000000 metloom-0.4.2/metloom.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:59:31.000000 metloom-0.4.2/metloom.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-06 16:59:31.000000 metloom-0.4.2/metloom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-06 16:59:31.000000 metloom-0.4.2/metloom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-06 16:59:31.827835 metloom-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-06 16:59:24.000000 metloom-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:59:31.823835 metloom-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 16:59:24.000000 metloom-0.4.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:59:31.827835 metloom-0.4.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-06 16:59:24.000000 metloom-0.4.2/tests/data/austria_box.cpg
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-06 16:59:24.000000 metloom-0.4.2/tests/data/austria_box.dbf
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-06 16:59:24.000000 metloom-0.4.2/tests/data/austria_box.prj
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-06 16:59:24.000000 metloom-0.4.2/tests/data/austria_box.shp
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-06 16:59:24.000000 metloom-0.4.2/tests/data/austria_box.shx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:59:31.827835 metloom-0.4.2/tests/data/cdec_mocks/
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-06 16:59:24.000000 metloom-0.4.2/tests/data/cdec_mocks/raw_tny_locations.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:59:31.827835 metloom-0.4.2/tests/data/geosphere_mocks/
--rw-r--r--   0 runner    (1001) docker     (127)   287245 2024-05-06 16:59:24.000000 metloom-0.4.2/tests/data/geosphere_mocks/klima_mock.json
--rw-r--r--   0 runner    (1001) docker     (127)   104970 2024-05-06 16:59:24.000000 metloom-0.4.2/tests/data/geosphere_mocks/meta_mock.json
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-06 16:59:24.000000 metloom-0.4.2/tests/data/testing.cpg
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-06 16:59:24.000000 metloom-0.4.2/tests/data/testing.dbf
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-06 16:59:24.000000 metloom-0.4.2/tests/data/testing.prj
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-06 16:59:24.000000 metloom-0.4.2/tests/data/testing.shp
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-06 16:59:24.000000 metloom-0.4.2/tests/data/testing.shx
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-06 16:59:24.000000 metloom-0.4.2/tests/data/triangle.cpg
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-06 16:59:24.000000 metloom-0.4.2/tests/data/triangle.dbf
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-06 16:59:24.000000 metloom-0.4.2/tests/data/triangle.prj
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-06 16:59:24.000000 metloom-0.4.2/tests/data/triangle.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-06 16:59:24.000000 metloom-0.4.2/tests/data/triangle.shp
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-06 16:59:24.000000 metloom-0.4.2/tests/data/triangle.shx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:59:31.827835 metloom-0.4.2/tests/data/usgs_mocks/
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-05-06 16:59:24.000000 metloom-0.4.2/tests/data/usgs_mocks/daily_response.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10027 2024-05-06 16:59:24.000000 metloom-0.4.2/tests/data/usgs_mocks/hourly_response.json
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-06 16:59:24.000000 metloom-0.4.2/tests/data/usgs_mocks/platoro_meta.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-06 16:59:24.000000 metloom-0.4.2/tests/data/usgs_mocks/station_search_response.txt
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-06 16:59:24.000000 metloom-0.4.2/tests/shp_to_boxshp.py
--rw-r--r--   0 runner    (1001) docker     (127)    23328 2024-05-06 16:59:24.000000 metloom-0.4.2/tests/test_cdec.py
--rw-r--r--   0 runner    (1001) docker     (127)     6377 2024-05-06 16:59:24.000000 metloom-0.4.2/tests/test_dataframe_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11844 2024-05-06 16:59:24.000000 metloom-0.4.2/tests/test_geosphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    13375 2024-05-06 16:59:24.000000 metloom-0.4.2/tests/test_mesowest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-06 16:59:24.000000 metloom-0.4.2/tests/test_point_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    15999 2024-05-06 16:59:24.000000 metloom-0.4.2/tests/test_snotel.py
--rw-r--r--   0 runner    (1001) docker     (127)     9142 2024-05-06 16:59:24.000000 metloom-0.4.2/tests/test_usgs.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-06 16:59:24.000000 metloom-0.4.2/tests/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:32:57.140506 metloom-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-22 22:32:52.000000 metloom-0.4.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-22 22:32:52.000000 metloom-0.4.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-22 22:32:52.000000 metloom-0.4.3/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-22 22:32:52.000000 metloom-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-22 22:32:52.000000 metloom-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6574 2024-05-22 22:32:57.140506 metloom-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-05-22 22:32:52.000000 metloom-0.4.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:32:57.128506 metloom-0.4.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-22 22:32:52.000000 metloom-0.4.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-22 22:32:52.000000 metloom-0.4.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-22 22:32:52.000000 metloom-0.4.3/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5069 2024-05-22 22:32:52.000000 metloom-0.4.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-22 22:32:52.000000 metloom-0.4.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-22 22:32:52.000000 metloom-0.4.3/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-22 22:32:52.000000 metloom-0.4.3/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-22 22:32:52.000000 metloom-0.4.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-22 22:32:52.000000 metloom-0.4.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-22 22:32:52.000000 metloom-0.4.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 22:32:52.000000 metloom-0.4.3/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-22 22:32:52.000000 metloom-0.4.3/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:32:57.128506 metloom-0.4.3/metloom/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-22 22:32:52.000000 metloom-0.4.3/metloom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-22 22:32:52.000000 metloom-0.4.3/metloom/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-22 22:32:52.000000 metloom-0.4.3/metloom/dataframe_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:32:57.132506 metloom-0.4.3/metloom/pointdata/
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-22 22:32:52.000000 metloom-0.4.3/metloom/pointdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9299 2024-05-22 22:32:52.000000 metloom-0.4.3/metloom/pointdata/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16704 2024-05-22 22:32:52.000000 metloom-0.4.3/metloom/pointdata/cdec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14252 2024-05-22 22:32:52.000000 metloom-0.4.3/metloom/pointdata/geosphere_austria.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13801 2024-05-22 22:32:52.000000 metloom-0.4.3/metloom/pointdata/mesowest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13870 2024-05-22 22:32:52.000000 metloom-0.4.3/metloom/pointdata/snotel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-05-22 22:32:52.000000 metloom-0.4.3/metloom/pointdata/snotel_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17138 2024-05-22 22:32:52.000000 metloom-0.4.3/metloom/pointdata/usgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-22 22:32:52.000000 metloom-0.4.3/metloom/request_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-05-22 22:32:52.000000 metloom-0.4.3/metloom/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:32:57.140506 metloom-0.4.3/metloom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6574 2024-05-22 22:32:57.000000 metloom-0.4.3/metloom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-22 22:32:57.000000 metloom-0.4.3/metloom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 22:32:57.000000 metloom-0.4.3/metloom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-22 22:32:57.000000 metloom-0.4.3/metloom.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 22:32:56.000000 metloom-0.4.3/metloom.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-22 22:32:57.000000 metloom-0.4.3/metloom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 22:32:57.000000 metloom-0.4.3/metloom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-22 22:32:57.140506 metloom-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-22 22:32:52.000000 metloom-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:32:57.136506 metloom-0.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:32:57.136506 metloom-0.4.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/austria_box.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/austria_box.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/austria_box.prj
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/austria_box.shp
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/austria_box.shx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:32:57.136506 metloom-0.4.3/tests/data/cdec_mocks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/cdec_mocks/raw_tny_locations.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:32:57.140506 metloom-0.4.3/tests/data/geosphere_mocks/
+-rw-r--r--   0 runner    (1001) docker     (127)   287245 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/geosphere_mocks/klima_mock.json
+-rw-r--r--   0 runner    (1001) docker     (127)   104970 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/geosphere_mocks/meta_mock.json
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/testing.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/testing.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/testing.prj
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/testing.shp
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/testing.shx
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/triangle.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/triangle.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/triangle.prj
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/triangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/triangle.shp
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/triangle.shx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:32:57.140506 metloom-0.4.3/tests/data/usgs_mocks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/usgs_mocks/daily_response.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10027 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/usgs_mocks/hourly_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/usgs_mocks/platoro_meta.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/usgs_mocks/station_search_response.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/shp_to_boxshp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23328 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/test_cdec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6377 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/test_dataframe_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11844 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/test_geosphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13375 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/test_mesowest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/test_point_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15999 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/test_snotel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9142 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/test_usgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/test_variables.py
```

### Comparing `metloom-0.4.2/CONTRIBUTING.rst` & `metloom-0.4.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `metloom-0.4.2/HISTORY.rst` & `metloom-0.4.3/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `metloom-0.4.2/LICENSE` & `metloom-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `metloom-0.4.2/PKG-INFO` & `metloom-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metloom
-Version: 0.4.2
+Version: 0.4.3
 Summary: Location Oriented Observed Meteorology (LOOM)
 Home-page: https://github.com/M3Works/metloom
 Author: M3Works
 Author-email: m3worksllc@gmail.com
 License: BSD license
 Keywords: metloom
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -132,16 +132,15 @@
 
 **NOTES:**
 PointData methods that get point data return a GeoDataFrame indexed
 on *both* datetime and station code. To reset the index simply run
 ``df.reset_index(inplace=True)``
 
 Simple usage examples are provided in this readme and in the docs. See
-our `examples <https://github.com/M3Works/metloom/tree/main/examples>`_ and
-`tutorial <https://github.com/M3Works/metloom/tree/main/examples/tutorial>`_
+our `examples <https://github.com/M3Works/metloom/tree/main/docs/gallery>`_
 for code walkthroughs and more complicated use cases.
 
 Usage Examples
 ==============
 
 Use metloom to find data for a station
```

### Comparing `metloom-0.4.2/README.rst` & `metloom-0.4.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -104,16 +104,15 @@
 
 **NOTES:**
 PointData methods that get point data return a GeoDataFrame indexed
 on *both* datetime and station code. To reset the index simply run
 ``df.reset_index(inplace=True)``
 
 Simple usage examples are provided in this readme and in the docs. See
-our `examples <https://github.com/M3Works/metloom/tree/main/examples>`_ and
-`tutorial <https://github.com/M3Works/metloom/tree/main/examples/tutorial>`_
+our `examples <https://github.com/M3Works/metloom/tree/main/docs/gallery>`_
 for code walkthroughs and more complicated use cases.
 
 Usage Examples
 ==============
 
 Use metloom to find data for a station
```

### Comparing `metloom-0.4.2/docs/Makefile` & `metloom-0.4.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `metloom-0.4.2/docs/conf.py` & `metloom-0.4.3/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode', 'sphinxcontrib.apidoc']
+extensions = ['sphinx.ext.autodoc','sphinxcontrib.apidoc', 'sphinx.ext.viewcode', 'nbsphinx', 'sphinx_gallery.load_style','sphinx.ext.autosectionlabel']
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
```

### Comparing `metloom-0.4.2/docs/installation.rst` & `metloom-0.4.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `metloom-0.4.2/docs/make.bat` & `metloom-0.4.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `metloom-0.4.2/docs/usage.rst` & `metloom-0.4.3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `metloom-0.4.2/metloom/cli.py` & `metloom-0.4.3/metloom/cli.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.2/metloom/dataframe_utils.py` & `metloom-0.4.3/metloom/dataframe_utils.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.2/metloom/pointdata/base.py` & `metloom-0.4.3/metloom/pointdata/base.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.2/metloom/pointdata/cdec.py` & `metloom-0.4.3/metloom/pointdata/cdec.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.2/metloom/pointdata/geosphere_austria.py` & `metloom-0.4.3/metloom/pointdata/geosphere_austria.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.2/metloom/pointdata/mesowest.py` & `metloom-0.4.3/metloom/pointdata/mesowest.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.2/metloom/pointdata/snotel.py` & `metloom-0.4.3/metloom/pointdata/snotel.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.2/metloom/pointdata/snotel_client.py` & `metloom-0.4.3/metloom/pointdata/snotel_client.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.2/metloom/pointdata/usgs.py` & `metloom-0.4.3/metloom/pointdata/usgs.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.2/metloom/request_utils.py` & `metloom-0.4.3/metloom/request_utils.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.2/metloom/variables.py` & `metloom-0.4.3/metloom/variables.py`

 * *Files 15% similar despite different names*

```diff
@@ -178,14 +178,46 @@
     STREAMFLOW = SensorDescription(
         "74082", "STREAMFLOW", "STREAMFLOW, DAILY VOLUME (AC-FT)"
     )
     SNOWDEPTH = SensorDescription("72189", "SNOWDEPTH", "Snow depth, Meters")
     SWE = SensorDescription(
         "72341", "SWE", "Water content of snow, millimeters"
     )
+    SOLARRADIATION = SensorDescription(
+        "72179", "SOLAR RADIATION",
+        "Shortwave solar radiation, watts per square meter"
+    )
+    UPSHORTWAVE = SensorDescription(
+        "72185", "UPWARD SHORTWAVE RADIATION",
+        "Shortwave radiation, upward intensity, watts per square meter"
+    )
+    DOWNSHORTWAVE = SensorDescription(
+        "72186", "DOWNWARD SHORTWAVE RADIATION",
+        "Shortwave radiation, downward intensity, watts per square meter"
+    )
+    NETSHORTWAVE = SensorDescription(
+        "72201", "NET SHORTWAVE RADIATION",
+        "Net incident shortwave radiation, watts per square meter",
+    )
+    NETLONGWAVE = SensorDescription(
+        "72202", "NET LONGWAVE RADIATION",
+        "Net emitted longwave radiation, watts per square meter"
+    )
+    DOWNLONGWAVE = SensorDescription(
+        "72175", "DOWNWARD LONGWAVE RADIATION",
+        "Longwave radiation, downward intensity, watts per square meter"
+    )
+    UPLONGWAVE = SensorDescription(
+        "72174", "UPWARD LONGWAVE RADIATION",
+        "Longwave radiation, upward intensity, watts per square meter"
+    )
+    SURFACETEMP = SensorDescription(
+        "72405", "SURFACE TEMPERATURE",
+        "Surface temperature, non-contact, degrees Celsius"
+    )
 
 
 class GeoSphereCurrentVariables(VariableBase):
     TEMP = SensorDescription("TL", "Air Temperature")
     SNOWDEPTH = SensorDescription(
         "SCHNEE", "Snowdepth"
     )
```

### Comparing `metloom-0.4.2/metloom.egg-info/PKG-INFO` & `metloom-0.4.3/metloom.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metloom
-Version: 0.4.2
+Version: 0.4.3
 Summary: Location Oriented Observed Meteorology (LOOM)
 Home-page: https://github.com/M3Works/metloom
 Author: M3Works
 Author-email: m3worksllc@gmail.com
 License: BSD license
 Keywords: metloom
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -132,16 +132,15 @@
 
 **NOTES:**
 PointData methods that get point data return a GeoDataFrame indexed
 on *both* datetime and station code. To reset the index simply run
 ``df.reset_index(inplace=True)``
 
 Simple usage examples are provided in this readme and in the docs. See
-our `examples <https://github.com/M3Works/metloom/tree/main/examples>`_ and
-`tutorial <https://github.com/M3Works/metloom/tree/main/examples/tutorial>`_
+our `examples <https://github.com/M3Works/metloom/tree/main/docs/gallery>`_
 for code walkthroughs and more complicated use cases.
 
 Usage Examples
 ==============
 
 Use metloom to find data for a station
```

### Comparing `metloom-0.4.2/metloom.egg-info/SOURCES.txt` & `metloom-0.4.3/metloom.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 setup.cfg
 setup.py
 docs/Makefile
 docs/api.rst
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
+docs/examples.rst
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 metloom/__init__.py
```

### Comparing `metloom-0.4.2/setup.py` & `metloom-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     include_package_data=True,
     keywords='metloom',
     name='metloom',
     packages=find_packages(include=['metloom', 'metloom.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/M3Works/metloom',
-    version='0.4.2',
+    version='0.4.3',
     zip_safe=False,
 )
```

### Comparing `metloom-0.4.2/tests/data/cdec_mocks/raw_tny_locations.csv` & `metloom-0.4.3/tests/data/cdec_mocks/raw_tny_locations.csv`

 * *Files identical despite different names*

### Comparing `metloom-0.4.2/tests/data/geosphere_mocks/klima_mock.json` & `metloom-0.4.3/tests/data/geosphere_mocks/klima_mock.json`

 * *Files identical despite different names*

### Comparing `metloom-0.4.2/tests/data/geosphere_mocks/meta_mock.json` & `metloom-0.4.3/tests/data/geosphere_mocks/meta_mock.json`

 * *Files identical despite different names*

### Comparing `metloom-0.4.2/tests/data/usgs_mocks/daily_response.txt` & `metloom-0.4.3/tests/data/usgs_mocks/daily_response.txt`

 * *Files identical despite different names*

### Comparing `metloom-0.4.2/tests/data/usgs_mocks/hourly_response.json` & `metloom-0.4.3/tests/data/usgs_mocks/hourly_response.json`

 * *Files identical despite different names*

### Comparing `metloom-0.4.2/tests/data/usgs_mocks/platoro_meta.txt` & `metloom-0.4.3/tests/data/usgs_mocks/platoro_meta.txt`

 * *Files identical despite different names*

### Comparing `metloom-0.4.2/tests/data/usgs_mocks/station_search_response.txt` & `metloom-0.4.3/tests/data/usgs_mocks/station_search_response.txt`

 * *Files identical despite different names*

### Comparing `metloom-0.4.2/tests/shp_to_boxshp.py` & `metloom-0.4.3/tests/shp_to_boxshp.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.2/tests/test_cdec.py` & `metloom-0.4.3/tests/test_cdec.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.2/tests/test_dataframe_utils.py` & `metloom-0.4.3/tests/test_dataframe_utils.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.2/tests/test_geosphere.py` & `metloom-0.4.3/tests/test_geosphere.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.2/tests/test_mesowest.py` & `metloom-0.4.3/tests/test_mesowest.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.2/tests/test_point_data.py` & `metloom-0.4.3/tests/test_point_data.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.2/tests/test_snotel.py` & `metloom-0.4.3/tests/test_snotel.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.2/tests/test_usgs.py` & `metloom-0.4.3/tests/test_usgs.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.2/tests/test_variables.py` & `metloom-0.4.3/tests/test_variables.py`

 * *Files identical despite different names*

