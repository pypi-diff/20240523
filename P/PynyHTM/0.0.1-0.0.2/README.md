# Comparing `tmp/pynyhtm-0.0.1.tar.gz` & `tmp/pynyhtm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynyhtm-0.0.1.tar", last modified: Sat May 18 18:07:18 2024, max compression
+gzip compressed data, was "pynyhtm-0.0.2.tar", last modified: Thu May 23 06:44:55 2024, max compression
```

## Comparing `pynyhtm-0.0.1.tar` & `pynyhtm-0.0.2.tar`

### file list

```diff
@@ -1,203 +1,207 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:07:18.666432 pynyhtm-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-18 18:06:42.000000 pynyhtm-0.0.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-18 18:06:42.000000 pynyhtm-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-18 18:06:42.000000 pynyhtm-0.0.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-18 18:07:18.666432 pynyhtm-0.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:07:18.662432 pynyhtm-0.0.1/PynyHTM.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-18 18:07:18.000000 pynyhtm-0.0.1/PynyHTM.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6833 2024-05-18 18:07:18.000000 pynyhtm-0.0.1/PynyHTM.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 18:07:18.000000 pynyhtm-0.0.1/PynyHTM.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-18 18:07:18.000000 pynyhtm-0.0.1/PynyHTM.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-18 18:07:18.000000 pynyhtm-0.0.1/PynyHTM.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-18 18:06:42.000000 pynyhtm-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:07:18.638431 pynyhtm-0.0.1/libtinyhtm/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/.git
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/README
--rw-r--r--   0 runner    (1001) docker     (127)    13889 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/boost.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/cxx14.py
--rw-r--r--   0 runner    (1001) docker     (127)    74592 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/doxygen.conf
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/hdf5_cxx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:07:18.642431 pynyhtm-0.0.1/libtinyhtm/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/Box.hxx
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/Cartesian.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/Cartesian.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     8576 2024-05-18 18:06:58.000000 pynyhtm-0.0.1/libtinyhtm/src/Cartesian.o
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/Circle.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/Ellipse.hxx
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/Exception.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/Polygon.hxx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:07:18.642431 pynyhtm-0.0.1/libtinyhtm/src/Query/
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/Query/Query.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/Query.hxx
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/Shape.hxx
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/Spherical.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/Spherical.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-05-18 18:06:59.000000 pynyhtm-0.0.1/libtinyhtm/src/Spherical.o
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/Tree.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/common.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-18 18:06:59.000000 pynyhtm-0.0.1/libtinyhtm/src/common.o
--rw-r--r--   0 runner    (1001) docker     (127)    47194 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/geometry.cxx
--rw-r--r--   0 runner    (1001) docker     (127)    39648 2024-05-18 18:06:59.000000 pynyhtm-0.0.1/libtinyhtm/src/geometry.o
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:07:18.650431 pynyhtm-0.0.1/libtinyhtm/src/htm/
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_ids_add.hxx
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_ids_init.cxx
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_ids_init.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-18 18:07:00.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_ids_init.o
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_s2circle_htmcov.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_s2circle_htmcov.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-05-18 18:07:00.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_s2circle_htmcov.o
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:07:18.650431 pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_s2cpoly_htmcov/
--rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_s2cpoly_htmcov/_htm_isect_test.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_s2cpoly_htmcov/_htm_s2cpoly_htmcov.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_s2cpoly_htmcov.hxx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:07:18.650431 pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_s2ellipse_htmcov/
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_s2ellipse_htmcov/_htm_s2ellipse_htmcov.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_s2ellipse_htmcov/_htm_s2ellipse_isect.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_s2ellipse_htmcov.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_simplify_ids.cxx
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_simplify_ids.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-18 18:07:01.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_simplify_ids.o
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_subdivide.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_subdivide.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-05-18 18:07:01.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_subdivide.o
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_v3_htmroot.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_s2circle_ids.cxx
--rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-05-18 18:07:01.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_s2circle_ids.o
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_s2cpoly_cv3_template.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_s2cpoly_ids.cxx
--rw-r--r--   0 runner    (1001) docker     (127)    10800 2024-05-18 18:07:01.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_s2cpoly_ids.o
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_s2ellipse_cv3_template.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_s2ellipse_ids.cxx
--rw-r--r--   0 runner    (1001) docker     (127)    10456 2024-05-18 18:07:01.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_s2ellipse_ids.o
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2circle.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-18 18:07:02.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2circle.o
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2circle_range.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     9696 2024-05-18 18:07:02.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2circle_range.o
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2circle_scan.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-18 18:07:02.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2circle_scan.o
--rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2cpoly.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-18 18:07:02.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2cpoly.o
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2cpoly_range.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     9648 2024-05-18 18:07:03.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2cpoly_range.o
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2cpoly_scan.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-18 18:07:03.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2cpoly_scan.o
--rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2ellipse.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-18 18:07:03.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2ellipse.o
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2ellipse_range.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     9304 2024-05-18 18:07:04.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2ellipse_range.o
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2ellipse_scan.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-18 18:07:04.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2ellipse_scan.o
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_v3_distance2.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_v3_id.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-05-18 18:07:04.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_v3_id.o
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:07:18.650431 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_v3p_idsort/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:07:18.650431 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_v3p_idsort/_htm_path_sort/
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_v3p_idsort/_htm_path_sort/_htm_partition.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_v3p_idsort/_htm_path_sort/_htm_path_sort.cxx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:07:18.654432 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_v3p_idsort/_htm_rootsort/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_v3p_idsort/_htm_rootsort/_htm_rootpart.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_v3p_idsort/_htm_rootsort/_htm_rootsort.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm/htm_v3p_idsort/htm_v3p_idsort.cxx
--rw-r--r--   0 runner    (1001) docker     (127)    10166 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     8395 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm.hxx
--rw-r--r--   0 runner    (1001) docker     (127)    17120 2024-05-18 18:06:59.000000 pynyhtm-0.0.1/libtinyhtm/src/htm.o
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm_convert_to_hdf5.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm_entry.hxx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:07:18.654432 pynyhtm-0.0.1/libtinyhtm/src/htm_tree_gen/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:07:18.654432 pynyhtm-0.0.1/libtinyhtm/src/htm_tree_gen/blk_sort_ascii/
--rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm_tree_gen/blk_sort_ascii/blk_sort_ascii.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm_tree_gen/blk_sort_ascii/eat_delim.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm_tree_gen/blk_sort_ascii/eat_ws.cxx
--rw-r--r--   0 runner    (1001) docker     (127)    14221 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm_tree_gen/htm_tree_gen.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/htm_tree_gen/usage.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     9613 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/id_list.cxx
--rw-r--r--   0 runner    (1001) docker     (127)    13640 2024-05-18 18:07:00.000000 pynyhtm-0.0.1/libtinyhtm/src/id_list.o
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/licence.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-18 18:07:00.000000 pynyhtm-0.0.1/libtinyhtm/src/licence.o
--rw-r--r--   0 runner    (1001) docker     (127)    12634 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/select.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-05-18 18:07:00.000000 pynyhtm-0.0.1/libtinyhtm/src/select.o
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:07:18.654432 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/append_htm.cxx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:07:18.654432 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/arena/
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/arena/arena_seg.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/arena.hxx
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/blk_write_state.hxx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:07:18.654432 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/blk_writer/
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/blk_writer/blk_write.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/blk_writer.hxx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:07:18.658432 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/ext_sort/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/ext_sort/mrg_npasses.cxx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:07:18.658432 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/ext_sort/mrg_pass/
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/ext_sort/mrg_pass/heap_down.hxx
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/ext_sort/mrg_pass/heap_up.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/ext_sort/mrg_pass.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/ext_sort/mrg_seg.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/ext_sort.hxx
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/mem_params.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/node.hxx
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/now.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/now.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/reverse_file.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/spherical_to_vec.hxx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:07:18.658432 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_compress/
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_compress/compress_node.cxx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:07:18.658432 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_compress/hash_table/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_compress/hash_table/hash_table_add.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_compress/hash_table/hash_table_destroy.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_compress/hash_table/hash_table_get.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_compress/hash_table/hash_table_grow.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_compress/hash_table/hash_table_init.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_compress/hash_table.hxx
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_compress/id_off.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_compress/tree_compress.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_compress/write_tree_header.cxx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:07:18.662432 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_gen/
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_gen/add_node.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_gen/assign_block.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_gen/assign_block.hxx
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_gen/child_info.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_gen/emit_node.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_gen/emit_node.hxx
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_gen/estimate_node_size.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_gen/finish_root.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_gen/layout_node.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_gen/layout_node.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_gen.hxx
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_gen_context.hxx
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_root.hxx
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/sort_and_index.hxx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:07:18.662432 pynyhtm-0.0.1/libtinyhtm/src/tinyhtm/
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/tinyhtm/common.h
--rw-r--r--   0 runner    (1001) docker     (127)    20243 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/tinyhtm/geometry.h
--rw-r--r--   0 runner    (1001) docker     (127)    14898 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/tinyhtm/htm.h
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/tinyhtm/select.h
--rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/tinyhtm/tree.h
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/tinyhtm/varint.h
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/tinyhtm.h
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/tree.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-05-18 18:07:00.000000 pynyhtm-0.0.1/libtinyhtm/src/tree.o
--rw-r--r--   0 runner    (1001) docker     (127)    16846 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/tree_count.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/tree_entry.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/src/tree_entry.hxx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:07:18.662432 pynyhtm-0.0.1/libtinyhtm/test/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/test/cmp.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/test/cmp.h
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/test/rand.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/test/rand.h
--rw-r--r--   0 runner    (1001) docker     (127)    43103 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/test/test_geometry.cxx
--rw-r--r--   0 runner    (1001) docker     (127)    32594 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/test/test_htm.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/test/test_ranges.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/test/test_select.cxx
--rwxr-xr-x   0 runner    (1001) docker     (127)   105122 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/waf
--rwxr-xr-x   0 runner    (1001) docker     (127)    90923 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/waf-1.7.10
--rwxr-xr-x   0 runner    (1001) docker     (127)   105122 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/waf-2.0.23
--rw-r--r--   0 runner    (1001) docker     (127)    15921 2024-05-18 18:06:43.000000 pynyhtm-0.0.1/libtinyhtm/wscript
--rw-r--r--   0 runner    (1001) docker     (127)   719393 2024-05-18 18:07:17.000000 pynyhtm-0.0.1/pynyhtm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-18 18:06:42.000000 pynyhtm-0.0.1/pynyhtm.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-18 18:06:42.000000 pynyhtm-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 18:07:18.666432 pynyhtm-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-18 18:06:42.000000 pynyhtm-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 18:07:18.662432 pynyhtm-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-05-18 18:06:42.000000 pynyhtm-0.0.1/tests/test_pynyhtm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.027933 pynyhtm-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-23 06:44:38.000000 pynyhtm-0.0.2/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-23 06:44:38.000000 pynyhtm-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-23 06:44:38.000000 pynyhtm-0.0.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-23 06:44:55.027933 pynyhtm-0.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.027933 pynyhtm-0.0.2/PynyHTM.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-23 06:44:54.000000 pynyhtm-0.0.2/PynyHTM.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-05-23 06:44:54.000000 pynyhtm-0.0.2/PynyHTM.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 06:44:54.000000 pynyhtm-0.0.2/PynyHTM.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-23 06:44:54.000000 pynyhtm-0.0.2/PynyHTM.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 06:44:54.000000 pynyhtm-0.0.2/PynyHTM.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-23 06:44:38.000000 pynyhtm-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:54.995932 pynyhtm-0.0.2/libtinyhtm/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-23 06:44:38.000000 pynyhtm-0.0.2/libtinyhtm/.git
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/README
+-rw-r--r--   0 runner    (1001) docker     (127)    13889 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/boost.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/cxx14.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74592 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/doxygen.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/hdf5_cxx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.003933 pynyhtm-0.0.2/libtinyhtm/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/Box.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/Cartesian.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/Cartesian.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     8576 2024-05-23 06:44:46.000000 pynyhtm-0.0.2/libtinyhtm/src/Cartesian.o
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/Circle.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/Ellipse.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/Exception.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/Polygon.hxx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.003933 pynyhtm-0.0.2/libtinyhtm/src/Query/
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/Query/Query.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/Query.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/Shape.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/Spherical.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/Spherical.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-05-23 06:44:46.000000 pynyhtm-0.0.2/libtinyhtm/src/Spherical.o
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/Tree.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/common.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-23 06:44:46.000000 pynyhtm-0.0.2/libtinyhtm/src/common.o
+-rw-r--r--   0 runner    (1001) docker     (127)    47194 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/geometry.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)    39648 2024-05-23 06:44:46.000000 pynyhtm-0.0.2/libtinyhtm/src/geometry.o
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.011933 pynyhtm-0.0.2/libtinyhtm/src/htm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_ids_add.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_ids_init.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_ids_init.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-23 06:44:48.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_ids_init.o
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_s2circle_htmcov.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_s2circle_htmcov.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-05-23 06:44:48.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_s2circle_htmcov.o
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.011933 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_s2cpoly_htmcov/
+-rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_s2cpoly_htmcov/_htm_isect_test.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_s2cpoly_htmcov/_htm_s2cpoly_htmcov.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_s2cpoly_htmcov.hxx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.011933 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_s2ellipse_htmcov/
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_s2ellipse_htmcov/_htm_s2ellipse_htmcov.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_s2ellipse_htmcov/_htm_s2ellipse_isect.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_s2ellipse_htmcov.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_simplify_ids.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_simplify_ids.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-23 06:44:48.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_simplify_ids.o
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_subdivide.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_subdivide.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-05-23 06:44:48.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_subdivide.o
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_v3_htmroot.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_s2circle_ids.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-05-23 06:44:48.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_s2circle_ids.o
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_s2cpoly_cv3_template.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_s2cpoly_ids.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)    10800 2024-05-23 06:44:48.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_s2cpoly_ids.o
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_s2ellipse_cv3_template.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_s2ellipse_ids.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)    10456 2024-05-23 06:44:48.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_s2ellipse_ids.o
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2circle.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-23 06:44:49.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2circle.o
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2circle_range.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     9696 2024-05-23 06:44:49.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2circle_range.o
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2circle_scan.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-23 06:44:50.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2circle_scan.o
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2cpoly.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-23 06:44:50.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2cpoly.o
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2cpoly_range.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     9648 2024-05-23 06:44:50.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2cpoly_range.o
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2cpoly_scan.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-23 06:44:51.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2cpoly_scan.o
+-rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2ellipse.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-23 06:44:51.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2ellipse.o
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2ellipse_range.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     9304 2024-05-23 06:44:51.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2ellipse_range.o
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2ellipse_scan.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-23 06:44:52.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2ellipse_scan.o
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3_distance2.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3_id.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-05-23 06:44:52.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3_id.o
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.011933 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3p_idsort/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.011933 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3p_idsort/_htm_path_sort/
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3p_idsort/_htm_path_sort/_htm_partition.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3p_idsort/_htm_path_sort/_htm_path_sort.cxx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.011933 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3p_idsort/_htm_rootsort/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3p_idsort/_htm_rootsort/_htm_rootpart.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3p_idsort/_htm_rootsort/_htm_rootsort.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3p_idsort/htm_v3p_idsort.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)    10166 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     8395 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)    17120 2024-05-23 06:44:47.000000 pynyhtm-0.0.2/libtinyhtm/src/htm.o
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm_convert_to_hdf5.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm_entry.hxx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.015933 pynyhtm-0.0.2/libtinyhtm/src/htm_tree_gen/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.015933 pynyhtm-0.0.2/libtinyhtm/src/htm_tree_gen/blk_sort_ascii/
+-rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm_tree_gen/blk_sort_ascii/blk_sort_ascii.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm_tree_gen/blk_sort_ascii/eat_delim.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm_tree_gen/blk_sort_ascii/eat_ws.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)    14221 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm_tree_gen/htm_tree_gen.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/htm_tree_gen/usage.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     9613 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/id_list.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)    13640 2024-05-23 06:44:47.000000 pynyhtm-0.0.2/libtinyhtm/src/id_list.o
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/licence.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-23 06:44:47.000000 pynyhtm-0.0.2/libtinyhtm/src/licence.o
+-rw-r--r--   0 runner    (1001) docker     (127)    12634 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/select.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-05-23 06:44:47.000000 pynyhtm-0.0.2/libtinyhtm/src/select.o
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.015933 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/append_htm.cxx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.015933 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/arena/
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/arena/arena_seg.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/arena.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/blk_write_state.hxx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.015933 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/blk_writer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/blk_writer/blk_write.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/blk_writer.hxx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.019933 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/ext_sort/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/ext_sort/mrg_npasses.cxx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.019933 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/ext_sort/mrg_pass/
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/ext_sort/mrg_pass/heap_down.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/ext_sort/mrg_pass/heap_up.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/ext_sort/mrg_pass.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/ext_sort/mrg_seg.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/ext_sort.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/mem_params.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/node.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/now.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/now.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/reverse_file.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/spherical_to_vec.hxx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.019933 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/compress_node.cxx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.019933 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/hash_table/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/hash_table/hash_table_add.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/hash_table/hash_table_destroy.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/hash_table/hash_table_get.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/hash_table/hash_table_grow.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/hash_table/hash_table_init.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/hash_table.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/id_off.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/tree_compress.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/write_tree_header.cxx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.023933 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/add_node.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/assign_block.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/assign_block.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/child_info.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/emit_node.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/emit_node.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/estimate_node_size.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/finish_root.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/layout_node.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/layout_node.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen_context.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_root.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/sort_and_index.hxx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.023933 pynyhtm-0.0.2/libtinyhtm/src/tinyhtm/
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/tinyhtm/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20243 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/tinyhtm/geometry.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14898 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/tinyhtm/htm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/tinyhtm/select.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/tinyhtm/tree.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/tinyhtm/varint.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/tinyhtm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/tree.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-05-23 06:44:47.000000 pynyhtm-0.0.2/libtinyhtm/src/tree.o
+-rw-r--r--   0 runner    (1001) docker     (127)    16846 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/tree_count.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/tree_entry.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/src/tree_entry.hxx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.023933 pynyhtm-0.0.2/libtinyhtm/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/test/cmp.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/test/cmp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/test/rand.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/test/rand.h
+-rw-r--r--   0 runner    (1001) docker     (127)    43103 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/test/test_geometry.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)    32594 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/test/test_htm.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/test/test_ranges.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/test/test_select.cxx
+-rwxr-xr-x   0 runner    (1001) docker     (127)   105122 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/waf
+-rwxr-xr-x   0 runner    (1001) docker     (127)    90923 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/waf-1.7.10
+-rwxr-xr-x   0 runner    (1001) docker     (127)   105122 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/waf-2.0.23
+-rw-r--r--   0 runner    (1001) docker     (127)    15921 2024-05-23 06:44:39.000000 pynyhtm-0.0.2/libtinyhtm/wscript
+-rw-r--r--   0 runner    (1001) docker     (127)  1528420 2024-05-23 06:44:53.000000 pynyhtm-0.0.2/pynyhtm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    35806 2024-05-23 06:44:38.000000 pynyhtm-0.0.2/pynyhtm.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-23 06:44:38.000000 pynyhtm-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 06:44:55.027933 pynyhtm-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-23 06:44:38.000000 pynyhtm-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 06:44:55.027933 pynyhtm-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-05-23 06:44:38.000000 pynyhtm-0.0.2/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-23 06:44:38.000000 pynyhtm-0.0.2/tests/test_pynyhtm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-23 06:44:38.000000 pynyhtm-0.0.2/tests/test_sc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-05-23 06:44:38.000000 pynyhtm-0.0.2/tests/test_triangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-05-23 06:44:38.000000 pynyhtm-0.0.2/tests/test_v3.py
```

### Comparing `pynyhtm-0.0.1/LICENCE` & `pynyhtm-0.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/Makefile` & `pynyhtm-0.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/PynyHTM.egg-info/SOURCES.txt` & `pynyhtm-0.0.2/PynyHTM.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -170,8 +170,12 @@
 libtinyhtm/test/cmp.h
 libtinyhtm/test/rand.cxx
 libtinyhtm/test/rand.h
 libtinyhtm/test/test_geometry.cxx
 libtinyhtm/test/test_htm.cxx
 libtinyhtm/test/test_ranges.cxx
 libtinyhtm/test/test_select.cxx
-tests/test_pynyhtm.py
+tests/test_geometry.py
+tests/test_pynyhtm.py
+tests/test_sc.py
+tests/test_triangle.py
+tests/test_v3.py
```

### Comparing `pynyhtm-0.0.1/libtinyhtm/LICENSE.txt` & `pynyhtm-0.0.2/libtinyhtm/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/Makefile` & `pynyhtm-0.0.2/libtinyhtm/Makefile`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/README` & `pynyhtm-0.0.2/libtinyhtm/README`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/boost.py` & `pynyhtm-0.0.2/libtinyhtm/boost.py`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/cxx14.py` & `pynyhtm-0.0.2/libtinyhtm/cxx14.py`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/doxygen.conf` & `pynyhtm-0.0.2/libtinyhtm/doxygen.conf`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/hdf5_cxx.py` & `pynyhtm-0.0.2/libtinyhtm/hdf5_cxx.py`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/Box.hxx` & `pynyhtm-0.0.2/libtinyhtm/src/Box.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/Cartesian.hxx` & `pynyhtm-0.0.2/libtinyhtm/src/Cartesian.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/Cartesian.o` & `pynyhtm-0.0.2/libtinyhtm/src/Cartesian.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/Circle.hxx` & `pynyhtm-0.0.2/libtinyhtm/src/Circle.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/Ellipse.hxx` & `pynyhtm-0.0.2/libtinyhtm/src/Ellipse.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/Polygon.hxx` & `pynyhtm-0.0.2/libtinyhtm/src/Polygon.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/Query/Query.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/Query/Query.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/Query.hxx` & `pynyhtm-0.0.2/libtinyhtm/src/Query.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/Shape.hxx` & `pynyhtm-0.0.2/libtinyhtm/src/Shape.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/Spherical.hxx` & `pynyhtm-0.0.2/libtinyhtm/src/Spherical.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/Spherical.o` & `pynyhtm-0.0.2/libtinyhtm/src/Spherical.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/common.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/common.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/common.o` & `pynyhtm-0.0.2/libtinyhtm/src/common.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/geometry.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/geometry.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/geometry.o` & `pynyhtm-0.0.2/libtinyhtm/src/geometry.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_ids_add.hxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_ids_add.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_ids_init.o` & `pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_ids_init.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_s2circle_htmcov.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_s2circle_htmcov.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_s2circle_htmcov.o` & `pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_s2circle_htmcov.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_s2cpoly_htmcov/_htm_isect_test.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_s2cpoly_htmcov/_htm_isect_test.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_s2cpoly_htmcov/_htm_s2cpoly_htmcov.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_s2cpoly_htmcov/_htm_s2cpoly_htmcov.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_s2ellipse_htmcov/_htm_s2ellipse_htmcov.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_s2ellipse_htmcov/_htm_s2ellipse_htmcov.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_s2ellipse_htmcov/_htm_s2ellipse_isect.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_s2ellipse_htmcov/_htm_s2ellipse_isect.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_simplify_ids.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_simplify_ids.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_simplify_ids.o` & `pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_simplify_ids.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_subdivide.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_subdivide.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_subdivide.o` & `pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_subdivide.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/_htm_v3_htmroot.hxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm/_htm_v3_htmroot.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/htm_s2circle_ids.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_s2circle_ids.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/htm_s2circle_ids.o` & `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_s2circle_ids.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/htm_s2cpoly_cv3_template.hxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_s2cpoly_cv3_template.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/htm_s2cpoly_ids.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_s2cpoly_ids.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/htm_s2cpoly_ids.o` & `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_s2cpoly_ids.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/htm_s2ellipse_ids.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_s2ellipse_ids.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/htm_s2ellipse_ids.o` & `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_s2ellipse_ids.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2circle.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2circle.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2circle.o` & `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2circle.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2circle_range.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2circle_range.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2circle_range.o` & `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2circle_range.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2circle_scan.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2circle_scan.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2circle_scan.o` & `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2circle_scan.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2cpoly.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2cpoly.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2cpoly.o` & `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2cpoly.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2cpoly_range.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2cpoly_range.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2cpoly_range.o` & `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2cpoly_range.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2cpoly_scan.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2cpoly_scan.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2cpoly_scan.o` & `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2cpoly_scan.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2ellipse.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2ellipse.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2ellipse.o` & `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2ellipse.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2ellipse_range.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2ellipse_range.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2ellipse_range.o` & `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2ellipse_range.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2ellipse_scan.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2ellipse_scan.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/htm_tree_s2ellipse_scan.o` & `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_tree_s2ellipse_scan.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/htm_v3_id.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3_id.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/htm_v3_id.o` & `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3_id.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/htm_v3p_idsort/_htm_path_sort/_htm_partition.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3p_idsort/_htm_path_sort/_htm_partition.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/htm_v3p_idsort/_htm_path_sort/_htm_path_sort.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3p_idsort/_htm_path_sort/_htm_path_sort.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/htm_v3p_idsort/_htm_rootsort/_htm_rootpart.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3p_idsort/_htm_rootsort/_htm_rootpart.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/htm_v3p_idsort/_htm_rootsort/_htm_rootsort.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3p_idsort/_htm_rootsort/_htm_rootsort.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm/htm_v3p_idsort/htm_v3p_idsort.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm/htm_v3p_idsort/htm_v3p_idsort.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm.hxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm.o` & `pynyhtm-0.0.2/libtinyhtm/src/htm.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm_convert_to_hdf5.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm_convert_to_hdf5.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm_tree_gen/blk_sort_ascii/blk_sort_ascii.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm_tree_gen/blk_sort_ascii/blk_sort_ascii.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm_tree_gen/blk_sort_ascii/eat_delim.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm_tree_gen/blk_sort_ascii/eat_delim.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm_tree_gen/blk_sort_ascii/eat_ws.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm_tree_gen/blk_sort_ascii/eat_ws.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm_tree_gen/htm_tree_gen.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm_tree_gen/htm_tree_gen.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/htm_tree_gen/usage.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/htm_tree_gen/usage.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/id_list.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/id_list.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/id_list.o` & `pynyhtm-0.0.2/libtinyhtm/src/id_list.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/licence.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/licence.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/licence.o` & `pynyhtm-0.0.2/libtinyhtm/src/licence.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/select.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/select.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/select.o` & `pynyhtm-0.0.2/libtinyhtm/src/select.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/append_htm.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/append_htm.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/arena/arena_seg.hxx` & `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/arena/arena_seg.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/arena.hxx` & `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/arena.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/blk_writer/blk_write.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/blk_writer/blk_write.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/blk_writer.hxx` & `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/blk_writer.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/ext_sort/mrg_pass/heap_down.hxx` & `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/ext_sort/mrg_pass/heap_down.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/ext_sort/mrg_pass.hxx` & `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/ext_sort/mrg_pass.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/ext_sort/mrg_seg.hxx` & `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/ext_sort/mrg_seg.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/ext_sort.hxx` & `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/ext_sort.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/mem_params.hxx` & `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/mem_params.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/node.hxx` & `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/node.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/reverse_file.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/reverse_file.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/spherical_to_vec.hxx` & `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/spherical_to_vec.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_compress/compress_node.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/compress_node.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_compress/hash_table/hash_table_add.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/hash_table/hash_table_add.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_compress/hash_table/hash_table_get.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/hash_table/hash_table_get.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_compress/hash_table/hash_table_grow.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/hash_table/hash_table_grow.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_compress/hash_table.hxx` & `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/hash_table.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_compress/tree_compress.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/tree_compress.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_compress/write_tree_header.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_compress/write_tree_header.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_gen/add_node.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/add_node.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_gen/assign_block.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/assign_block.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_gen/assign_block.hxx` & `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/assign_block.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_gen/emit_node.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/emit_node.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_gen/estimate_node_size.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/estimate_node_size.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_gen/finish_root.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/finish_root.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_gen/layout_node.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen/layout_node.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_gen.hxx` & `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/sort_and_index/tree_gen_context.hxx` & `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index/tree_gen_context.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/sort_and_index.hxx` & `pynyhtm-0.0.2/libtinyhtm/src/sort_and_index.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/tinyhtm/common.h` & `pynyhtm-0.0.2/libtinyhtm/src/tinyhtm/common.h`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/tinyhtm/geometry.h` & `pynyhtm-0.0.2/libtinyhtm/src/tinyhtm/geometry.h`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/tinyhtm/htm.h` & `pynyhtm-0.0.2/libtinyhtm/src/tinyhtm/htm.h`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/tinyhtm/select.h` & `pynyhtm-0.0.2/libtinyhtm/src/tinyhtm/select.h`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/tinyhtm/tree.h` & `pynyhtm-0.0.2/libtinyhtm/src/tinyhtm/tree.h`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/tinyhtm/varint.h` & `pynyhtm-0.0.2/libtinyhtm/src/tinyhtm/varint.h`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/tinyhtm.h` & `pynyhtm-0.0.2/libtinyhtm/src/tinyhtm.h`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/tree.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/tree.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/tree.o` & `pynyhtm-0.0.2/libtinyhtm/src/tree.o`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/tree_count.cxx` & `pynyhtm-0.0.2/libtinyhtm/src/tree_count.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/src/tree_entry.hxx` & `pynyhtm-0.0.2/libtinyhtm/src/tree_entry.hxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/test/cmp.cxx` & `pynyhtm-0.0.2/libtinyhtm/test/cmp.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/test/cmp.h` & `pynyhtm-0.0.2/libtinyhtm/test/cmp.h`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/test/rand.cxx` & `pynyhtm-0.0.2/libtinyhtm/test/rand.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/test/test_geometry.cxx` & `pynyhtm-0.0.2/libtinyhtm/test/test_geometry.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/test/test_htm.cxx` & `pynyhtm-0.0.2/libtinyhtm/test/test_htm.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/test/test_ranges.cxx` & `pynyhtm-0.0.2/libtinyhtm/test/test_ranges.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/test/test_select.cxx` & `pynyhtm-0.0.2/libtinyhtm/test/test_select.cxx`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/waf` & `pynyhtm-0.0.2/libtinyhtm/waf`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/waf-1.7.10` & `pynyhtm-0.0.2/libtinyhtm/waf-1.7.10`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/waf-2.0.23` & `pynyhtm-0.0.2/libtinyhtm/waf-2.0.23`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/libtinyhtm/wscript` & `pynyhtm-0.0.2/libtinyhtm/wscript`

 * *Files identical despite different names*

### Comparing `pynyhtm-0.0.1/pyproject.toml` & `pynyhtm-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -19,28 +19,28 @@
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 py-modules = []
 
 [tool.cibuildwheel]
-skip = ["cp36-*", "cp37-*", "cp38-*", "cp39-*"]
+skip = ["cp36-*", "cp37-*", "pp*"]
 test-requires = [
     "pytest",
     "numpy"
 ]
 test-command = "pytest {project}/tests"
 
 [project.optional-dependencies]
 dev = ["black", "isort", "pytest"]
 
 
 [project]
 name = "PynyHTM"
-version = "0.0.1"
+version = "0.0.2"
 description = "Python wrapper for the libtinyhtm library."
 readme = "README.md"
 authors = [{ name = "Till", email = "till@fleisch.dev" }]
 license = { file = "LICENSE" }
 keywords = ["htm", "libtinyhtm", "hierarchial triangular mesh", "triangle subdivision", "index"]
 dependencies = [
     "numpy",
```

### Comparing `pynyhtm-0.0.1/setup.py` & `pynyhtm-0.0.2/setup.py`

 * *Files identical despite different names*

