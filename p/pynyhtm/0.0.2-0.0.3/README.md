# Comparing `tmp/pynyhtm-0.0.2.tar.gz` & `tmp/pynyhtm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynyhtm-0.0.2.tar", last modified: Thu May 23 06:44:55 2024, max compression
+gzip compressed data, was "pynyhtm-0.0.3.tar", last modified: Thu May 23 09:37:41 2024, max compression
```

## Comparing `pynyhtm-0.0.2.tar` & `pynyhtm-0.0.3.tar`

### file list

```diff
@@ -1,207 +1,207 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.027933 pynyhtm-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-23 06:44:38.000000 pynyhtm-0.0.2/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-23 06:44:38.000000 pynyhtm-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-23 06:44:38.000000 pynyhtm-0.0.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-23 06:44:55.027933 pynyhtm-0.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.027933 pynyhtm-0.0.2/PynyHTM.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-23 06:44:54.000000 pynyhtm-0.0.2/PynyHTM.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-05-23 06:44:54.000000 pynyhtm-0.0.2/PynyHTM.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 06:44:54.000000 pynyhtm-0.0.2/PynyHTM.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-23 06:44:54.000000 pynyhtm-0.0.2/PynyHTM.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 06:44:54.000000 pynyhtm-0.0.2/PynyHTM.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-23 06:44:38.000000 pynyhtm-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:54.995932 pynyhtm-0.0.2/libtinyhtm/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-23 06:44:38.000000 pynyhtm-0.0.2/libtinyhtm/.git
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/README
--rw-r--r--   0 runner    (1001) docker     (127)    13889 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/boost.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/cxx14.py
--rw-r--r--   0 runner    (1001) docker     (127)    74592 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/doxygen.conf
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/hdf5_cxx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.003933 pynyhtm-0.0.2/libtinyhtm/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/Box.hxx
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/Cartesian.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/Cartesian.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     8576 2024-05-23 06:44:46.000000 pynyhtm-0.0.2/libtinyhtm/src/Cartesian.o
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/Circle.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/Ellipse.hxx
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/Exception.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/Polygon.hxx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.003933 pynyhtm-0.0.2/libtinyhtm/src/Query/
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/Query/Query.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/Query.hxx
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/Shape.hxx
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/Spherical.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/Spherical.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-05-23 06:44:46.000000 pynyhtm-0.0.2/libtinyhtm/src/Spherical.o
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/Tree.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/common.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-23 06:44:46.000000 pynyhtm-0.0.2/libtinyhtm/src/common.o
--rw-r--r--   0 runner    (1001) docker     (127)    47194 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/geometry.cxx
--rw-r--r--   0 runner    (1001) docker     (127)    39648 2024-05-23 06:44:46.000000 pynyhtm-0.0.2/libtinyhtm/src/geometry.o
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.011933 pynyhtm-0.0.2/libtinyhtm/src/htm/
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_ids_add.hxx
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_ids_init.cxx
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_ids_init.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-23 06:44:48.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_ids_init.o
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_s2circle_htmcov.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_s2circle_htmcov.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-05-23 06:44:48.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_s2circle_htmcov.o
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.011933 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_s2cpoly_htmcov/
--rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_s2cpoly_htmcov/_htm_isect_test.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_s2cpoly_htmcov/_htm_s2cpoly_htmcov.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_s2cpoly_htmcov.hxx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.011933 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_s2ellipse_htmcov/
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_s2ellipse_htmcov/_htm_s2ellipse_htmcov.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_s2ellipse_htmcov/_htm_s2ellipse_isect.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_s2ellipse_htmcov.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_simplify_ids.cxx
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_simplify_ids.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-23 06:44:48.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_simplify_ids.o
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_subdivide.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_subdivide.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-05-23 06:44:48.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_subdivide.o
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_v3_htmroot.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_s2circle_ids.cxx
--rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-05-23 06:44:48.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_s2circle_ids.o
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_s2cpoly_cv3_template.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_s2cpoly_ids.cxx
--rw-r--r--   0 runner    (1001) docker     (127)    10800 2024-05-23 06:44:48.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_s2cpoly_ids.o
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_s2ellipse_cv3_template.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_s2ellipse_ids.cxx
--rw-r--r--   0 runner    (1001) docker     (127)    10456 2024-05-23 06:44:48.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_s2ellipse_ids.o
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2circle.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-23 06:44:49.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2circle.o
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2circle_range.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     9696 2024-05-23 06:44:49.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2circle_range.o
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2circle_scan.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-23 06:44:50.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2circle_scan.o
--rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2cpoly.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-23 06:44:50.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2cpoly.o
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2cpoly_range.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     9648 2024-05-23 06:44:50.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2cpoly_range.o
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2cpoly_scan.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-23 06:44:51.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2cpoly_scan.o
--rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2ellipse.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-23 06:44:51.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2ellipse.o
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2ellipse_range.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     9304 2024-05-23 06:44:51.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2ellipse_range.o
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2ellipse_scan.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-23 06:44:52.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2ellipse_scan.o
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3_distance2.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3_id.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-05-23 06:44:52.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3_id.o
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.011933 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3p_idsort/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.011933 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3p_idsort/_htm_path_sort/
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3p_idsort/_htm_path_sort/_htm_partition.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3p_idsort/_htm_path_sort/_htm_path_sort.cxx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.011933 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3p_idsort/_htm_rootsort/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3p_idsort/_htm_rootsort/_htm_rootpart.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3p_idsort/_htm_rootsort/_htm_rootsort.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3p_idsort/htm_v3p_idsort.cxx
--rw-r--r--   0 runner    (1001) docker     (127)    10166 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     8395 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm.hxx
--rw-r--r--   0 runner    (1001) docker     (127)    17120 2024-05-23 06:44:47.000000 pynyhtm-0.0.2/libtinyhtm/src/htm.o
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm_convert_to_hdf5.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm_entry.hxx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.015933 pynyhtm-0.0.2/libtinyhtm/src/htm_tree_gen/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.015933 pynyhtm-0.0.2/libtinyhtm/src/htm_tree_gen/blk_sort_ascii/
--rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm_tree_gen/blk_sort_ascii/blk_sort_ascii.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm_tree_gen/blk_sort_ascii/eat_delim.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm_tree_gen/blk_sort_ascii/eat_ws.cxx
--rw-r--r--   0 runner    (1001) docker     (127)    14221 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm_tree_gen/htm_tree_gen.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm_tree_gen/usage.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     9613 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/id_list.cxx
--rw-r--r--   0 runner    (1001) docker     (127)    13640 2024-05-23 06:44:47.000000 pynyhtm-0.0.2/libtinyhtm/src/id_list.o
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/licence.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-23 06:44:47.000000 pynyhtm-0.0.2/libtinyhtm/src/licence.o
--rw-r--r--   0 runner    (1001) docker     (127)    12634 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/select.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-05-23 06:44:47.000000 pynyhtm-0.0.2/libtinyhtm/src/select.o
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.015933 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/append_htm.cxx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.015933 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/arena/
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/arena/arena_seg.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/arena.hxx
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/blk_write_state.hxx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.015933 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/blk_writer/
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/blk_writer/blk_write.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/blk_writer.hxx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.019933 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/ext_sort/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/ext_sort/mrg_npasses.cxx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.019933 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/ext_sort/mrg_pass/
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/ext_sort/mrg_pass/heap_down.hxx
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/ext_sort/mrg_pass/heap_up.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/ext_sort/mrg_pass.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/ext_sort/mrg_seg.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/ext_sort.hxx
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/mem_params.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/node.hxx
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/now.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/now.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/reverse_file.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/spherical_to_vec.hxx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.019933 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/compress_node.cxx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.019933 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/hash_table/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/hash_table/hash_table_add.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/hash_table/hash_table_destroy.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/hash_table/hash_table_get.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/hash_table/hash_table_grow.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/hash_table/hash_table_init.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/hash_table.hxx
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/id_off.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/tree_compress.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/write_tree_header.cxx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.023933 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/add_node.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/assign_block.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/assign_block.hxx
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/child_info.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/emit_node.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/emit_node.hxx
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/estimate_node_size.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/finish_root.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/layout_node.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/layout_node.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen.hxx
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen_context.hxx
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_root.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index.hxx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.023933 pynyhtm-0.0.2/libtinyhtm/src/tinyhtm/
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/tinyhtm/common.h
--rw-r--r--   0 runner    (1001) docker     (127)    20243 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/tinyhtm/geometry.h
--rw-r--r--   0 runner    (1001) docker     (127)    14898 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/tinyhtm/htm.h
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/tinyhtm/select.h
--rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/tinyhtm/tree.h
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/tinyhtm/varint.h
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/tinyhtm.h
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/tree.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-05-23 06:44:47.000000 pynyhtm-0.0.2/libtinyhtm/src/tree.o
--rw-r--r--   0 runner    (1001) docker     (127)    16846 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/tree_count.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/tree_entry.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/tree_entry.hxx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.023933 pynyhtm-0.0.2/libtinyhtm/test/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/test/cmp.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/test/cmp.h
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/test/rand.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/test/rand.h
--rw-r--r--   0 runner    (1001) docker     (127)    43103 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/test/test_geometry.cxx
--rw-r--r--   0 runner    (1001) docker     (127)    32594 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/test/test_htm.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/test/test_ranges.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/test/test_select.cxx
--rwxr-xr-x   0 runner    (1001) docker     (127)   105122 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/waf
--rwxr-xr-x   0 runner    (1001) docker     (127)    90923 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/waf-1.7.10
--rwxr-xr-x   0 runner    (1001) docker     (127)   105122 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/waf-2.0.23
--rw-r--r--   0 runner    (1001) docker     (127)    15921 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/wscript
--rw-r--r--   0 runner    (1001) docker     (127)  1528420 2024-05-23 06:44:53.000000 pynyhtm-0.0.2/pynyhtm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    35806 2024-05-23 06:44:38.000000 pynyhtm-0.0.2/pynyhtm.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-23 06:44:38.000000 pynyhtm-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 06:44:55.027933 pynyhtm-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-23 06:44:38.000000 pynyhtm-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.027933 pynyhtm-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-05-23 06:44:38.000000 pynyhtm-0.0.2/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-23 06:44:38.000000 pynyhtm-0.0.2/tests/test_pynyhtm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-23 06:44:38.000000 pynyhtm-0.0.2/tests/test_sc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-05-23 06:44:38.000000 pynyhtm-0.0.2/tests/test_triangle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-05-23 06:44:38.000000 pynyhtm-0.0.2/tests/test_v3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:37:41.375137 pynyhtm-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-23 09:37:25.000000 pynyhtm-0.0.3/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-23 09:37:25.000000 pynyhtm-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-23 09:37:25.000000 pynyhtm-0.0.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-23 09:37:41.375137 pynyhtm-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-23 09:37:25.000000 pynyhtm-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:37:41.343136 pynyhtm-0.0.3/libtinyhtm/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/.git
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/README
+-rw-r--r--   0 runner    (1001) docker     (127)    13889 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/boost.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/cxx14.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74592 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/doxygen.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/hdf5_cxx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:37:41.351137 pynyhtm-0.0.3/libtinyhtm/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/Box.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/Cartesian.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/Cartesian.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     8576 2024-05-23 09:37:32.000000 pynyhtm-0.0.3/libtinyhtm/src/Cartesian.o
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/Circle.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/Ellipse.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/Exception.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/Polygon.hxx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:37:41.351137 pynyhtm-0.0.3/libtinyhtm/src/Query/
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/Query/Query.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/Query.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/Shape.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/Spherical.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/Spherical.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-05-23 09:37:33.000000 pynyhtm-0.0.3/libtinyhtm/src/Spherical.o
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/Tree.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/common.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-23 09:37:33.000000 pynyhtm-0.0.3/libtinyhtm/src/common.o
+-rw-r--r--   0 runner    (1001) docker     (127)    47194 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/geometry.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)    39648 2024-05-23 09:37:33.000000 pynyhtm-0.0.3/libtinyhtm/src/geometry.o
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:37:41.359137 pynyhtm-0.0.3/libtinyhtm/src/htm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_ids_add.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_ids_init.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_ids_init.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-23 09:37:34.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_ids_init.o
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_s2circle_htmcov.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_s2circle_htmcov.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-05-23 09:37:34.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_s2circle_htmcov.o
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:37:41.359137 pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_s2cpoly_htmcov/
+-rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_s2cpoly_htmcov/_htm_isect_test.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_s2cpoly_htmcov/_htm_s2cpoly_htmcov.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_s2cpoly_htmcov.hxx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:37:41.359137 pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_s2ellipse_htmcov/
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_s2ellipse_htmcov/_htm_s2ellipse_htmcov.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_s2ellipse_htmcov/_htm_s2ellipse_isect.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_s2ellipse_htmcov.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_simplify_ids.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_simplify_ids.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-23 09:37:35.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_simplify_ids.o
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_subdivide.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_subdivide.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-05-23 09:37:35.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_subdivide.o
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_v3_htmroot.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_s2circle_ids.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-05-23 09:37:35.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_s2circle_ids.o
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_s2cpoly_cv3_template.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_s2cpoly_ids.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)    10800 2024-05-23 09:37:35.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_s2cpoly_ids.o
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_s2ellipse_cv3_template.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_s2ellipse_ids.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)    10456 2024-05-23 09:37:35.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_s2ellipse_ids.o
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2circle.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-23 09:37:35.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2circle.o
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2circle_range.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     9696 2024-05-23 09:37:36.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2circle_range.o
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2circle_scan.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-23 09:37:36.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2circle_scan.o
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2cpoly.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-23 09:37:36.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2cpoly.o
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2cpoly_range.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     9648 2024-05-23 09:37:37.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2cpoly_range.o
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2cpoly_scan.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-23 09:37:37.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2cpoly_scan.o
+-rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2ellipse.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-23 09:37:38.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2ellipse.o
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2ellipse_range.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     9304 2024-05-23 09:37:38.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2ellipse_range.o
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2ellipse_scan.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-23 09:37:38.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2ellipse_scan.o
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_v3_distance2.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_v3_id.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-05-23 09:37:38.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_v3_id.o
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:37:41.359137 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_v3p_idsort/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:37:41.359137 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_v3p_idsort/_htm_path_sort/
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_v3p_idsort/_htm_path_sort/_htm_partition.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_v3p_idsort/_htm_path_sort/_htm_path_sort.cxx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:37:41.359137 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_v3p_idsort/_htm_rootsort/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_v3p_idsort/_htm_rootsort/_htm_rootpart.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_v3p_idsort/_htm_rootsort/_htm_rootsort.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm/htm_v3p_idsort/htm_v3p_idsort.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)    10166 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     8395 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)    17120 2024-05-23 09:37:34.000000 pynyhtm-0.0.3/libtinyhtm/src/htm.o
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm_convert_to_hdf5.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm_entry.hxx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:37:41.359137 pynyhtm-0.0.3/libtinyhtm/src/htm_tree_gen/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:37:41.363137 pynyhtm-0.0.3/libtinyhtm/src/htm_tree_gen/blk_sort_ascii/
+-rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm_tree_gen/blk_sort_ascii/blk_sort_ascii.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm_tree_gen/blk_sort_ascii/eat_delim.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm_tree_gen/blk_sort_ascii/eat_ws.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)    14221 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm_tree_gen/htm_tree_gen.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/htm_tree_gen/usage.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     9613 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/id_list.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)    13640 2024-05-23 09:37:34.000000 pynyhtm-0.0.3/libtinyhtm/src/id_list.o
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/licence.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-23 09:37:34.000000 pynyhtm-0.0.3/libtinyhtm/src/licence.o
+-rw-r--r--   0 runner    (1001) docker     (127)    12634 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/select.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-05-23 09:37:34.000000 pynyhtm-0.0.3/libtinyhtm/src/select.o
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:37:41.363137 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/append_htm.cxx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:37:41.363137 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/arena/
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/arena/arena_seg.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/arena.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/blk_write_state.hxx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:37:41.363137 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/blk_writer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/blk_writer/blk_write.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/blk_writer.hxx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:37:41.363137 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/ext_sort/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/ext_sort/mrg_npasses.cxx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:37:41.363137 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/ext_sort/mrg_pass/
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/ext_sort/mrg_pass/heap_down.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/ext_sort/mrg_pass/heap_up.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/ext_sort/mrg_pass.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/ext_sort/mrg_seg.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/ext_sort.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/mem_params.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/node.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/now.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/now.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/reverse_file.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/spherical_to_vec.hxx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:37:41.367137 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_compress/
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_compress/compress_node.cxx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:37:41.367137 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_compress/hash_table/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_compress/hash_table/hash_table_add.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_compress/hash_table/hash_table_destroy.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_compress/hash_table/hash_table_get.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_compress/hash_table/hash_table_grow.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_compress/hash_table/hash_table_init.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_compress/hash_table.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_compress/id_off.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_compress/tree_compress.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_compress/write_tree_header.cxx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:37:41.367137 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_gen/
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_gen/add_node.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_gen/assign_block.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_gen/assign_block.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_gen/child_info.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_gen/emit_node.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_gen/emit_node.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_gen/estimate_node_size.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_gen/finish_root.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_gen/layout_node.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_gen/layout_node.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_gen.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_gen_context.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_root.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/sort_and_index.hxx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:37:41.371137 pynyhtm-0.0.3/libtinyhtm/src/tinyhtm/
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/tinyhtm/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20243 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/tinyhtm/geometry.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14898 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/tinyhtm/htm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/tinyhtm/select.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/tinyhtm/tree.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/tinyhtm/varint.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/tinyhtm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/tree.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-05-23 09:37:34.000000 pynyhtm-0.0.3/libtinyhtm/src/tree.o
+-rw-r--r--   0 runner    (1001) docker     (127)    16846 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/tree_count.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/tree_entry.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/src/tree_entry.hxx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:37:41.371137 pynyhtm-0.0.3/libtinyhtm/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/test/cmp.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/test/cmp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/test/rand.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/test/rand.h
+-rw-r--r--   0 runner    (1001) docker     (127)    43103 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/test/test_geometry.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)    32594 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/test/test_htm.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/test/test_ranges.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/test/test_select.cxx
+-rwxr-xr-x   0 runner    (1001) docker     (127)   105122 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/waf
+-rwxr-xr-x   0 runner    (1001) docker     (127)    90923 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/waf-1.7.10
+-rwxr-xr-x   0 runner    (1001) docker     (127)   105122 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/waf-2.0.23
+-rw-r--r--   0 runner    (1001) docker     (127)    15921 2024-05-23 09:37:26.000000 pynyhtm-0.0.3/libtinyhtm/wscript
+-rw-r--r--   0 runner    (1001) docker     (127)  1528420 2024-05-23 09:37:40.000000 pynyhtm-0.0.3/pynyhtm.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:37:41.375137 pynyhtm-0.0.3/pynyhtm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-23 09:37:41.000000 pynyhtm-0.0.3/pynyhtm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-05-23 09:37:41.000000 pynyhtm-0.0.3/pynyhtm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 09:37:41.000000 pynyhtm-0.0.3/pynyhtm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-23 09:37:41.000000 pynyhtm-0.0.3/pynyhtm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 09:37:41.000000 pynyhtm-0.0.3/pynyhtm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35806 2024-05-23 09:37:25.000000 pynyhtm-0.0.3/pynyhtm.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-23 09:37:25.000000 pynyhtm-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 09:37:41.375137 pynyhtm-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-23 09:37:25.000000 pynyhtm-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:37:41.375137 pynyhtm-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-05-23 09:37:25.000000 pynyhtm-0.0.3/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-23 09:37:25.000000 pynyhtm-0.0.3/tests/test_pynyhtm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-23 09:37:25.000000 pynyhtm-0.0.3/tests/test_sc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7107 2024-05-23 09:37:25.000000 pynyhtm-0.0.3/tests/test_triangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-05-23 09:37:25.000000 pynyhtm-0.0.3/tests/test_v3.py
```

### Comparing `pynyhtm-0.0.2/LICENCE` & `pynyhtm-0.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/Makefile` & `pynyhtm-0.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/PKG-INFO` & `pynyhtm-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: PynyHTM
-Version: 0.0.2
+Name: pynyhtm
+Version: 0.0.3
 Summary: Python wrapper for the libtinyhtm library.
 Author-email: Till <till@fleisch.dev>
 Project-URL: Homepage, https://github.com/TillFleisch/PynyHTM
 Project-URL: Repository, https://github.com/TillFleisch/PynyHTM.git
 Project-URL: Issues, https://github.com/TillFleisch/PynyHTM/issues
 Keywords: htm,libtinyhtm,hierarchial triangular mesh,triangle subdivision,index
 Description-Content-Type: text/markdown
@@ -25,15 +25,15 @@
 
 ## Usage sample
 
 The code snippets below are available in [this example file](example.py).
 Classes `SphericalCoordinate` and `V3` cover basic functionality for expressing points in 3D space.
 
 ```python
-from PynyHTM import HTM, SphericalCoordinate, Triangle, V3
+from pynyhtm import HTM, SphericalCoordinate, Triangle, V3
 
 # Retrieve HTM ID for a spherical coordinate
 sc_1 = SphericalCoordinate(10.1234, -20.1234)
 id = sc_1.get_htm_id(level=14)
 print(f"HTM-ID for sc_1: {id} at level 14")
 # >>> HTM-ID for sc_1: 3278525534 at level 14
```

### Comparing `pynyhtm-0.0.2/PynyHTM.egg-info/PKG-INFO` & `pynyhtm-0.0.3/pynyhtm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: PynyHTM
-Version: 0.0.2
+Name: pynyhtm
+Version: 0.0.3
 Summary: Python wrapper for the libtinyhtm library.
 Author-email: Till <till@fleisch.dev>
 Project-URL: Homepage, https://github.com/TillFleisch/PynyHTM
 Project-URL: Repository, https://github.com/TillFleisch/PynyHTM.git
 Project-URL: Issues, https://github.com/TillFleisch/PynyHTM/issues
 Keywords: htm,libtinyhtm,hierarchial triangular mesh,triangle subdivision,index
 Description-Content-Type: text/markdown
@@ -25,15 +25,15 @@
 
 ## Usage sample
 
 The code snippets below are available in [this example file](example.py).
 Classes `SphericalCoordinate` and `V3` cover basic functionality for expressing points in 3D space.
 
 ```python
-from PynyHTM import HTM, SphericalCoordinate, Triangle, V3
+from pynyhtm import HTM, SphericalCoordinate, Triangle, V3
 
 # Retrieve HTM ID for a spherical coordinate
 sc_1 = SphericalCoordinate(10.1234, -20.1234)
 id = sc_1.get_htm_id(level=14)
 print(f"HTM-ID for sc_1: {id} at level 14")
 # >>> HTM-ID for sc_1: 3278525534 at level 14
```

### Comparing `pynyhtm-0.0.2/PynyHTM.egg-info/SOURCES.txt` & `pynyhtm-0.0.3/pynyhtm.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,14 @@
 MANIFEST.in
 Makefile
 README.md
 pynyhtm.cpp
 pynyhtm.pyx
 pyproject.toml
 setup.py
-PynyHTM.egg-info/PKG-INFO
-PynyHTM.egg-info/SOURCES.txt
-PynyHTM.egg-info/dependency_links.txt
-PynyHTM.egg-info/requires.txt
-PynyHTM.egg-info/top_level.txt
 libtinyhtm/.git
 libtinyhtm/LICENSE.txt
 libtinyhtm/Makefile
 libtinyhtm/README
 libtinyhtm/boost.py
 libtinyhtm/cxx14.py
 libtinyhtm/doxygen.conf
@@ -170,12 +165,17 @@
 libtinyhtm/test/cmp.h
 libtinyhtm/test/rand.cxx
 libtinyhtm/test/rand.h
 libtinyhtm/test/test_geometry.cxx
 libtinyhtm/test/test_htm.cxx
 libtinyhtm/test/test_ranges.cxx
 libtinyhtm/test/test_select.cxx
+pynyhtm.egg-info/PKG-INFO
+pynyhtm.egg-info/SOURCES.txt
+pynyhtm.egg-info/dependency_links.txt
+pynyhtm.egg-info/requires.txt
+pynyhtm.egg-info/top_level.txt
 tests/test_geometry.py
 tests/test_pynyhtm.py
 tests/test_sc.py
 tests/test_triangle.py
 tests/test_v3.py
```

### Comparing `pynyhtm-0.0.2/README.md` & `pynyhtm-0.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 ## Usage sample
 
 The code snippets below are available in [this example file](example.py).
 Classes `SphericalCoordinate` and `V3` cover basic functionality for expressing points in 3D space.
 
 ```python
-from PynyHTM import HTM, SphericalCoordinate, Triangle, V3
+from pynyhtm import HTM, SphericalCoordinate, Triangle, V3
 
 # Retrieve HTM ID for a spherical coordinate
 sc_1 = SphericalCoordinate(10.1234, -20.1234)
 id = sc_1.get_htm_id(level=14)
 print(f"HTM-ID for sc_1: {id} at level 14")
 # >>> HTM-ID for sc_1: 3278525534 at level 14
```

### Comparing `pynyhtm-0.0.2/libtinyhtm/LICENSE.txt` & `pynyhtm-0.0.3/libtinyhtm/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/Makefile` & `pynyhtm-0.0.3/libtinyhtm/Makefile`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/README` & `pynyhtm-0.0.3/libtinyhtm/README`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/boost.py` & `pynyhtm-0.0.3/libtinyhtm/boost.py`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/cxx14.py` & `pynyhtm-0.0.3/libtinyhtm/cxx14.py`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/doxygen.conf` & `pynyhtm-0.0.3/libtinyhtm/doxygen.conf`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/hdf5_cxx.py` & `pynyhtm-0.0.3/libtinyhtm/hdf5_cxx.py`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/Box.hxx` & `pynyhtm-0.0.3/libtinyhtm/src/Box.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/Cartesian.hxx` & `pynyhtm-0.0.3/libtinyhtm/src/Cartesian.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/Cartesian.o` & `pynyhtm-0.0.3/libtinyhtm/src/Cartesian.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/Circle.hxx` & `pynyhtm-0.0.3/libtinyhtm/src/Circle.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/Ellipse.hxx` & `pynyhtm-0.0.3/libtinyhtm/src/Ellipse.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/Polygon.hxx` & `pynyhtm-0.0.3/libtinyhtm/src/Polygon.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/Query/Query.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/Query/Query.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/Query.hxx` & `pynyhtm-0.0.3/libtinyhtm/src/Query.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/Shape.hxx` & `pynyhtm-0.0.3/libtinyhtm/src/Shape.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/Spherical.hxx` & `pynyhtm-0.0.3/libtinyhtm/src/Spherical.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/Spherical.o` & `pynyhtm-0.0.3/libtinyhtm/src/Spherical.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/common.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/common.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/common.o` & `pynyhtm-0.0.3/libtinyhtm/src/common.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/geometry.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/geometry.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/geometry.o` & `pynyhtm-0.0.3/libtinyhtm/src/geometry.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_ids_add.hxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_ids_add.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_ids_init.o` & `pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_ids_init.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_s2circle_htmcov.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_s2circle_htmcov.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_s2circle_htmcov.o` & `pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_s2circle_htmcov.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_s2cpoly_htmcov/_htm_isect_test.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_s2cpoly_htmcov/_htm_isect_test.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_s2cpoly_htmcov/_htm_s2cpoly_htmcov.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_s2cpoly_htmcov/_htm_s2cpoly_htmcov.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_s2ellipse_htmcov/_htm_s2ellipse_htmcov.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_s2ellipse_htmcov/_htm_s2ellipse_htmcov.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_s2ellipse_htmcov/_htm_s2ellipse_isect.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_s2ellipse_htmcov/_htm_s2ellipse_isect.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_simplify_ids.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_simplify_ids.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_simplify_ids.o` & `pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_simplify_ids.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_subdivide.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_subdivide.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_subdivide.o` & `pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_subdivide.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_v3_htmroot.hxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm/_htm_v3_htmroot.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_s2circle_ids.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm/htm_s2circle_ids.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_s2circle_ids.o` & `pynyhtm-0.0.3/libtinyhtm/src/htm/htm_s2circle_ids.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_s2cpoly_cv3_template.hxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm/htm_s2cpoly_cv3_template.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_s2cpoly_ids.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm/htm_s2cpoly_ids.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_s2cpoly_ids.o` & `pynyhtm-0.0.3/libtinyhtm/src/htm/htm_s2cpoly_ids.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_s2ellipse_ids.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm/htm_s2ellipse_ids.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_s2ellipse_ids.o` & `pynyhtm-0.0.3/libtinyhtm/src/htm/htm_s2ellipse_ids.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2circle.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2circle.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2circle.o` & `pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2circle.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2circle_range.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2circle_range.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2circle_range.o` & `pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2circle_range.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2circle_scan.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2circle_scan.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2circle_scan.o` & `pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2circle_scan.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2cpoly.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2cpoly.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2cpoly.o` & `pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2cpoly.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2cpoly_range.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2cpoly_range.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2cpoly_range.o` & `pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2cpoly_range.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2cpoly_scan.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2cpoly_scan.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2cpoly_scan.o` & `pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2cpoly_scan.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2ellipse.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2ellipse.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2ellipse.o` & `pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2ellipse.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2ellipse_range.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2ellipse_range.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2ellipse_range.o` & `pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2ellipse_range.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2ellipse_scan.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2ellipse_scan.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2ellipse_scan.o` & `pynyhtm-0.0.3/libtinyhtm/src/htm/htm_tree_s2ellipse_scan.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3_id.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm/htm_v3_id.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3_id.o` & `pynyhtm-0.0.3/libtinyhtm/src/htm/htm_v3_id.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3p_idsort/_htm_path_sort/_htm_partition.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm/htm_v3p_idsort/_htm_path_sort/_htm_partition.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3p_idsort/_htm_path_sort/_htm_path_sort.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm/htm_v3p_idsort/_htm_path_sort/_htm_path_sort.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3p_idsort/_htm_rootsort/_htm_rootpart.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm/htm_v3p_idsort/_htm_rootsort/_htm_rootpart.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3p_idsort/_htm_rootsort/_htm_rootsort.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm/htm_v3p_idsort/_htm_rootsort/_htm_rootsort.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3p_idsort/htm_v3p_idsort.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm/htm_v3p_idsort/htm_v3p_idsort.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm.hxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm.o` & `pynyhtm-0.0.3/libtinyhtm/src/htm.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm_convert_to_hdf5.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm_convert_to_hdf5.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm_tree_gen/blk_sort_ascii/blk_sort_ascii.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm_tree_gen/blk_sort_ascii/blk_sort_ascii.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm_tree_gen/blk_sort_ascii/eat_delim.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm_tree_gen/blk_sort_ascii/eat_delim.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm_tree_gen/blk_sort_ascii/eat_ws.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm_tree_gen/blk_sort_ascii/eat_ws.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm_tree_gen/htm_tree_gen.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm_tree_gen/htm_tree_gen.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/htm_tree_gen/usage.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/htm_tree_gen/usage.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/id_list.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/id_list.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/id_list.o` & `pynyhtm-0.0.3/libtinyhtm/src/id_list.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/licence.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/licence.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/licence.o` & `pynyhtm-0.0.3/libtinyhtm/src/licence.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/select.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/select.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/select.o` & `pynyhtm-0.0.3/libtinyhtm/src/select.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/append_htm.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/append_htm.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/arena/arena_seg.hxx` & `pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/arena/arena_seg.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/arena.hxx` & `pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/arena.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/blk_writer/blk_write.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/blk_writer/blk_write.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/blk_writer.hxx` & `pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/blk_writer.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/ext_sort/mrg_pass/heap_down.hxx` & `pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/ext_sort/mrg_pass/heap_down.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/ext_sort/mrg_pass.hxx` & `pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/ext_sort/mrg_pass.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/ext_sort/mrg_seg.hxx` & `pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/ext_sort/mrg_seg.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/ext_sort.hxx` & `pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/ext_sort.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/mem_params.hxx` & `pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/mem_params.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/node.hxx` & `pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/node.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/reverse_file.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/reverse_file.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/spherical_to_vec.hxx` & `pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/spherical_to_vec.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/compress_node.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_compress/compress_node.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/hash_table/hash_table_add.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_compress/hash_table/hash_table_add.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/hash_table/hash_table_get.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_compress/hash_table/hash_table_get.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/hash_table/hash_table_grow.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_compress/hash_table/hash_table_grow.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/hash_table.hxx` & `pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_compress/hash_table.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/tree_compress.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_compress/tree_compress.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/write_tree_header.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_compress/write_tree_header.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/add_node.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_gen/add_node.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/assign_block.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_gen/assign_block.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/assign_block.hxx` & `pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_gen/assign_block.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/emit_node.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_gen/emit_node.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/estimate_node_size.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_gen/estimate_node_size.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/finish_root.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_gen/finish_root.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/layout_node.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_gen/layout_node.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen.hxx` & `pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_gen.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen_context.hxx` & `pynyhtm-0.0.3/libtinyhtm/src/sort_and_index/tree_gen_context.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index.hxx` & `pynyhtm-0.0.3/libtinyhtm/src/sort_and_index.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/tinyhtm/common.h` & `pynyhtm-0.0.3/libtinyhtm/src/tinyhtm/common.h`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/tinyhtm/geometry.h` & `pynyhtm-0.0.3/libtinyhtm/src/tinyhtm/geometry.h`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/tinyhtm/htm.h` & `pynyhtm-0.0.3/libtinyhtm/src/tinyhtm/htm.h`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/tinyhtm/select.h` & `pynyhtm-0.0.3/libtinyhtm/src/tinyhtm/select.h`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/tinyhtm/tree.h` & `pynyhtm-0.0.3/libtinyhtm/src/tinyhtm/tree.h`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/tinyhtm/varint.h` & `pynyhtm-0.0.3/libtinyhtm/src/tinyhtm/varint.h`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/tinyhtm.h` & `pynyhtm-0.0.3/libtinyhtm/src/tinyhtm.h`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/tree.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/tree.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/tree.o` & `pynyhtm-0.0.3/libtinyhtm/src/tree.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/tree_count.cxx` & `pynyhtm-0.0.3/libtinyhtm/src/tree_count.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/src/tree_entry.hxx` & `pynyhtm-0.0.3/libtinyhtm/src/tree_entry.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/test/cmp.cxx` & `pynyhtm-0.0.3/libtinyhtm/test/cmp.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/test/cmp.h` & `pynyhtm-0.0.3/libtinyhtm/test/cmp.h`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/test/rand.cxx` & `pynyhtm-0.0.3/libtinyhtm/test/rand.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/test/test_geometry.cxx` & `pynyhtm-0.0.3/libtinyhtm/test/test_geometry.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/test/test_htm.cxx` & `pynyhtm-0.0.3/libtinyhtm/test/test_htm.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/test/test_ranges.cxx` & `pynyhtm-0.0.3/libtinyhtm/test/test_ranges.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/test/test_select.cxx` & `pynyhtm-0.0.3/libtinyhtm/test/test_select.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/waf` & `pynyhtm-0.0.3/libtinyhtm/waf`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/waf-1.7.10` & `pynyhtm-0.0.3/libtinyhtm/waf-1.7.10`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/waf-2.0.23` & `pynyhtm-0.0.3/libtinyhtm/waf-2.0.23`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/libtinyhtm/wscript` & `pynyhtm-0.0.3/libtinyhtm/wscript`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/pynyhtm.cpp` & `pynyhtm-0.0.3/pynyhtm.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 /* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "libtinyhtm/src/licence.cxx",
             "libtinyhtm/src/tinyhtm/common.h",
             "libtinyhtm/src/tinyhtm/geometry.h",
             "libtinyhtm/src/tinyhtm/htm.h"
         ],
         "include_dirs": [
-            "/tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/core/include"
+            "/tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/core/include"
         ],
         "language": "c++",
         "libraries": [
             ":libtinyhtm.a"
         ],
         "library_dirs": [
             "."
         ],
-        "name": "PynyHTM",
+        "name": "pynyhtm",
         "sources": [
             "pynyhtm.pyx"
         ]
     },
-    "module_name": "PynyHTM"
+    "module_name": "pynyhtm"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #if defined(CYTHON_LIMITED_API) && 0
@@ -1257,16 +1257,16 @@
     #else
     #warning Please do not define the '__PYX_EXTERN_C' macro externally. Use 'CYTHON_EXTERN_C' instead.
     #endif
 #else
     #define __PYX_EXTERN_C extern "C++"
 #endif
 
-#define __PYX_HAVE__PynyHTM
-#define __PYX_HAVE_API__PynyHTM
+#define __PYX_HAVE__pynyhtm
+#define __PYX_HAVE_API__pynyhtm
 /* Early includes */
 #include <string.h>
 #include <stdio.h>
 
     /* Using NumPy API declarations from "numpy/__init__.cython-30.pxd" */
     
 #include "numpy/arrayobject.h"
@@ -1557,177 +1557,177 @@
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1756,90 +1756,90 @@
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
-struct __pyx_ctuple_7PynyHTM_htm_errcode__and_7PynyHTM_struct__space_htm_sc;
-typedef struct __pyx_ctuple_7PynyHTM_htm_errcode__and_7PynyHTM_struct__space_htm_sc __pyx_ctuple_7PynyHTM_htm_errcode__and_7PynyHTM_struct__space_htm_sc;
-struct __pyx_ctuple_7PynyHTM_htm_errcode__and_7PynyHTM_struct__space_htm_v3;
-typedef struct __pyx_ctuple_7PynyHTM_htm_errcode__and_7PynyHTM_struct__space_htm_v3 __pyx_ctuple_7PynyHTM_htm_errcode__and_7PynyHTM_struct__space_htm_v3;
-struct __pyx_ctuple_7PynyHTM_htm_errcode__and_7PynyHTM_struct__space_htm_tri;
-typedef struct __pyx_ctuple_7PynyHTM_htm_errcode__and_7PynyHTM_struct__space_htm_tri __pyx_ctuple_7PynyHTM_htm_errcode__and_7PynyHTM_struct__space_htm_tri;
+struct __pyx_ctuple_7pynyhtm_htm_errcode__and_7pynyhtm_struct__space_htm_sc;
+typedef struct __pyx_ctuple_7pynyhtm_htm_errcode__and_7pynyhtm_struct__space_htm_sc __pyx_ctuple_7pynyhtm_htm_errcode__and_7pynyhtm_struct__space_htm_sc;
+struct __pyx_ctuple_7pynyhtm_htm_errcode__and_7pynyhtm_struct__space_htm_v3;
+typedef struct __pyx_ctuple_7pynyhtm_htm_errcode__and_7pynyhtm_struct__space_htm_v3 __pyx_ctuple_7pynyhtm_htm_errcode__and_7pynyhtm_struct__space_htm_v3;
+struct __pyx_ctuple_7pynyhtm_htm_errcode__and_7pynyhtm_struct__space_htm_tri;
+typedef struct __pyx_ctuple_7pynyhtm_htm_errcode__and_7pynyhtm_struct__space_htm_tri __pyx_ctuple_7pynyhtm_htm_errcode__and_7pynyhtm_struct__space_htm_tri;
 struct __pyx_defaults;
 typedef struct __pyx_defaults __pyx_defaults;
 
 /* "pynyhtm.pyx":323
  * 
  * 
  * def htm_sc_init_raw(latitude: float, longitude: float) -> tuple[htm_errcode, htm_sc]:             # <<<<<<<<<<<<<<
  *     """
  *     Wraps htm_sc_init, instantiates a htm_sc struct.
  */
-struct __pyx_ctuple_7PynyHTM_htm_errcode__and_7PynyHTM_struct__space_htm_sc {
+struct __pyx_ctuple_7pynyhtm_htm_errcode__and_7pynyhtm_struct__space_htm_sc {
   htm_errcode f0;
   struct htm_sc f1;
 };
 
 /* "pynyhtm.pyx":363
  * 
  * 
  * def htm_v3_init_raw(x: float, y: float, z: float) -> tuple[htm_errcode, htm_v3]:             # <<<<<<<<<<<<<<
  *     """
  *     Wraps htm_v3_init, instantiates a htm_v3 struct.
  */
-struct __pyx_ctuple_7PynyHTM_htm_errcode__and_7PynyHTM_struct__space_htm_v3 {
+struct __pyx_ctuple_7pynyhtm_htm_errcode__and_7pynyhtm_struct__space_htm_v3 {
   htm_errcode f0;
   struct htm_v3 f1;
 };
 
 /* "pynyhtm.pyx":599
  * 
  * 
  * def htm_tri_init_raw(id: int64_t) -> tuple[htm_errcode, htm_tri]:             # <<<<<<<<<<<<<<
  *     """
  *     Instantiate a htm_tri struct for a given triangle id.
  */
-struct __pyx_ctuple_7PynyHTM_htm_errcode__and_7PynyHTM_struct__space_htm_tri {
+struct __pyx_ctuple_7pynyhtm_htm_errcode__and_7pynyhtm_struct__space_htm_tri {
   htm_errcode f0;
   struct htm_tri f1;
 };
 struct __pyx_defaults {
   PyObject *__pyx_arg_max_ranges;
 };
 /* #### Code section: utility_code_proto ### */
@@ -2843,28 +2843,28 @@
 
 /* Module declarations from "cpython.ref" */
 
 /* Module declarations from "numpy" */
 
 /* Module declarations from "numpy" */
 
-/* Module declarations from "PynyHTM" */
+/* Module declarations from "pynyhtm" */
 static struct htm_sc __pyx_convert__from_py_struct__htm_sc(PyObject *); /*proto*/
 static struct htm_v3 __pyx_convert__from_py_struct__htm_v3(PyObject *); /*proto*/
 static int __Pyx_carray_from_py_struct__htm_v3(PyObject *, struct htm_v3 *, Py_ssize_t); /*proto*/
 static struct htm_tri __pyx_convert__from_py_struct__htm_tri(PyObject *); /*proto*/
 static CYTHON_INLINE PyObject *__Pyx_carray_to_py_struct__htm_v3(struct htm_v3 *, Py_ssize_t); /*proto*/
 static CYTHON_INLINE PyObject *__Pyx_carray_to_tuple_struct__htm_v3(struct htm_v3 *, Py_ssize_t); /*proto*/
 /* #### Code section: typeinfo ### */
 /* #### Code section: before_global_var ### */
-#define __Pyx_MODULE_NAME "PynyHTM"
-extern int __pyx_module_is_main_PynyHTM;
-int __pyx_module_is_main_PynyHTM = 0;
+#define __Pyx_MODULE_NAME "pynyhtm"
+extern int __pyx_module_is_main_pynyhtm;
+int __pyx_module_is_main_pynyhtm = 0;
 
-/* Implementation of "PynyHTM" */
+/* Implementation of "pynyhtm" */
 /* #### Code section: global_var ### */
 static PyObject *__pyx_builtin_property;
 static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_TypeError;
 static PyObject *__pyx_builtin_range;
 static PyObject *__pyx_builtin_NotImplementedError;
 static PyObject *__pyx_builtin_RuntimeError;
@@ -2962,21 +2962,21 @@
 static const char __pyx_k_return[] = "return";
 static const char __pyx_k_scalar[] = "scalar";
 static const char __pyx_k_struct[] = "struct";
 static const char __pyx_k_vertex[] = "vertex";
 static const char __pyx_k_HTM_EID[] = "HTM_EID";
 static const char __pyx_k_HTM_EIO[] = "HTM_EIO";
 static const char __pyx_k_OC_ZERO[] = "OC_ZERO";
-static const char __pyx_k_PynyHTM[] = "PynyHTM";
 static const char __pyx_k_from_id[] = "from_id";
 static const char __pyx_k_htm_tri[] = "htm_tri";
 static const char __pyx_k_int64_t[] = "int64_t";
 static const char __pyx_k_level_2[] = "_level";
 static const char __pyx_k_license[] = "license";
 static const char __pyx_k_prepare[] = "__prepare__";
+static const char __pyx_k_pynyhtm[] = "pynyhtm";
 static const char __pyx_k_truediv[] = "__truediv__";
 static const char __pyx_k_HTM_EANG[] = "HTM_EANG";
 static const char __pyx_k_HTM_EINV[] = "HTM_EINV";
 static const char __pyx_k_HTM_ELAT[] = "HTM_ELAT";
 static const char __pyx_k_HTM_ELEN[] = "HTM_ELEN";
 static const char __pyx_k_KeyError[] = "KeyError";
 static const char __pyx_k_Triangle[] = "Triangle(";
@@ -3138,77 +3138,77 @@
 static const char __pyx_k_No_value_specified_for_struct_at_5[] = "No value specified for struct attribute 'z'";
 static const char __pyx_k_No_value_specified_for_struct_at_6[] = "No value specified for struct attribute 'verts'";
 static const char __pyx_k_No_value_specified_for_struct_at_7[] = "No value specified for struct attribute 'center'";
 static const char __pyx_k_No_value_specified_for_struct_at_8[] = "No value specified for struct attribute 'radius'";
 static const char __pyx_k_No_value_specified_for_struct_at_9[] = "No value specified for struct attribute 'id'";
 static const char __pyx_k_No_value_specified_for_struct_at_10[] = "No value specified for struct attribute 'level'";
 /* #### Code section: decls ### */
-static PyObject *__pyx_pf_7PynyHTM_lib_get_license(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_19SphericalCoordinate_latitude(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_19SphericalCoordinate_2longitude(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_19SphericalCoordinate_4__init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, double __pyx_v_latitude, double __pyx_v_longitude); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_19SphericalCoordinate_6__repr__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_19SphericalCoordinate_8get_htm_sc(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_19SphericalCoordinate_10from_htm_sc(CYTHON_UNUSED PyObject *__pyx_self, struct htm_sc __pyx_v_sc); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_19SphericalCoordinate_12to_v3(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_19SphericalCoordinate_14angle_separation(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_other); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_19SphericalCoordinate_16get_htm_id(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_level); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_2V3_x(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_2V3_2y(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_2V3_4z(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_2V3_6__init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, double __pyx_v_x, double __pyx_v_y, double __pyx_v_z); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_2V3_8__repr__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_2V3_10get_htm_v3(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_2V3_12from_htm_v3(CYTHON_UNUSED PyObject *__pyx_self, struct htm_v3 __pyx_v_v3); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_2V3_14to_sc(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_2V3_16get_htm_id(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_level); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_2V3_18add(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_other); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_2V3_20__add__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_other); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_2V3_22sub(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_other); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_2V3_24__sub__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_other); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_2V3_26neg(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_2V3_28__neg__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_2V3_30mul(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, double __pyx_v_scalar); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_2V3_32__mul__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, double __pyx_v_scalar); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_2V3_34div(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, double __pyx_v_scalar); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_2V3_36__truediv__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, double __pyx_v_scalar); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_2htm_sc_init_raw(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_latitude, double __pyx_v_longitude); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_4htm_sc_init_wrapped(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_latitude, double __pyx_v_longitude); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_6htm_sc_angsep_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_sc __pyx_v_sc1, struct htm_sc __pyx_v_sc2); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_8htm_v3_init_raw(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_x, double __pyx_v_y, double __pyx_v_z); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_10htm_v3_init_wrapped(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_x, double __pyx_v_y, double __pyx_v_z); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_12htm_sc_to_v3_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_sc __pyx_v_sc); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_14htm_v3_to_sc_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_v3 __pyx_v_v3); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_16htm_v3_add_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_v3 __pyx_v_v1, struct htm_v3 __pyx_v_v2); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_18htm_v3_sub_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_v3 __pyx_v_v1, struct htm_v3 __pyx_v_v2); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_20htm_v3_neg_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_v3 __pyx_v_v1); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_22htm_v3_mul_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_v3 __pyx_v_v1, double __pyx_v_scalar); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_24htm_v3_div_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_v3 __pyx_v_v1, double __pyx_v_scalar); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_8Triangle_vertices(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_8Triangle_2center(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_8Triangle_4radius(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_8Triangle_6id(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_8Triangle_8level(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_8Triangle_10__init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_vertices, PyObject *__pyx_v_center, double __pyx_v_radius, PyObject *__pyx_v_id, PyObject *__pyx_v_level); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_8Triangle_12__repr__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_8Triangle_14from_htm_tri(CYTHON_UNUSED PyObject *__pyx_self, struct htm_tri __pyx_v_struct); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_8Triangle_16from_id(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_26htm_v3_id_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_v3 __pyx_v_v, PyObject *__pyx_v_level); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_28htm_tri_init_raw(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_30htm_tri_init_wrapped(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_3HTM_get_level(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_3HTM_2id_to_dec(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_3HTM_4parent(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_3HTM_6children(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_3HTM_8neighbors(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_3HTM_10neighbor(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id, PyObject *__pyx_v_direction); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_36__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_3HTM_12circle_search(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_center, double __pyx_v_radius, PyObject *__pyx_v_level, PyObject *__pyx_v_max_ranges); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_32htm_level_raw(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id); /* proto */
-static PyObject *__pyx_pf_7PynyHTM_34htm_id_to_dec(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_lib_get_license(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_19SphericalCoordinate_latitude(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_19SphericalCoordinate_2longitude(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_19SphericalCoordinate_4__init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, double __pyx_v_latitude, double __pyx_v_longitude); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_19SphericalCoordinate_6__repr__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_19SphericalCoordinate_8get_htm_sc(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_19SphericalCoordinate_10from_htm_sc(CYTHON_UNUSED PyObject *__pyx_self, struct htm_sc __pyx_v_sc); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_19SphericalCoordinate_12to_v3(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_19SphericalCoordinate_14angle_separation(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_other); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_19SphericalCoordinate_16get_htm_id(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_level); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_2V3_x(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_2V3_2y(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_2V3_4z(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_2V3_6__init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, double __pyx_v_x, double __pyx_v_y, double __pyx_v_z); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_2V3_8__repr__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_2V3_10get_htm_v3(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_2V3_12from_htm_v3(CYTHON_UNUSED PyObject *__pyx_self, struct htm_v3 __pyx_v_v3); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_2V3_14to_sc(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_2V3_16get_htm_id(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_level); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_2V3_18add(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_other); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_2V3_20__add__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_other); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_2V3_22sub(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_other); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_2V3_24__sub__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_other); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_2V3_26neg(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_2V3_28__neg__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_2V3_30mul(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, double __pyx_v_scalar); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_2V3_32__mul__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, double __pyx_v_scalar); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_2V3_34div(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, double __pyx_v_scalar); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_2V3_36__truediv__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, double __pyx_v_scalar); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_2htm_sc_init_raw(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_latitude, double __pyx_v_longitude); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_4htm_sc_init_wrapped(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_latitude, double __pyx_v_longitude); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_6htm_sc_angsep_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_sc __pyx_v_sc1, struct htm_sc __pyx_v_sc2); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_8htm_v3_init_raw(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_x, double __pyx_v_y, double __pyx_v_z); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_10htm_v3_init_wrapped(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_x, double __pyx_v_y, double __pyx_v_z); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_12htm_sc_to_v3_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_sc __pyx_v_sc); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_14htm_v3_to_sc_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_v3 __pyx_v_v3); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_16htm_v3_add_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_v3 __pyx_v_v1, struct htm_v3 __pyx_v_v2); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_18htm_v3_sub_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_v3 __pyx_v_v1, struct htm_v3 __pyx_v_v2); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_20htm_v3_neg_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_v3 __pyx_v_v1); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_22htm_v3_mul_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_v3 __pyx_v_v1, double __pyx_v_scalar); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_24htm_v3_div_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_v3 __pyx_v_v1, double __pyx_v_scalar); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_8Triangle_vertices(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_8Triangle_2center(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_8Triangle_4radius(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_8Triangle_6id(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_8Triangle_8level(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_8Triangle_10__init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_vertices, PyObject *__pyx_v_center, double __pyx_v_radius, PyObject *__pyx_v_id, PyObject *__pyx_v_level); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_8Triangle_12__repr__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_8Triangle_14from_htm_tri(CYTHON_UNUSED PyObject *__pyx_self, struct htm_tri __pyx_v_struct); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_8Triangle_16from_id(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_26htm_v3_id_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_v3 __pyx_v_v, PyObject *__pyx_v_level); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_28htm_tri_init_raw(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_30htm_tri_init_wrapped(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_3HTM_get_level(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_3HTM_2id_to_dec(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_3HTM_4parent(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_3HTM_6children(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_3HTM_8neighbors(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_3HTM_10neighbor(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id, PyObject *__pyx_v_direction); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_36__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_3HTM_12circle_search(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_center, double __pyx_v_radius, PyObject *__pyx_v_level, PyObject *__pyx_v_max_ranges); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_32htm_level_raw(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id); /* proto */
+static PyObject *__pyx_pf_7pynyhtm_34htm_id_to_dec(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id); /* proto */
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
   PyObject *__pyx_d;
   PyObject *__pyx_b;
   PyObject *__pyx_cython_runtime;
   PyObject *__pyx_empty_tuple;
@@ -3326,15 +3326,14 @@
   PyObject *__pyx_kp_s_No_value_specified_for_struct_at_9;
   PyObject *__pyx_n_s_None;
   PyObject *__pyx_n_s_NotImplementedError;
   PyObject *__pyx_n_s_OC_ONE;
   PyObject *__pyx_n_s_OC_TWO;
   PyObject *__pyx_n_s_OC_ZERO;
   PyObject *__pyx_n_s_OverflowError;
-  PyObject *__pyx_n_s_PynyHTM;
   PyObject *__pyx_kp_u_Root_level_neighbor_lookup_not_i;
   PyObject *__pyx_kp_u_Root_triangle;
   PyObject *__pyx_n_s_RuntimeError;
   PyObject *__pyx_kp_u_Search_failed_with_errorcode;
   PyObject *__pyx_kp_u_SphericalCoordinate;
   PyObject *__pyx_n_s_SphericalCoordinate_2;
   PyObject *__pyx_n_s_SphericalCoordinate___init;
@@ -3485,14 +3484,15 @@
   PyObject *__pyx_kp_s_numpy_core_umath_failed_to_impor;
   PyObject *__pyx_n_s_other;
   PyObject *__pyx_n_s_out;
   PyObject *__pyx_n_s_parent;
   PyObject *__pyx_n_s_parent_tail;
   PyObject *__pyx_n_s_prepare;
   PyObject *__pyx_n_s_property;
+  PyObject *__pyx_n_s_pynyhtm;
   PyObject *__pyx_kp_s_pynyhtm_pyx;
   PyObject *__pyx_n_s_qualname;
   PyObject *__pyx_n_s_radius;
   PyObject *__pyx_n_s_radius_2;
   PyObject *__pyx_n_s_range;
   PyObject *__pyx_n_s_ranges;
   PyObject *__pyx_n_s_repr;
@@ -3775,15 +3775,14 @@
   Py_CLEAR(clear_module_state->__pyx_kp_s_No_value_specified_for_struct_at_9);
   Py_CLEAR(clear_module_state->__pyx_n_s_None);
   Py_CLEAR(clear_module_state->__pyx_n_s_NotImplementedError);
   Py_CLEAR(clear_module_state->__pyx_n_s_OC_ONE);
   Py_CLEAR(clear_module_state->__pyx_n_s_OC_TWO);
   Py_CLEAR(clear_module_state->__pyx_n_s_OC_ZERO);
   Py_CLEAR(clear_module_state->__pyx_n_s_OverflowError);
-  Py_CLEAR(clear_module_state->__pyx_n_s_PynyHTM);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Root_level_neighbor_lookup_not_i);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Root_triangle);
   Py_CLEAR(clear_module_state->__pyx_n_s_RuntimeError);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Search_failed_with_errorcode);
   Py_CLEAR(clear_module_state->__pyx_kp_u_SphericalCoordinate);
   Py_CLEAR(clear_module_state->__pyx_n_s_SphericalCoordinate_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_SphericalCoordinate___init);
@@ -3934,14 +3933,15 @@
   Py_CLEAR(clear_module_state->__pyx_kp_s_numpy_core_umath_failed_to_impor);
   Py_CLEAR(clear_module_state->__pyx_n_s_other);
   Py_CLEAR(clear_module_state->__pyx_n_s_out);
   Py_CLEAR(clear_module_state->__pyx_n_s_parent);
   Py_CLEAR(clear_module_state->__pyx_n_s_parent_tail);
   Py_CLEAR(clear_module_state->__pyx_n_s_prepare);
   Py_CLEAR(clear_module_state->__pyx_n_s_property);
+  Py_CLEAR(clear_module_state->__pyx_n_s_pynyhtm);
   Py_CLEAR(clear_module_state->__pyx_kp_s_pynyhtm_pyx);
   Py_CLEAR(clear_module_state->__pyx_n_s_qualname);
   Py_CLEAR(clear_module_state->__pyx_n_s_radius);
   Py_CLEAR(clear_module_state->__pyx_n_s_radius_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_range);
   Py_CLEAR(clear_module_state->__pyx_n_s_ranges);
   Py_CLEAR(clear_module_state->__pyx_n_s_repr);
@@ -4202,15 +4202,14 @@
   Py_VISIT(traverse_module_state->__pyx_kp_s_No_value_specified_for_struct_at_9);
   Py_VISIT(traverse_module_state->__pyx_n_s_None);
   Py_VISIT(traverse_module_state->__pyx_n_s_NotImplementedError);
   Py_VISIT(traverse_module_state->__pyx_n_s_OC_ONE);
   Py_VISIT(traverse_module_state->__pyx_n_s_OC_TWO);
   Py_VISIT(traverse_module_state->__pyx_n_s_OC_ZERO);
   Py_VISIT(traverse_module_state->__pyx_n_s_OverflowError);
-  Py_VISIT(traverse_module_state->__pyx_n_s_PynyHTM);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Root_level_neighbor_lookup_not_i);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Root_triangle);
   Py_VISIT(traverse_module_state->__pyx_n_s_RuntimeError);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Search_failed_with_errorcode);
   Py_VISIT(traverse_module_state->__pyx_kp_u_SphericalCoordinate);
   Py_VISIT(traverse_module_state->__pyx_n_s_SphericalCoordinate_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_SphericalCoordinate___init);
@@ -4361,14 +4360,15 @@
   Py_VISIT(traverse_module_state->__pyx_kp_s_numpy_core_umath_failed_to_impor);
   Py_VISIT(traverse_module_state->__pyx_n_s_other);
   Py_VISIT(traverse_module_state->__pyx_n_s_out);
   Py_VISIT(traverse_module_state->__pyx_n_s_parent);
   Py_VISIT(traverse_module_state->__pyx_n_s_parent_tail);
   Py_VISIT(traverse_module_state->__pyx_n_s_prepare);
   Py_VISIT(traverse_module_state->__pyx_n_s_property);
+  Py_VISIT(traverse_module_state->__pyx_n_s_pynyhtm);
   Py_VISIT(traverse_module_state->__pyx_kp_s_pynyhtm_pyx);
   Py_VISIT(traverse_module_state->__pyx_n_s_qualname);
   Py_VISIT(traverse_module_state->__pyx_n_s_radius);
   Py_VISIT(traverse_module_state->__pyx_n_s_radius_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_range);
   Py_VISIT(traverse_module_state->__pyx_n_s_ranges);
   Py_VISIT(traverse_module_state->__pyx_n_s_repr);
@@ -4657,15 +4657,14 @@
 #define __pyx_kp_s_No_value_specified_for_struct_at_9 __pyx_mstate_global->__pyx_kp_s_No_value_specified_for_struct_at_9
 #define __pyx_n_s_None __pyx_mstate_global->__pyx_n_s_None
 #define __pyx_n_s_NotImplementedError __pyx_mstate_global->__pyx_n_s_NotImplementedError
 #define __pyx_n_s_OC_ONE __pyx_mstate_global->__pyx_n_s_OC_ONE
 #define __pyx_n_s_OC_TWO __pyx_mstate_global->__pyx_n_s_OC_TWO
 #define __pyx_n_s_OC_ZERO __pyx_mstate_global->__pyx_n_s_OC_ZERO
 #define __pyx_n_s_OverflowError __pyx_mstate_global->__pyx_n_s_OverflowError
-#define __pyx_n_s_PynyHTM __pyx_mstate_global->__pyx_n_s_PynyHTM
 #define __pyx_kp_u_Root_level_neighbor_lookup_not_i __pyx_mstate_global->__pyx_kp_u_Root_level_neighbor_lookup_not_i
 #define __pyx_kp_u_Root_triangle __pyx_mstate_global->__pyx_kp_u_Root_triangle
 #define __pyx_n_s_RuntimeError __pyx_mstate_global->__pyx_n_s_RuntimeError
 #define __pyx_kp_u_Search_failed_with_errorcode __pyx_mstate_global->__pyx_kp_u_Search_failed_with_errorcode
 #define __pyx_kp_u_SphericalCoordinate __pyx_mstate_global->__pyx_kp_u_SphericalCoordinate
 #define __pyx_n_s_SphericalCoordinate_2 __pyx_mstate_global->__pyx_n_s_SphericalCoordinate_2
 #define __pyx_n_s_SphericalCoordinate___init __pyx_mstate_global->__pyx_n_s_SphericalCoordinate___init
@@ -4816,14 +4815,15 @@
 #define __pyx_kp_s_numpy_core_umath_failed_to_impor __pyx_mstate_global->__pyx_kp_s_numpy_core_umath_failed_to_impor
 #define __pyx_n_s_other __pyx_mstate_global->__pyx_n_s_other
 #define __pyx_n_s_out __pyx_mstate_global->__pyx_n_s_out
 #define __pyx_n_s_parent __pyx_mstate_global->__pyx_n_s_parent
 #define __pyx_n_s_parent_tail __pyx_mstate_global->__pyx_n_s_parent_tail
 #define __pyx_n_s_prepare __pyx_mstate_global->__pyx_n_s_prepare
 #define __pyx_n_s_property __pyx_mstate_global->__pyx_n_s_property
+#define __pyx_n_s_pynyhtm __pyx_mstate_global->__pyx_n_s_pynyhtm
 #define __pyx_kp_s_pynyhtm_pyx __pyx_mstate_global->__pyx_kp_s_pynyhtm_pyx
 #define __pyx_n_s_qualname __pyx_mstate_global->__pyx_n_s_qualname
 #define __pyx_n_s_radius __pyx_mstate_global->__pyx_n_s_radius
 #define __pyx_n_s_radius_2 __pyx_mstate_global->__pyx_n_s_radius_2
 #define __pyx_n_s_range __pyx_mstate_global->__pyx_n_s_range
 #define __pyx_n_s_ranges __pyx_mstate_global->__pyx_n_s_ranges
 #define __pyx_n_s_repr __pyx_mstate_global->__pyx_n_s_repr
@@ -6816,261 +6816,261 @@
   __Pyx_XDECREF(__pyx_v_value);
   __Pyx_XDECREF(__pyx_v_t);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -7079,29 +7079,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -7112,15 +7112,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -7129,29 +7129,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -7162,15 +7162,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -7179,29 +7179,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -7212,15 +7212,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -7229,29 +7229,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -7262,15 +7262,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -7279,29 +7279,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -7312,217 +7312,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 970, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -7538,15 +7538,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -7554,68 +7554,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 982, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -7623,15 +7623,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -7646,15 +7646,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7670,15 +7670,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -7686,68 +7686,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 988, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -7755,15 +7755,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7778,15 +7778,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7802,15 +7802,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -7818,68 +7818,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 994, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -7887,15 +7887,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7910,170 +7910,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -8087,31 +8087,31 @@
  * 
  * def lib_get_license() -> str:             # <<<<<<<<<<<<<<
  *     """Retrieves the licence from the compiled library."""
  *     cdef const char* license = get_license()
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_1lib_get_license(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_lib_get_license, "Retrieves the licence from the compiled library.");
-static PyMethodDef __pyx_mdef_7PynyHTM_1lib_get_license = {"lib_get_license", (PyCFunction)__pyx_pw_7PynyHTM_1lib_get_license, METH_NOARGS, __pyx_doc_7PynyHTM_lib_get_license};
-static PyObject *__pyx_pw_7PynyHTM_1lib_get_license(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7pynyhtm_1lib_get_license(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_lib_get_license, "Retrieves the licence from the compiled library.");
+static PyMethodDef __pyx_mdef_7pynyhtm_1lib_get_license = {"lib_get_license", (PyCFunction)__pyx_pw_7pynyhtm_1lib_get_license, METH_NOARGS, __pyx_doc_7pynyhtm_lib_get_license};
+static PyObject *__pyx_pw_7pynyhtm_1lib_get_license(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("lib_get_license (wrapper)", 0);
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
-  __pyx_r = __pyx_pf_7PynyHTM_lib_get_license(__pyx_self);
+  __pyx_r = __pyx_pf_7pynyhtm_lib_get_license(__pyx_self);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_lib_get_license(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_7pynyhtm_lib_get_license(CYTHON_UNUSED PyObject *__pyx_self) {
   char const *__pyx_v_license;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -8150,15 +8150,15 @@
  *     """Retrieves the licence from the compiled library."""
  *     cdef const char* license = get_license()
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("PynyHTM.lib_get_license", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.lib_get_license", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -8167,24 +8167,24 @@
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def latitude(self) -> float:
  *         """Latitude of this spherical coordinate."""
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_19SphericalCoordinate_1latitude(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_19SphericalCoordinate_1latitude(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_19SphericalCoordinate_latitude, "Latitude of this spherical coordinate.");
-static PyMethodDef __pyx_mdef_7PynyHTM_19SphericalCoordinate_1latitude = {"latitude", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_19SphericalCoordinate_1latitude, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_19SphericalCoordinate_latitude};
-static PyObject *__pyx_pw_7PynyHTM_19SphericalCoordinate_1latitude(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_19SphericalCoordinate_latitude, "Latitude of this spherical coordinate.");
+static PyMethodDef __pyx_mdef_7pynyhtm_19SphericalCoordinate_1latitude = {"latitude", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_19SphericalCoordinate_1latitude, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_19SphericalCoordinate_latitude};
+static PyObject *__pyx_pw_7pynyhtm_19SphericalCoordinate_1latitude(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -8246,32 +8246,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.SphericalCoordinate.latitude", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.SphericalCoordinate.latitude", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_19SphericalCoordinate_latitude(__pyx_self, __pyx_v_self);
+  __pyx_r = __pyx_pf_7pynyhtm_19SphericalCoordinate_latitude(__pyx_self, __pyx_v_self);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_19SphericalCoordinate_latitude(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pf_7pynyhtm_19SphericalCoordinate_latitude(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("latitude", 1);
@@ -8297,15 +8297,15 @@
  *     def latitude(self) -> float:
  *         """Latitude of this spherical coordinate."""
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("PynyHTM.SphericalCoordinate.latitude", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.SphericalCoordinate.latitude", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -8314,24 +8314,24 @@
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def longitude(self) -> float:
  *         """Longitude of this spherical coordinate."""
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_19SphericalCoordinate_3longitude(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_19SphericalCoordinate_3longitude(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_19SphericalCoordinate_2longitude, "Longitude of this spherical coordinate.");
-static PyMethodDef __pyx_mdef_7PynyHTM_19SphericalCoordinate_3longitude = {"longitude", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_19SphericalCoordinate_3longitude, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_19SphericalCoordinate_2longitude};
-static PyObject *__pyx_pw_7PynyHTM_19SphericalCoordinate_3longitude(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_19SphericalCoordinate_2longitude, "Longitude of this spherical coordinate.");
+static PyMethodDef __pyx_mdef_7pynyhtm_19SphericalCoordinate_3longitude = {"longitude", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_19SphericalCoordinate_3longitude, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_19SphericalCoordinate_2longitude};
+static PyObject *__pyx_pw_7pynyhtm_19SphericalCoordinate_3longitude(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -8393,32 +8393,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.SphericalCoordinate.longitude", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.SphericalCoordinate.longitude", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_19SphericalCoordinate_2longitude(__pyx_self, __pyx_v_self);
+  __pyx_r = __pyx_pf_7pynyhtm_19SphericalCoordinate_2longitude(__pyx_self, __pyx_v_self);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_19SphericalCoordinate_2longitude(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pf_7pynyhtm_19SphericalCoordinate_2longitude(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("longitude", 1);
@@ -8444,15 +8444,15 @@
  *     def longitude(self) -> float:
  *         """Longitude of this spherical coordinate."""
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("PynyHTM.SphericalCoordinate.longitude", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.SphericalCoordinate.longitude", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -8461,24 +8461,24 @@
  * 
  *     def __init__(self, latitude: float, longitude: float) -> None:             # <<<<<<<<<<<<<<
  *         """
  *         Initializes this spherical coordinate with given latitude and longitude.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_19SphericalCoordinate_5__init__(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_19SphericalCoordinate_5__init__(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_19SphericalCoordinate_4__init__, "\n        Initializes this spherical coordinate with given latitude and longitude.\n\n        :param latitude: latitude of the spherical coordinate\n        :param longitude: longitude of the spherical coordinate\n        ");
-static PyMethodDef __pyx_mdef_7PynyHTM_19SphericalCoordinate_5__init__ = {"__init__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_19SphericalCoordinate_5__init__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_19SphericalCoordinate_4__init__};
-static PyObject *__pyx_pw_7PynyHTM_19SphericalCoordinate_5__init__(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_19SphericalCoordinate_4__init__, "\n        Initializes this spherical coordinate with given latitude and longitude.\n\n        :param latitude: latitude of the spherical coordinate\n        :param longitude: longitude of the spherical coordinate\n        ");
+static PyMethodDef __pyx_mdef_7pynyhtm_19SphericalCoordinate_5__init__ = {"__init__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_19SphericalCoordinate_5__init__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_19SphericalCoordinate_4__init__};
+static PyObject *__pyx_pw_7pynyhtm_19SphericalCoordinate_5__init__(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -8570,32 +8570,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.SphericalCoordinate.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.SphericalCoordinate.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_19SphericalCoordinate_4__init__(__pyx_self, __pyx_v_self, __pyx_v_latitude, __pyx_v_longitude);
+  __pyx_r = __pyx_pf_7pynyhtm_19SphericalCoordinate_4__init__(__pyx_self, __pyx_v_self, __pyx_v_latitude, __pyx_v_longitude);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_19SphericalCoordinate_4__init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, double __pyx_v_latitude, double __pyx_v_longitude) {
+static PyObject *__pyx_pf_7pynyhtm_19SphericalCoordinate_4__init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, double __pyx_v_latitude, double __pyx_v_longitude) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 1);
@@ -8633,15 +8633,15 @@
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("PynyHTM.SphericalCoordinate.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.SphericalCoordinate.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -8650,24 +8650,24 @@
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         """Detailed representation of this SphericalCoordinate."""
  *         return f"SphericalCoordinate({str(self.__dict__)})"
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_19SphericalCoordinate_7__repr__(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_19SphericalCoordinate_7__repr__(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_19SphericalCoordinate_6__repr__, "Detailed representation of this SphericalCoordinate.");
-static PyMethodDef __pyx_mdef_7PynyHTM_19SphericalCoordinate_7__repr__ = {"__repr__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_19SphericalCoordinate_7__repr__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_19SphericalCoordinate_6__repr__};
-static PyObject *__pyx_pw_7PynyHTM_19SphericalCoordinate_7__repr__(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_19SphericalCoordinate_6__repr__, "Detailed representation of this SphericalCoordinate.");
+static PyMethodDef __pyx_mdef_7pynyhtm_19SphericalCoordinate_7__repr__ = {"__repr__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_19SphericalCoordinate_7__repr__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_19SphericalCoordinate_6__repr__};
+static PyObject *__pyx_pw_7pynyhtm_19SphericalCoordinate_7__repr__(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -8729,32 +8729,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.SphericalCoordinate.__repr__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.SphericalCoordinate.__repr__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_19SphericalCoordinate_6__repr__(__pyx_self, __pyx_v_self);
+  __pyx_r = __pyx_pf_7pynyhtm_19SphericalCoordinate_6__repr__(__pyx_self, __pyx_v_self);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_19SphericalCoordinate_6__repr__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pf_7pynyhtm_19SphericalCoordinate_6__repr__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   Py_ssize_t __pyx_t_2;
   Py_UCS4 __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
@@ -8812,15 +8812,15 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("PynyHTM.SphericalCoordinate.__repr__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.SphericalCoordinate.__repr__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -8829,24 +8829,24 @@
  * 
  *     def get_htm_sc(self):             # <<<<<<<<<<<<<<
  *         """Gets a htm_sc strcut based on this spherical coordinate."""
  *         return htm_sc(self._longitude, self._latitude)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_19SphericalCoordinate_9get_htm_sc(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_19SphericalCoordinate_9get_htm_sc(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_19SphericalCoordinate_8get_htm_sc, "Gets a htm_sc strcut based on this spherical coordinate.");
-static PyMethodDef __pyx_mdef_7PynyHTM_19SphericalCoordinate_9get_htm_sc = {"get_htm_sc", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_19SphericalCoordinate_9get_htm_sc, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_19SphericalCoordinate_8get_htm_sc};
-static PyObject *__pyx_pw_7PynyHTM_19SphericalCoordinate_9get_htm_sc(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_19SphericalCoordinate_8get_htm_sc, "Gets a htm_sc strcut based on this spherical coordinate.");
+static PyMethodDef __pyx_mdef_7pynyhtm_19SphericalCoordinate_9get_htm_sc = {"get_htm_sc", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_19SphericalCoordinate_9get_htm_sc, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_19SphericalCoordinate_8get_htm_sc};
+static PyObject *__pyx_pw_7pynyhtm_19SphericalCoordinate_9get_htm_sc(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -8908,32 +8908,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.SphericalCoordinate.get_htm_sc", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.SphericalCoordinate.get_htm_sc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_19SphericalCoordinate_8get_htm_sc(__pyx_self, __pyx_v_self);
+  __pyx_r = __pyx_pf_7pynyhtm_19SphericalCoordinate_8get_htm_sc(__pyx_self, __pyx_v_self);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_19SphericalCoordinate_8get_htm_sc(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pf_7pynyhtm_19SphericalCoordinate_8get_htm_sc(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   double __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -8978,15 +8978,15 @@
  *         return htm_sc(self._longitude, self._latitude)
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("PynyHTM.SphericalCoordinate.get_htm_sc", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.SphericalCoordinate.get_htm_sc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -8995,24 +8995,24 @@
  * 
  *     def from_htm_sc(sc: htm_sc) -> SphericalCoordinate:             # <<<<<<<<<<<<<<
  *         """
  *         Creates a Spherical coordinate based on a htm_sc struct.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_19SphericalCoordinate_11from_htm_sc(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_19SphericalCoordinate_11from_htm_sc(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_19SphericalCoordinate_10from_htm_sc, "\n        Creates a Spherical coordinate based on a htm_sc struct.\n\n        :param sc: htm_sc struct which contains the latitude and longitude\n        :returns: A SphericalCoordinate object with values from the provided htm_sc struct\n        :raises valueError: if the provided spherical coordinate struct object is invalid\n        ");
-static PyMethodDef __pyx_mdef_7PynyHTM_19SphericalCoordinate_11from_htm_sc = {"from_htm_sc", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_19SphericalCoordinate_11from_htm_sc, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_19SphericalCoordinate_10from_htm_sc};
-static PyObject *__pyx_pw_7PynyHTM_19SphericalCoordinate_11from_htm_sc(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_19SphericalCoordinate_10from_htm_sc, "\n        Creates a Spherical coordinate based on a htm_sc struct.\n\n        :param sc: htm_sc struct which contains the latitude and longitude\n        :returns: A SphericalCoordinate object with values from the provided htm_sc struct\n        :raises valueError: if the provided spherical coordinate struct object is invalid\n        ");
+static PyMethodDef __pyx_mdef_7pynyhtm_19SphericalCoordinate_11from_htm_sc = {"from_htm_sc", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_19SphericalCoordinate_11from_htm_sc, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_19SphericalCoordinate_10from_htm_sc};
+static PyObject *__pyx_pw_7pynyhtm_19SphericalCoordinate_11from_htm_sc(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   struct htm_sc __pyx_v_sc;
@@ -9074,32 +9074,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.SphericalCoordinate.from_htm_sc", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.SphericalCoordinate.from_htm_sc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_19SphericalCoordinate_10from_htm_sc(__pyx_self, __pyx_v_sc);
+  __pyx_r = __pyx_pf_7pynyhtm_19SphericalCoordinate_10from_htm_sc(__pyx_self, __pyx_v_sc);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_19SphericalCoordinate_10from_htm_sc(CYTHON_UNUSED PyObject *__pyx_self, struct htm_sc __pyx_v_sc) {
+static PyObject *__pyx_pf_7pynyhtm_19SphericalCoordinate_10from_htm_sc(CYTHON_UNUSED PyObject *__pyx_self, struct htm_sc __pyx_v_sc) {
   PyObject *__pyx_v_latitude = NULL;
   PyObject *__pyx_v_longitude = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
@@ -9244,15 +9244,15 @@
  *             return SphericalCoordinate(latitude=latitude, longitude=longitude)
  *         except Exception:             # <<<<<<<<<<<<<<
  *             raise ValueError(f"{sc} does not have lat,lon attribute.")
  * 
  */
     __pyx_t_7 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_7) {
-      __Pyx_AddTraceback("PynyHTM.SphericalCoordinate.from_htm_sc", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("pynyhtm.SphericalCoordinate.from_htm_sc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_6, &__pyx_t_5, &__pyx_t_4) < 0) __PYX_ERR(0, 134, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_4);
 
       /* "pynyhtm.pyx":135
  *             return SphericalCoordinate(latitude=latitude, longitude=longitude)
@@ -9310,15 +9310,15 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_9);
-  __Pyx_AddTraceback("PynyHTM.SphericalCoordinate.from_htm_sc", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.SphericalCoordinate.from_htm_sc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_latitude);
   __Pyx_XDECREF(__pyx_v_longitude);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
@@ -9329,24 +9329,24 @@
  * 
  *     def to_v3(self) -> V3:             # <<<<<<<<<<<<<<
  *         """
  *         Transforms this spherical coordinate into a v3 vector.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_19SphericalCoordinate_13to_v3(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_19SphericalCoordinate_13to_v3(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_19SphericalCoordinate_12to_v3, "\n        Transforms this spherical coordinate into a v3 vector.\n\n        :return: v3 equivalent\n        :raises valueError: if conversation failed\n        ");
-static PyMethodDef __pyx_mdef_7PynyHTM_19SphericalCoordinate_13to_v3 = {"to_v3", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_19SphericalCoordinate_13to_v3, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_19SphericalCoordinate_12to_v3};
-static PyObject *__pyx_pw_7PynyHTM_19SphericalCoordinate_13to_v3(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_19SphericalCoordinate_12to_v3, "\n        Transforms this spherical coordinate into a v3 vector.\n\n        :return: v3 equivalent\n        :raises valueError: if conversation failed\n        ");
+static PyMethodDef __pyx_mdef_7pynyhtm_19SphericalCoordinate_13to_v3 = {"to_v3", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_19SphericalCoordinate_13to_v3, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_19SphericalCoordinate_12to_v3};
+static PyObject *__pyx_pw_7pynyhtm_19SphericalCoordinate_13to_v3(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -9408,32 +9408,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.SphericalCoordinate.to_v3", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.SphericalCoordinate.to_v3", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_19SphericalCoordinate_12to_v3(__pyx_self, __pyx_v_self);
+  __pyx_r = __pyx_pf_7pynyhtm_19SphericalCoordinate_12to_v3(__pyx_self, __pyx_v_self);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_19SphericalCoordinate_12to_v3(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pf_7pynyhtm_19SphericalCoordinate_12to_v3(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_v_ec = NULL;
   PyObject *__pyx_v_v3 = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
@@ -9675,15 +9675,15 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("PynyHTM.SphericalCoordinate.to_v3", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.SphericalCoordinate.to_v3", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_ec);
   __Pyx_XDECREF(__pyx_v_v3);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
@@ -9694,24 +9694,24 @@
  * 
  *     def angle_separation(self, other: SphericalCoordinate) -> float:             # <<<<<<<<<<<<<<
  *         """
  *         Determine the angle difference between the two given spherical coordinates.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_19SphericalCoordinate_15angle_separation(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_19SphericalCoordinate_15angle_separation(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_19SphericalCoordinate_14angle_separation, "\n        Determine the angle difference between the two given spherical coordinates.\n\n        :param other: second reference point\n        :returns: angle between sc1 and sc2\n        ");
-static PyMethodDef __pyx_mdef_7PynyHTM_19SphericalCoordinate_15angle_separation = {"angle_separation", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_19SphericalCoordinate_15angle_separation, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_19SphericalCoordinate_14angle_separation};
-static PyObject *__pyx_pw_7PynyHTM_19SphericalCoordinate_15angle_separation(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_19SphericalCoordinate_14angle_separation, "\n        Determine the angle difference between the two given spherical coordinates.\n\n        :param other: second reference point\n        :returns: angle between sc1 and sc2\n        ");
+static PyMethodDef __pyx_mdef_7pynyhtm_19SphericalCoordinate_15angle_separation = {"angle_separation", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_19SphericalCoordinate_15angle_separation, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_19SphericalCoordinate_14angle_separation};
+static PyObject *__pyx_pw_7pynyhtm_19SphericalCoordinate_15angle_separation(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -9788,32 +9788,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.SphericalCoordinate.angle_separation", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.SphericalCoordinate.angle_separation", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_19SphericalCoordinate_14angle_separation(__pyx_self, __pyx_v_self, __pyx_v_other);
+  __pyx_r = __pyx_pf_7pynyhtm_19SphericalCoordinate_14angle_separation(__pyx_self, __pyx_v_self, __pyx_v_other);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_19SphericalCoordinate_14angle_separation(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
+static PyObject *__pyx_pf_7pynyhtm_19SphericalCoordinate_14angle_separation(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
@@ -9922,15 +9922,15 @@
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_AddTraceback("PynyHTM.SphericalCoordinate.angle_separation", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.SphericalCoordinate.angle_separation", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -9939,24 +9939,24 @@
  * 
  *     def get_htm_id(self, level: int) -> int64_t:             # <<<<<<<<<<<<<<
  *         """Gets the HTM id for this spherical coordinate at the given level.
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_19SphericalCoordinate_17get_htm_id(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_19SphericalCoordinate_17get_htm_id(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_19SphericalCoordinate_16get_htm_id, "Gets the HTM id for this spherical coordinate at the given level.\n\n        :param level: depth at which the id should be determined.\n        :returns: id of the trixel in which this spherical coordinate lands\n        :raises valueError: if the provided htm_v3 struct object is invalid\n        ");
-static PyMethodDef __pyx_mdef_7PynyHTM_19SphericalCoordinate_17get_htm_id = {"get_htm_id", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_19SphericalCoordinate_17get_htm_id, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_19SphericalCoordinate_16get_htm_id};
-static PyObject *__pyx_pw_7PynyHTM_19SphericalCoordinate_17get_htm_id(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_19SphericalCoordinate_16get_htm_id, "Gets the HTM id for this spherical coordinate at the given level.\n\n        :param level: depth at which the id should be determined.\n        :returns: id of the trixel in which this spherical coordinate lands\n        :raises valueError: if the provided htm_v3 struct object is invalid\n        ");
+static PyMethodDef __pyx_mdef_7pynyhtm_19SphericalCoordinate_17get_htm_id = {"get_htm_id", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_19SphericalCoordinate_17get_htm_id, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_19SphericalCoordinate_16get_htm_id};
+static PyObject *__pyx_pw_7pynyhtm_19SphericalCoordinate_17get_htm_id(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -10033,20 +10033,20 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.SphericalCoordinate.get_htm_id", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.SphericalCoordinate.get_htm_id", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_level), (&PyInt_Type), 0, "level", 1))) __PYX_ERR(0, 158, __pyx_L1_error)
-  __pyx_r = __pyx_pf_7PynyHTM_19SphericalCoordinate_16get_htm_id(__pyx_self, __pyx_v_self, __pyx_v_level);
+  __pyx_r = __pyx_pf_7pynyhtm_19SphericalCoordinate_16get_htm_id(__pyx_self, __pyx_v_self, __pyx_v_level);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   {
@@ -10055,15 +10055,15 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_19SphericalCoordinate_16get_htm_id(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_level) {
+static PyObject *__pyx_pf_7pynyhtm_19SphericalCoordinate_16get_htm_id(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_level) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
@@ -10143,15 +10143,15 @@
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("PynyHTM.SphericalCoordinate.get_htm_id", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.SphericalCoordinate.get_htm_id", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -10160,24 +10160,24 @@
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def x(self) -> float:
  *         """X coordinate of this vector."""
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_2V3_1x(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_2V3_1x(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_2V3_x, "X coordinate of this vector.");
-static PyMethodDef __pyx_mdef_7PynyHTM_2V3_1x = {"x", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_2V3_1x, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_2V3_x};
-static PyObject *__pyx_pw_7PynyHTM_2V3_1x(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_2V3_x, "X coordinate of this vector.");
+static PyMethodDef __pyx_mdef_7pynyhtm_2V3_1x = {"x", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_2V3_1x, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_2V3_x};
+static PyObject *__pyx_pw_7pynyhtm_2V3_1x(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -10239,32 +10239,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.V3.x", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.x", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_2V3_x(__pyx_self, __pyx_v_self);
+  __pyx_r = __pyx_pf_7pynyhtm_2V3_x(__pyx_self, __pyx_v_self);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_2V3_x(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pf_7pynyhtm_2V3_x(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("x", 1);
@@ -10290,15 +10290,15 @@
  *     def x(self) -> float:
  *         """X coordinate of this vector."""
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("PynyHTM.V3.x", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.x", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -10307,24 +10307,24 @@
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def y(self) -> float:
  *         """Y coordinate of this vector."""
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_2V3_3y(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_2V3_3y(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_2V3_2y, "Y coordinate of this vector.");
-static PyMethodDef __pyx_mdef_7PynyHTM_2V3_3y = {"y", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_2V3_3y, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_2V3_2y};
-static PyObject *__pyx_pw_7PynyHTM_2V3_3y(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_2V3_2y, "Y coordinate of this vector.");
+static PyMethodDef __pyx_mdef_7pynyhtm_2V3_3y = {"y", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_2V3_3y, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_2V3_2y};
+static PyObject *__pyx_pw_7pynyhtm_2V3_3y(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -10386,32 +10386,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.V3.y", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.y", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_2V3_2y(__pyx_self, __pyx_v_self);
+  __pyx_r = __pyx_pf_7pynyhtm_2V3_2y(__pyx_self, __pyx_v_self);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_2V3_2y(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pf_7pynyhtm_2V3_2y(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("y", 1);
@@ -10437,15 +10437,15 @@
  *     def y(self) -> float:
  *         """Y coordinate of this vector."""
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("PynyHTM.V3.y", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.y", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -10454,24 +10454,24 @@
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def z(self) -> float:
  *         """Z coordinate of this vector."""
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_2V3_5z(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_2V3_5z(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_2V3_4z, "Z coordinate of this vector.");
-static PyMethodDef __pyx_mdef_7PynyHTM_2V3_5z = {"z", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_2V3_5z, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_2V3_4z};
-static PyObject *__pyx_pw_7PynyHTM_2V3_5z(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_2V3_4z, "Z coordinate of this vector.");
+static PyMethodDef __pyx_mdef_7pynyhtm_2V3_5z = {"z", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_2V3_5z, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_2V3_4z};
+static PyObject *__pyx_pw_7pynyhtm_2V3_5z(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -10533,32 +10533,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.V3.z", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.z", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_2V3_4z(__pyx_self, __pyx_v_self);
+  __pyx_r = __pyx_pf_7pynyhtm_2V3_4z(__pyx_self, __pyx_v_self);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_2V3_4z(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pf_7pynyhtm_2V3_4z(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("z", 1);
@@ -10584,15 +10584,15 @@
  *     def z(self) -> float:
  *         """Z coordinate of this vector."""
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("PynyHTM.V3.z", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.z", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -10601,24 +10601,24 @@
  * 
  *     def __init__(self, x: float, y: float, z: float) -> None:             # <<<<<<<<<<<<<<
  *         """
  *         Initializes this v3 vector with the given values.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_2V3_7__init__(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_2V3_7__init__(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_2V3_6__init__, "\n        Initializes this v3 vector with the given values.\n\n        :param x: x (first) value\n        :param y: y (second) value\n        :param z: z (third) value\n        ");
-static PyMethodDef __pyx_mdef_7PynyHTM_2V3_7__init__ = {"__init__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_2V3_7__init__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_2V3_6__init__};
-static PyObject *__pyx_pw_7PynyHTM_2V3_7__init__(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_2V3_6__init__, "\n        Initializes this v3 vector with the given values.\n\n        :param x: x (first) value\n        :param y: y (second) value\n        :param z: z (third) value\n        ");
+static PyMethodDef __pyx_mdef_7pynyhtm_2V3_7__init__ = {"__init__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_2V3_7__init__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_2V3_6__init__};
+static PyObject *__pyx_pw_7pynyhtm_2V3_7__init__(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -10725,32 +10725,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.V3.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_2V3_6__init__(__pyx_self, __pyx_v_self, __pyx_v_x, __pyx_v_y, __pyx_v_z);
+  __pyx_r = __pyx_pf_7pynyhtm_2V3_6__init__(__pyx_self, __pyx_v_self, __pyx_v_x, __pyx_v_y, __pyx_v_z);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_2V3_6__init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, double __pyx_v_x, double __pyx_v_y, double __pyx_v_z) {
+static PyObject *__pyx_pf_7pynyhtm_2V3_6__init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, double __pyx_v_x, double __pyx_v_y, double __pyx_v_z) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 1);
@@ -10800,15 +10800,15 @@
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("PynyHTM.V3.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -10817,24 +10817,24 @@
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         """Detailed representation of this V3 Vector."""
  *         return f"V3({str(self.__dict__)})"
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_2V3_9__repr__(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_2V3_9__repr__(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_2V3_8__repr__, "Detailed representation of this V3 Vector.");
-static PyMethodDef __pyx_mdef_7PynyHTM_2V3_9__repr__ = {"__repr__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_2V3_9__repr__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_2V3_8__repr__};
-static PyObject *__pyx_pw_7PynyHTM_2V3_9__repr__(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_2V3_8__repr__, "Detailed representation of this V3 Vector.");
+static PyMethodDef __pyx_mdef_7pynyhtm_2V3_9__repr__ = {"__repr__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_2V3_9__repr__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_2V3_8__repr__};
+static PyObject *__pyx_pw_7pynyhtm_2V3_9__repr__(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -10896,32 +10896,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.V3.__repr__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.__repr__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_2V3_8__repr__(__pyx_self, __pyx_v_self);
+  __pyx_r = __pyx_pf_7pynyhtm_2V3_8__repr__(__pyx_self, __pyx_v_self);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_2V3_8__repr__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pf_7pynyhtm_2V3_8__repr__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   Py_ssize_t __pyx_t_2;
   Py_UCS4 __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
@@ -10979,15 +10979,15 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("PynyHTM.V3.__repr__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.__repr__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -10996,24 +10996,24 @@
  * 
  *     def get_htm_v3(self):             # <<<<<<<<<<<<<<
  *         """Gets a htm_v3 strcut based on this v3 object."""
  *         return htm_v3(self._x, self._y, self._z)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_2V3_11get_htm_v3(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_2V3_11get_htm_v3(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_2V3_10get_htm_v3, "Gets a htm_v3 strcut based on this v3 object.");
-static PyMethodDef __pyx_mdef_7PynyHTM_2V3_11get_htm_v3 = {"get_htm_v3", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_2V3_11get_htm_v3, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_2V3_10get_htm_v3};
-static PyObject *__pyx_pw_7PynyHTM_2V3_11get_htm_v3(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_2V3_10get_htm_v3, "Gets a htm_v3 strcut based on this v3 object.");
+static PyMethodDef __pyx_mdef_7pynyhtm_2V3_11get_htm_v3 = {"get_htm_v3", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_2V3_11get_htm_v3, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_2V3_10get_htm_v3};
+static PyObject *__pyx_pw_7pynyhtm_2V3_11get_htm_v3(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -11075,32 +11075,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.V3.get_htm_v3", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.get_htm_v3", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_2V3_10get_htm_v3(__pyx_self, __pyx_v_self);
+  __pyx_r = __pyx_pf_7pynyhtm_2V3_10get_htm_v3(__pyx_self, __pyx_v_self);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_2V3_10get_htm_v3(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pf_7pynyhtm_2V3_10get_htm_v3(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   double __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -11153,15 +11153,15 @@
  *         return htm_v3(self._x, self._y, self._z)
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("PynyHTM.V3.get_htm_v3", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.get_htm_v3", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -11170,24 +11170,24 @@
  * 
  *     def from_htm_v3(v3: htm_v3) -> V3:             # <<<<<<<<<<<<<<
  *         """
  *         Creates a V3 object based on a htm_v3 struct.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_2V3_13from_htm_v3(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_2V3_13from_htm_v3(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_2V3_12from_htm_v3, "\n        Creates a V3 object based on a htm_v3 struct.\n\n        :param v3: htm_v3 struct which contains x,y,z\n        :returns: A V3 object with values from the provided htm_v3 struct\n        :raises valueError: if the provided htm_v3 struct object is invalid\n        ");
-static PyMethodDef __pyx_mdef_7PynyHTM_2V3_13from_htm_v3 = {"from_htm_v3", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_2V3_13from_htm_v3, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_2V3_12from_htm_v3};
-static PyObject *__pyx_pw_7PynyHTM_2V3_13from_htm_v3(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_2V3_12from_htm_v3, "\n        Creates a V3 object based on a htm_v3 struct.\n\n        :param v3: htm_v3 struct which contains x,y,z\n        :returns: A V3 object with values from the provided htm_v3 struct\n        :raises valueError: if the provided htm_v3 struct object is invalid\n        ");
+static PyMethodDef __pyx_mdef_7pynyhtm_2V3_13from_htm_v3 = {"from_htm_v3", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_2V3_13from_htm_v3, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_2V3_12from_htm_v3};
+static PyObject *__pyx_pw_7pynyhtm_2V3_13from_htm_v3(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   struct htm_v3 __pyx_v_v3;
@@ -11249,32 +11249,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.V3.from_htm_v3", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.from_htm_v3", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_2V3_12from_htm_v3(__pyx_self, __pyx_v_v3);
+  __pyx_r = __pyx_pf_7pynyhtm_2V3_12from_htm_v3(__pyx_self, __pyx_v_v3);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_2V3_12from_htm_v3(CYTHON_UNUSED PyObject *__pyx_self, struct htm_v3 __pyx_v_v3) {
+static PyObject *__pyx_pf_7pynyhtm_2V3_12from_htm_v3(CYTHON_UNUSED PyObject *__pyx_self, struct htm_v3 __pyx_v_v3) {
   PyObject *__pyx_v_x = NULL;
   PyObject *__pyx_v_y = NULL;
   PyObject *__pyx_v_z = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
@@ -11458,15 +11458,15 @@
  *             return V3(x=x, y=y, z=z)
  *         except Exception:             # <<<<<<<<<<<<<<
  *             raise ValueError(f"{v3} does not have x,y,z attributes.")
  * 
  */
     __pyx_t_7 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_7) {
-      __Pyx_AddTraceback("PynyHTM.V3.from_htm_v3", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("pynyhtm.V3.from_htm_v3", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_4) < 0) __PYX_ERR(0, 219, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_4);
 
       /* "pynyhtm.pyx":220
  *             return V3(x=x, y=y, z=z)
@@ -11524,15 +11524,15 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_9);
-  __Pyx_AddTraceback("PynyHTM.V3.from_htm_v3", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.from_htm_v3", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_x);
   __Pyx_XDECREF(__pyx_v_y);
   __Pyx_XDECREF(__pyx_v_z);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -11544,24 +11544,24 @@
  * 
  *     def to_sc(self) -> SphericalCoordinate:             # <<<<<<<<<<<<<<
  *         """
  *         Transforms this V3 vector into a sphercial coordinate.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_2V3_15to_sc(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_2V3_15to_sc(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_2V3_14to_sc, "\n        Transforms this V3 vector into a sphercial coordinate.\n\n        :returns: Spherical coordinate equivalent\n        :raises valueError: if conversion failed\n        ");
-static PyMethodDef __pyx_mdef_7PynyHTM_2V3_15to_sc = {"to_sc", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_2V3_15to_sc, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_2V3_14to_sc};
-static PyObject *__pyx_pw_7PynyHTM_2V3_15to_sc(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_2V3_14to_sc, "\n        Transforms this V3 vector into a sphercial coordinate.\n\n        :returns: Spherical coordinate equivalent\n        :raises valueError: if conversion failed\n        ");
+static PyMethodDef __pyx_mdef_7pynyhtm_2V3_15to_sc = {"to_sc", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_2V3_15to_sc, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_2V3_14to_sc};
+static PyObject *__pyx_pw_7pynyhtm_2V3_15to_sc(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -11623,32 +11623,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.V3.to_sc", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.to_sc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_2V3_14to_sc(__pyx_self, __pyx_v_self);
+  __pyx_r = __pyx_pf_7pynyhtm_2V3_14to_sc(__pyx_self, __pyx_v_self);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_2V3_14to_sc(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pf_7pynyhtm_2V3_14to_sc(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_v_ec = NULL;
   PyObject *__pyx_v_sc = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
@@ -11890,15 +11890,15 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("PynyHTM.V3.to_sc", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.to_sc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_ec);
   __Pyx_XDECREF(__pyx_v_sc);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
@@ -11909,24 +11909,24 @@
  * 
  *     def get_htm_id(self, level: int) -> int64_t:             # <<<<<<<<<<<<<<
  *         """Gets the HTM id for this v3 vector at the given level.
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_2V3_17get_htm_id(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_2V3_17get_htm_id(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_2V3_16get_htm_id, "Gets the HTM id for this v3 vector at the given level.\n\n        :param level: depth at which the id should be determined.\n        :returns: id of the trixel in which this v3 lands\n        ");
-static PyMethodDef __pyx_mdef_7PynyHTM_2V3_17get_htm_id = {"get_htm_id", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_2V3_17get_htm_id, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_2V3_16get_htm_id};
-static PyObject *__pyx_pw_7PynyHTM_2V3_17get_htm_id(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_2V3_16get_htm_id, "Gets the HTM id for this v3 vector at the given level.\n\n        :param level: depth at which the id should be determined.\n        :returns: id of the trixel in which this v3 lands\n        ");
+static PyMethodDef __pyx_mdef_7pynyhtm_2V3_17get_htm_id = {"get_htm_id", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_2V3_17get_htm_id, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_2V3_16get_htm_id};
+static PyObject *__pyx_pw_7pynyhtm_2V3_17get_htm_id(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -12003,20 +12003,20 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.V3.get_htm_id", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.get_htm_id", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_level), (&PyInt_Type), 0, "level", 1))) __PYX_ERR(0, 234, __pyx_L1_error)
-  __pyx_r = __pyx_pf_7PynyHTM_2V3_16get_htm_id(__pyx_self, __pyx_v_self, __pyx_v_level);
+  __pyx_r = __pyx_pf_7pynyhtm_2V3_16get_htm_id(__pyx_self, __pyx_v_self, __pyx_v_level);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   {
@@ -12025,15 +12025,15 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_2V3_16get_htm_id(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_level) {
+static PyObject *__pyx_pf_7pynyhtm_2V3_16get_htm_id(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_level) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
@@ -12115,15 +12115,15 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("PynyHTM.V3.get_htm_id", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.get_htm_id", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -12132,24 +12132,24 @@
  * 
  *     def add(self, other: V3) -> V3:             # <<<<<<<<<<<<<<
  *         """
  *         Adds the other vector to this vector.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_2V3_19add(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_2V3_19add(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_2V3_18add, "\n        Adds the other vector to this vector.\n\n        :param other: vector to add\n        :returns: self + vector\n        ");
-static PyMethodDef __pyx_mdef_7PynyHTM_2V3_19add = {"add", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_2V3_19add, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_2V3_18add};
-static PyObject *__pyx_pw_7PynyHTM_2V3_19add(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_2V3_18add, "\n        Adds the other vector to this vector.\n\n        :param other: vector to add\n        :returns: self + vector\n        ");
+static PyMethodDef __pyx_mdef_7pynyhtm_2V3_19add = {"add", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_2V3_19add, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_2V3_18add};
+static PyObject *__pyx_pw_7pynyhtm_2V3_19add(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -12226,32 +12226,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.V3.add", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.add", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_2V3_18add(__pyx_self, __pyx_v_self, __pyx_v_other);
+  __pyx_r = __pyx_pf_7pynyhtm_2V3_18add(__pyx_self, __pyx_v_self, __pyx_v_other);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_2V3_18add(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
+static PyObject *__pyx_pf_7pynyhtm_2V3_18add(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
   PyObject *__pyx_v_result = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
   Py_ssize_t __pyx_t_4;
@@ -12461,15 +12461,15 @@
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_9);
   __Pyx_XDECREF(__pyx_t_11);
-  __Pyx_AddTraceback("PynyHTM.V3.add", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.add", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -12479,23 +12479,23 @@
  * 
  *     def __add__(self, other: V3) -> V3:             # <<<<<<<<<<<<<<
  *         return self.add(other)
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_2V3_21__add__(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_2V3_21__add__(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_7PynyHTM_2V3_21__add__ = {"__add__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_2V3_21__add__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_7PynyHTM_2V3_21__add__(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_7pynyhtm_2V3_21__add__ = {"__add__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_2V3_21__add__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7pynyhtm_2V3_21__add__(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -12572,32 +12572,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.V3.__add__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.__add__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_2V3_20__add__(__pyx_self, __pyx_v_self, __pyx_v_other);
+  __pyx_r = __pyx_pf_7pynyhtm_2V3_20__add__(__pyx_self, __pyx_v_self, __pyx_v_other);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_2V3_20__add__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
+static PyObject *__pyx_pf_7pynyhtm_2V3_20__add__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
@@ -12650,15 +12650,15 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("PynyHTM.V3.__add__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.__add__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -12667,24 +12667,24 @@
  * 
  *     def sub(self, other: V3) -> V3:             # <<<<<<<<<<<<<<
  *         """
  *         Subtracts other from this vector.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_2V3_23sub(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_2V3_23sub(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_2V3_22sub, "\n        Subtracts other from this vector.\n\n        :param other: vector to subtract\n        :returns: self - vector\n        ");
-static PyMethodDef __pyx_mdef_7PynyHTM_2V3_23sub = {"sub", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_2V3_23sub, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_2V3_22sub};
-static PyObject *__pyx_pw_7PynyHTM_2V3_23sub(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_2V3_22sub, "\n        Subtracts other from this vector.\n\n        :param other: vector to subtract\n        :returns: self - vector\n        ");
+static PyMethodDef __pyx_mdef_7pynyhtm_2V3_23sub = {"sub", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_2V3_23sub, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_2V3_22sub};
+static PyObject *__pyx_pw_7pynyhtm_2V3_23sub(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -12761,32 +12761,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.V3.sub", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.sub", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_2V3_22sub(__pyx_self, __pyx_v_self, __pyx_v_other);
+  __pyx_r = __pyx_pf_7pynyhtm_2V3_22sub(__pyx_self, __pyx_v_self, __pyx_v_other);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_2V3_22sub(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
+static PyObject *__pyx_pf_7pynyhtm_2V3_22sub(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
   PyObject *__pyx_v_result = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
   Py_ssize_t __pyx_t_4;
@@ -12996,15 +12996,15 @@
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_9);
   __Pyx_XDECREF(__pyx_t_11);
-  __Pyx_AddTraceback("PynyHTM.V3.sub", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.sub", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -13014,23 +13014,23 @@
  * 
  *     def __sub__(self, other: V3) -> V3:             # <<<<<<<<<<<<<<
  *         return self.sub(other)
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_2V3_25__sub__(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_2V3_25__sub__(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_7PynyHTM_2V3_25__sub__ = {"__sub__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_2V3_25__sub__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_7PynyHTM_2V3_25__sub__(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_7pynyhtm_2V3_25__sub__ = {"__sub__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_2V3_25__sub__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7pynyhtm_2V3_25__sub__(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -13107,32 +13107,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.V3.__sub__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.__sub__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_2V3_24__sub__(__pyx_self, __pyx_v_self, __pyx_v_other);
+  __pyx_r = __pyx_pf_7pynyhtm_2V3_24__sub__(__pyx_self, __pyx_v_self, __pyx_v_other);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_2V3_24__sub__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
+static PyObject *__pyx_pf_7pynyhtm_2V3_24__sub__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
@@ -13185,15 +13185,15 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("PynyHTM.V3.__sub__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.__sub__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -13202,24 +13202,24 @@
  * 
  *     def neg(self) -> V3:             # <<<<<<<<<<<<<<
  *         """
  *         Negates this vector.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_2V3_27neg(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_2V3_27neg(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_2V3_26neg, "\n        Negates this vector.\n\n        :returns: vector with inverted components\n        ");
-static PyMethodDef __pyx_mdef_7PynyHTM_2V3_27neg = {"neg", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_2V3_27neg, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_2V3_26neg};
-static PyObject *__pyx_pw_7PynyHTM_2V3_27neg(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_2V3_26neg, "\n        Negates this vector.\n\n        :returns: vector with inverted components\n        ");
+static PyMethodDef __pyx_mdef_7pynyhtm_2V3_27neg = {"neg", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_2V3_27neg, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_2V3_26neg};
+static PyObject *__pyx_pw_7pynyhtm_2V3_27neg(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -13281,32 +13281,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.V3.neg", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.neg", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_2V3_26neg(__pyx_self, __pyx_v_self);
+  __pyx_r = __pyx_pf_7pynyhtm_2V3_26neg(__pyx_self, __pyx_v_self);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_2V3_26neg(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pf_7pynyhtm_2V3_26neg(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_v_result = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
@@ -13426,15 +13426,15 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("PynyHTM.V3.neg", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.neg", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -13444,23 +13444,23 @@
  * 
  *     def __neg__(self) -> V3:             # <<<<<<<<<<<<<<
  *         return self.neg()
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_2V3_29__neg__(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_2V3_29__neg__(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_7PynyHTM_2V3_29__neg__ = {"__neg__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_2V3_29__neg__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_7PynyHTM_2V3_29__neg__(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_7pynyhtm_2V3_29__neg__ = {"__neg__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_2V3_29__neg__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7pynyhtm_2V3_29__neg__(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -13522,32 +13522,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.V3.__neg__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.__neg__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_2V3_28__neg__(__pyx_self, __pyx_v_self);
+  __pyx_r = __pyx_pf_7pynyhtm_2V3_28__neg__(__pyx_self, __pyx_v_self);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_2V3_28__neg__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pf_7pynyhtm_2V3_28__neg__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
@@ -13600,15 +13600,15 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("PynyHTM.V3.__neg__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.__neg__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -13617,24 +13617,24 @@
  * 
  *     def mul(self, scalar: float) -> V3:             # <<<<<<<<<<<<<<
  *         """
  *         Scalar multiplication with this v3.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_2V3_31mul(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_2V3_31mul(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_2V3_30mul, "\n        Scalar multiplication with this v3.\n\n        :param scalar: scalar\n        :returns: self * scalar\n        ");
-static PyMethodDef __pyx_mdef_7PynyHTM_2V3_31mul = {"mul", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_2V3_31mul, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_2V3_30mul};
-static PyObject *__pyx_pw_7PynyHTM_2V3_31mul(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_2V3_30mul, "\n        Scalar multiplication with this v3.\n\n        :param scalar: scalar\n        :returns: self * scalar\n        ");
+static PyMethodDef __pyx_mdef_7pynyhtm_2V3_31mul = {"mul", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_2V3_31mul, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_2V3_30mul};
+static PyObject *__pyx_pw_7pynyhtm_2V3_31mul(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -13711,32 +13711,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.V3.mul", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.mul", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_2V3_30mul(__pyx_self, __pyx_v_self, __pyx_v_scalar);
+  __pyx_r = __pyx_pf_7pynyhtm_2V3_30mul(__pyx_self, __pyx_v_self, __pyx_v_scalar);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_2V3_30mul(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, double __pyx_v_scalar) {
+static PyObject *__pyx_pf_7pynyhtm_2V3_30mul(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, double __pyx_v_scalar) {
   PyObject *__pyx_v_result = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
@@ -13906,15 +13906,15 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_AddTraceback("PynyHTM.V3.mul", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.mul", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -13924,23 +13924,23 @@
  * 
  *     def __mul__(self, scalar: float) -> V3:             # <<<<<<<<<<<<<<
  *         return self.mul(scalar)
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_2V3_33__mul__(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_2V3_33__mul__(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_7PynyHTM_2V3_33__mul__ = {"__mul__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_2V3_33__mul__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_7PynyHTM_2V3_33__mul__(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_7pynyhtm_2V3_33__mul__ = {"__mul__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_2V3_33__mul__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7pynyhtm_2V3_33__mul__(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -14017,32 +14017,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.V3.__mul__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.__mul__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_2V3_32__mul__(__pyx_self, __pyx_v_self, __pyx_v_scalar);
+  __pyx_r = __pyx_pf_7pynyhtm_2V3_32__mul__(__pyx_self, __pyx_v_self, __pyx_v_scalar);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_2V3_32__mul__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, double __pyx_v_scalar) {
+static PyObject *__pyx_pf_7pynyhtm_2V3_32__mul__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, double __pyx_v_scalar) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
@@ -14100,15 +14100,15 @@
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("PynyHTM.V3.__mul__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.__mul__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -14117,24 +14117,24 @@
  * 
  *     def div(self, scalar: float) -> V3:             # <<<<<<<<<<<<<<
  *         """
  *         Scalar division with this v3.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_2V3_35div(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_2V3_35div(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_2V3_34div, "\n        Scalar division with this v3.\n\n        :param scalar: scalar divisor\n        :returns: self / scalar\n        ");
-static PyMethodDef __pyx_mdef_7PynyHTM_2V3_35div = {"div", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_2V3_35div, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_2V3_34div};
-static PyObject *__pyx_pw_7PynyHTM_2V3_35div(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_2V3_34div, "\n        Scalar division with this v3.\n\n        :param scalar: scalar divisor\n        :returns: self / scalar\n        ");
+static PyMethodDef __pyx_mdef_7pynyhtm_2V3_35div = {"div", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_2V3_35div, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_2V3_34div};
+static PyObject *__pyx_pw_7pynyhtm_2V3_35div(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -14211,32 +14211,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.V3.div", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.div", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_2V3_34div(__pyx_self, __pyx_v_self, __pyx_v_scalar);
+  __pyx_r = __pyx_pf_7pynyhtm_2V3_34div(__pyx_self, __pyx_v_self, __pyx_v_scalar);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_2V3_34div(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, double __pyx_v_scalar) {
+static PyObject *__pyx_pf_7pynyhtm_2V3_34div(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, double __pyx_v_scalar) {
   PyObject *__pyx_v_result = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
@@ -14447,15 +14447,15 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_AddTraceback("PynyHTM.V3.div", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.div", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -14465,23 +14465,23 @@
  * 
  *     def __truediv__(self, scalar: float) -> V3:             # <<<<<<<<<<<<<<
  *         return self.div(scalar)
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_2V3_37__truediv__(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_2V3_37__truediv__(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_7PynyHTM_2V3_37__truediv__ = {"__truediv__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_2V3_37__truediv__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_7PynyHTM_2V3_37__truediv__(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_7pynyhtm_2V3_37__truediv__ = {"__truediv__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_2V3_37__truediv__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7pynyhtm_2V3_37__truediv__(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -14558,32 +14558,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.V3.__truediv__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.__truediv__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_2V3_36__truediv__(__pyx_self, __pyx_v_self, __pyx_v_scalar);
+  __pyx_r = __pyx_pf_7pynyhtm_2V3_36__truediv__(__pyx_self, __pyx_v_self, __pyx_v_scalar);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_2V3_36__truediv__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, double __pyx_v_scalar) {
+static PyObject *__pyx_pf_7pynyhtm_2V3_36__truediv__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, double __pyx_v_scalar) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
@@ -14641,15 +14641,15 @@
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("PynyHTM.V3.__truediv__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.V3.__truediv__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -14658,24 +14658,24 @@
  * 
  * def htm_sc_init_raw(latitude: float, longitude: float) -> tuple[htm_errcode, htm_sc]:             # <<<<<<<<<<<<<<
  *     """
  *     Wraps htm_sc_init, instantiates a htm_sc struct.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_3htm_sc_init_raw(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_3htm_sc_init_raw(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_2htm_sc_init_raw, "\n    Wraps htm_sc_init, instantiates a htm_sc struct.\n\n    :param latitude: latitude of the new struct\n    :param longitude: longitude of the new struct\n    :returns: tuple containing the htm_errcode and htm_sc struct\n    ");
-static PyMethodDef __pyx_mdef_7PynyHTM_3htm_sc_init_raw = {"htm_sc_init_raw", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_3htm_sc_init_raw, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_2htm_sc_init_raw};
-static PyObject *__pyx_pw_7PynyHTM_3htm_sc_init_raw(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_2htm_sc_init_raw, "\n    Wraps htm_sc_init, instantiates a htm_sc struct.\n\n    :param latitude: latitude of the new struct\n    :param longitude: longitude of the new struct\n    :returns: tuple containing the htm_errcode and htm_sc struct\n    ");
+static PyMethodDef __pyx_mdef_7pynyhtm_3htm_sc_init_raw = {"htm_sc_init_raw", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_3htm_sc_init_raw, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_2htm_sc_init_raw};
+static PyObject *__pyx_pw_7pynyhtm_3htm_sc_init_raw(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   double __pyx_v_latitude;
@@ -14752,32 +14752,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.htm_sc_init_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.htm_sc_init_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_2htm_sc_init_raw(__pyx_self, __pyx_v_latitude, __pyx_v_longitude);
+  __pyx_r = __pyx_pf_7pynyhtm_2htm_sc_init_raw(__pyx_self, __pyx_v_latitude, __pyx_v_longitude);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_2htm_sc_init_raw(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_latitude, double __pyx_v_longitude) {
+static PyObject *__pyx_pf_7pynyhtm_2htm_sc_init_raw(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_latitude, double __pyx_v_longitude) {
   struct htm_sc __pyx_v_out;
   htm_errcode __pyx_v_err_code;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
@@ -14828,15 +14828,15 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("PynyHTM.htm_sc_init_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.htm_sc_init_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -14845,24 +14845,24 @@
  * 
  * def htm_sc_init_wrapped(latitude: float, longitude: float) -> SphericalCoordinate:             # <<<<<<<<<<<<<<
  *     """
  *     Wraps htm_sc_init, instantiates a wrapped htm_sc struct with given latitude and longitude.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_5htm_sc_init_wrapped(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_5htm_sc_init_wrapped(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_4htm_sc_init_wrapped, "\n    Wraps htm_sc_init, instantiates a wrapped htm_sc struct with given latitude and longitude.\n\n    :param latitude: latitude of the new struct\n    :param longitude: longitude of the new struct\n    :returns: wrapped htm_sc struct as SphericalCoordinate object\n    :raises valueError: if struct instantiation failed\n    ");
-static PyMethodDef __pyx_mdef_7PynyHTM_5htm_sc_init_wrapped = {"htm_sc_init_wrapped", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_5htm_sc_init_wrapped, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_4htm_sc_init_wrapped};
-static PyObject *__pyx_pw_7PynyHTM_5htm_sc_init_wrapped(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_4htm_sc_init_wrapped, "\n    Wraps htm_sc_init, instantiates a wrapped htm_sc struct with given latitude and longitude.\n\n    :param latitude: latitude of the new struct\n    :param longitude: longitude of the new struct\n    :returns: wrapped htm_sc struct as SphericalCoordinate object\n    :raises valueError: if struct instantiation failed\n    ");
+static PyMethodDef __pyx_mdef_7pynyhtm_5htm_sc_init_wrapped = {"htm_sc_init_wrapped", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_5htm_sc_init_wrapped, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_4htm_sc_init_wrapped};
+static PyObject *__pyx_pw_7pynyhtm_5htm_sc_init_wrapped(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   double __pyx_v_latitude;
@@ -14939,32 +14939,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.htm_sc_init_wrapped", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.htm_sc_init_wrapped", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_4htm_sc_init_wrapped(__pyx_self, __pyx_v_latitude, __pyx_v_longitude);
+  __pyx_r = __pyx_pf_7pynyhtm_4htm_sc_init_wrapped(__pyx_self, __pyx_v_latitude, __pyx_v_longitude);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_4htm_sc_init_wrapped(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_latitude, double __pyx_v_longitude) {
+static PyObject *__pyx_pf_7pynyhtm_4htm_sc_init_wrapped(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_latitude, double __pyx_v_longitude) {
   PyObject *__pyx_v_ec = NULL;
   PyObject *__pyx_v_sc = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
@@ -15171,15 +15171,15 @@
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("PynyHTM.htm_sc_init_wrapped", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.htm_sc_init_wrapped", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_ec);
   __Pyx_XDECREF(__pyx_v_sc);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
@@ -15190,24 +15190,24 @@
  * 
  * def htm_sc_angsep_raw(sc1: htm_sc, sc2: htm_sc) -> float:             # <<<<<<<<<<<<<<
  *     """
  *     Determine the angle difference between the two given spherical coordinates.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_7htm_sc_angsep_raw(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_7htm_sc_angsep_raw(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_6htm_sc_angsep_raw, "\n    Determine the angle difference between the two given spherical coordinates.\n\n    :param sc1: first position\n    :param sc2: second position\n    :returns: angle between sc1 and sc2\n    ");
-static PyMethodDef __pyx_mdef_7PynyHTM_7htm_sc_angsep_raw = {"htm_sc_angsep_raw", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_7htm_sc_angsep_raw, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_6htm_sc_angsep_raw};
-static PyObject *__pyx_pw_7PynyHTM_7htm_sc_angsep_raw(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_6htm_sc_angsep_raw, "\n    Determine the angle difference between the two given spherical coordinates.\n\n    :param sc1: first position\n    :param sc2: second position\n    :returns: angle between sc1 and sc2\n    ");
+static PyMethodDef __pyx_mdef_7pynyhtm_7htm_sc_angsep_raw = {"htm_sc_angsep_raw", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_7htm_sc_angsep_raw, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_6htm_sc_angsep_raw};
+static PyObject *__pyx_pw_7pynyhtm_7htm_sc_angsep_raw(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   struct htm_sc __pyx_v_sc1;
@@ -15284,32 +15284,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.htm_sc_angsep_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.htm_sc_angsep_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_6htm_sc_angsep_raw(__pyx_self, __pyx_v_sc1, __pyx_v_sc2);
+  __pyx_r = __pyx_pf_7pynyhtm_6htm_sc_angsep_raw(__pyx_self, __pyx_v_sc1, __pyx_v_sc2);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_6htm_sc_angsep_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_sc __pyx_v_sc1, struct htm_sc __pyx_v_sc2) {
+static PyObject *__pyx_pf_7pynyhtm_6htm_sc_angsep_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_sc __pyx_v_sc1, struct htm_sc __pyx_v_sc2) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("htm_sc_angsep_raw", 1);
@@ -15335,15 +15335,15 @@
  *     """
  *     Determine the angle difference between the two given spherical coordinates.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("PynyHTM.htm_sc_angsep_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.htm_sc_angsep_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -15352,24 +15352,24 @@
  * 
  * def htm_v3_init_raw(x: float, y: float, z: float) -> tuple[htm_errcode, htm_v3]:             # <<<<<<<<<<<<<<
  *     """
  *     Wraps htm_v3_init, instantiates a htm_v3 struct.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_9htm_v3_init_raw(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_9htm_v3_init_raw(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_8htm_v3_init_raw, "\n    Wraps htm_v3_init, instantiates a htm_v3 struct.\n\n    :param x: x (first) value of the new struct\n    :param y: y (second) value of the new struct\n    :param z: z (third) value of the new struct\n    :returns: tuple containing the htm_errcode and htm_v3 struct\n    ");
-static PyMethodDef __pyx_mdef_7PynyHTM_9htm_v3_init_raw = {"htm_v3_init_raw", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_9htm_v3_init_raw, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_8htm_v3_init_raw};
-static PyObject *__pyx_pw_7PynyHTM_9htm_v3_init_raw(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_8htm_v3_init_raw, "\n    Wraps htm_v3_init, instantiates a htm_v3 struct.\n\n    :param x: x (first) value of the new struct\n    :param y: y (second) value of the new struct\n    :param z: z (third) value of the new struct\n    :returns: tuple containing the htm_errcode and htm_v3 struct\n    ");
+static PyMethodDef __pyx_mdef_7pynyhtm_9htm_v3_init_raw = {"htm_v3_init_raw", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_9htm_v3_init_raw, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_8htm_v3_init_raw};
+static PyObject *__pyx_pw_7pynyhtm_9htm_v3_init_raw(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   double __pyx_v_x;
@@ -15461,32 +15461,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.htm_v3_init_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.htm_v3_init_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_8htm_v3_init_raw(__pyx_self, __pyx_v_x, __pyx_v_y, __pyx_v_z);
+  __pyx_r = __pyx_pf_7pynyhtm_8htm_v3_init_raw(__pyx_self, __pyx_v_x, __pyx_v_y, __pyx_v_z);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_8htm_v3_init_raw(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_x, double __pyx_v_y, double __pyx_v_z) {
+static PyObject *__pyx_pf_7pynyhtm_8htm_v3_init_raw(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_x, double __pyx_v_y, double __pyx_v_z) {
   struct htm_v3 __pyx_v_out;
   htm_errcode __pyx_v_err_code;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
@@ -15537,15 +15537,15 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("PynyHTM.htm_v3_init_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.htm_v3_init_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -15554,24 +15554,24 @@
  * 
  * def htm_v3_init_wrapped(x: float, y: float, z: float) -> V3:             # <<<<<<<<<<<<<<
  *     """
  *     Wraps htm_v3_init, instantiates a wrapped htm_v3 struct with given x,y,z.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_11htm_v3_init_wrapped(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_11htm_v3_init_wrapped(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_10htm_v3_init_wrapped, "\n    Wraps htm_v3_init, instantiates a wrapped htm_v3 struct with given x,y,z.\n\n    :param x: x (first) value of the new struct\n    :param y: y (second) value of the new struct\n    :param z: z (third) value of the new struct\n    :returns: tuple containing the wrapped error code and wrapped htm_v3 struct\n    :raises valueError: if struct instantiation failed\n    ");
-static PyMethodDef __pyx_mdef_7PynyHTM_11htm_v3_init_wrapped = {"htm_v3_init_wrapped", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_11htm_v3_init_wrapped, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_10htm_v3_init_wrapped};
-static PyObject *__pyx_pw_7PynyHTM_11htm_v3_init_wrapped(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_10htm_v3_init_wrapped, "\n    Wraps htm_v3_init, instantiates a wrapped htm_v3 struct with given x,y,z.\n\n    :param x: x (first) value of the new struct\n    :param y: y (second) value of the new struct\n    :param z: z (third) value of the new struct\n    :returns: tuple containing the wrapped error code and wrapped htm_v3 struct\n    :raises valueError: if struct instantiation failed\n    ");
+static PyMethodDef __pyx_mdef_7pynyhtm_11htm_v3_init_wrapped = {"htm_v3_init_wrapped", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_11htm_v3_init_wrapped, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_10htm_v3_init_wrapped};
+static PyObject *__pyx_pw_7pynyhtm_11htm_v3_init_wrapped(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   double __pyx_v_x;
@@ -15663,32 +15663,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.htm_v3_init_wrapped", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.htm_v3_init_wrapped", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_10htm_v3_init_wrapped(__pyx_self, __pyx_v_x, __pyx_v_y, __pyx_v_z);
+  __pyx_r = __pyx_pf_7pynyhtm_10htm_v3_init_wrapped(__pyx_self, __pyx_v_x, __pyx_v_y, __pyx_v_z);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_10htm_v3_init_wrapped(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_x, double __pyx_v_y, double __pyx_v_z) {
+static PyObject *__pyx_pf_7pynyhtm_10htm_v3_init_wrapped(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_x, double __pyx_v_y, double __pyx_v_z) {
   PyObject *__pyx_v_ec = NULL;
   PyObject *__pyx_v_v3 = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
@@ -15916,15 +15916,15 @@
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("PynyHTM.htm_v3_init_wrapped", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.htm_v3_init_wrapped", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_ec);
   __Pyx_XDECREF(__pyx_v_v3);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
@@ -15935,24 +15935,24 @@
  * 
  * def htm_sc_to_v3_raw(sc: htm_sc) -> tuple[htm_errcode, htm_v3]:             # <<<<<<<<<<<<<<
  *     """
  *     Wraps htm_sc_tov3, transforms a htm_sc struct into a htm_v3 struct.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_13htm_sc_to_v3_raw(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_13htm_sc_to_v3_raw(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_12htm_sc_to_v3_raw, "\n    Wraps htm_sc_tov3, transforms a htm_sc struct into a htm_v3 struct.\n\n    :param sc: htm_sc struct with latitude and longitude\n    :returns: tuple containing the htm_errorcode and htm_v3 struct\n    ");
-static PyMethodDef __pyx_mdef_7PynyHTM_13htm_sc_to_v3_raw = {"htm_sc_to_v3_raw", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_13htm_sc_to_v3_raw, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_12htm_sc_to_v3_raw};
-static PyObject *__pyx_pw_7PynyHTM_13htm_sc_to_v3_raw(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_12htm_sc_to_v3_raw, "\n    Wraps htm_sc_tov3, transforms a htm_sc struct into a htm_v3 struct.\n\n    :param sc: htm_sc struct with latitude and longitude\n    :returns: tuple containing the htm_errorcode and htm_v3 struct\n    ");
+static PyMethodDef __pyx_mdef_7pynyhtm_13htm_sc_to_v3_raw = {"htm_sc_to_v3_raw", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_13htm_sc_to_v3_raw, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_12htm_sc_to_v3_raw};
+static PyObject *__pyx_pw_7pynyhtm_13htm_sc_to_v3_raw(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   struct htm_sc __pyx_v_sc;
@@ -16014,32 +16014,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.htm_sc_to_v3_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.htm_sc_to_v3_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_12htm_sc_to_v3_raw(__pyx_self, __pyx_v_sc);
+  __pyx_r = __pyx_pf_7pynyhtm_12htm_sc_to_v3_raw(__pyx_self, __pyx_v_sc);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_12htm_sc_to_v3_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_sc __pyx_v_sc) {
+static PyObject *__pyx_pf_7pynyhtm_12htm_sc_to_v3_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_sc __pyx_v_sc) {
   struct htm_v3 __pyx_v_out;
   htm_errcode __pyx_v_err_code;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
@@ -16090,15 +16090,15 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("PynyHTM.htm_sc_to_v3_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.htm_sc_to_v3_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -16107,24 +16107,24 @@
  * 
  * def htm_v3_to_sc_raw(v3: htm_v3) -> tuple[htm_errcode, htm_sc]:             # <<<<<<<<<<<<<<
  *     """
  *     Wraps htm_v3_tosc, transforms a htm_v3 struct into a htm_sc struct.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_15htm_v3_to_sc_raw(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_15htm_v3_to_sc_raw(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_14htm_v3_to_sc_raw, "\n    Wraps htm_v3_tosc, transforms a htm_v3 struct into a htm_sc struct.\n\n    :param v3: htm_v3 struct with x,y,z\n    :returns: tuple containing the htm_errorcode and htm_sc struct\n    ");
-static PyMethodDef __pyx_mdef_7PynyHTM_15htm_v3_to_sc_raw = {"htm_v3_to_sc_raw", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_15htm_v3_to_sc_raw, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_14htm_v3_to_sc_raw};
-static PyObject *__pyx_pw_7PynyHTM_15htm_v3_to_sc_raw(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_14htm_v3_to_sc_raw, "\n    Wraps htm_v3_tosc, transforms a htm_v3 struct into a htm_sc struct.\n\n    :param v3: htm_v3 struct with x,y,z\n    :returns: tuple containing the htm_errorcode and htm_sc struct\n    ");
+static PyMethodDef __pyx_mdef_7pynyhtm_15htm_v3_to_sc_raw = {"htm_v3_to_sc_raw", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_15htm_v3_to_sc_raw, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_14htm_v3_to_sc_raw};
+static PyObject *__pyx_pw_7pynyhtm_15htm_v3_to_sc_raw(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   struct htm_v3 __pyx_v_v3;
@@ -16186,32 +16186,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.htm_v3_to_sc_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.htm_v3_to_sc_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_14htm_v3_to_sc_raw(__pyx_self, __pyx_v_v3);
+  __pyx_r = __pyx_pf_7pynyhtm_14htm_v3_to_sc_raw(__pyx_self, __pyx_v_v3);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_14htm_v3_to_sc_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_v3 __pyx_v_v3) {
+static PyObject *__pyx_pf_7pynyhtm_14htm_v3_to_sc_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_v3 __pyx_v_v3) {
   struct htm_sc __pyx_v_out;
   htm_errcode __pyx_v_err_code;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
@@ -16262,15 +16262,15 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("PynyHTM.htm_v3_to_sc_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.htm_v3_to_sc_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -16279,24 +16279,24 @@
  * 
  * def htm_v3_add_raw(v1: htm_v3, v2: htm_v3) -> htm_v3:             # <<<<<<<<<<<<<<
  *     """
  *     Adds two vectors.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_17htm_v3_add_raw(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_17htm_v3_add_raw(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_16htm_v3_add_raw, "\n    Adds two vectors.\n\n    :param v1: first vector\n    :param v2: second vector\n    :returns: sum of v1 and v2\n    ");
-static PyMethodDef __pyx_mdef_7PynyHTM_17htm_v3_add_raw = {"htm_v3_add_raw", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_17htm_v3_add_raw, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_16htm_v3_add_raw};
-static PyObject *__pyx_pw_7PynyHTM_17htm_v3_add_raw(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_16htm_v3_add_raw, "\n    Adds two vectors.\n\n    :param v1: first vector\n    :param v2: second vector\n    :returns: sum of v1 and v2\n    ");
+static PyMethodDef __pyx_mdef_7pynyhtm_17htm_v3_add_raw = {"htm_v3_add_raw", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_17htm_v3_add_raw, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_16htm_v3_add_raw};
+static PyObject *__pyx_pw_7pynyhtm_17htm_v3_add_raw(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   struct htm_v3 __pyx_v_v1;
@@ -16373,32 +16373,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.htm_v3_add_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.htm_v3_add_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_16htm_v3_add_raw(__pyx_self, __pyx_v_v1, __pyx_v_v2);
+  __pyx_r = __pyx_pf_7pynyhtm_16htm_v3_add_raw(__pyx_self, __pyx_v_v1, __pyx_v_v2);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_16htm_v3_add_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_v3 __pyx_v_v1, struct htm_v3 __pyx_v_v2) {
+static PyObject *__pyx_pf_7pynyhtm_16htm_v3_add_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_v3 __pyx_v_v1, struct htm_v3 __pyx_v_v2) {
   struct htm_v3 __pyx_v_out;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -16434,15 +16434,15 @@
  *     """
  *     Adds two vectors.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("PynyHTM.htm_v3_add_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.htm_v3_add_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -16451,24 +16451,24 @@
  * 
  * def htm_v3_sub_raw(v1: htm_v3, v2: htm_v3) -> htm_v3:             # <<<<<<<<<<<<<<
  *     """
  *     Subtracts two vectors.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_19htm_v3_sub_raw(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_19htm_v3_sub_raw(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_18htm_v3_sub_raw, "\n    Subtracts two vectors.\n\n    :param v1: first vector\n    :param v2: second vector\n    :returns:  v1 - v2\n    ");
-static PyMethodDef __pyx_mdef_7PynyHTM_19htm_v3_sub_raw = {"htm_v3_sub_raw", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_19htm_v3_sub_raw, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_18htm_v3_sub_raw};
-static PyObject *__pyx_pw_7PynyHTM_19htm_v3_sub_raw(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_18htm_v3_sub_raw, "\n    Subtracts two vectors.\n\n    :param v1: first vector\n    :param v2: second vector\n    :returns:  v1 - v2\n    ");
+static PyMethodDef __pyx_mdef_7pynyhtm_19htm_v3_sub_raw = {"htm_v3_sub_raw", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_19htm_v3_sub_raw, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_18htm_v3_sub_raw};
+static PyObject *__pyx_pw_7pynyhtm_19htm_v3_sub_raw(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   struct htm_v3 __pyx_v_v1;
@@ -16545,32 +16545,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.htm_v3_sub_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.htm_v3_sub_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_18htm_v3_sub_raw(__pyx_self, __pyx_v_v1, __pyx_v_v2);
+  __pyx_r = __pyx_pf_7pynyhtm_18htm_v3_sub_raw(__pyx_self, __pyx_v_v1, __pyx_v_v2);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_18htm_v3_sub_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_v3 __pyx_v_v1, struct htm_v3 __pyx_v_v2) {
+static PyObject *__pyx_pf_7pynyhtm_18htm_v3_sub_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_v3 __pyx_v_v1, struct htm_v3 __pyx_v_v2) {
   struct htm_v3 __pyx_v_out;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -16606,15 +16606,15 @@
  *     """
  *     Subtracts two vectors.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("PynyHTM.htm_v3_sub_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.htm_v3_sub_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -16623,24 +16623,24 @@
  * 
  * def htm_v3_neg_raw(v1: htm_v3) -> htm_v3:             # <<<<<<<<<<<<<<
  *     """
  *     Negates the given vector.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_21htm_v3_neg_raw(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_21htm_v3_neg_raw(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_20htm_v3_neg_raw, "\n    Negates the given vector.\n\n    :param v1: first vector\n    :returns:  v1 - v2\n    ");
-static PyMethodDef __pyx_mdef_7PynyHTM_21htm_v3_neg_raw = {"htm_v3_neg_raw", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_21htm_v3_neg_raw, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_20htm_v3_neg_raw};
-static PyObject *__pyx_pw_7PynyHTM_21htm_v3_neg_raw(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_20htm_v3_neg_raw, "\n    Negates the given vector.\n\n    :param v1: first vector\n    :returns:  v1 - v2\n    ");
+static PyMethodDef __pyx_mdef_7pynyhtm_21htm_v3_neg_raw = {"htm_v3_neg_raw", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_21htm_v3_neg_raw, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_20htm_v3_neg_raw};
+static PyObject *__pyx_pw_7pynyhtm_21htm_v3_neg_raw(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   struct htm_v3 __pyx_v_v1;
@@ -16702,32 +16702,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.htm_v3_neg_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.htm_v3_neg_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_20htm_v3_neg_raw(__pyx_self, __pyx_v_v1);
+  __pyx_r = __pyx_pf_7pynyhtm_20htm_v3_neg_raw(__pyx_self, __pyx_v_v1);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_20htm_v3_neg_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_v3 __pyx_v_v1) {
+static PyObject *__pyx_pf_7pynyhtm_20htm_v3_neg_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_v3 __pyx_v_v1) {
   struct htm_v3 __pyx_v_out;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -16763,15 +16763,15 @@
  *     """
  *     Negates the given vector.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("PynyHTM.htm_v3_neg_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.htm_v3_neg_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -16780,24 +16780,24 @@
  * 
  * def htm_v3_mul_raw(v1: htm_v3, scalar: float) -> htm_v3:             # <<<<<<<<<<<<<<
  *     """
  *     Scalar vector multiplication.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_23htm_v3_mul_raw(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_23htm_v3_mul_raw(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_22htm_v3_mul_raw, "\n    Scalar vector multiplication.\n\n    :param v1: first vector\n    :param scalar: scalar multiplier\n    :returns:  v1 * scalar\n    ");
-static PyMethodDef __pyx_mdef_7PynyHTM_23htm_v3_mul_raw = {"htm_v3_mul_raw", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_23htm_v3_mul_raw, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_22htm_v3_mul_raw};
-static PyObject *__pyx_pw_7PynyHTM_23htm_v3_mul_raw(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_22htm_v3_mul_raw, "\n    Scalar vector multiplication.\n\n    :param v1: first vector\n    :param scalar: scalar multiplier\n    :returns:  v1 * scalar\n    ");
+static PyMethodDef __pyx_mdef_7pynyhtm_23htm_v3_mul_raw = {"htm_v3_mul_raw", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_23htm_v3_mul_raw, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_22htm_v3_mul_raw};
+static PyObject *__pyx_pw_7pynyhtm_23htm_v3_mul_raw(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   struct htm_v3 __pyx_v_v1;
@@ -16874,32 +16874,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.htm_v3_mul_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.htm_v3_mul_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_22htm_v3_mul_raw(__pyx_self, __pyx_v_v1, __pyx_v_scalar);
+  __pyx_r = __pyx_pf_7pynyhtm_22htm_v3_mul_raw(__pyx_self, __pyx_v_v1, __pyx_v_scalar);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_22htm_v3_mul_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_v3 __pyx_v_v1, double __pyx_v_scalar) {
+static PyObject *__pyx_pf_7pynyhtm_22htm_v3_mul_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_v3 __pyx_v_v1, double __pyx_v_scalar) {
   struct htm_v3 __pyx_v_out;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -16935,15 +16935,15 @@
  *     """
  *     Scalar vector multiplication.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("PynyHTM.htm_v3_mul_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.htm_v3_mul_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -16952,24 +16952,24 @@
  * 
  * def htm_v3_div_raw(v1: htm_v3, scalar: float) -> htm_v3:             # <<<<<<<<<<<<<<
  *     """
  *     Scalar vector division.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_25htm_v3_div_raw(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_25htm_v3_div_raw(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_24htm_v3_div_raw, "\n    Scalar vector division.\n\n    :param v1: first vector\n    :param scalar: scalar divisor\n    :returns:  v1 / divisor\n    ");
-static PyMethodDef __pyx_mdef_7PynyHTM_25htm_v3_div_raw = {"htm_v3_div_raw", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_25htm_v3_div_raw, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_24htm_v3_div_raw};
-static PyObject *__pyx_pw_7PynyHTM_25htm_v3_div_raw(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_24htm_v3_div_raw, "\n    Scalar vector division.\n\n    :param v1: first vector\n    :param scalar: scalar divisor\n    :returns:  v1 / divisor\n    ");
+static PyMethodDef __pyx_mdef_7pynyhtm_25htm_v3_div_raw = {"htm_v3_div_raw", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_25htm_v3_div_raw, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_24htm_v3_div_raw};
+static PyObject *__pyx_pw_7pynyhtm_25htm_v3_div_raw(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   struct htm_v3 __pyx_v_v1;
@@ -17046,32 +17046,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.htm_v3_div_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.htm_v3_div_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_24htm_v3_div_raw(__pyx_self, __pyx_v_v1, __pyx_v_scalar);
+  __pyx_r = __pyx_pf_7pynyhtm_24htm_v3_div_raw(__pyx_self, __pyx_v_v1, __pyx_v_scalar);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_24htm_v3_div_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_v3 __pyx_v_v1, double __pyx_v_scalar) {
+static PyObject *__pyx_pf_7pynyhtm_24htm_v3_div_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_v3 __pyx_v_v1, double __pyx_v_scalar) {
   struct htm_v3 __pyx_v_out;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
@@ -17151,15 +17151,15 @@
  *     Scalar vector division.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("PynyHTM.htm_v3_div_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.htm_v3_div_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -17168,24 +17168,24 @@
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def vertices(self) -> V3[3]:
  *         """Vertices making up this triangle."""
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_8Triangle_1vertices(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_8Triangle_1vertices(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_8Triangle_vertices, "Vertices making up this triangle.");
-static PyMethodDef __pyx_mdef_7PynyHTM_8Triangle_1vertices = {"vertices", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_8Triangle_1vertices, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_8Triangle_vertices};
-static PyObject *__pyx_pw_7PynyHTM_8Triangle_1vertices(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_8Triangle_vertices, "Vertices making up this triangle.");
+static PyMethodDef __pyx_mdef_7pynyhtm_8Triangle_1vertices = {"vertices", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_8Triangle_1vertices, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_8Triangle_vertices};
+static PyObject *__pyx_pw_7pynyhtm_8Triangle_1vertices(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -17247,32 +17247,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.Triangle.vertices", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.Triangle.vertices", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_8Triangle_vertices(__pyx_self, __pyx_v_self);
+  __pyx_r = __pyx_pf_7pynyhtm_8Triangle_vertices(__pyx_self, __pyx_v_self);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_8Triangle_vertices(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pf_7pynyhtm_8Triangle_vertices(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("vertices", 1);
@@ -17298,15 +17298,15 @@
  *     def vertices(self) -> V3[3]:
  *         """Vertices making up this triangle."""
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("PynyHTM.Triangle.vertices", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.Triangle.vertices", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -17315,24 +17315,24 @@
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def center(self) -> V3:
  *         """Center point of this triangle."""
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_8Triangle_3center(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_8Triangle_3center(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_8Triangle_2center, "Center point of this triangle.");
-static PyMethodDef __pyx_mdef_7PynyHTM_8Triangle_3center = {"center", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_8Triangle_3center, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_8Triangle_2center};
-static PyObject *__pyx_pw_7PynyHTM_8Triangle_3center(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_8Triangle_2center, "Center point of this triangle.");
+static PyMethodDef __pyx_mdef_7pynyhtm_8Triangle_3center = {"center", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_8Triangle_3center, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_8Triangle_2center};
+static PyObject *__pyx_pw_7pynyhtm_8Triangle_3center(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -17394,32 +17394,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.Triangle.center", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.Triangle.center", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_8Triangle_2center(__pyx_self, __pyx_v_self);
+  __pyx_r = __pyx_pf_7pynyhtm_8Triangle_2center(__pyx_self, __pyx_v_self);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_8Triangle_2center(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pf_7pynyhtm_8Triangle_2center(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("center", 1);
@@ -17445,15 +17445,15 @@
  *     def center(self) -> V3:
  *         """Center point of this triangle."""
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("PynyHTM.Triangle.center", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.Triangle.center", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -17462,24 +17462,24 @@
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def radius(self) -> float:
  *         """Radius of the circle given by the three corners of the triangle."""
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_8Triangle_5radius(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_8Triangle_5radius(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_8Triangle_4radius, "Radius of the circle given by the three corners of the triangle.");
-static PyMethodDef __pyx_mdef_7PynyHTM_8Triangle_5radius = {"radius", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_8Triangle_5radius, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_8Triangle_4radius};
-static PyObject *__pyx_pw_7PynyHTM_8Triangle_5radius(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_8Triangle_4radius, "Radius of the circle given by the three corners of the triangle.");
+static PyMethodDef __pyx_mdef_7pynyhtm_8Triangle_5radius = {"radius", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_8Triangle_5radius, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_8Triangle_4radius};
+static PyObject *__pyx_pw_7pynyhtm_8Triangle_5radius(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -17541,32 +17541,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.Triangle.radius", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.Triangle.radius", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_8Triangle_4radius(__pyx_self, __pyx_v_self);
+  __pyx_r = __pyx_pf_7pynyhtm_8Triangle_4radius(__pyx_self, __pyx_v_self);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_8Triangle_4radius(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pf_7pynyhtm_8Triangle_4radius(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("radius", 1);
@@ -17592,15 +17592,15 @@
  *     def radius(self) -> float:
  *         """Radius of the circle given by the three corners of the triangle."""
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("PynyHTM.Triangle.radius", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.Triangle.radius", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -17609,24 +17609,24 @@
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def id(self) -> int64_t:
  *         """HTM ID of this triangle."""
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_8Triangle_7id(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_8Triangle_7id(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_8Triangle_6id, "HTM ID of this triangle.");
-static PyMethodDef __pyx_mdef_7PynyHTM_8Triangle_7id = {"id", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_8Triangle_7id, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_8Triangle_6id};
-static PyObject *__pyx_pw_7PynyHTM_8Triangle_7id(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_8Triangle_6id, "HTM ID of this triangle.");
+static PyMethodDef __pyx_mdef_7pynyhtm_8Triangle_7id = {"id", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_8Triangle_7id, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_8Triangle_6id};
+static PyObject *__pyx_pw_7pynyhtm_8Triangle_7id(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -17688,32 +17688,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.Triangle.id", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.Triangle.id", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_8Triangle_6id(__pyx_self, __pyx_v_self);
+  __pyx_r = __pyx_pf_7pynyhtm_8Triangle_6id(__pyx_self, __pyx_v_self);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_8Triangle_6id(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pf_7pynyhtm_8Triangle_6id(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("id", 1);
@@ -17739,15 +17739,15 @@
  *     def id(self) -> int64_t:
  *         """HTM ID of this triangle."""
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("PynyHTM.Triangle.id", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.Triangle.id", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -17756,24 +17756,24 @@
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def level(self) -> int:
  *         """Level at which this triangle is within the htm."""
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_8Triangle_9level(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_8Triangle_9level(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_8Triangle_8level, "Level at which this triangle is within the htm.");
-static PyMethodDef __pyx_mdef_7PynyHTM_8Triangle_9level = {"level", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_8Triangle_9level, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_8Triangle_8level};
-static PyObject *__pyx_pw_7PynyHTM_8Triangle_9level(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_8Triangle_8level, "Level at which this triangle is within the htm.");
+static PyMethodDef __pyx_mdef_7pynyhtm_8Triangle_9level = {"level", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_8Triangle_9level, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_8Triangle_8level};
+static PyObject *__pyx_pw_7pynyhtm_8Triangle_9level(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -17835,32 +17835,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.Triangle.level", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.Triangle.level", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_8Triangle_8level(__pyx_self, __pyx_v_self);
+  __pyx_r = __pyx_pf_7pynyhtm_8Triangle_8level(__pyx_self, __pyx_v_self);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_8Triangle_8level(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pf_7pynyhtm_8Triangle_8level(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("level", 1);
@@ -17887,15 +17887,15 @@
  *     def level(self) -> int:
  *         """Level at which this triangle is within the htm."""
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("PynyHTM.Triangle.level", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.Triangle.level", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -17904,24 +17904,24 @@
  * 
  *     def __init__(self, vertices: V3[3], center: V3, radius: float, id: int, level: int) -> None:             # <<<<<<<<<<<<<<
  *         """
  *         Instantiates a triangle and with the given parameters.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_8Triangle_11__init__(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_8Triangle_11__init__(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_8Triangle_10__init__, "\n        Instantiates a triangle and with the given parameters.\n\n        :param vertices: vertices of the triangle\n        :param center: center of the triangle\n        :param radius: radius of the circle defined by the three vertices\n        :param id: htm id of the triangle\n        :param level: level at which the triangle is within the htm\n        ");
-static PyMethodDef __pyx_mdef_7PynyHTM_8Triangle_11__init__ = {"__init__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_8Triangle_11__init__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_8Triangle_10__init__};
-static PyObject *__pyx_pw_7PynyHTM_8Triangle_11__init__(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_8Triangle_10__init__, "\n        Instantiates a triangle and with the given parameters.\n\n        :param vertices: vertices of the triangle\n        :param center: center of the triangle\n        :param radius: radius of the circle defined by the three vertices\n        :param id: htm id of the triangle\n        :param level: level at which the triangle is within the htm\n        ");
+static PyMethodDef __pyx_mdef_7pynyhtm_8Triangle_11__init__ = {"__init__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_8Triangle_11__init__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_8Triangle_10__init__};
+static PyObject *__pyx_pw_7pynyhtm_8Triangle_11__init__(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -18058,21 +18058,21 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.Triangle.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.Triangle.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_id), (&PyInt_Type), 0, "id", 1))) __PYX_ERR(0, 543, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_level), (&PyInt_Type), 0, "level", 1))) __PYX_ERR(0, 543, __pyx_L1_error)
-  __pyx_r = __pyx_pf_7PynyHTM_8Triangle_10__init__(__pyx_self, __pyx_v_self, __pyx_v_vertices, __pyx_v_center, __pyx_v_radius, __pyx_v_id, __pyx_v_level);
+  __pyx_r = __pyx_pf_7pynyhtm_8Triangle_10__init__(__pyx_self, __pyx_v_self, __pyx_v_vertices, __pyx_v_center, __pyx_v_radius, __pyx_v_id, __pyx_v_level);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   {
@@ -18081,15 +18081,15 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_8Triangle_10__init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_vertices, PyObject *__pyx_v_center, double __pyx_v_radius, PyObject *__pyx_v_id, PyObject *__pyx_v_level) {
+static PyObject *__pyx_pf_7pynyhtm_8Triangle_10__init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_vertices, PyObject *__pyx_v_center, double __pyx_v_radius, PyObject *__pyx_v_id, PyObject *__pyx_v_level) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 1);
@@ -18151,15 +18151,15 @@
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("PynyHTM.Triangle.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.Triangle.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -18168,24 +18168,24 @@
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         """Detailed representation of this Triangle."""
  *         return f"Triangle({str(self.__dict__)})"
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_8Triangle_13__repr__(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_8Triangle_13__repr__(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_8Triangle_12__repr__, "Detailed representation of this Triangle.");
-static PyMethodDef __pyx_mdef_7PynyHTM_8Triangle_13__repr__ = {"__repr__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_8Triangle_13__repr__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_8Triangle_12__repr__};
-static PyObject *__pyx_pw_7PynyHTM_8Triangle_13__repr__(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_8Triangle_12__repr__, "Detailed representation of this Triangle.");
+static PyMethodDef __pyx_mdef_7pynyhtm_8Triangle_13__repr__ = {"__repr__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_8Triangle_13__repr__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_8Triangle_12__repr__};
+static PyObject *__pyx_pw_7pynyhtm_8Triangle_13__repr__(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -18247,32 +18247,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.Triangle.__repr__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.Triangle.__repr__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_8Triangle_12__repr__(__pyx_self, __pyx_v_self);
+  __pyx_r = __pyx_pf_7pynyhtm_8Triangle_12__repr__(__pyx_self, __pyx_v_self);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_8Triangle_12__repr__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pf_7pynyhtm_8Triangle_12__repr__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   Py_ssize_t __pyx_t_2;
   Py_UCS4 __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
@@ -18330,15 +18330,15 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("PynyHTM.Triangle.__repr__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.Triangle.__repr__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -18347,24 +18347,24 @@
  * 
  *     def from_htm_tri(struct: htm_tri) -> Triangle:             # <<<<<<<<<<<<<<
  *         """
  *         Instantiates a triangle based on a htm_tri struct.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_8Triangle_15from_htm_tri(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_8Triangle_15from_htm_tri(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_8Triangle_14from_htm_tri, "\n        Instantiates a triangle based on a htm_tri struct.\n\n        :param struct: struct describing the triangle\n        ");
-static PyMethodDef __pyx_mdef_7PynyHTM_8Triangle_15from_htm_tri = {"from_htm_tri", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_8Triangle_15from_htm_tri, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_8Triangle_14from_htm_tri};
-static PyObject *__pyx_pw_7PynyHTM_8Triangle_15from_htm_tri(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_8Triangle_14from_htm_tri, "\n        Instantiates a triangle based on a htm_tri struct.\n\n        :param struct: struct describing the triangle\n        ");
+static PyMethodDef __pyx_mdef_7pynyhtm_8Triangle_15from_htm_tri = {"from_htm_tri", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_8Triangle_15from_htm_tri, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_8Triangle_14from_htm_tri};
+static PyObject *__pyx_pw_7pynyhtm_8Triangle_15from_htm_tri(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   struct htm_tri __pyx_v_struct;
@@ -18426,32 +18426,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.Triangle.from_htm_tri", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.Triangle.from_htm_tri", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_8Triangle_14from_htm_tri(__pyx_self, __pyx_v_struct);
+  __pyx_r = __pyx_pf_7pynyhtm_8Triangle_14from_htm_tri(__pyx_self, __pyx_v_struct);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_8Triangle_14from_htm_tri(CYTHON_UNUSED PyObject *__pyx_self, struct htm_tri __pyx_v_struct) {
+static PyObject *__pyx_pf_7pynyhtm_8Triangle_14from_htm_tri(CYTHON_UNUSED PyObject *__pyx_self, struct htm_tri __pyx_v_struct) {
   PyObject *__pyx_v_vertices = NULL;
   PyObject *__pyx_v_center = NULL;
   PyObject *__pyx_v_radius = NULL;
   PyObject *__pyx_v_id = NULL;
   PyObject *__pyx_v_level = NULL;
   PyObject *__pyx_7genexpr__pyx_v_vertex = NULL;
   PyObject *__pyx_r = NULL;
@@ -18828,15 +18828,15 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("PynyHTM.Triangle.from_htm_tri", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.Triangle.from_htm_tri", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_vertices);
   __Pyx_XDECREF(__pyx_v_center);
   __Pyx_XDECREF(__pyx_v_radius);
   __Pyx_XDECREF(__pyx_v_id);
   __Pyx_XDECREF(__pyx_v_level);
@@ -18851,24 +18851,24 @@
  * 
  *     def from_id(id: int64_t) -> Triangle:             # <<<<<<<<<<<<<<
  *         """
  *         Instantiates a Triangle object from a given htm id.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_8Triangle_17from_id(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_8Triangle_17from_id(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_8Triangle_16from_id, "\n        Instantiates a Triangle object from a given htm id.\n\n        :param id: triangle id\n        :returns: triangle object\n        ");
-static PyMethodDef __pyx_mdef_7PynyHTM_8Triangle_17from_id = {"from_id", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_8Triangle_17from_id, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_8Triangle_16from_id};
-static PyObject *__pyx_pw_7PynyHTM_8Triangle_17from_id(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_8Triangle_16from_id, "\n        Instantiates a Triangle object from a given htm id.\n\n        :param id: triangle id\n        :returns: triangle object\n        ");
+static PyMethodDef __pyx_mdef_7pynyhtm_8Triangle_17from_id = {"from_id", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_8Triangle_17from_id, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_8Triangle_16from_id};
+static PyObject *__pyx_pw_7pynyhtm_8Triangle_17from_id(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   __pyx_t_5numpy_int64_t __pyx_v_id;
@@ -18930,32 +18930,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.Triangle.from_id", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.Triangle.from_id", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_8Triangle_16from_id(__pyx_self, __pyx_v_id);
+  __pyx_r = __pyx_pf_7pynyhtm_8Triangle_16from_id(__pyx_self, __pyx_v_id);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_8Triangle_16from_id(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id) {
+static PyObject *__pyx_pf_7pynyhtm_8Triangle_16from_id(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
@@ -19013,15 +19013,15 @@
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("PynyHTM.Triangle.from_id", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.Triangle.from_id", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -19030,24 +19030,24 @@
  * 
  * def htm_v3_id_raw(v: htm_v3, level: int) -> int64_t:             # <<<<<<<<<<<<<<
  *     """
  *     Retrieves the trixel is for a given v3.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_27htm_v3_id_raw(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_27htm_v3_id_raw(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_26htm_v3_id_raw, "\n    Retrieves the trixel is for a given v3.\n\n    :param v: v3 vector\n    :param level: trixel depth\n    :returns: id of the trixel in which v3 lands at the given level\n    ");
-static PyMethodDef __pyx_mdef_7PynyHTM_27htm_v3_id_raw = {"htm_v3_id_raw", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_27htm_v3_id_raw, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_26htm_v3_id_raw};
-static PyObject *__pyx_pw_7PynyHTM_27htm_v3_id_raw(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_26htm_v3_id_raw, "\n    Retrieves the trixel is for a given v3.\n\n    :param v: v3 vector\n    :param level: trixel depth\n    :returns: id of the trixel in which v3 lands at the given level\n    ");
+static PyMethodDef __pyx_mdef_7pynyhtm_27htm_v3_id_raw = {"htm_v3_id_raw", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_27htm_v3_id_raw, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_26htm_v3_id_raw};
+static PyObject *__pyx_pw_7pynyhtm_27htm_v3_id_raw(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   struct htm_v3 __pyx_v_v;
@@ -19124,20 +19124,20 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.htm_v3_id_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.htm_v3_id_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_level), (&PyInt_Type), 0, "level", 1))) __PYX_ERR(0, 588, __pyx_L1_error)
-  __pyx_r = __pyx_pf_7PynyHTM_26htm_v3_id_raw(__pyx_self, __pyx_v_v, __pyx_v_level);
+  __pyx_r = __pyx_pf_7pynyhtm_26htm_v3_id_raw(__pyx_self, __pyx_v_v, __pyx_v_level);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   {
@@ -19146,15 +19146,15 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_26htm_v3_id_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_v3 __pyx_v_v, PyObject *__pyx_v_level) {
+static PyObject *__pyx_pf_7pynyhtm_26htm_v3_id_raw(CYTHON_UNUSED PyObject *__pyx_self, struct htm_v3 __pyx_v_v, PyObject *__pyx_v_level) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -19182,15 +19182,15 @@
  *     """
  *     Retrieves the trixel is for a given v3.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("PynyHTM.htm_v3_id_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.htm_v3_id_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -19199,24 +19199,24 @@
  * 
  * def htm_tri_init_raw(id: int64_t) -> tuple[htm_errcode, htm_tri]:             # <<<<<<<<<<<<<<
  *     """
  *     Instantiate a htm_tri struct for a given triangle id.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_29htm_tri_init_raw(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_29htm_tri_init_raw(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_28htm_tri_init_raw, "\n    Instantiate a htm_tri struct for a given triangle id.\n\n    :param id: Id of the triangle\n    ");
-static PyMethodDef __pyx_mdef_7PynyHTM_29htm_tri_init_raw = {"htm_tri_init_raw", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_29htm_tri_init_raw, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_28htm_tri_init_raw};
-static PyObject *__pyx_pw_7PynyHTM_29htm_tri_init_raw(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_28htm_tri_init_raw, "\n    Instantiate a htm_tri struct for a given triangle id.\n\n    :param id: Id of the triangle\n    ");
+static PyMethodDef __pyx_mdef_7pynyhtm_29htm_tri_init_raw = {"htm_tri_init_raw", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_29htm_tri_init_raw, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_28htm_tri_init_raw};
+static PyObject *__pyx_pw_7pynyhtm_29htm_tri_init_raw(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   __pyx_t_5numpy_int64_t __pyx_v_id;
@@ -19278,32 +19278,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.htm_tri_init_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.htm_tri_init_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_28htm_tri_init_raw(__pyx_self, __pyx_v_id);
+  __pyx_r = __pyx_pf_7pynyhtm_28htm_tri_init_raw(__pyx_self, __pyx_v_id);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_28htm_tri_init_raw(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id) {
+static PyObject *__pyx_pf_7pynyhtm_28htm_tri_init_raw(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id) {
   struct htm_tri __pyx_v_triangle;
   PyObject *__pyx_v_err_code = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
@@ -19353,15 +19353,15 @@
  *     Instantiate a htm_tri struct for a given triangle id.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("PynyHTM.htm_tri_init_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.htm_tri_init_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_err_code);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -19371,24 +19371,24 @@
  * 
  * def htm_tri_init_wrapped(id: int64_t) -> Triangle:             # <<<<<<<<<<<<<<
  *     """
  *     Instantiate a Triangle object for a given triangle id.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_31htm_tri_init_wrapped(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_31htm_tri_init_wrapped(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_30htm_tri_init_wrapped, "\n    Instantiate a Triangle object for a given triangle id.\n\n    :param id: id of the triangle\n    ");
-static PyMethodDef __pyx_mdef_7PynyHTM_31htm_tri_init_wrapped = {"htm_tri_init_wrapped", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_31htm_tri_init_wrapped, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_30htm_tri_init_wrapped};
-static PyObject *__pyx_pw_7PynyHTM_31htm_tri_init_wrapped(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_30htm_tri_init_wrapped, "\n    Instantiate a Triangle object for a given triangle id.\n\n    :param id: id of the triangle\n    ");
+static PyMethodDef __pyx_mdef_7pynyhtm_31htm_tri_init_wrapped = {"htm_tri_init_wrapped", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_31htm_tri_init_wrapped, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_30htm_tri_init_wrapped};
+static PyObject *__pyx_pw_7pynyhtm_31htm_tri_init_wrapped(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   __pyx_t_5numpy_int64_t __pyx_v_id;
@@ -19450,32 +19450,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.htm_tri_init_wrapped", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.htm_tri_init_wrapped", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_30htm_tri_init_wrapped(__pyx_self, __pyx_v_id);
+  __pyx_r = __pyx_pf_7pynyhtm_30htm_tri_init_wrapped(__pyx_self, __pyx_v_id);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_30htm_tri_init_wrapped(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id) {
+static PyObject *__pyx_pf_7pynyhtm_30htm_tri_init_wrapped(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id) {
   struct htm_tri __pyx_v_triangle;
   htm_errcode __pyx_v_ec;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
@@ -19699,15 +19699,15 @@
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("PynyHTM.htm_tri_init_wrapped", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.htm_tri_init_wrapped", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -19716,24 +19716,24 @@
  * 
  *     def get_level(id: int64_t) -> int:             # <<<<<<<<<<<<<<
  *         """
  *         Retrieves the level of a given ID.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_3HTM_1get_level(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_3HTM_1get_level(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_3HTM_get_level, "\n        Retrieves the level of a given ID.\n\n        :param: htm id\n        :returns: level of the id\n        :raises valueError: if the provided id is invalid\n        ");
-static PyMethodDef __pyx_mdef_7PynyHTM_3HTM_1get_level = {"get_level", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_3HTM_1get_level, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_3HTM_get_level};
-static PyObject *__pyx_pw_7PynyHTM_3HTM_1get_level(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_3HTM_get_level, "\n        Retrieves the level of a given ID.\n\n        :param: htm id\n        :returns: level of the id\n        :raises valueError: if the provided id is invalid\n        ");
+static PyMethodDef __pyx_mdef_7pynyhtm_3HTM_1get_level = {"get_level", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_3HTM_1get_level, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_3HTM_get_level};
+static PyObject *__pyx_pw_7pynyhtm_3HTM_1get_level(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   __pyx_t_5numpy_int64_t __pyx_v_id;
@@ -19795,32 +19795,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.HTM.get_level", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.HTM.get_level", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_3HTM_get_level(__pyx_self, __pyx_v_id);
+  __pyx_r = __pyx_pf_7pynyhtm_3HTM_get_level(__pyx_self, __pyx_v_id);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_3HTM_get_level(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id) {
+static PyObject *__pyx_pf_7pynyhtm_3HTM_get_level(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
@@ -19879,15 +19879,15 @@
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("PynyHTM.HTM.get_level", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.HTM.get_level", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -19896,24 +19896,24 @@
  * 
  *     def id_to_dec(id: int64_t) -> int64_t:             # <<<<<<<<<<<<<<
  *         """
  *         Retrieves the decimal representation of an id.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_3HTM_3id_to_dec(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_3HTM_3id_to_dec(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_3HTM_2id_to_dec, "\n        Retrieves the decimal representation of an id.\n\n        :param id: triangle id\n        :returns: decimal id representation (concatenated [0-3]*)\n        ");
-static PyMethodDef __pyx_mdef_7PynyHTM_3HTM_3id_to_dec = {"id_to_dec", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_3HTM_3id_to_dec, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_3HTM_2id_to_dec};
-static PyObject *__pyx_pw_7PynyHTM_3HTM_3id_to_dec(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_3HTM_2id_to_dec, "\n        Retrieves the decimal representation of an id.\n\n        :param id: triangle id\n        :returns: decimal id representation (concatenated [0-3]*)\n        ");
+static PyMethodDef __pyx_mdef_7pynyhtm_3HTM_3id_to_dec = {"id_to_dec", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_3HTM_3id_to_dec, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_3HTM_2id_to_dec};
+static PyObject *__pyx_pw_7pynyhtm_3HTM_3id_to_dec(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   __pyx_t_5numpy_int64_t __pyx_v_id;
@@ -19975,32 +19975,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.HTM.id_to_dec", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.HTM.id_to_dec", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_3HTM_2id_to_dec(__pyx_self, __pyx_v_id);
+  __pyx_r = __pyx_pf_7pynyhtm_3HTM_2id_to_dec(__pyx_self, __pyx_v_id);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_3HTM_2id_to_dec(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id) {
+static PyObject *__pyx_pf_7pynyhtm_3HTM_2id_to_dec(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
@@ -20058,15 +20058,15 @@
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("PynyHTM.HTM.id_to_dec", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.HTM.id_to_dec", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -20075,24 +20075,24 @@
  * 
  *     def parent(id: int64_t) -> int64_t:             # <<<<<<<<<<<<<<
  *         """
  *         Determines the parent id of the triangle identified by id.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_3HTM_5parent(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_3HTM_5parent(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_3HTM_4parent, "\n        Determines the parent id of the triangle identified by id.\n\n        :param id: target triangle\n        :returns: parent triangle id\n        :raises valueError: if the provided id is invalid or the triangle is a root triangle\n        ");
-static PyMethodDef __pyx_mdef_7PynyHTM_3HTM_5parent = {"parent", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_3HTM_5parent, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_3HTM_4parent};
-static PyObject *__pyx_pw_7PynyHTM_3HTM_5parent(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_3HTM_4parent, "\n        Determines the parent id of the triangle identified by id.\n\n        :param id: target triangle\n        :returns: parent triangle id\n        :raises valueError: if the provided id is invalid or the triangle is a root triangle\n        ");
+static PyMethodDef __pyx_mdef_7pynyhtm_3HTM_5parent = {"parent", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_3HTM_5parent, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_3HTM_4parent};
+static PyObject *__pyx_pw_7pynyhtm_3HTM_5parent(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   __pyx_t_5numpy_int64_t __pyx_v_id;
@@ -20154,32 +20154,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.HTM.parent", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.HTM.parent", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_3HTM_4parent(__pyx_self, __pyx_v_id);
+  __pyx_r = __pyx_pf_7pynyhtm_3HTM_4parent(__pyx_self, __pyx_v_id);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_3HTM_4parent(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id) {
+static PyObject *__pyx_pf_7pynyhtm_3HTM_4parent(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
@@ -20306,15 +20306,15 @@
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("PynyHTM.HTM.parent", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.HTM.parent", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -20323,24 +20323,24 @@
  * 
  *     def children(id: int64_t) -> list[int64_t]:             # <<<<<<<<<<<<<<
  *         """
  *         Gets the children contained in the triangle identified by id.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_3HTM_7children(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_3HTM_7children(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_3HTM_6children, "\n        Gets the children contained in the triangle identified by id.\n\n        :param id: target triangle\n        :returns: list of 4 children\n        :raises valueError: if the provided id is invalid\n        ");
-static PyMethodDef __pyx_mdef_7PynyHTM_3HTM_7children = {"children", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_3HTM_7children, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_3HTM_6children};
-static PyObject *__pyx_pw_7PynyHTM_3HTM_7children(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_3HTM_6children, "\n        Gets the children contained in the triangle identified by id.\n\n        :param id: target triangle\n        :returns: list of 4 children\n        :raises valueError: if the provided id is invalid\n        ");
+static PyMethodDef __pyx_mdef_7pynyhtm_3HTM_7children = {"children", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_3HTM_7children, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_3HTM_6children};
+static PyObject *__pyx_pw_7pynyhtm_3HTM_7children(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   __pyx_t_5numpy_int64_t __pyx_v_id;
@@ -20402,32 +20402,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.HTM.children", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.HTM.children", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_3HTM_6children(__pyx_self, __pyx_v_id);
+  __pyx_r = __pyx_pf_7pynyhtm_3HTM_6children(__pyx_self, __pyx_v_id);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_3HTM_6children(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id) {
+static PyObject *__pyx_pf_7pynyhtm_3HTM_6children(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id) {
   PyObject *__pyx_v_children = NULL;
   long __pyx_v_i;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
@@ -20536,15 +20536,15 @@
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("PynyHTM.HTM.children", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.HTM.children", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_children);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -20554,24 +20554,24 @@
  * 
  *     def neighbors(id: int64_t) -> list[int64_t]:             # <<<<<<<<<<<<<<
  *         """
  *         Gets the neighboring trixels for the given id.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_3HTM_9neighbors(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_3HTM_9neighbors(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_3HTM_8neighbors, "\n        Gets the neighboring trixels for the given id.\n\n        :param id: id of the source triangle\n        :returns: list of neighboring triangle ids\n        :raises ValueError: if the provided id is invalid\n        ");
-static PyMethodDef __pyx_mdef_7PynyHTM_3HTM_9neighbors = {"neighbors", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_3HTM_9neighbors, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_3HTM_8neighbors};
-static PyObject *__pyx_pw_7PynyHTM_3HTM_9neighbors(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_3HTM_8neighbors, "\n        Gets the neighboring trixels for the given id.\n\n        :param id: id of the source triangle\n        :returns: list of neighboring triangle ids\n        :raises ValueError: if the provided id is invalid\n        ");
+static PyMethodDef __pyx_mdef_7pynyhtm_3HTM_9neighbors = {"neighbors", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_3HTM_9neighbors, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_3HTM_8neighbors};
+static PyObject *__pyx_pw_7pynyhtm_3HTM_9neighbors(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   __pyx_t_5numpy_int64_t __pyx_v_id;
@@ -20633,32 +20633,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.HTM.neighbors", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.HTM.neighbors", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_3HTM_8neighbors(__pyx_self, __pyx_v_id);
+  __pyx_r = __pyx_pf_7pynyhtm_3HTM_8neighbors(__pyx_self, __pyx_v_id);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_3HTM_8neighbors(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id) {
+static PyObject *__pyx_pf_7pynyhtm_3HTM_8neighbors(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
@@ -20894,15 +20894,15 @@
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("PynyHTM.HTM.neighbors", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.HTM.neighbors", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -20911,24 +20911,24 @@
  * 
  *     def neighbor(id: int64_t, direction: NeighborDirection) -> tuple[int64_t, bool]:             # <<<<<<<<<<<<<<
  *         """
  *         Gets the neighboring trixel for the given id and direction.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_3HTM_11neighbor(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_3HTM_11neighbor(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_3HTM_10neighbor, "\n        Gets the neighboring trixel for the given id and direction.\n\n        The adjecent trixels can be determined recursively due to the subdividing nature of their generation.\n        Since the orientation of triangles can change at different depth, the neighbor relation is expressed relative\n        to the children of the given triangle.\n        The neighbor in direction \"OC_ZERO\" for triangle 3 is given by the triangle in the opposite direction of the\n        child with index 0.\n        The opposite direction of the child \"30\" is the large top right triangle.\n        Similarly OC_ONE and OC_ZERO describe the other two directions which neighbors can have.\n\n\n                 -------------------------\n                \\          /\\          /\n                 \\ OC_1   /32\\  OC_0  /\n                  \\      -------      /\n                   \\    /\\33  /\\   /\n                    \\  /  \\  /  \\ /\n                     \\/ 30 \\/ 31\\/\n                       -------------\n                       \\         /\n                        \\ OC_2  /\n                         \\     /\n                          \\   /\n                           \\ /\n\n\n        In the simplest case (a \"center\"/id=3 triangle) the neighbors are given by changing the last two bits of the\n        triangle id. In this case they are direct neighbors and lookup is trivial.\n\n        For all other children of a triangle (id = 0,1,2) one neighbor is given as the center triangle of the parent.\n        The two other neighbors are child triangles (also with id = 0,1,2) from neighbors of the parent triangle.\n        Example: The neighbors of \"32\" (see above) are contained within OC_ZERO and OC_ONE of the parent triangle.\n        I.e. the neighbors of edge triangles (id = 0,1,2) are given by their counter part in the parents neighbors in\n        the direction of the remaining two edge triangles.\n\n        This can be performed recursively until a center triangl""e is reached, in which case the trivial case holds.\n\n\n        Since the root triangles (8-15) are not oriented in the same fashion as all other triangles, the transition\n        between two of them must be handled separately.\n        Therefore, once a root triangle has been reached during recursion, the correct neighboring triangle is\n        determined using a LUT and a correction Flag is set. This Flag is set to NONE, EAST_WEST (adjecent triangles in\n        the same hemisphere) or NORTH_SOUTH (adjecent triangles in different hemispheres).\n        Based on the Flag, the correct child of the root triangle is determined, such that the children of root\n        triangles align with one another.\n\n\n        Note: This is a rather large function and splitting it into smaller parts would make sense.\n        I have opted against this due to the recursive nature of this method.\n\n\n        :param id: source triangle id\n        :param direction: direction in which the neighbor is to be determined\n        :returns: tuple containing the neighbor id and flip direction if applicable\n        ");
-static PyMethodDef __pyx_mdef_7PynyHTM_3HTM_11neighbor = {"neighbor", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_3HTM_11neighbor, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_3HTM_10neighbor};
-static PyObject *__pyx_pw_7PynyHTM_3HTM_11neighbor(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_3HTM_10neighbor, "\n        Gets the neighboring trixel for the given id and direction.\n\n        The adjecent trixels can be determined recursively due to the subdividing nature of their generation.\n        Since the orientation of triangles can change at different depth, the neighbor relation is expressed relative\n        to the children of the given triangle.\n        The neighbor in direction \"OC_ZERO\" for triangle 3 is given by the triangle in the opposite direction of the\n        child with index 0.\n        The opposite direction of the child \"30\" is the large top right triangle.\n        Similarly OC_ONE and OC_ZERO describe the other two directions which neighbors can have.\n\n\n                 -------------------------\n                \\          /\\          /\n                 \\ OC_1   /32\\  OC_0  /\n                  \\      -------      /\n                   \\    /\\33  /\\   /\n                    \\  /  \\  /  \\ /\n                     \\/ 30 \\/ 31\\/\n                       -------------\n                       \\         /\n                        \\ OC_2  /\n                         \\     /\n                          \\   /\n                           \\ /\n\n\n        In the simplest case (a \"center\"/id=3 triangle) the neighbors are given by changing the last two bits of the\n        triangle id. In this case they are direct neighbors and lookup is trivial.\n\n        For all other children of a triangle (id = 0,1,2) one neighbor is given as the center triangle of the parent.\n        The two other neighbors are child triangles (also with id = 0,1,2) from neighbors of the parent triangle.\n        Example: The neighbors of \"32\" (see above) are contained within OC_ZERO and OC_ONE of the parent triangle.\n        I.e. the neighbors of edge triangles (id = 0,1,2) are given by their counter part in the parents neighbors in\n        the direction of the remaining two edge triangles.\n\n        This can be performed recursively until a center triangl""e is reached, in which case the trivial case holds.\n\n\n        Since the root triangles (8-15) are not oriented in the same fashion as all other triangles, the transition\n        between two of them must be handled separately.\n        Therefore, once a root triangle has been reached during recursion, the correct neighboring triangle is\n        determined using a LUT and a correction Flag is set. This Flag is set to NONE, EAST_WEST (adjecent triangles in\n        the same hemisphere) or NORTH_SOUTH (adjecent triangles in different hemispheres).\n        Based on the Flag, the correct child of the root triangle is determined, such that the children of root\n        triangles align with one another.\n\n\n        Note: This is a rather large function and splitting it into smaller parts would make sense.\n        I have opted against this due to the recursive nature of this method.\n\n\n        :param id: source triangle id\n        :param direction: direction in which the neighbor is to be determined\n        :returns: tuple containing the neighbor id and flip direction if applicable\n        ");
+static PyMethodDef __pyx_mdef_7pynyhtm_3HTM_11neighbor = {"neighbor", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_3HTM_11neighbor, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_3HTM_10neighbor};
+static PyObject *__pyx_pw_7pynyhtm_3HTM_11neighbor(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   __pyx_t_5numpy_int64_t __pyx_v_id;
@@ -21005,32 +21005,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.HTM.neighbor", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.HTM.neighbor", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_3HTM_10neighbor(__pyx_self, __pyx_v_id, __pyx_v_direction);
+  __pyx_r = __pyx_pf_7pynyhtm_3HTM_10neighbor(__pyx_self, __pyx_v_id, __pyx_v_direction);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_3HTM_10neighbor(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id, PyObject *__pyx_v_direction) {
+static PyObject *__pyx_pf_7pynyhtm_3HTM_10neighbor(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id, PyObject *__pyx_v_direction) {
   PyObject *__pyx_v_tail = NULL;
   PyObject *__pyx_v_blank_head = NULL;
   PyObject *__pyx_v_parent_tail = NULL;
   PyObject *__pyx_v_flip = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
@@ -25665,15 +25665,15 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("PynyHTM.HTM.neighbor", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.HTM.neighbor", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_tail);
   __Pyx_XDECREF(__pyx_v_blank_head);
   __Pyx_XDECREF(__pyx_v_parent_tail);
   __Pyx_XDECREF(__pyx_v_flip);
   __Pyx_XGIVEREF(__pyx_r);
@@ -25685,15 +25685,15 @@
  *     # TODO: searching an area could also be implemented with a flooding algorithm using the neighbor function
  * 
  *     def circle_search(center: V3,             # <<<<<<<<<<<<<<
  *                       radius: float,
  *                       level: int,
  */
 
-static PyObject *__pyx_pf_7PynyHTM_36__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_7pynyhtm_36__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -25716,33 +25716,33 @@
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("PynyHTM.__defaults__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.__defaults__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_3HTM_13circle_search(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_3HTM_13circle_search(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_3HTM_12circle_search, "\n        Retrieves triangle id's in a given circular region by wrapping the htm_s2circle_ids function.\n\n        :param center:center of the search circle\n        :param radius: radius of the search circle in degrees\n        :param level: level at which the search is performed\n        :param max_ranges: highest number of ranges to use for the search\n        :returns: list of triangle id's which are within the search area\n        :raises runtimeError: if the search failed\n        ");
-static PyMethodDef __pyx_mdef_7PynyHTM_3HTM_13circle_search = {"circle_search", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_3HTM_13circle_search, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_3HTM_12circle_search};
-static PyObject *__pyx_pw_7PynyHTM_3HTM_13circle_search(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_3HTM_12circle_search, "\n        Retrieves triangle id's in a given circular region by wrapping the htm_s2circle_ids function.\n\n        :param center:center of the search circle\n        :param radius: radius of the search circle in degrees\n        :param level: level at which the search is performed\n        :param max_ranges: highest number of ranges to use for the search\n        :returns: list of triangle id's which are within the search area\n        :raises runtimeError: if the search failed\n        ");
+static PyMethodDef __pyx_mdef_7pynyhtm_3HTM_13circle_search = {"circle_search", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_3HTM_13circle_search, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_3HTM_12circle_search};
+static PyObject *__pyx_pw_7pynyhtm_3HTM_13circle_search(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_center = 0;
@@ -25851,21 +25851,21 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.HTM.circle_search", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.HTM.circle_search", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_level), (&PyInt_Type), 0, "level", 1))) __PYX_ERR(0, 1049, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_max_ranges), (&PyInt_Type), 0, "max_ranges", 1))) __PYX_ERR(0, 1050, __pyx_L1_error)
-  __pyx_r = __pyx_pf_7PynyHTM_3HTM_12circle_search(__pyx_self, __pyx_v_center, __pyx_v_radius, __pyx_v_level, __pyx_v_max_ranges);
+  __pyx_r = __pyx_pf_7pynyhtm_3HTM_12circle_search(__pyx_self, __pyx_v_center, __pyx_v_radius, __pyx_v_level, __pyx_v_max_ranges);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   {
@@ -25874,15 +25874,15 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_3HTM_12circle_search(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_center, double __pyx_v_radius, PyObject *__pyx_v_level, PyObject *__pyx_v_max_ranges) {
+static PyObject *__pyx_pf_7pynyhtm_3HTM_12circle_search(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_center, double __pyx_v_radius, PyObject *__pyx_v_level, PyObject *__pyx_v_max_ranges) {
   struct htm_v3 __pyx_v_center_htm;
   htm_errcode __pyx_v_error_code;
   struct htm_ids *__pyx_v_result;
   PyObject *__pyx_v_ids = NULL;
   struct htm_range *__pyx_v_ranges;
   size_t __pyx_v_i;
   PyObject *__pyx_r = NULL;
@@ -26153,15 +26153,15 @@
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_AddTraceback("PynyHTM.HTM.circle_search", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.HTM.circle_search", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_ids);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -26171,24 +26171,24 @@
  * 
  * def htm_level_raw(id: int64_t) -> int:             # <<<<<<<<<<<<<<
  *     """
  *     Retrieves the level of a given ID.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_33htm_level_raw(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_33htm_level_raw(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_32htm_level_raw, "\n    Retrieves the level of a given ID.\n\n    :param: htm id\n    :returns: level of the id\n    :raises valueError: if the provided id is invalid\n    ");
-static PyMethodDef __pyx_mdef_7PynyHTM_33htm_level_raw = {"htm_level_raw", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_33htm_level_raw, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_32htm_level_raw};
-static PyObject *__pyx_pw_7PynyHTM_33htm_level_raw(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_32htm_level_raw, "\n    Retrieves the level of a given ID.\n\n    :param: htm id\n    :returns: level of the id\n    :raises valueError: if the provided id is invalid\n    ");
+static PyMethodDef __pyx_mdef_7pynyhtm_33htm_level_raw = {"htm_level_raw", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_33htm_level_raw, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_32htm_level_raw};
+static PyObject *__pyx_pw_7pynyhtm_33htm_level_raw(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   __pyx_t_5numpy_int64_t __pyx_v_id;
@@ -26250,32 +26250,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.htm_level_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.htm_level_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_32htm_level_raw(__pyx_self, __pyx_v_id);
+  __pyx_r = __pyx_pf_7pynyhtm_32htm_level_raw(__pyx_self, __pyx_v_id);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_32htm_level_raw(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id) {
+static PyObject *__pyx_pf_7pynyhtm_32htm_level_raw(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id) {
   int __pyx_v_level;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
@@ -26356,15 +26356,15 @@
  *     Retrieves the level of a given ID.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("PynyHTM.htm_level_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.htm_level_raw", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -26373,24 +26373,24 @@
  * 
  * def htm_id_to_dec(id: int64_t) -> int64_t:             # <<<<<<<<<<<<<<
  *     """
  *     Retrieves the decimal representation of an id.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7PynyHTM_35htm_id_to_dec(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_7pynyhtm_35htm_id_to_dec(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_7PynyHTM_34htm_id_to_dec, "\n    Retrieves the decimal representation of an id.\n\n    :param id: triangle id\n    :returns: decimal id representation (concatenated [0-3]*)\n    ");
-static PyMethodDef __pyx_mdef_7PynyHTM_35htm_id_to_dec = {"htm_id_to_dec", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7PynyHTM_35htm_id_to_dec, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7PynyHTM_34htm_id_to_dec};
-static PyObject *__pyx_pw_7PynyHTM_35htm_id_to_dec(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_7pynyhtm_34htm_id_to_dec, "\n    Retrieves the decimal representation of an id.\n\n    :param id: triangle id\n    :returns: decimal id representation (concatenated [0-3]*)\n    ");
+static PyMethodDef __pyx_mdef_7pynyhtm_35htm_id_to_dec = {"htm_id_to_dec", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pynyhtm_35htm_id_to_dec, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pynyhtm_34htm_id_to_dec};
+static PyObject *__pyx_pw_7pynyhtm_35htm_id_to_dec(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   __pyx_t_5numpy_int64_t __pyx_v_id;
@@ -26452,32 +26452,32 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("PynyHTM.htm_id_to_dec", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.htm_id_to_dec", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7PynyHTM_34htm_id_to_dec(__pyx_self, __pyx_v_id);
+  __pyx_r = __pyx_pf_7pynyhtm_34htm_id_to_dec(__pyx_self, __pyx_v_id);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7PynyHTM_34htm_id_to_dec(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id) {
+static PyObject *__pyx_pf_7pynyhtm_34htm_id_to_dec(CYTHON_UNUSED PyObject *__pyx_self, __pyx_t_5numpy_int64_t __pyx_v_id) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("htm_id_to_dec", 1);
@@ -26501,15 +26501,15 @@
  *     """
  *     Retrieves the decimal representation of an id.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("PynyHTM.htm_id_to_dec", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pynyhtm.htm_id_to_dec", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -26587,15 +26587,14 @@
     {&__pyx_kp_s_No_value_specified_for_struct_at_9, __pyx_k_No_value_specified_for_struct_at_9, sizeof(__pyx_k_No_value_specified_for_struct_at_9), 0, 0, 1, 0},
     {&__pyx_n_s_None, __pyx_k_None, sizeof(__pyx_k_None), 0, 0, 1, 1},
     {&__pyx_n_s_NotImplementedError, __pyx_k_NotImplementedError, sizeof(__pyx_k_NotImplementedError), 0, 0, 1, 1},
     {&__pyx_n_s_OC_ONE, __pyx_k_OC_ONE, sizeof(__pyx_k_OC_ONE), 0, 0, 1, 1},
     {&__pyx_n_s_OC_TWO, __pyx_k_OC_TWO, sizeof(__pyx_k_OC_TWO), 0, 0, 1, 1},
     {&__pyx_n_s_OC_ZERO, __pyx_k_OC_ZERO, sizeof(__pyx_k_OC_ZERO), 0, 0, 1, 1},
     {&__pyx_n_s_OverflowError, __pyx_k_OverflowError, sizeof(__pyx_k_OverflowError), 0, 0, 1, 1},
-    {&__pyx_n_s_PynyHTM, __pyx_k_PynyHTM, sizeof(__pyx_k_PynyHTM), 0, 0, 1, 1},
     {&__pyx_kp_u_Root_level_neighbor_lookup_not_i, __pyx_k_Root_level_neighbor_lookup_not_i, sizeof(__pyx_k_Root_level_neighbor_lookup_not_i), 0, 1, 0, 0},
     {&__pyx_kp_u_Root_triangle, __pyx_k_Root_triangle, sizeof(__pyx_k_Root_triangle), 0, 1, 0, 0},
     {&__pyx_n_s_RuntimeError, __pyx_k_RuntimeError, sizeof(__pyx_k_RuntimeError), 0, 0, 1, 1},
     {&__pyx_kp_u_Search_failed_with_errorcode, __pyx_k_Search_failed_with_errorcode, sizeof(__pyx_k_Search_failed_with_errorcode), 0, 1, 0, 0},
     {&__pyx_kp_u_SphericalCoordinate, __pyx_k_SphericalCoordinate, sizeof(__pyx_k_SphericalCoordinate), 0, 1, 0, 0},
     {&__pyx_n_s_SphericalCoordinate_2, __pyx_k_SphericalCoordinate_2, sizeof(__pyx_k_SphericalCoordinate_2), 0, 0, 1, 1},
     {&__pyx_n_s_SphericalCoordinate___init, __pyx_k_SphericalCoordinate___init, sizeof(__pyx_k_SphericalCoordinate___init), 0, 0, 1, 1},
@@ -26746,14 +26745,15 @@
     {&__pyx_kp_s_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 0, 1, 0},
     {&__pyx_n_s_other, __pyx_k_other, sizeof(__pyx_k_other), 0, 0, 1, 1},
     {&__pyx_n_s_out, __pyx_k_out, sizeof(__pyx_k_out), 0, 0, 1, 1},
     {&__pyx_n_s_parent, __pyx_k_parent, sizeof(__pyx_k_parent), 0, 0, 1, 1},
     {&__pyx_n_s_parent_tail, __pyx_k_parent_tail, sizeof(__pyx_k_parent_tail), 0, 0, 1, 1},
     {&__pyx_n_s_prepare, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
     {&__pyx_n_s_property, __pyx_k_property, sizeof(__pyx_k_property), 0, 0, 1, 1},
+    {&__pyx_n_s_pynyhtm, __pyx_k_pynyhtm, sizeof(__pyx_k_pynyhtm), 0, 0, 1, 1},
     {&__pyx_kp_s_pynyhtm_pyx, __pyx_k_pynyhtm_pyx, sizeof(__pyx_k_pynyhtm_pyx), 0, 0, 1, 0},
     {&__pyx_n_s_qualname, __pyx_k_qualname, sizeof(__pyx_k_qualname), 0, 0, 1, 1},
     {&__pyx_n_s_radius, __pyx_k_radius, sizeof(__pyx_k_radius), 0, 0, 1, 1},
     {&__pyx_n_s_radius_2, __pyx_k_radius_2, sizeof(__pyx_k_radius_2), 0, 0, 1, 1},
     {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
     {&__pyx_n_s_ranges, __pyx_k_ranges, sizeof(__pyx_k_ranges), 0, 0, 1, 1},
     {&__pyx_n_s_repr, __pyx_k_repr, sizeof(__pyx_k_repr), 0, 0, 1, 1},
@@ -26928,26 +26928,26 @@
  *     result.level = value
  *     return result
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_No_value_specified_for_struct_at_10); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(2, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
 
-  /* "../../../../../tmp/build-env-tuk_0wzp/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../../tmp/build-env-22q13c7o/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(2, 990, __pyx_L1_error)
@@ -27774,31 +27774,31 @@
   return 0;
 }
 
 
 #if PY_MAJOR_VERSION >= 3
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
-static int __pyx_pymod_exec_PynyHTM(PyObject* module); /*proto*/
+static int __pyx_pymod_exec_pynyhtm(PyObject* module); /*proto*/
 static PyModuleDef_Slot __pyx_moduledef_slots[] = {
   {Py_mod_create, (void*)__pyx_pymod_create},
-  {Py_mod_exec, (void*)__pyx_pymod_exec_PynyHTM},
+  {Py_mod_exec, (void*)__pyx_pymod_exec_pynyhtm},
   {0, NULL}
 };
 #endif
 
 #ifdef __cplusplus
 namespace {
   struct PyModuleDef __pyx_moduledef =
   #else
   static struct PyModuleDef __pyx_moduledef =
   #endif
   {
       PyModuleDef_HEAD_INIT,
-      "PynyHTM",
+      "pynyhtm",
       __pyx_k_Wrapping_classes_and_methods_for, /* m_doc */
     #if CYTHON_PEP489_MULTI_PHASE_INIT
       0, /* m_size */
     #elif CYTHON_USE_MODULE_STATE
       sizeof(__pyx_mstate), /* m_size */
     #else
       -1, /* m_size */
@@ -27838,19 +27838,19 @@
 #else
 #define __Pyx_PyMODINIT_FUNC PyObject *
 #endif
 #endif
 
 
 #if PY_MAJOR_VERSION < 3
-__Pyx_PyMODINIT_FUNC initPynyHTM(void) CYTHON_SMALL_CODE; /*proto*/
-__Pyx_PyMODINIT_FUNC initPynyHTM(void)
+__Pyx_PyMODINIT_FUNC initpynyhtm(void) CYTHON_SMALL_CODE; /*proto*/
+__Pyx_PyMODINIT_FUNC initpynyhtm(void)
 #else
-__Pyx_PyMODINIT_FUNC PyInit_PynyHTM(void) CYTHON_SMALL_CODE; /*proto*/
-__Pyx_PyMODINIT_FUNC PyInit_PynyHTM(void)
+__Pyx_PyMODINIT_FUNC PyInit_pynyhtm(void) CYTHON_SMALL_CODE; /*proto*/
+__Pyx_PyMODINIT_FUNC PyInit_pynyhtm(void)
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 {
   return PyModuleDef_Init(&__pyx_moduledef);
 }
 static CYTHON_SMALL_CODE int __Pyx_check_single_interpreter(void) {
     #if PY_VERSION_HEX >= 0x030700A1
     static PY_INT64_T main_interpreter_id = -1;
@@ -27923,15 +27923,15 @@
     return module;
 bad:
     Py_XDECREF(module);
     return NULL;
 }
 
 
-static CYTHON_SMALL_CODE int __pyx_pymod_exec_PynyHTM(PyObject *__pyx_pyinit_module)
+static CYTHON_SMALL_CODE int __pyx_pymod_exec_pynyhtm(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
   int stringtab_initialized = 0;
   #if CYTHON_USE_MODULE_STATE
   int pystate_addmodule_run = 0;
   #endif
@@ -27943,33 +27943,33 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
-    PyErr_SetString(PyExc_RuntimeError, "Module 'PynyHTM' has already been imported. Re-initialisation is not supported.");
+    PyErr_SetString(PyExc_RuntimeError, "Module 'pynyhtm' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
   #elif PY_MAJOR_VERSION >= 3
   if (__pyx_m) return __Pyx_NewRef(__pyx_m);
   #endif
   /*--- Module creation code ---*/
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
-  __pyx_m = Py_InitModule4("PynyHTM", __pyx_methods, __pyx_k_Wrapping_classes_and_methods_for, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
+  __pyx_m = Py_InitModule4("pynyhtm", __pyx_methods, __pyx_k_Wrapping_classes_and_methods_for, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #elif CYTHON_USE_MODULE_STATE
   __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   {
     int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
-    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to "PynyHTM" pseudovariable */
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to "pynyhtm" pseudovariable */
     if (unlikely((add_module_result < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
     pystate_addmodule_run = 1;
   }
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
@@ -27985,15 +27985,15 @@
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
 }
 #endif
-  __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit_PynyHTM(void)", 0);
+  __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit_pynyhtm(void)", 0);
   if (__Pyx_check_binary_version(__PYX_LIMITED_VERSION_HEX, __Pyx_get_runtime_version(), CYTHON_COMPILING_IN_LIMITED_API) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -28023,22 +28023,22 @@
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   stringtab_initialized = 1;
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
-  if (__pyx_module_is_main_PynyHTM) {
+  if (__pyx_module_is_main_pynyhtm) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
-    if (!PyDict_GetItemString(modules, "PynyHTM")) {
-      if (unlikely((PyDict_SetItemString(modules, "PynyHTM", __pyx_m) < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
+    if (!PyDict_GetItemString(modules, "pynyhtm")) {
+      if (unlikely((PyDict_SetItemString(modules, "pynyhtm", __pyx_m) < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -28081,15 +28081,15 @@
  * def lib_get_license() -> str:             # <<<<<<<<<<<<<<
  *     """Retrieves the licence from the compiled library."""
  *     cdef const char* license = get_license()
  */
   __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_str) < 0) __PYX_ERR(0, 10, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_1lib_get_license, 0, __pyx_n_s_lib_get_license, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_1lib_get_license, 0, __pyx_n_s_lib_get_license, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_lib_get_license, __pyx_t_2) < 0) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pynyhtm.pyx":40
@@ -28106,15 +28106,15 @@
   __Pyx_GIVEREF(__pyx_t_2);
   if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2)) __PYX_ERR(0, 40, __pyx_L1_error);
   __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_PEP560_update_bases(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_2, __pyx_n_s_Errorcode, __pyx_n_s_Errorcode, (PyObject *) NULL, __pyx_n_s_PynyHTM, __pyx_kp_s_Errorcodes_used_by_libtinyhtm); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_2, __pyx_n_s_Errorcode, __pyx_n_s_Errorcode, (PyObject *) NULL, __pyx_n_s_pynyhtm, __pyx_kp_s_Errorcodes_used_by_libtinyhtm); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (__pyx_t_2 != __pyx_t_3) {
     if (unlikely((PyDict_SetItemString(__pyx_t_5, "__orig_bases__", __pyx_t_3) < 0))) __PYX_ERR(0, 40, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "pynyhtm.pyx":42
@@ -28279,28 +28279,28 @@
   /* "pynyhtm.pyx":91
  * 
  * 
  * class SphericalCoordinate():             # <<<<<<<<<<<<<<
  *     """Wrapping class for the htm_sc struct."""
  * 
  */
-  __pyx_t_2 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_SphericalCoordinate_2, __pyx_n_s_SphericalCoordinate_2, (PyObject *) NULL, __pyx_n_s_PynyHTM, __pyx_kp_s_Wrapping_class_for_the_htm_sc_st); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 91, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_SphericalCoordinate_2, __pyx_n_s_SphericalCoordinate_2, (PyObject *) NULL, __pyx_n_s_pynyhtm, __pyx_kp_s_Wrapping_class_for_the_htm_sc_st); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
   /* "pynyhtm.pyx":94
  *     """Wrapping class for the htm_sc struct."""
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def latitude(self) -> float:
  *         """Latitude of this spherical coordinate."""
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 94, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_19SphericalCoordinate_1latitude, 0, __pyx_n_s_SphericalCoordinate_latitude, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_19SphericalCoordinate_1latitude, 0, __pyx_n_s_SphericalCoordinate_latitude, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_latitude_2, __pyx_t_4) < 0) __PYX_ERR(0, 94, __pyx_L1_error)
@@ -28312,15 +28312,15 @@
  *     @property             # <<<<<<<<<<<<<<
  *     def longitude(self) -> float:
  *         """Longitude of this spherical coordinate."""
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_19SphericalCoordinate_3longitude, 0, __pyx_n_s_SphericalCoordinate_longitude, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_19SphericalCoordinate_3longitude, 0, __pyx_n_s_SphericalCoordinate_longitude, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_longitude_2, __pyx_t_4) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
@@ -28334,41 +28334,41 @@
  *         Initializes this spherical coordinate with given latitude and longitude.
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 104, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_latitude_2, __pyx_n_s_float) < 0) __PYX_ERR(0, 104, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_longitude_2, __pyx_n_s_float) < 0) __PYX_ERR(0, 104, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(0, 104, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_19SphericalCoordinate_5__init__, 0, __pyx_n_s_SphericalCoordinate___init, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__22)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 104, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_19SphericalCoordinate_5__init__, 0, __pyx_n_s_SphericalCoordinate___init, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__22)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 104, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_init, __pyx_t_5) < 0) __PYX_ERR(0, 104, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "pynyhtm.pyx":114
  *         self._longitude=longitude
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         """Detailed representation of this SphericalCoordinate."""
  *         return f"SphericalCoordinate({str(self.__dict__)})"
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_19SphericalCoordinate_7__repr__, 0, __pyx_n_s_SphericalCoordinate___repr, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 114, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_19SphericalCoordinate_7__repr__, 0, __pyx_n_s_SphericalCoordinate___repr, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 114, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_repr, __pyx_t_5) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "pynyhtm.pyx":118
  *         return f"SphericalCoordinate({str(self.__dict__)})"
  * 
  *     def get_htm_sc(self):             # <<<<<<<<<<<<<<
  *         """Gets a htm_sc strcut based on this spherical coordinate."""
  *         return htm_sc(self._longitude, self._latitude)
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_19SphericalCoordinate_9get_htm_sc, 0, __pyx_n_s_SphericalCoordinate_get_htm_sc, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 118, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_19SphericalCoordinate_9get_htm_sc, 0, __pyx_n_s_SphericalCoordinate_get_htm_sc, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 118, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_get_htm_sc, __pyx_t_5) < 0) __PYX_ERR(0, 118, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "pynyhtm.pyx":122
  *         return htm_sc(self._longitude, self._latitude)
  * 
@@ -28376,15 +28376,15 @@
  *         """
  *         Creates a Spherical coordinate based on a htm_sc struct.
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_sc, __pyx_n_s_htm_sc) < 0) __PYX_ERR(0, 122, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_SphericalCoordinate_2) < 0) __PYX_ERR(0, 122, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_19SphericalCoordinate_11from_htm_sc, 0, __pyx_n_s_SphericalCoordinate_from_htm_sc, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__26)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 122, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_19SphericalCoordinate_11from_htm_sc, 0, __pyx_n_s_SphericalCoordinate_from_htm_sc, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__26)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_from_htm_sc, __pyx_t_4) < 0) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "pynyhtm.pyx":137
@@ -28393,15 +28393,15 @@
  *     def to_v3(self) -> V3:             # <<<<<<<<<<<<<<
  *         """
  *         Transforms this spherical coordinate into a v3 vector.
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_V3) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_19SphericalCoordinate_13to_v3, 0, __pyx_n_s_SphericalCoordinate_to_v3, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__28)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 137, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_19SphericalCoordinate_13to_v3, 0, __pyx_n_s_SphericalCoordinate_to_v3, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__28)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_to_v3, __pyx_t_5) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "pynyhtm.pyx":149
@@ -28411,15 +28411,15 @@
  *         """
  *         Determine the angle difference between the two given spherical coordinates.
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_other, __pyx_n_s_SphericalCoordinate_2) < 0) __PYX_ERR(0, 149, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 149, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_19SphericalCoordinate_15angle_separation, 0, __pyx_n_s_SphericalCoordinate_angle_separa, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__30)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_19SphericalCoordinate_15angle_separation, 0, __pyx_n_s_SphericalCoordinate_angle_separa, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__30)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_angle_separation, __pyx_t_4) < 0) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "pynyhtm.pyx":158
@@ -28429,15 +28429,15 @@
  *         """Gets the HTM id for this spherical coordinate at the given level.
  * 
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 158, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_level, __pyx_n_s_int) < 0) __PYX_ERR(0, 158, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_int64_t) < 0) __PYX_ERR(0, 158, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_19SphericalCoordinate_17get_htm_id, 0, __pyx_n_s_SphericalCoordinate_get_htm_id, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 158, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_19SphericalCoordinate_17get_htm_id, 0, __pyx_n_s_SphericalCoordinate_get_htm_id, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 158, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_get_htm_id, __pyx_t_5) < 0) __PYX_ERR(0, 158, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "pynyhtm.pyx":91
@@ -28456,28 +28456,28 @@
   /* "pynyhtm.pyx":168
  * 
  * 
  * class V3():             # <<<<<<<<<<<<<<
  *     """Wrapping class for the v3 struct (vector)."""
  * 
  */
-  __pyx_t_2 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_V3, __pyx_n_s_V3, (PyObject *) NULL, __pyx_n_s_PynyHTM, __pyx_kp_s_Wrapping_class_for_the_v3_struct); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 168, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_V3, __pyx_n_s_V3, (PyObject *) NULL, __pyx_n_s_pynyhtm, __pyx_kp_s_Wrapping_class_for_the_v3_struct); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 168, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
   /* "pynyhtm.pyx":171
  *     """Wrapping class for the v3 struct (vector)."""
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def x(self) -> float:
  *         """X coordinate of this vector."""
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 171, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 171, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_2V3_1x, 0, __pyx_n_s_V3_x, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 171, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_2V3_1x, 0, __pyx_n_s_V3_x, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 171, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 171, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_x, __pyx_t_5) < 0) __PYX_ERR(0, 171, __pyx_L1_error)
@@ -28489,15 +28489,15 @@
  *     @property             # <<<<<<<<<<<<<<
  *     def y(self) -> float:
  *         """Y coordinate of this vector."""
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 176, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 176, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_2V3_3y, 0, __pyx_n_s_V3_y, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__34)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 176, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_2V3_3y, 0, __pyx_n_s_V3_y, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__34)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 176, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 176, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_y, __pyx_t_5) < 0) __PYX_ERR(0, 176, __pyx_L1_error)
@@ -28509,15 +28509,15 @@
  *     @property             # <<<<<<<<<<<<<<
  *     def z(self) -> float:
  *         """Z coordinate of this vector."""
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 181, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 181, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_2V3_5z, 0, __pyx_n_s_V3_z, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__35)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_2V3_5z, 0, __pyx_n_s_V3_z, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__35)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 181, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 181, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_z, __pyx_t_5) < 0) __PYX_ERR(0, 181, __pyx_L1_error)
@@ -28532,41 +28532,41 @@
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 186, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_x, __pyx_n_s_float) < 0) __PYX_ERR(0, 186, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_y, __pyx_n_s_float) < 0) __PYX_ERR(0, 186, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_z, __pyx_n_s_float) < 0) __PYX_ERR(0, 186, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(0, 186, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_2V3_7__init__, 0, __pyx_n_s_V3___init, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__37)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 186, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_2V3_7__init__, 0, __pyx_n_s_V3___init, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__37)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 186, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 186, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "pynyhtm.pyx":198
  *         self._z=z
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         """Detailed representation of this V3 Vector."""
  *         return f"V3({str(self.__dict__)})"
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_2V3_9__repr__, 0, __pyx_n_s_V3___repr, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__38)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_2V3_9__repr__, 0, __pyx_n_s_V3___repr, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__38)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_repr, __pyx_t_4) < 0) __PYX_ERR(0, 198, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "pynyhtm.pyx":202
  *         return f"V3({str(self.__dict__)})"
  * 
  *     def get_htm_v3(self):             # <<<<<<<<<<<<<<
  *         """Gets a htm_v3 strcut based on this v3 object."""
  *         return htm_v3(self._x, self._y, self._z)
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_2V3_11get_htm_v3, 0, __pyx_n_s_V3_get_htm_v3, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 202, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_2V3_11get_htm_v3, 0, __pyx_n_s_V3_get_htm_v3, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_get_htm_v3, __pyx_t_4) < 0) __PYX_ERR(0, 202, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "pynyhtm.pyx":206
  *         return htm_v3(self._x, self._y, self._z)
  * 
@@ -28574,15 +28574,15 @@
  *         """
  *         Creates a V3 object based on a htm_v3 struct.
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 206, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_v3, __pyx_n_s_htm_v3) < 0) __PYX_ERR(0, 206, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_V3) < 0) __PYX_ERR(0, 206, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_2V3_13from_htm_v3, 0, __pyx_n_s_V3_from_htm_v3, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__41)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 206, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_2V3_13from_htm_v3, 0, __pyx_n_s_V3_from_htm_v3, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__41)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 206, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_from_htm_v3, __pyx_t_5) < 0) __PYX_ERR(0, 206, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "pynyhtm.pyx":222
@@ -28591,15 +28591,15 @@
  *     def to_sc(self) -> SphericalCoordinate:             # <<<<<<<<<<<<<<
  *         """
  *         Transforms this V3 vector into a sphercial coordinate.
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 222, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_SphericalCoordinate_2) < 0) __PYX_ERR(0, 222, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_2V3_15to_sc, 0, __pyx_n_s_V3_to_sc, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__43)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 222, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_2V3_15to_sc, 0, __pyx_n_s_V3_to_sc, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__43)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 222, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_to_sc, __pyx_t_4) < 0) __PYX_ERR(0, 222, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "pynyhtm.pyx":234
@@ -28609,15 +28609,15 @@
  *         """Gets the HTM id for this v3 vector at the given level.
  * 
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 234, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_level, __pyx_n_s_int) < 0) __PYX_ERR(0, 234, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_int64_t) < 0) __PYX_ERR(0, 234, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_2V3_17get_htm_id, 0, __pyx_n_s_V3_get_htm_id, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 234, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_2V3_17get_htm_id, 0, __pyx_n_s_V3_get_htm_id, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 234, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_get_htm_id, __pyx_t_5) < 0) __PYX_ERR(0, 234, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "pynyhtm.pyx":243
@@ -28627,15 +28627,15 @@
  *         """
  *         Adds the other vector to this vector.
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 243, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_other, __pyx_n_s_V3) < 0) __PYX_ERR(0, 243, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_V3) < 0) __PYX_ERR(0, 243, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_2V3_19add, 0, __pyx_n_s_V3_add, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__46)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_2V3_19add, 0, __pyx_n_s_V3_add, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__46)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 243, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_add, __pyx_t_4) < 0) __PYX_ERR(0, 243, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "pynyhtm.pyx":256
@@ -28645,15 +28645,15 @@
  *         return self.add(other)
  * 
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_other, __pyx_n_s_V3) < 0) __PYX_ERR(0, 256, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_V3) < 0) __PYX_ERR(0, 256, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_2V3_21__add__, 0, __pyx_n_s_V3___add, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__47)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 256, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_2V3_21__add__, 0, __pyx_n_s_V3___add, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__47)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_add_2, __pyx_t_5) < 0) __PYX_ERR(0, 256, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "pynyhtm.pyx":259
@@ -28663,15 +28663,15 @@
  *         """
  *         Subtracts other from this vector.
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_other, __pyx_n_s_V3) < 0) __PYX_ERR(0, 259, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_V3) < 0) __PYX_ERR(0, 259, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_2V3_23sub, 0, __pyx_n_s_V3_sub, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__48)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 259, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_2V3_23sub, 0, __pyx_n_s_V3_sub, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__48)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_sub, __pyx_t_4) < 0) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "pynyhtm.pyx":272
@@ -28681,15 +28681,15 @@
  *         return self.sub(other)
  * 
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 272, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_other, __pyx_n_s_V3) < 0) __PYX_ERR(0, 272, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_V3) < 0) __PYX_ERR(0, 272, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_2V3_25__sub__, 0, __pyx_n_s_V3___sub, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__49)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 272, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_2V3_25__sub__, 0, __pyx_n_s_V3___sub, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__49)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 272, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_sub_2, __pyx_t_5) < 0) __PYX_ERR(0, 272, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "pynyhtm.pyx":275
@@ -28698,15 +28698,15 @@
  *     def neg(self) -> V3:             # <<<<<<<<<<<<<<
  *         """
  *         Negates this vector.
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 275, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_V3) < 0) __PYX_ERR(0, 275, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_2V3_27neg, 0, __pyx_n_s_V3_neg, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__51)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 275, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_2V3_27neg, 0, __pyx_n_s_V3_neg, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__51)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 275, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_neg, __pyx_t_4) < 0) __PYX_ERR(0, 275, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "pynyhtm.pyx":284
@@ -28715,15 +28715,15 @@
  *     def __neg__(self) -> V3:             # <<<<<<<<<<<<<<
  *         return self.neg()
  * 
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_V3) < 0) __PYX_ERR(0, 284, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_2V3_29__neg__, 0, __pyx_n_s_V3___neg, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__52)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 284, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_2V3_29__neg__, 0, __pyx_n_s_V3___neg, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__52)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_neg_2, __pyx_t_5) < 0) __PYX_ERR(0, 284, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "pynyhtm.pyx":287
@@ -28733,15 +28733,15 @@
  *         """
  *         Scalar multiplication with this v3.
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_scalar, __pyx_n_s_float) < 0) __PYX_ERR(0, 287, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_V3) < 0) __PYX_ERR(0, 287, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_2V3_31mul, 0, __pyx_n_s_V3_mul, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__54)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 287, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_2V3_31mul, 0, __pyx_n_s_V3_mul, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__54)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_mul, __pyx_t_4) < 0) __PYX_ERR(0, 287, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "pynyhtm.pyx":300
@@ -28751,15 +28751,15 @@
  *         return self.mul(scalar)
  * 
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 300, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_scalar, __pyx_n_s_float) < 0) __PYX_ERR(0, 300, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_V3) < 0) __PYX_ERR(0, 300, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_2V3_33__mul__, 0, __pyx_n_s_V3___mul, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__56)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 300, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_2V3_33__mul__, 0, __pyx_n_s_V3___mul, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__56)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 300, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_mul_2, __pyx_t_5) < 0) __PYX_ERR(0, 300, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "pynyhtm.pyx":303
@@ -28769,15 +28769,15 @@
  *         """
  *         Scalar division with this v3.
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 303, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_scalar, __pyx_n_s_float) < 0) __PYX_ERR(0, 303, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_V3) < 0) __PYX_ERR(0, 303, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_2V3_35div, 0, __pyx_n_s_V3_div, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__57)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 303, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_2V3_35div, 0, __pyx_n_s_V3_div, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__57)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 303, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_div, __pyx_t_4) < 0) __PYX_ERR(0, 303, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "pynyhtm.pyx":319
@@ -28787,15 +28787,15 @@
  *         return self.div(scalar)
  * 
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 319, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_scalar, __pyx_n_s_float) < 0) __PYX_ERR(0, 319, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_V3) < 0) __PYX_ERR(0, 319, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_2V3_37__truediv__, 0, __pyx_n_s_V3___truediv, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__58)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 319, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_2V3_37__truediv__, 0, __pyx_n_s_V3___truediv, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__58)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 319, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_truediv, __pyx_t_5) < 0) __PYX_ERR(0, 319, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "pynyhtm.pyx":168
@@ -28819,15 +28819,15 @@
  *     Wraps htm_sc_init, instantiates a htm_sc struct.
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 323, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_latitude_2, __pyx_n_s_float) < 0) __PYX_ERR(0, 323, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_longitude_2, __pyx_n_s_float) < 0) __PYX_ERR(0, 323, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_kp_s_tuple_htm_errcode_htm_sc) < 0) __PYX_ERR(0, 323, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_3htm_sc_init_raw, 0, __pyx_n_s_htm_sc_init_raw, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__60)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 323, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_3htm_sc_init_raw, 0, __pyx_n_s_htm_sc_init_raw, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__60)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 323, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_htm_sc_init_raw, __pyx_t_5) < 0) __PYX_ERR(0, 323, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "pynyhtm.pyx":337
@@ -28838,15 +28838,15 @@
  *     Wraps htm_sc_init, instantiates a wrapped htm_sc struct with given latitude and longitude.
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 337, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_latitude_2, __pyx_n_s_float) < 0) __PYX_ERR(0, 337, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_longitude_2, __pyx_n_s_float) < 0) __PYX_ERR(0, 337, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_SphericalCoordinate_2) < 0) __PYX_ERR(0, 337, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_5htm_sc_init_wrapped, 0, __pyx_n_s_htm_sc_init_wrapped, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__62)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 337, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_5htm_sc_init_wrapped, 0, __pyx_n_s_htm_sc_init_wrapped, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__62)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 337, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_htm_sc_init_wrapped, __pyx_t_2) < 0) __PYX_ERR(0, 337, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pynyhtm.pyx":352
@@ -28857,15 +28857,15 @@
  *     Determine the angle difference between the two given spherical coordinates.
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 352, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_sc1, __pyx_n_s_htm_sc) < 0) __PYX_ERR(0, 352, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_sc2, __pyx_n_s_htm_sc) < 0) __PYX_ERR(0, 352, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 352, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_7htm_sc_angsep_raw, 0, __pyx_n_s_htm_sc_angsep_raw, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__64)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 352, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_7htm_sc_angsep_raw, 0, __pyx_n_s_htm_sc_angsep_raw, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__64)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 352, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_htm_sc_angsep_raw, __pyx_t_5) < 0) __PYX_ERR(0, 352, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "pynyhtm.pyx":363
@@ -28877,15 +28877,15 @@
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 363, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_x, __pyx_n_s_float) < 0) __PYX_ERR(0, 363, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_y, __pyx_n_s_float) < 0) __PYX_ERR(0, 363, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_z, __pyx_n_s_float) < 0) __PYX_ERR(0, 363, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_kp_s_tuple_htm_errcode_htm_v3) < 0) __PYX_ERR(0, 363, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_9htm_v3_init_raw, 0, __pyx_n_s_htm_v3_init_raw, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__66)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 363, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_9htm_v3_init_raw, 0, __pyx_n_s_htm_v3_init_raw, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__66)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 363, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_htm_v3_init_raw, __pyx_t_2) < 0) __PYX_ERR(0, 363, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pynyhtm.pyx":378
@@ -28897,15 +28897,15 @@
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 378, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_x, __pyx_n_s_float) < 0) __PYX_ERR(0, 378, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_y, __pyx_n_s_float) < 0) __PYX_ERR(0, 378, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_z, __pyx_n_s_float) < 0) __PYX_ERR(0, 378, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_V3) < 0) __PYX_ERR(0, 378, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_11htm_v3_init_wrapped, 0, __pyx_n_s_htm_v3_init_wrapped, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__68)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 378, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_11htm_v3_init_wrapped, 0, __pyx_n_s_htm_v3_init_wrapped, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__68)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 378, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_htm_v3_init_wrapped, __pyx_t_5) < 0) __PYX_ERR(0, 378, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "pynyhtm.pyx":394
@@ -28915,15 +28915,15 @@
  *     """
  *     Wraps htm_sc_tov3, transforms a htm_sc struct into a htm_v3 struct.
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 394, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_sc, __pyx_n_s_htm_sc) < 0) __PYX_ERR(0, 394, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_kp_s_tuple_htm_errcode_htm_v3) < 0) __PYX_ERR(0, 394, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_13htm_sc_to_v3_raw, 0, __pyx_n_s_htm_sc_to_v3_raw, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__70)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 394, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_13htm_sc_to_v3_raw, 0, __pyx_n_s_htm_sc_to_v3_raw, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__70)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 394, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_htm_sc_to_v3_raw, __pyx_t_2) < 0) __PYX_ERR(0, 394, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pynyhtm.pyx":407
@@ -28933,15 +28933,15 @@
  *     """
  *     Wraps htm_v3_tosc, transforms a htm_v3 struct into a htm_sc struct.
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 407, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_v3, __pyx_n_s_htm_v3) < 0) __PYX_ERR(0, 407, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_kp_s_tuple_htm_errcode_htm_sc) < 0) __PYX_ERR(0, 407, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_15htm_v3_to_sc_raw, 0, __pyx_n_s_htm_v3_to_sc_raw, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__72)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 407, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_15htm_v3_to_sc_raw, 0, __pyx_n_s_htm_v3_to_sc_raw, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__72)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 407, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_htm_v3_to_sc_raw, __pyx_t_5) < 0) __PYX_ERR(0, 407, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "pynyhtm.pyx":420
@@ -28952,15 +28952,15 @@
  *     Adds two vectors.
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 420, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_v1, __pyx_n_s_htm_v3) < 0) __PYX_ERR(0, 420, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_v2, __pyx_n_s_htm_v3) < 0) __PYX_ERR(0, 420, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_htm_v3) < 0) __PYX_ERR(0, 420, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_17htm_v3_add_raw, 0, __pyx_n_s_htm_v3_add_raw, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__74)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 420, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_17htm_v3_add_raw, 0, __pyx_n_s_htm_v3_add_raw, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__74)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 420, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_htm_v3_add_raw, __pyx_t_2) < 0) __PYX_ERR(0, 420, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pynyhtm.pyx":433
@@ -28971,15 +28971,15 @@
  *     Subtracts two vectors.
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 433, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_v1, __pyx_n_s_htm_v3) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_v2, __pyx_n_s_htm_v3) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_htm_v3) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_19htm_v3_sub_raw, 0, __pyx_n_s_htm_v3_sub_raw, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__75)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 433, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_19htm_v3_sub_raw, 0, __pyx_n_s_htm_v3_sub_raw, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__75)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 433, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_htm_v3_sub_raw, __pyx_t_5) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "pynyhtm.pyx":446
@@ -28989,15 +28989,15 @@
  *     """
  *     Negates the given vector.
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 446, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_v1, __pyx_n_s_htm_v3) < 0) __PYX_ERR(0, 446, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_htm_v3) < 0) __PYX_ERR(0, 446, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_21htm_v3_neg_raw, 0, __pyx_n_s_htm_v3_neg_raw, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__77)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 446, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_21htm_v3_neg_raw, 0, __pyx_n_s_htm_v3_neg_raw, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__77)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 446, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_htm_v3_neg_raw, __pyx_t_2) < 0) __PYX_ERR(0, 446, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pynyhtm.pyx":458
@@ -29008,15 +29008,15 @@
  *     Scalar vector multiplication.
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 458, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_v1, __pyx_n_s_htm_v3) < 0) __PYX_ERR(0, 458, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_scalar, __pyx_n_s_float) < 0) __PYX_ERR(0, 458, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_htm_v3) < 0) __PYX_ERR(0, 458, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_23htm_v3_mul_raw, 0, __pyx_n_s_htm_v3_mul_raw, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__79)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 458, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_23htm_v3_mul_raw, 0, __pyx_n_s_htm_v3_mul_raw, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__79)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 458, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_htm_v3_mul_raw, __pyx_t_5) < 0) __PYX_ERR(0, 458, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "pynyhtm.pyx":471
@@ -29027,42 +29027,42 @@
  *     Scalar vector division.
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 471, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_v1, __pyx_n_s_htm_v3) < 0) __PYX_ERR(0, 471, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_scalar, __pyx_n_s_float) < 0) __PYX_ERR(0, 471, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_htm_v3) < 0) __PYX_ERR(0, 471, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_25htm_v3_div_raw, 0, __pyx_n_s_htm_v3_div_raw, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__80)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 471, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_25htm_v3_div_raw, 0, __pyx_n_s_htm_v3_div_raw, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__80)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 471, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_htm_v3_div_raw, __pyx_t_2) < 0) __PYX_ERR(0, 471, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pynyhtm.pyx":516
  * 
  * 
  * class Triangle():             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
-  __pyx_t_2 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_Triangle_2, __pyx_n_s_Triangle_2, (PyObject *) NULL, __pyx_n_s_PynyHTM, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 516, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_Triangle_2, __pyx_n_s_Triangle_2, (PyObject *) NULL, __pyx_n_s_pynyhtm, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 516, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
   /* "pynyhtm.pyx":518
  * class Triangle():
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def vertices(self) -> V3[3]:
  *         """Vertices making up this triangle."""
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 518, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_kp_s_V3_3) < 0) __PYX_ERR(0, 518, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_8Triangle_1vertices, 0, __pyx_n_s_Triangle_vertices, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__81)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 518, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_8Triangle_1vertices, 0, __pyx_n_s_Triangle_vertices, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__81)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 518, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 518, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_vertices_2, __pyx_t_5) < 0) __PYX_ERR(0, 518, __pyx_L1_error)
@@ -29074,15 +29074,15 @@
  *     @property             # <<<<<<<<<<<<<<
  *     def center(self) -> V3:
  *         """Center point of this triangle."""
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 523, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_V3) < 0) __PYX_ERR(0, 523, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_8Triangle_3center, 0, __pyx_n_s_Triangle_center, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__82)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 523, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_8Triangle_3center, 0, __pyx_n_s_Triangle_center, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__82)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 523, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 523, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_center, __pyx_t_5) < 0) __PYX_ERR(0, 523, __pyx_L1_error)
@@ -29094,15 +29094,15 @@
  *     @property             # <<<<<<<<<<<<<<
  *     def radius(self) -> float:
  *         """Radius of the circle given by the three corners of the triangle."""
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 528, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 528, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_8Triangle_5radius, 0, __pyx_n_s_Triangle_radius, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__83)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 528, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_8Triangle_5radius, 0, __pyx_n_s_Triangle_radius, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__83)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 528, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 528, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_radius, __pyx_t_5) < 0) __PYX_ERR(0, 528, __pyx_L1_error)
@@ -29114,15 +29114,15 @@
  *     @property             # <<<<<<<<<<<<<<
  *     def id(self) -> int64_t:
  *         """HTM ID of this triangle."""
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 533, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_int64_t) < 0) __PYX_ERR(0, 533, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_8Triangle_7id, 0, __pyx_n_s_Triangle_id, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__84)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 533, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_8Triangle_7id, 0, __pyx_n_s_Triangle_id, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__84)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 533, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 533, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_id, __pyx_t_5) < 0) __PYX_ERR(0, 533, __pyx_L1_error)
@@ -29134,15 +29134,15 @@
  *     @property             # <<<<<<<<<<<<<<
  *     def level(self) -> int:
  *         """Level at which this triangle is within the htm."""
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 538, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_int) < 0) __PYX_ERR(0, 538, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_8Triangle_9level, 0, __pyx_n_s_Triangle_level, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__85)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 538, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_8Triangle_9level, 0, __pyx_n_s_Triangle_level, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__85)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 538, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_property, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 538, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_level, __pyx_t_5) < 0) __PYX_ERR(0, 538, __pyx_L1_error)
@@ -29159,29 +29159,29 @@
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_vertices_2, __pyx_kp_s_V3_3) < 0) __PYX_ERR(0, 543, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_center, __pyx_n_s_V3) < 0) __PYX_ERR(0, 543, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_radius, __pyx_n_s_float) < 0) __PYX_ERR(0, 543, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_id, __pyx_n_s_int) < 0) __PYX_ERR(0, 543, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_level, __pyx_n_s_int) < 0) __PYX_ERR(0, 543, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(0, 543, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_8Triangle_11__init__, 0, __pyx_n_s_Triangle___init, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__87)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 543, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_8Triangle_11__init__, 0, __pyx_n_s_Triangle___init, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__87)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 543, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 543, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "pynyhtm.pyx":559
  *         self._level = level
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         """Detailed representation of this Triangle."""
  *         return f"Triangle({str(self.__dict__)})"
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_8Triangle_13__repr__, 0, __pyx_n_s_Triangle___repr, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__88)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 559, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_8Triangle_13__repr__, 0, __pyx_n_s_Triangle___repr, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__88)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 559, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_repr, __pyx_t_4) < 0) __PYX_ERR(0, 559, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "pynyhtm.pyx":563
  *         return f"Triangle({str(self.__dict__)})"
  * 
@@ -29189,15 +29189,15 @@
  *         """
  *         Instantiates a triangle based on a htm_tri struct.
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 563, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_struct, __pyx_n_s_htm_tri) < 0) __PYX_ERR(0, 563, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_Triangle_2) < 0) __PYX_ERR(0, 563, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_8Triangle_15from_htm_tri, 0, __pyx_n_s_Triangle_from_htm_tri, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__90)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 563, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_8Triangle_15from_htm_tri, 0, __pyx_n_s_Triangle_from_htm_tri, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__90)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 563, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_5, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_from_htm_tri, __pyx_t_5) < 0) __PYX_ERR(0, 563, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "pynyhtm.pyx":578
@@ -29207,15 +29207,15 @@
  *         """
  *         Instantiates a Triangle object from a given htm id.
  */
   __pyx_t_5 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 578, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_id, __pyx_n_s_int64_t) < 0) __PYX_ERR(0, 578, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_return, __pyx_n_s_Triangle_2) < 0) __PYX_ERR(0, 578, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_8Triangle_17from_id, 0, __pyx_n_s_Triangle_from_id, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__92)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 578, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_8Triangle_17from_id, 0, __pyx_n_s_Triangle_from_id, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__92)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 578, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_from_id, __pyx_t_4) < 0) __PYX_ERR(0, 578, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "pynyhtm.pyx":516
@@ -29239,15 +29239,15 @@
  *     Retrieves the trixel is for a given v3.
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 588, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_v, __pyx_n_s_htm_v3) < 0) __PYX_ERR(0, 588, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_level, __pyx_n_s_int) < 0) __PYX_ERR(0, 588, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_int64_t) < 0) __PYX_ERR(0, 588, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_27htm_v3_id_raw, 0, __pyx_n_s_htm_v3_id_raw, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__94)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 588, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_27htm_v3_id_raw, 0, __pyx_n_s_htm_v3_id_raw, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__94)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 588, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_htm_v3_id_raw, __pyx_t_4) < 0) __PYX_ERR(0, 588, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "pynyhtm.pyx":599
@@ -29257,15 +29257,15 @@
  *     """
  *     Instantiate a htm_tri struct for a given triangle id.
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 599, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_id, __pyx_n_s_int64_t) < 0) __PYX_ERR(0, 599, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_kp_s_tuple_htm_errcode_htm_tri) < 0) __PYX_ERR(0, 599, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_29htm_tri_init_raw, 0, __pyx_n_s_htm_tri_init_raw, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__96)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 599, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_29htm_tri_init_raw, 0, __pyx_n_s_htm_tri_init_raw, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__96)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 599, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_htm_tri_init_raw, __pyx_t_2) < 0) __PYX_ERR(0, 599, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pynyhtm.pyx":611
@@ -29275,15 +29275,15 @@
  *     """
  *     Instantiate a Triangle object for a given triangle id.
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 611, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_id, __pyx_n_s_int64_t) < 0) __PYX_ERR(0, 611, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_Triangle_2) < 0) __PYX_ERR(0, 611, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_31htm_tri_init_wrapped, 0, __pyx_n_s_htm_tri_init_wrapped, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__98)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 611, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_31htm_tri_init_wrapped, 0, __pyx_n_s_htm_tri_init_wrapped, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__98)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 611, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_htm_tri_init_wrapped, __pyx_t_4) < 0) __PYX_ERR(0, 611, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "pynyhtm.pyx":629
@@ -29300,15 +29300,15 @@
   __Pyx_GIVEREF(__pyx_t_4);
   if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_4)) __PYX_ERR(0, 629, __pyx_L1_error);
   __pyx_t_4 = 0;
   __pyx_t_4 = __Pyx_PEP560_update_bases(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 629, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = __Pyx_CalculateMetaclass(NULL, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 629, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_5, __pyx_t_4, __pyx_n_s_NeighborDirection, __pyx_n_s_NeighborDirection, (PyObject *) NULL, __pyx_n_s_PynyHTM, __pyx_kp_s_Direction_in_which_the_neighbor); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 629, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_5, __pyx_t_4, __pyx_n_s_NeighborDirection, __pyx_n_s_NeighborDirection, (PyObject *) NULL, __pyx_n_s_pynyhtm, __pyx_kp_s_Direction_in_which_the_neighbor); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 629, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__pyx_t_4 != __pyx_t_2) {
     if (unlikely((PyDict_SetItemString(__pyx_t_3, "__orig_bases__", __pyx_t_2) < 0))) __PYX_ERR(0, 629, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pynyhtm.pyx":634
@@ -29367,15 +29367,15 @@
   __Pyx_GIVEREF(__pyx_t_4);
   if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4)) __PYX_ERR(0, 639, __pyx_L1_error);
   __pyx_t_4 = 0;
   __pyx_t_4 = __Pyx_PEP560_update_bases(__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 639, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_3 = __Pyx_CalculateMetaclass(NULL, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 639, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_Py3MetaclassPrepare(__pyx_t_3, __pyx_t_4, __pyx_n_s_FlipDirection, __pyx_n_s_FlipDirection, (PyObject *) NULL, __pyx_n_s_PynyHTM, __pyx_kp_s_The_direction_in_which_the_looku); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 639, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Py3MetaclassPrepare(__pyx_t_3, __pyx_t_4, __pyx_n_s_FlipDirection, __pyx_n_s_FlipDirection, (PyObject *) NULL, __pyx_n_s_pynyhtm, __pyx_kp_s_The_direction_in_which_the_looku); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 639, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__pyx_t_4 != __pyx_t_5) {
     if (unlikely((PyDict_SetItemString(__pyx_t_2, "__orig_bases__", __pyx_t_5) < 0))) __PYX_ERR(0, 639, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "pynyhtm.pyx":641
@@ -29423,29 +29423,29 @@
   /* "pynyhtm.pyx":646
  * 
  * 
  * class HTM():             # <<<<<<<<<<<<<<
  * 
  *     def get_level(id: int64_t) -> int:
  */
-  __pyx_t_4 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_HTM, __pyx_n_s_HTM, (PyObject *) NULL, __pyx_n_s_PynyHTM, (PyObject *) NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 646, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_HTM, __pyx_n_s_HTM, (PyObject *) NULL, __pyx_n_s_pynyhtm, (PyObject *) NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 646, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
 
   /* "pynyhtm.pyx":648
  * class HTM():
  * 
  *     def get_level(id: int64_t) -> int:             # <<<<<<<<<<<<<<
  *         """
  *         Retrieves the level of a given ID.
  */
   __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 648, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_id, __pyx_n_s_int64_t) < 0) __PYX_ERR(0, 648, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_int) < 0) __PYX_ERR(0, 648, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_3HTM_1get_level, 0, __pyx_n_s_HTM_get_level, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__99)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 648, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_3HTM_1get_level, 0, __pyx_n_s_HTM_get_level, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__99)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 648, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_4, __pyx_n_s_get_level, __pyx_t_2) < 0) __PYX_ERR(0, 648, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pynyhtm.pyx":658
@@ -29455,15 +29455,15 @@
  *         """
  *         Retrieves the decimal representation of an id.
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 658, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_id, __pyx_n_s_int64_t) < 0) __PYX_ERR(0, 658, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_int64_t) < 0) __PYX_ERR(0, 658, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_3HTM_3id_to_dec, 0, __pyx_n_s_HTM_id_to_dec, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__100)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 658, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_3HTM_3id_to_dec, 0, __pyx_n_s_HTM_id_to_dec, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__100)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 658, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_4, __pyx_n_s_id_to_dec, __pyx_t_3) < 0) __PYX_ERR(0, 658, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "pynyhtm.pyx":667
@@ -29473,15 +29473,15 @@
  *         """
  *         Determines the parent id of the triangle identified by id.
  */
   __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 667, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_id, __pyx_n_s_int64_t) < 0) __PYX_ERR(0, 667, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_int64_t) < 0) __PYX_ERR(0, 667, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_3HTM_5parent, 0, __pyx_n_s_HTM_parent, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__101)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 667, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_3HTM_5parent, 0, __pyx_n_s_HTM_parent, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__101)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 667, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_4, __pyx_n_s_parent, __pyx_t_2) < 0) __PYX_ERR(0, 667, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pynyhtm.pyx":681
@@ -29491,15 +29491,15 @@
  *         """
  *         Gets the children contained in the triangle identified by id.
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 681, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_id, __pyx_n_s_int64_t) < 0) __PYX_ERR(0, 681, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_kp_s_list_int64_t) < 0) __PYX_ERR(0, 681, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_3HTM_7children, 0, __pyx_n_s_HTM_children, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__103)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 681, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_3HTM_7children, 0, __pyx_n_s_HTM_children, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__103)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 681, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_4, __pyx_n_s_children, __pyx_t_3) < 0) __PYX_ERR(0, 681, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "pynyhtm.pyx":699
@@ -29509,15 +29509,15 @@
  *         """
  *         Gets the neighboring trixels for the given id.
  */
   __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 699, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_id, __pyx_n_s_int64_t) < 0) __PYX_ERR(0, 699, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_kp_s_list_int64_t) < 0) __PYX_ERR(0, 699, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_3HTM_9neighbors, 0, __pyx_n_s_HTM_neighbors, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__104)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 699, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_3HTM_9neighbors, 0, __pyx_n_s_HTM_neighbors, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__104)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 699, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_4, __pyx_n_s_neighbors, __pyx_t_2) < 0) __PYX_ERR(0, 699, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pynyhtm.pyx":718
@@ -29528,15 +29528,15 @@
  *         Gets the neighboring trixel for the given id and direction.
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 718, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_id, __pyx_n_s_int64_t) < 0) __PYX_ERR(0, 718, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_direction, __pyx_n_s_NeighborDirection) < 0) __PYX_ERR(0, 718, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_kp_s_tuple_int64_t_bool) < 0) __PYX_ERR(0, 718, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_3HTM_11neighbor, 0, __pyx_n_s_HTM_neighbor, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__106)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 718, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_3HTM_11neighbor, 0, __pyx_n_s_HTM_neighbor, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__106)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 718, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_4, __pyx_n_s_neighbor, __pyx_t_3) < 0) __PYX_ERR(0, 718, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "pynyhtm.pyx":1047
@@ -29549,30 +29549,30 @@
   __pyx_t_3 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1047, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_center, __pyx_n_s_V3) < 0) __PYX_ERR(0, 1047, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_radius, __pyx_n_s_float) < 0) __PYX_ERR(0, 1047, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_level, __pyx_n_s_int) < 0) __PYX_ERR(0, 1047, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_max_ranges, __pyx_n_s_int) < 0) __PYX_ERR(0, 1047, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_kp_s_list_int) < 0) __PYX_ERR(0, 1047, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_3HTM_13circle_search, 0, __pyx_n_s_HTM_circle_search, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__108)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1047, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_3HTM_13circle_search, 0, __pyx_n_s_HTM_circle_search, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__108)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1047, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (!__Pyx_CyFunction_InitDefaults(__pyx_t_2, sizeof(__pyx_defaults), 1)) __PYX_ERR(0, 1047, __pyx_L1_error)
 
   /* "pynyhtm.pyx":1050
  *                       radius: float,
  *                       level: int,
  *                       max_ranges: int = 50             # <<<<<<<<<<<<<<
  *                       ) -> list[int]:
  *         """
  */
   if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_50)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_50))) __PYX_ERR(0, 1050, __pyx_L1_error)
   __Pyx_INCREF(__pyx_int_50);
   __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_t_2)->__pyx_arg_max_ranges = ((PyObject*)__pyx_int_50);
   __Pyx_GIVEREF(__pyx_int_50);
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_2, __pyx_pf_7PynyHTM_36__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_2, __pyx_pf_7pynyhtm_36__defaults__);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_4, __pyx_n_s_circle_search, __pyx_t_2) < 0) __PYX_ERR(0, 1047, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pynyhtm.pyx":646
  * 
@@ -29594,15 +29594,15 @@
  *     """
  *     Retrieves the level of a given ID.
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1079, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_id, __pyx_n_s_int64_t) < 0) __PYX_ERR(0, 1079, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_int) < 0) __PYX_ERR(0, 1079, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_33htm_level_raw, 0, __pyx_n_s_htm_level_raw, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__110)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1079, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_33htm_level_raw, 0, __pyx_n_s_htm_level_raw, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__110)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1079, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_htm_level_raw, __pyx_t_2) < 0) __PYX_ERR(0, 1079, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pynyhtm.pyx":1095
@@ -29612,15 +29612,15 @@
  *     """
  *     Retrieves the decimal representation of an id.
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1095, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_id, __pyx_n_s_int64_t) < 0) __PYX_ERR(0, 1095, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_int64_t) < 0) __PYX_ERR(0, 1095, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7PynyHTM_35htm_id_to_dec, 0, __pyx_n_s_htm_id_to_dec, NULL, __pyx_n_s_PynyHTM, __pyx_d, ((PyObject *)__pyx_codeobj__111)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1095, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7pynyhtm_35htm_id_to_dec, 0, __pyx_n_s_htm_id_to_dec, NULL, __pyx_n_s_pynyhtm, __pyx_d, ((PyObject *)__pyx_codeobj__111)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1095, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_htm_id_to_dec, __pyx_t_4) < 0) __PYX_ERR(0, 1095, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "pynyhtm.pyx":1
@@ -29639,29 +29639,29 @@
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   if (__pyx_m) {
     if (__pyx_d && stringtab_initialized) {
-      __Pyx_AddTraceback("init PynyHTM", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("init pynyhtm", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     #if !CYTHON_USE_MODULE_STATE
     Py_CLEAR(__pyx_m);
     #else
     Py_DECREF(__pyx_m);
     if (pystate_addmodule_run) {
       PyObject *tp, *value, *tb;
       PyErr_Fetch(&tp, &value, &tb);
       PyState_RemoveModule(&__pyx_moduledef);
       PyErr_Restore(tp, value, tb);
     }
     #endif
   } else if (!PyErr_Occurred()) {
-    PyErr_SetString(PyExc_ImportError, "init PynyHTM");
+    PyErr_SetString(PyExc_ImportError, "init pynyhtm");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
```

### Comparing `pynyhtm-0.0.2/pynyhtm.pyx` & `pynyhtm-0.0.3/pynyhtm.pyx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.2/pyproject.toml` & `pynyhtm-0.0.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 line-length = 120
 
 [tool.flake8]
 max-line-length = 120
 
 [tool.isort]
 profile = "black"
+known_third_party = "pynyhtm"
 
 [tool.cython-lint]
 max-line-length = 120
 
 [build-system]
 requires = [
     "setuptools",
@@ -31,16 +32,16 @@
 test-command = "pytest {project}/tests"
 
 [project.optional-dependencies]
 dev = ["black", "isort", "pytest"]
 
 
 [project]
-name = "PynyHTM"
-version = "0.0.2"
+name = "pynyhtm"
+version = "0.0.3"
 description = "Python wrapper for the libtinyhtm library."
 readme = "README.md"
 authors = [{ name = "Till", email = "till@fleisch.dev" }]
 license = { file = "LICENSE" }
 keywords = ["htm", "libtinyhtm", "hierarchial triangular mesh", "triangle subdivision", "index"]
 dependencies = [
     "numpy",
```

### Comparing `pynyhtm-0.0.2/setup.py` & `pynyhtm-0.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 proc = subprocess.Popen("make", stderr=subprocess.STDOUT, shell=True)
 output, stderr = proc.communicate(input)
 status = proc.wait()
 if status:
     raise Exception("failed to *make* libtinyhtm")
 
 pynyHTM_extension = Extension(
-    name="PynyHTM",
+    name="pynyhtm",
     sources=["pynyhtm.pyx"],
     libraries=[":libtinyhtm.a"],
     library_dirs=["."],
     include_dirs=[numpy.get_include()],
     language="c++",
     py_limited_api=True,
 )
 
-setup(name="PynyHTM", ext_modules=cythonize([pynyHTM_extension]))
+setup(name="pynyhtm", ext_modules=cythonize([pynyHTM_extension]))
```

### Comparing `pynyhtm-0.0.2/tests/test_geometry.py` & `pynyhtm-0.0.3/tests/test_geometry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,49 @@
 """Geometry related (raw) tests for the PynyHTM wrapper."""
 
+import pynyhtm
 import pytest
-
-import PynyHTM
-from PynyHTM import V3, SphericalCoordinate
+from pynyhtm import V3, SphericalCoordinate
 
 
 @pytest.mark.parametrize("lat, lon", [(0, 0), (10, 10), (5, 10), (10, 5), (-10, -10)])
 def test_sc_init_raw_valid(lat: float, lon: float):
     """Test instantiation of valid sc using raw function."""
-    ec, sc = PynyHTM.htm_sc_init_raw(lat, lon)
+    ec, sc = pynyhtm.htm_sc_init_raw(lat, lon)
     assert ec == 0
     assert sc.get("lon") == lon and sc.get("lat") == lat
 
 
 @pytest.mark.parametrize("lat, lon", [(-97, 0), (-100, 0), (-100, -100)])
 def test_sc_init_raw_invalid(lat: float, lon: float):
     """Test instantiation of invalid sc using raw function."""
-    ec, _ = PynyHTM.htm_sc_init_raw(lat, lon)
+    ec, _ = pynyhtm.htm_sc_init_raw(lat, lon)
     assert ec != 0
 
 
 @pytest.mark.parametrize("x, y, z", [(10, 10, 10), (1, 5, 10), (10, 5, 1), (-10, -5, -1)])
 def test_v3_init_raw_valid(x: float, y: float, z: float):
     """Test instantiation of valid v3 using raw function."""
-    ec, v3 = PynyHTM.htm_v3_init_raw(x, y, z)
+    ec, v3 = pynyhtm.htm_v3_init_raw(x, y, z)
     assert ec == 0
     assert v3.get("x") == x and v3.get("y") == y and v3.get("z") == z
 
 
 def test_v3_to_sc_raw():
     """Tests v3 vector conversion to spherical coordinates."""
-    _, v3 = PynyHTM.htm_v3_init_raw(1, 1, 1)
-    ec, sc = PynyHTM.htm_v3_to_sc_raw(v3)
+    _, v3 = pynyhtm.htm_v3_init_raw(1, 1, 1)
+    ec, sc = pynyhtm.htm_v3_to_sc_raw(v3)
     assert ec == 0
     assert sc.get("lat") != 0 and sc.get("lon") != 0
 
 
 def test_sc_to_v3_raw():
     """Tests vector conversion from spherical coordinates."""
-    _, sc = PynyHTM.htm_sc_init_raw(10, 10)
-    ec, v3 = PynyHTM.htm_sc_to_v3_raw(sc)
+    _, sc = pynyhtm.htm_sc_init_raw(10, 10)
+    ec, v3 = pynyhtm.htm_sc_to_v3_raw(sc)
     assert ec == 0
     assert v3.get("x") != 0 and v3.get("y") != 0 and v3.get("z") != 0
 
 
 @pytest.mark.parametrize("latitude, longitude", [(10, 0), (15, 0), (20, 20)])
 def test_sc_to_v3_to_sc(latitude: float, longitude: float):
     """Tests wrapped conversion from v3 vector to spherical coordinates."""
@@ -62,35 +61,35 @@
         (51.7444480, 10.6862911, 20, 16843849991222),
     ],
 )
 def test_v3_to_id_raw(latitude: float, longitude: float, level: float, id: int):
     """Tests trixel id wrapping for a given v3 vector."""
     sc = SphericalCoordinate(latitude, longitude)
     v3 = sc.to_v3()
-    assert PynyHTM.htm_v3_id_raw(v3.get_htm_v3(), level) == id
+    assert pynyhtm.htm_v3_id_raw(v3.get_htm_v3(), level) == id
 
 
 @pytest.mark.parametrize(
     "x1, y1, z1, x2, y2, z2",
     [
         (0, 0, 0, 0, 0, 0),
         (1, 1, 1, 0, 0, 0),
         (1, 1, 1, 1, 1, 1),
         (1, 2, 3, 4, 5, 6),
         (-1, 2, -3, -4, -5, 6),
     ],
 )
 def test_htm_v3_add_raw(x1: float, y1: float, z1: float, x2: float, y2: float, z2: float):
     """Tests addition of v3 vectors."""
-    ec, v1 = PynyHTM.htm_v3_init_raw(x1, y1, z1)
+    ec, v1 = pynyhtm.htm_v3_init_raw(x1, y1, z1)
     assert ec == 0
-    ec, v2 = PynyHTM.htm_v3_init_raw(x2, y2, z2)
+    ec, v2 = pynyhtm.htm_v3_init_raw(x2, y2, z2)
     assert ec == 0
 
-    res = PynyHTM.htm_v3_add_raw(v1, v2)
+    res = pynyhtm.htm_v3_add_raw(v1, v2)
     res = V3.from_htm_v3(res)
     assert res.x == x1 + x2 and res.y == y1 + y2 and res.z == z1 + z2
 
 
 @pytest.mark.parametrize(
     "x1, y1, z1, x2, y2, z2",
     [
@@ -99,20 +98,20 @@
         (1, 1, 1, 1, 1, 1),
         (1, 2, 3, 4, 5, 6),
         (-1, 2, -3, -4, -5, 6),
     ],
 )
 def test_htm_v3_sub_raw(x1: float, y1: float, z1: float, x2: float, y2: float, z2: float):
     """Tests subtraction of v3 vectors."""
-    ec, v1 = PynyHTM.htm_v3_init_raw(x1, y1, z1)
+    ec, v1 = pynyhtm.htm_v3_init_raw(x1, y1, z1)
     assert ec == 0
-    ec, v2 = PynyHTM.htm_v3_init_raw(x2, y2, z2)
+    ec, v2 = pynyhtm.htm_v3_init_raw(x2, y2, z2)
     assert ec == 0
 
-    res = PynyHTM.htm_v3_sub_raw(v1, v2)
+    res = pynyhtm.htm_v3_sub_raw(v1, v2)
     res = V3.from_htm_v3(res)
     assert res.x == x1 - x2 and res.y == y1 - y2 and res.z == z1 - z2
 
 
 @pytest.mark.parametrize(
     "x, y, z",
     [
@@ -120,18 +119,18 @@
         (1, 1, 1),
         (1, 2, 3),
         (-1, -2, 3),
     ],
 )
 def test_htm_v3_neg_raw(x: float, y: float, z: float):
     """Tests the negation of vectors."""
-    ec, v1 = PynyHTM.htm_v3_init_raw(x, y, z)
+    ec, v1 = pynyhtm.htm_v3_init_raw(x, y, z)
     assert ec == 0
 
-    res = PynyHTM.htm_v3_neg_raw(v1)
+    res = pynyhtm.htm_v3_neg_raw(v1)
     res = V3.from_htm_v3(res)
     assert res.x == -x and res.y == -y and res.z == -z
 
 
 @pytest.mark.parametrize(
     "x, y, z, scalar",
     [
@@ -140,18 +139,18 @@
         (1, 1, 1, 0),
         (1, 2, 3, 3.14),
         (-1, -2, 3, 0),
     ],
 )
 def test_htm_v3_mul_raw(x: float, y: float, z: float, scalar: float):
     """Tests the scalar multiplication of vectors."""
-    ec, v1 = PynyHTM.htm_v3_init_raw(x, y, z)
+    ec, v1 = pynyhtm.htm_v3_init_raw(x, y, z)
     assert ec == 0
 
-    res = PynyHTM.htm_v3_mul_raw(v1, scalar)
+    res = pynyhtm.htm_v3_mul_raw(v1, scalar)
     res = V3.from_htm_v3(res)
     assert res.x == x * scalar and res.y == y * scalar and res.z == z * scalar
 
 
 @pytest.mark.parametrize(
     "x, y, z, scalar",
     [
@@ -160,18 +159,18 @@
         (1, 1, 1, 2.0),
         (1, 2, 3, 3.14),
         (-1, -2, 3, 3),
     ],
 )
 def test_htm_v3_div_raw(x: float, y: float, z: float, scalar: float):
     """Tests the scalar division of vectors."""
-    ec, v1 = PynyHTM.htm_v3_init_raw(x, y, z)
+    ec, v1 = pynyhtm.htm_v3_init_raw(x, y, z)
     assert ec == 0
 
-    res = PynyHTM.htm_v3_div_raw(v1, scalar)
+    res = pynyhtm.htm_v3_div_raw(v1, scalar)
     res = V3.from_htm_v3(res)
     assert res.x == x / scalar and res.y == y / scalar and res.z == z / scalar
 
 
 @pytest.mark.parametrize(
     "lat1, lon1, lat2, lon2, target",
     [
@@ -184,15 +183,15 @@
         (0, -90, 0, 180, 90),
         (0, 0, 90, 0, 90),
         (-90, -90, 90, 90, 180),
     ],
 )
 def test_htm_sc_angsep_raw(lat1, lon1, lat2, lon2, target):
     """Test the raw angle distance function for sc."""
-    ec, sc1 = PynyHTM.htm_sc_init_raw(lat1, lon1)
+    ec, sc1 = pynyhtm.htm_sc_init_raw(lat1, lon1)
     assert ec == 0
 
-    ec, sc2 = PynyHTM.htm_sc_init_raw(lat2, lon2)
+    ec, sc2 = pynyhtm.htm_sc_init_raw(lat2, lon2)
     assert ec == 0
 
-    result = PynyHTM.htm_sc_angsep_raw(sc1, sc2)
+    result = pynyhtm.htm_sc_angsep_raw(sc1, sc2)
     assert abs(result - target) < 0.0001
```

### Comparing `pynyhtm-0.0.2/tests/test_sc.py` & `pynyhtm-0.0.3/tests/test_sc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """Spherical coordinate related (wrapped) tests for the PynyHTM wrapper."""
 
+import pynyhtm
 import pytest
-
-import PynyHTM
-from PynyHTM import SphericalCoordinate
+from pynyhtm import SphericalCoordinate
 
 
 @pytest.mark.parametrize("lat, lon", [(0, 0), (10, 10), (5, 10), (10, 5), (-10, -10)])
 def test_sc_init_wrapped_valid(lat: float, lon: float):
     """Test instantiation of valid sc using wrapping method."""
-    sc = PynyHTM.htm_sc_init_wrapped(lat, lon)
+    sc = pynyhtm.htm_sc_init_wrapped(lat, lon)
     assert sc.longitude == lon and sc.latitude == lat
 
 
 @pytest.mark.parametrize("lat, lon", [(-97, 0), (-100, 0), (-100, -100)])
 def test_sc_init_wrapped_invalid(lat: float, lon: float):
     """Test instantiation of invalid sc using wrapping method."""
     with pytest.raises(ValueError):
-        PynyHTM.htm_sc_init_wrapped(lat, lon)
+        pynyhtm.htm_sc_init_wrapped(lat, lon)
 
 
 def test_sc_to_v3_wrapped():
     """Test wrapped conversion from spherical coordinates to v3."""
     sc = SphericalCoordinate(10, 10)
     v3 = sc.to_v3()
     assert v3.x != 0 and v3.y != 0 and v3.z != 0
```

### Comparing `pynyhtm-0.0.2/tests/test_triangle.py` & `pynyhtm-0.0.3/tests/test_triangle.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """Triangle related tests for the PynyHTM wrapper."""
 
 import random
 
+import pynyhtm
 import pytest
 from numpy import int64
-
-import PynyHTM
-from PynyHTM import Triangle
+from pynyhtm import Triangle
 
 
 @pytest.mark.parametrize("id, level", [(15, 0), (980, 3), (1003971, 8), (16843849991222, 20)])
 def test_htm_tri_init_raw(id: int64, level: int):
     """Test instantiation of htm_tri struct for an id."""
-    ec, htm_tri = PynyHTM.htm_tri_init_raw(id)
+    ec, htm_tri = pynyhtm.htm_tri_init_raw(id)
     assert ec == 0
 
     assert htm_tri is not None
     assert htm_tri.get("center") is not None
     assert htm_tri.get("level") == level
 
 
@@ -36,61 +35,61 @@
     with pytest.raises(ValueError):
         Triangle.from_id(id)
 
 
 @pytest.mark.parametrize("id, level", [(15, 0), (980, 3), (1003971, 8), (16843849991222, 20)])
 def test_htm_level_raw(id: int, level: int):
     """Test id to level conversion."""
-    assert PynyHTM.htm_level_raw(id) == level
-    assert PynyHTM.HTM.get_level(id) == level
+    assert pynyhtm.htm_level_raw(id) == level
+    assert pynyhtm.HTM.get_level(id) == level
 
 
 @pytest.mark.parametrize("id", [(0), (-1)])
 def test_htm_level_raw_invalid(id: int):
     """Test invalid id during level conversion."""
     with pytest.raises(ValueError):
-        PynyHTM.htm_level_raw(id)
+        pynyhtm.htm_level_raw(id)
     with pytest.raises(ValueError):
-        PynyHTM.HTM.get_level(id)
+        pynyhtm.HTM.get_level(id)
 
 
 def test_htm_id_to_dec():
     """Test if htm_idtodec is wrapped."""
-    assert PynyHTM.htm_id_to_dec(12345) > 0
-    assert PynyHTM.HTM.id_to_dec(12345) > 0
+    assert pynyhtm.htm_id_to_dec(12345) > 0
+    assert pynyhtm.HTM.id_to_dec(12345) > 0
 
 
 @pytest.mark.parametrize("id, parent_id", [(61, 15), (16062643, 4015660)])
 def test_htm_parent(id: int64, parent_id: int64):
     """Test parent id determination."""
-    assert PynyHTM.HTM.parent(id) == parent_id
+    assert pynyhtm.HTM.parent(id) == parent_id
 
 
 @pytest.mark.parametrize("id", [(-1), (123), (15)])
 def test_htm_parent_invalid(id: int64):
     """Test invalid id for parent determination."""
     with pytest.raises(ValueError):
-        assert PynyHTM.HTM.parent(id)
+        assert pynyhtm.HTM.parent(id)
 
 
 @pytest.mark.parametrize("id", [(61), (15), (16062643), (4015660)])
 def test_htm_children(id: int64):
     """Validate generated children are valid."""
-    children = PynyHTM.HTM.children(id)
+    children = pynyhtm.HTM.children(id)
 
     # Instantiate child to verify it's id is correct
     for child in children:
         assert Triangle.from_id(child) is not None
 
 
 @pytest.mark.parametrize("id", [(123), (-1)])
 def test_htm_children_invalid(id: int64):
     """Test invalid id during child generation."""
     with pytest.raises(ValueError):
-        PynyHTM.HTM.children(id)
+        pynyhtm.HTM.children(id)
 
 
 @pytest.mark.parametrize(
     "id, dir, target_id",
     [
         # N3 (15)
         # west side
@@ -160,21 +159,21 @@
         (11268, 1, 10760),
         # sides covered by other root triangles
     ],
 )
 def test_directional_neighbor(id: int64, dir: int, target_id: int64):
     """Test if the correct neighbor is retrieved across root level changes."""
     if dir == 0:
-        dir = PynyHTM.NeighborDirection.OC_ZERO
+        dir = pynyhtm.NeighborDirection.OC_ZERO
     elif dir == 1:
-        dir = PynyHTM.NeighborDirection.OC_ONE
+        dir = pynyhtm.NeighborDirection.OC_ONE
     elif dir == 2:
-        dir = PynyHTM.NeighborDirection.OC_TWO
+        dir = pynyhtm.NeighborDirection.OC_TWO
 
-    neighbor = PynyHTM.HTM.neighbor(id, dir)[0]
+    neighbor = pynyhtm.HTM.neighbor(id, dir)[0]
     assert neighbor == target_id
 
 
 @pytest.mark.parametrize(
     "id, n1, n2, n3",
     [
         # 3 - center
@@ -189,15 +188,15 @@
         # 2 - edge
         (53182, 53174, 53169, 53183),  # upright
         (53178, 53125, 53179, 53180),  # upside down
     ],
 )
 def test_neighbors(id: int64, n1: int64, n3: int64, n2: int64):
     """Test if the correct neighbors are retrieved."""
-    neighbors = PynyHTM.HTM.neighbors(id)
+    neighbors = pynyhtm.HTM.neighbors(id)
 
     assert n1 in neighbors
     assert n2 in neighbors
     assert n3 in neighbors
 
 
 def test_neighbors_fuzz():
@@ -206,31 +205,31 @@
     for _ in range(0, samples):
         layer = random.randrange(2, 20)
         id_prefix = random.choice([x for x in range(8, 16)])
         id_suffix = random.getrandbits((layer - 1) * 2)
         id = id_prefix << (layer * 2) | id_suffix
 
         # Test using neighbor symmetry
-        neighbors = PynyHTM.HTM.neighbors(id)
+        neighbors = pynyhtm.HTM.neighbors(id)
         for neighbor in neighbors:
-            back_neighbors = PynyHTM.HTM.neighbors(neighbor)
+            back_neighbors = pynyhtm.HTM.neighbors(neighbor)
             assert id in back_neighbors
 
 
 @pytest.mark.parametrize(
     "latitude, longitude, level",
     [
         (38.0926507, 140.1839152, 5),
         (51.3892857, 30.0988303, 12),
         (53.0466026, 7.6294813, 10),
         (6.2489561, -75.5580277, 4),
     ],
 )
 def test_circle_search(latitude: float, longitude: float, level: float):
     """Test circle search by checking if a result is returned and if direct neighbors are contained."""
-    sc = PynyHTM.SphericalCoordinate(latitude, longitude)
-    neighbors = PynyHTM.HTM.neighbors(sc.get_htm_id(level))
+    sc = pynyhtm.SphericalCoordinate(latitude, longitude)
+    neighbors = pynyhtm.HTM.neighbors(sc.get_htm_id(level))
 
-    area_ids = PynyHTM.HTM.circle_search(sc.to_v3(), 20, level)
+    area_ids = pynyhtm.HTM.circle_search(sc.to_v3(), 20, level)
 
     for neighbor in neighbors:
         assert neighbor in area_ids
```

### Comparing `pynyhtm-0.0.2/tests/test_v3.py` & `pynyhtm-0.0.3/tests/test_v3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """Vector v3 related (wrapped) tests for the PynyHTM wrapper."""
 
+import pynyhtm
 import pytest
-
-import PynyHTM
-from PynyHTM import V3, SphericalCoordinate
+from pynyhtm import V3, SphericalCoordinate
 
 
 @pytest.mark.parametrize("x, y, z", [(10, 10, 10), (1, 5, 10), (10, 5, 1), (-10, -5, -1)])
 def test_v3_init_wrapped_valid(x: float, y: float, z: float):
     """Test instantiation of valid v3 using wrapping method."""
-    v3 = PynyHTM.htm_v3_init_wrapped(x, y, z)
+    v3 = pynyhtm.htm_v3_init_wrapped(x, y, z)
     assert v3.x == x and v3.y == y and v3.z == z
 
 
 def test_v3_to_sc_wrapped():
     """Tests wrapped conversion from v3 vector to spherical coordinates."""
     v3 = V3(1, 1, 1)
     sc = v3.to_sc()
```

