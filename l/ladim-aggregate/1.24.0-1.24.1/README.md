# Comparing `tmp/ladim_aggregate-1.24.0.tar.gz` & `tmp/ladim_aggregate-1.24.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ladim_aggregate-1.24.0.tar", last modified: Wed Jan 17 13:11:12 2024, max compression
+gzip compressed data, was "ladim_aggregate-1.24.1.tar", last modified: Thu May 23 08:24:16 2024, max compression
```

## Comparing `ladim_aggregate-1.24.0.tar` & `ladim_aggregate-1.24.1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 13:11:12.443762 ladim_aggregate-1.24.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-01-17 13:11:12.443762 ladim_aggregate-1.24.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-01-17 13:11:12.443762 ladim_aggregate-1.24.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 13:11:12.427762 ladim_aggregate-1.24.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 13:11:12.431762 ladim_aggregate-1.24.0/src/ladim_aggregate/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 13:11:12.431762 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 13:11:12.435762 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/complex/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/complex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/complex/aggregate.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/complex/count.nc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/complex/count_20190703000000_12345.nc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/complex/count_20190703000000_12346.nc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/complex/count_20200703000000_12345.nc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/complex/count_20200703000000_12346.nc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/complex/ladim_2019.nc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/complex/ladim_2020.nc.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 13:11:12.435762 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/connect/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/connect/aggregate.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/connect/count.nc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/connect/ladim.nc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/connect/regions.geojson
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 13:11:12.435762 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/filter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/filter/aggregate.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/filter/count.nc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/filter/ladim.nc.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 13:11:12.435762 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/grid_2D/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/grid_2D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/grid_2D/aggregate.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/grid_2D/count.nc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/grid_2D/ladim.nc.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 13:11:12.435762 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/groupby/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/groupby/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/groupby/aggregate.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/groupby/count.nc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/groupby/ladim.nc.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 13:11:12.439762 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/multi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/multi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/multi/aggregate.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/multi/count.nc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/multi/count_12345.nc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/multi/count_12346.nc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/multi/ladim_2019.nc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/multi/ladim_2020.nc.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 13:11:12.439762 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/proj/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/proj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/proj/aggregate.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/proj/count.nc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/proj/ladim.nc.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 13:11:12.439762 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/time/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/time/aggregate.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/time/count.nc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/time/ladim.nc.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 13:11:12.439762 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/weights/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/weights/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/weights/aggregate.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/weights/count.nc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/weights/external.nc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/examples/weights/ladim.nc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/geotag.py
--rw-r--r--   0 runner    (1001) docker     (127)    12475 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)    18321 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/input.py
--rw-r--r--   0 runner    (1001) docker     (127)    15620 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/parseconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/proj.py
--rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/src/ladim_aggregate/script.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 13:11:12.443762 ladim_aggregate-1.24.0/src/ladim_aggregate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-01-17 13:11:12.000000 ladim_aggregate-1.24.0/src/ladim_aggregate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-01-17 13:11:12.000000 ladim_aggregate-1.24.0/src/ladim_aggregate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-17 13:11:12.000000 ladim_aggregate-1.24.0/src/ladim_aggregate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-01-17 13:11:12.000000 ladim_aggregate-1.24.0/src/ladim_aggregate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-01-17 13:11:12.000000 ladim_aggregate-1.24.0/src/ladim_aggregate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-17 13:11:12.000000 ladim_aggregate-1.24.0/src/ladim_aggregate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 13:11:12.443762 ladim_aggregate-1.24.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/tests/test_geotag.py
--rw-r--r--   0 runner    (1001) docker     (127)    13344 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/tests/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)    16753 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/tests/test_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     9713 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/tests/test_output.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/tests/test_parseconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/tests/test_proj.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-01-17 13:11:04.000000 ladim_aggregate-1.24.0/tests/test_script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:24:16.966468 ladim_aggregate-1.24.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-23 08:24:16.966468 ladim_aggregate-1.24.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-23 08:24:16.966468 ladim_aggregate-1.24.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:24:16.954468 ladim_aggregate-1.24.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:24:16.958468 ladim_aggregate-1.24.1/src/ladim_aggregate/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:24:16.958468 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:24:16.958468 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/complex/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/complex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/complex/aggregate.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/complex/count.nc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/complex/count_20190703000000_12345.nc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/complex/count_20190703000000_12346.nc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/complex/count_20200703000000_12345.nc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/complex/count_20200703000000_12346.nc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/complex/ladim_2019.nc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/complex/ladim_2020.nc.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:24:16.958468 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/connect/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/connect/aggregate.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/connect/count.nc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/connect/ladim.nc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/connect/regions.geojson
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:24:16.962468 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/filter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/filter/aggregate.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/filter/count.nc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/filter/ladim.nc.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:24:16.962468 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/grid_2D/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/grid_2D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/grid_2D/aggregate.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/grid_2D/count.nc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/grid_2D/ladim.nc.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:24:16.962468 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/groupby/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/groupby/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/groupby/aggregate.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/groupby/count.nc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/groupby/ladim.nc.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:24:16.962468 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/multi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/multi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/multi/aggregate.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/multi/count.nc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/multi/count_12345.nc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/multi/count_12346.nc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/multi/ladim_2019.nc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/multi/ladim_2020.nc.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:24:16.962468 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/proj/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/proj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/proj/aggregate.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/proj/count.nc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/proj/ladim.nc.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:24:16.962468 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/time/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/time/aggregate.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/time/count.nc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/time/ladim.nc.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:24:16.966468 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/weights/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/weights/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/weights/aggregate.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/weights/count.nc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/weights/external.nc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/examples/weights/ladim.nc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/geotag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12475 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18323 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15620 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/parseconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/proj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/src/ladim_aggregate/script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:24:16.966468 ladim_aggregate-1.24.1/src/ladim_aggregate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-23 08:24:16.000000 ladim_aggregate-1.24.1/src/ladim_aggregate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-23 08:24:16.000000 ladim_aggregate-1.24.1/src/ladim_aggregate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 08:24:16.000000 ladim_aggregate-1.24.1/src/ladim_aggregate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-23 08:24:16.000000 ladim_aggregate-1.24.1/src/ladim_aggregate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-23 08:24:16.000000 ladim_aggregate-1.24.1/src/ladim_aggregate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-23 08:24:16.000000 ladim_aggregate-1.24.1/src/ladim_aggregate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:24:16.966468 ladim_aggregate-1.24.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/tests/test_geotag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13344 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/tests/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16753 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/tests/test_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9713 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/tests/test_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/tests/test_parseconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/tests/test_proj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-23 08:24:13.000000 ladim_aggregate-1.24.1/tests/test_script.py
```

### Comparing `ladim_aggregate-1.24.0/LICENSE` & `ladim_aggregate-1.24.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ladim_aggregate-1.24.0/PKG-INFO` & `ladim_aggregate-1.24.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ladim_aggregate
-Version: 1.24.0
+Version: 1.24.1
 Summary: Aggregate tool for LADiM output files
 Author: Pål Næverlid Sævik
 Author-email: paal.naeverlid.saevik@hi.no
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ladim_aggregate-1.24.0/setup.cfg` & `ladim_aggregate-1.24.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ladim_aggregate-1.24.0/src/ladim_aggregate/examples/__init__.py` & `ladim_aggregate-1.24.1/src/ladim_aggregate/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `ladim_aggregate-1.24.0/src/ladim_aggregate/examples/complex/aggregate.yaml` & `ladim_aggregate-1.24.1/src/ladim_aggregate/examples/complex/aggregate.yaml`

 * *Files identical despite different names*

### Comparing `ladim_aggregate-1.24.0/src/ladim_aggregate/examples/complex/count.nc.yaml` & `ladim_aggregate-1.24.1/src/ladim_aggregate/examples/complex/count.nc.yaml`

 * *Files identical despite different names*

### Comparing `ladim_aggregate-1.24.0/src/ladim_aggregate/examples/complex/count_20190703000000_12345.nc.yaml` & `ladim_aggregate-1.24.1/src/ladim_aggregate/examples/complex/count_20190703000000_12345.nc.yaml`

 * *Files identical despite different names*

### Comparing `ladim_aggregate-1.24.0/src/ladim_aggregate/examples/complex/count_20190703000000_12346.nc.yaml` & `ladim_aggregate-1.24.1/src/ladim_aggregate/examples/complex/count_20190703000000_12346.nc.yaml`

 * *Files identical despite different names*

### Comparing `ladim_aggregate-1.24.0/src/ladim_aggregate/examples/complex/count_20200703000000_12345.nc.yaml` & `ladim_aggregate-1.24.1/src/ladim_aggregate/examples/complex/count_20200703000000_12345.nc.yaml`

 * *Files identical despite different names*

### Comparing `ladim_aggregate-1.24.0/src/ladim_aggregate/examples/complex/count_20200703000000_12346.nc.yaml` & `ladim_aggregate-1.24.1/src/ladim_aggregate/examples/complex/count_20200703000000_12346.nc.yaml`

 * *Files identical despite different names*

### Comparing `ladim_aggregate-1.24.0/src/ladim_aggregate/examples/complex/ladim_2019.nc.yaml` & `ladim_aggregate-1.24.1/src/ladim_aggregate/examples/complex/ladim_2019.nc.yaml`

 * *Files identical despite different names*

### Comparing `ladim_aggregate-1.24.0/src/ladim_aggregate/examples/connect/aggregate.yaml` & `ladim_aggregate-1.24.1/src/ladim_aggregate/examples/connect/aggregate.yaml`

 * *Files identical despite different names*

### Comparing `ladim_aggregate-1.24.0/src/ladim_aggregate/examples/connect/regions.geojson` & `ladim_aggregate-1.24.1/src/ladim_aggregate/examples/connect/regions.geojson`

 * *Files identical despite different names*

### Comparing `ladim_aggregate-1.24.0/src/ladim_aggregate/examples/filter/aggregate.yaml` & `ladim_aggregate-1.24.1/src/ladim_aggregate/examples/filter/aggregate.yaml`

 * *Files identical despite different names*

### Comparing `ladim_aggregate-1.24.0/src/ladim_aggregate/examples/grid_2D/aggregate.yaml` & `ladim_aggregate-1.24.1/src/ladim_aggregate/examples/grid_2D/aggregate.yaml`

 * *Files identical despite different names*

### Comparing `ladim_aggregate-1.24.0/src/ladim_aggregate/examples/multi/aggregate.yaml` & `ladim_aggregate-1.24.1/src/ladim_aggregate/examples/multi/aggregate.yaml`

 * *Files identical despite different names*

### Comparing `ladim_aggregate-1.24.0/src/ladim_aggregate/examples/proj/aggregate.yaml` & `ladim_aggregate-1.24.1/src/ladim_aggregate/examples/proj/aggregate.yaml`

 * *Files identical despite different names*

### Comparing `ladim_aggregate-1.24.0/src/ladim_aggregate/examples/proj/count.nc.yaml` & `ladim_aggregate-1.24.1/src/ladim_aggregate/examples/proj/count.nc.yaml`

 * *Files identical despite different names*

### Comparing `ladim_aggregate-1.24.0/src/ladim_aggregate/examples/time/aggregate.yaml` & `ladim_aggregate-1.24.1/src/ladim_aggregate/examples/time/aggregate.yaml`

 * *Files identical despite different names*

### Comparing `ladim_aggregate-1.24.0/src/ladim_aggregate/examples/weights/aggregate.yaml` & `ladim_aggregate-1.24.1/src/ladim_aggregate/examples/weights/aggregate.yaml`

 * *Files identical despite different names*

### Comparing `ladim_aggregate-1.24.0/src/ladim_aggregate/geotag.py` & `ladim_aggregate-1.24.1/src/ladim_aggregate/geotag.py`

 * *Files identical despite different names*

### Comparing `ladim_aggregate-1.24.0/src/ladim_aggregate/histogram.py` & `ladim_aggregate-1.24.1/src/ladim_aggregate/histogram.py`

 * *Files identical despite different names*

### Comparing `ladim_aggregate-1.24.0/src/ladim_aggregate/input.py` & `ladim_aggregate-1.24.1/src/ladim_aggregate/input.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,21 +356,21 @@
     tidx_start = 0
     if timesteps is not None:
         timesteps = np.unique(timesteps)
 
     for dset in dset_iterator(ladim_dsets):
         instance_offset = dset.get('instance_offset', 0)
         pcount_cum = np.concatenate([[0], np.cumsum(dset.particle_count.values)])
-        tidx_list = range(dset.dims['time'])
+        tidx_list = range(dset.sizes['time'])
 
         # Potentially filter out some time steps
         if timesteps is not None:
             include_steps = timesteps - tidx_start
             tidx_list = np.intersect1d(tidx_list, include_steps)
-            tidx_start += dset.dims['time']
+            tidx_start += dset.sizes['time']
 
         for tidx in tidx_list:
             timestr = str(get_time(dset.time[tidx]).astype('datetime64[s]')).replace("T", " ")
             logger.info(f'Read time step {timestr} (time={dset.time[tidx].values.item()})')
             iidx = slice(pcount_cum[tidx], pcount_cum[tidx + 1])
             logger.debug(f'Number of particles: {iidx.stop - iidx.start}')
             if iidx.stop == iidx.start:
```

### Comparing `ladim_aggregate-1.24.0/src/ladim_aggregate/output.py` & `ladim_aggregate-1.24.1/src/ladim_aggregate/output.py`

 * *Files identical despite different names*

### Comparing `ladim_aggregate-1.24.0/src/ladim_aggregate/parseconfig.py` & `ladim_aggregate-1.24.1/src/ladim_aggregate/parseconfig.py`

 * *Files identical despite different names*

### Comparing `ladim_aggregate-1.24.0/src/ladim_aggregate/proj.py` & `ladim_aggregate-1.24.1/src/ladim_aggregate/proj.py`

 * *Files identical despite different names*

### Comparing `ladim_aggregate-1.24.0/src/ladim_aggregate/script.py` & `ladim_aggregate-1.24.1/src/ladim_aggregate/script.py`

 * *Files identical despite different names*

### Comparing `ladim_aggregate-1.24.0/src/ladim_aggregate.egg-info/PKG-INFO` & `ladim_aggregate-1.24.1/src/ladim_aggregate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ladim_aggregate
-Version: 1.24.0
+Version: 1.24.1
 Summary: Aggregate tool for LADiM output files
 Author: Pål Næverlid Sævik
 Author-email: paal.naeverlid.saevik@hi.no
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ladim_aggregate-1.24.0/src/ladim_aggregate.egg-info/SOURCES.txt` & `ladim_aggregate-1.24.1/src/ladim_aggregate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ladim_aggregate-1.24.0/tests/test_examples.py` & `ladim_aggregate-1.24.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `ladim_aggregate-1.24.0/tests/test_geotag.py` & `ladim_aggregate-1.24.1/tests/test_geotag.py`

 * *Files identical despite different names*

### Comparing `ladim_aggregate-1.24.0/tests/test_histogram.py` & `ladim_aggregate-1.24.1/tests/test_histogram.py`

 * *Files identical despite different names*

### Comparing `ladim_aggregate-1.24.0/tests/test_input.py` & `ladim_aggregate-1.24.1/tests/test_input.py`

 * *Files identical despite different names*

### Comparing `ladim_aggregate-1.24.0/tests/test_output.py` & `ladim_aggregate-1.24.1/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `ladim_aggregate-1.24.0/tests/test_parseconfig.py` & `ladim_aggregate-1.24.1/tests/test_parseconfig.py`

 * *Files identical despite different names*

### Comparing `ladim_aggregate-1.24.0/tests/test_proj.py` & `ladim_aggregate-1.24.1/tests/test_proj.py`

 * *Files identical despite different names*

### Comparing `ladim_aggregate-1.24.0/tests/test_script.py` & `ladim_aggregate-1.24.1/tests/test_script.py`

 * *Files identical despite different names*

