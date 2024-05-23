# Comparing `tmp/impose-0.4.6.tar.gz` & `tmp/impose-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impose-0.4.6.tar", last modified: Fri Sep  8 13:46:32 2023, max compression
+gzip compressed data, was "impose-0.4.8.tar", last modified: Thu May 16 21:52:00 2024, max compression
```

## Comparing `impose-0.4.6.tar` & `impose-0.4.8.tar`

### file list

```diff
@@ -1,108 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:46:32.383792 impose-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2023-09-08 13:45:47.000000 impose-0.4.6/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-09-08 13:45:47.000000 impose-0.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      282 2023-09-08 13:45:47.000000 impose-0.4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2023-09-08 13:46:32.383792 impose-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2023-09-08 13:45:47.000000 impose-0.4.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:46:32.367792 impose-0.4.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2023-09-08 13:45:47.000000 impose-0.4.6/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6434 2023-09-08 13:45:47.000000 impose-0.4.6/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:46:32.367792 impose-0.4.6/docs/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2023-09-08 13:45:47.000000 impose-0.4.6/docs/extensions/github_changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-09-08 13:45:47.000000 impose-0.4.6/docs/impose.bib
--rw-r--r--   0 runner    (1001) docker     (127)      638 2023-09-08 13:45:47.000000 impose-0.4.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      114 2023-09-08 13:45:47.000000 impose-0.4.6/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2023-09-08 13:45:47.000000 impose-0.4.6/docs/sec_changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)      623 2023-09-08 13:45:47.000000 impose-0.4.6/docs/sec_getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-09-08 13:45:47.000000 impose-0.4.6/docs/sec_z_bib.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:46:32.367792 impose-0.4.6/impose/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2023-09-08 13:45:47.000000 impose-0.4.6/impose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2023-09-08 13:45:47.000000 impose-0.4.6/impose/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7035 2023-09-08 13:45:47.000000 impose-0.4.6/impose/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-09-08 13:46:01.000000 impose-0.4.6/impose/_version_save.py
--rw-r--r--   0 runner    (1001) docker     (127)     7783 2023-09-08 13:45:47.000000 impose-0.4.6/impose/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9185 2023-09-08 13:45:47.000000 impose-0.4.6/impose/flblend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:46:32.367792 impose-0.4.6/impose/formats/
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2023-09-08 13:45:47.000000 impose-0.4.6/impose/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2023-09-08 13:45:47.000000 impose-0.4.6/impose/formats/fmt_bf_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2023-09-08 13:45:47.000000 impose-0.4.6/impose/formats/fmt_bm_bmlab.py
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2023-09-08 13:45:47.000000 impose-0.4.6/impose/formats/fmt_fl_zeiss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:46:32.371792 impose-0.4.6/impose/geometry/
--rw-r--r--   0 runner    (1001) docker     (127)      704 2023-09-08 13:45:47.000000 impose-0.4.6/impose/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2023-09-08 13:45:47.000000 impose-0.4.6/impose/geometry/mask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:46:32.371792 impose-0.4.6/impose/geometry/shapes/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2023-09-08 13:45:47.000000 impose-0.4.6/impose/geometry/shapes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2023-09-08 13:45:47.000000 impose-0.4.6/impose/geometry/shapes/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2023-09-08 13:45:47.000000 impose-0.4.6/impose/geometry/shapes/sh_circle.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2023-09-08 13:45:47.000000 impose-0.4.6/impose/geometry/shapes/sh_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2023-09-08 13:45:47.000000 impose-0.4.6/impose/geometry/shapes/sh_polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4977 2023-09-08 13:45:47.000000 impose-0.4.6/impose/geometry/shapes/sh_rectangle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:46:32.375792 impose-0.4.6/impose/gui/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-09-08 13:45:47.000000 impose-0.4.6/impose/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11665 2023-09-08 13:45:47.000000 impose-0.4.6/impose/gui/collect.py
--rw-r--r--   0 runner    (1001) docker     (127)    11634 2023-09-08 13:45:47.000000 impose-0.4.6/impose/gui/collect.ui
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2023-09-08 13:45:47.000000 impose-0.4.6/impose/gui/collect_pgrois.py
--rw-r--r--   0 runner    (1001) docker     (127)     5799 2023-09-08 13:45:47.000000 impose-0.4.6/impose/gui/collect_shape_controls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2023-09-08 13:45:47.000000 impose-0.4.6/impose/gui/collect_shape_controls.ui
--rw-r--r--   0 runner    (1001) docker     (127)    14301 2023-09-08 13:45:47.000000 impose-0.4.6/impose/gui/colocalize.py
--rw-r--r--   0 runner    (1001) docker     (127)    15704 2023-09-08 13:45:47.000000 impose-0.4.6/impose/gui/colocalize.ui
--rw-r--r--   0 runner    (1001) docker     (127)    11685 2023-09-08 13:45:47.000000 impose-0.4.6/impose/gui/colocalize_pgrois.py
--rw-r--r--   0 runner    (1001) docker     (127)     4257 2023-09-08 13:45:47.000000 impose-0.4.6/impose/gui/dlg_edit_circle.ui
--rw-r--r--   0 runner    (1001) docker     (127)     5564 2023-09-08 13:45:47.000000 impose-0.4.6/impose/gui/dlg_edit_ellipse.ui
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2023-09-08 13:45:47.000000 impose-0.4.6/impose/gui/dlg_edit_polygon.ui
--rw-r--r--   0 runner    (1001) docker     (127)     5569 2023-09-08 13:45:47.000000 impose-0.4.6/impose/gui/dlg_edit_rectangle.ui
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2023-09-08 13:45:47.000000 impose-0.4.6/impose/gui/dlg_edit_shape.py
--rw-r--r--   0 runner    (1001) docker     (127)     6651 2023-09-08 13:45:47.000000 impose-0.4.6/impose/gui/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2023-09-08 13:45:47.000000 impose-0.4.6/impose/gui/main.ui
--rw-r--r--   0 runner    (1001) docker     (127)    10090 2023-09-08 13:45:47.000000 impose-0.4.6/impose/gui/visualize.py
--rw-r--r--   0 runner    (1001) docker     (127)    11148 2023-09-08 13:45:47.000000 impose-0.4.6/impose/gui/visualize.ui
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:46:32.375792 impose-0.4.6/impose/gui/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2023-09-08 13:45:47.000000 impose-0.4.6/impose/gui/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2023-09-08 13:45:47.000000 impose-0.4.6/impose/gui/widgets/simple_image_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2023-09-08 13:45:47.000000 impose-0.4.6/impose/gui/widgets/simple_plot_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2023-09-08 13:45:47.000000 impose-0.4.6/impose/gui/widgets/wait_cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    11748 2023-09-08 13:45:47.000000 impose-0.4.6/impose/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:46:32.375792 impose-0.4.6/impose/structure/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2023-09-08 13:45:47.000000 impose-0.4.6/impose/structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7937 2023-09-08 13:45:47.000000 impose-0.4.6/impose/structure/composite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2023-09-08 13:45:47.000000 impose-0.4.6/impose/structure/composite_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     7235 2023-09-08 13:45:47.000000 impose-0.4.6/impose/structure/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2023-09-08 13:45:47.000000 impose-0.4.6/impose/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:46:32.367792 impose-0.4.6/impose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2023-09-08 13:46:32.000000 impose-0.4.6/impose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2023-09-08 13:46:32.000000 impose-0.4.6/impose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-08 13:46:32.000000 impose-0.4.6/impose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2023-09-08 13:46:32.000000 impose-0.4.6/impose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-09-08 13:46:32.000000 impose-0.4.6/impose.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-09-08 13:46:32.383792 impose-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2023-09-08 13:45:47.000000 impose-0.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:46:32.379792 impose-0.4.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2023-09-08 13:45:47.000000 impose-0.4.6/tests/common_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2023-09-08 13:45:47.000000 impose-0.4.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 13:46:32.383792 impose-0.4.6/tests/data/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4464 2023-09-08 13:45:47.000000 impose-0.4.6/tests/data/brillouin-invalid.h5
--rw-r--r--   0 runner    (1001) docker     (127)     7566 2023-09-08 13:45:47.000000 impose-0.4.6/tests/data/brillouin-wo-signature.impose-session
--rw-r--r--   0 runner    (1001) docker     (127)   118968 2023-09-08 13:45:47.000000 impose-0.4.6/tests/data/brillouin.h5
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2023-09-08 13:45:47.000000 impose-0.4.6/tests/data/brillouin.impose-composite
--rw-r--r--   0 runner    (1001) docker     (127)     7894 2023-09-08 13:45:47.000000 impose-0.4.6/tests/data/brillouin.impose-session
--rw-r--r--   0 runner    (1001) docker     (127)     6301 2023-09-08 13:45:47.000000 impose-0.4.6/tests/data/brillouin_cutout.impose-session
--rw-r--r--   0 runner    (1001) docker     (127)    99622 2023-09-08 13:45:47.000000 impose-0.4.6/tests/data/fmt_brillouin-h5_bmlab-session_2022.zip
--rw-r--r--   0 runner    (1001) docker     (127)   194328 2023-09-08 13:45:47.000000 impose-0.4.6/tests/data/fmt_brillouin-h5_bmlab-session_2022_2-rep.zip
--rw-r--r--   0 runner    (1001) docker     (127)   426967 2023-09-08 13:45:47.000000 impose-0.4.6/tests/data/fmt_brillouin-h5_bmlab-session_2022_water.zip
--rw-r--r--   0 runner    (1001) docker     (127)   881709 2023-09-08 13:45:47.000000 impose-0.4.6/tests/data/fmt_brillouin-h5_bmlab-session_2022_water_2-rep.zip
--rw-r--r--   0 runner    (1001) docker     (127)   333519 2023-09-08 13:45:47.000000 impose-0.4.6/tests/data/lsm-fish.zip
--rw-r--r--   0 runner    (1001) docker     (127)      450 2023-09-08 13:45:47.000000 impose-0.4.6/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-09-08 13:45:47.000000 impose-0.4.6/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2023-09-08 13:45:47.000000 impose-0.4.6/tests/test_data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2023-09-08 13:45:47.000000 impose-0.4.6/tests/test_flblend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2023-09-08 13:45:47.000000 impose-0.4.6/tests/test_fmt_czi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2023-09-08 13:45:47.000000 impose-0.4.6/tests/test_fmt_h5_brillouin_bmlab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2023-09-08 13:45:47.000000 impose-0.4.6/tests/test_fmt_h5_brillouin_legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)    12289 2023-09-08 13:45:47.000000 impose-0.4.6/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3852 2023-09-08 13:45:47.000000 impose-0.4.6/tests/test_gui_collect.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2023-09-08 13:45:47.000000 impose-0.4.6/tests/test_gui_colocalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     9366 2023-09-08 13:45:47.000000 impose-0.4.6/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     8281 2023-09-08 13:45:47.000000 impose-0.4.6/tests/test_structure_composite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2023-09-08 13:45:47.000000 impose-0.4.6/tests/test_structure_composite_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2023-09-08 13:45:47.000000 impose-0.4.6/tests/test_structure_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2023-09-08 13:45:47.000000 impose-0.4.6/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:52:00.076837 impose-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-16 21:51:33.000000 impose-0.4.8/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-16 21:51:33.000000 impose-0.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-16 21:51:33.000000 impose-0.4.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-16 21:52:00.076837 impose-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-16 21:51:33.000000 impose-0.4.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:52:00.060837 impose-0.4.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-16 21:51:33.000000 impose-0.4.8/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6434 2024-05-16 21:51:33.000000 impose-0.4.8/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:52:00.060837 impose-0.4.8/docs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-16 21:51:33.000000 impose-0.4.8/docs/extensions/github_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-16 21:51:33.000000 impose-0.4.8/docs/impose.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-16 21:51:33.000000 impose-0.4.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-16 21:51:33.000000 impose-0.4.8/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-16 21:51:33.000000 impose-0.4.8/docs/sec_changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-16 21:51:33.000000 impose-0.4.8/docs/sec_getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-16 21:51:33.000000 impose-0.4.8/docs/sec_z_bib.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:52:00.060837 impose-0.4.8/impose/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-16 21:51:33.000000 impose-0.4.8/impose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-16 21:51:33.000000 impose-0.4.8/impose/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7035 2024-05-16 21:51:33.000000 impose-0.4.8/impose/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-16 21:51:40.000000 impose-0.4.8/impose/_version_save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7783 2024-05-16 21:51:33.000000 impose-0.4.8/impose/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9185 2024-05-16 21:51:33.000000 impose-0.4.8/impose/flblend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:52:00.064837 impose-0.4.8/impose/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-16 21:51:33.000000 impose-0.4.8/impose/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-16 21:51:33.000000 impose-0.4.8/impose/formats/fmt_bf_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-16 21:51:33.000000 impose-0.4.8/impose/formats/fmt_bm_bmlab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-16 21:51:33.000000 impose-0.4.8/impose/formats/fmt_fl_ometif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-05-16 21:51:33.000000 impose-0.4.8/impose/formats/fmt_fl_zeiss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:52:00.064837 impose-0.4.8/impose/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-16 21:51:33.000000 impose-0.4.8/impose/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-16 21:51:33.000000 impose-0.4.8/impose/geometry/mask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:52:00.064837 impose-0.4.8/impose/geometry/shapes/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-16 21:51:33.000000 impose-0.4.8/impose/geometry/shapes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-16 21:51:33.000000 impose-0.4.8/impose/geometry/shapes/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-16 21:51:33.000000 impose-0.4.8/impose/geometry/shapes/sh_circle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-05-16 21:51:33.000000 impose-0.4.8/impose/geometry/shapes/sh_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-05-16 21:51:33.000000 impose-0.4.8/impose/geometry/shapes/sh_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-05-16 21:51:33.000000 impose-0.4.8/impose/geometry/shapes/sh_rectangle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:52:00.068837 impose-0.4.8/impose/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-16 21:51:33.000000 impose-0.4.8/impose/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11665 2024-05-16 21:51:33.000000 impose-0.4.8/impose/gui/collect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11634 2024-05-16 21:51:33.000000 impose-0.4.8/impose/gui/collect.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-16 21:51:33.000000 impose-0.4.8/impose/gui/collect_pgrois.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-05-16 21:51:33.000000 impose-0.4.8/impose/gui/collect_shape_controls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-05-16 21:51:33.000000 impose-0.4.8/impose/gui/collect_shape_controls.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    14301 2024-05-16 21:51:33.000000 impose-0.4.8/impose/gui/colocalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15704 2024-05-16 21:51:33.000000 impose-0.4.8/impose/gui/colocalize.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    11685 2024-05-16 21:51:33.000000 impose-0.4.8/impose/gui/colocalize_pgrois.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-05-16 21:51:33.000000 impose-0.4.8/impose/gui/dlg_edit_circle.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     5564 2024-05-16 21:51:33.000000 impose-0.4.8/impose/gui/dlg_edit_ellipse.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-16 21:51:33.000000 impose-0.4.8/impose/gui/dlg_edit_polygon.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-05-16 21:51:33.000000 impose-0.4.8/impose/gui/dlg_edit_rectangle.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-16 21:51:33.000000 impose-0.4.8/impose/gui/dlg_edit_shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-05-16 21:51:33.000000 impose-0.4.8/impose/gui/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-05-16 21:51:33.000000 impose-0.4.8/impose/gui/main.ui
+-rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-05-16 21:51:33.000000 impose-0.4.8/impose/gui/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11148 2024-05-16 21:51:33.000000 impose-0.4.8/impose/gui/visualize.ui
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:52:00.068837 impose-0.4.8/impose/gui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-16 21:51:33.000000 impose-0.4.8/impose/gui/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-16 21:51:33.000000 impose-0.4.8/impose/gui/widgets/simple_image_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-05-16 21:51:33.000000 impose-0.4.8/impose/gui/widgets/simple_plot_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-16 21:51:33.000000 impose-0.4.8/impose/gui/widgets/wait_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11748 2024-05-16 21:51:33.000000 impose-0.4.8/impose/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:52:00.068837 impose-0.4.8/impose/structure/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-16 21:51:33.000000 impose-0.4.8/impose/structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-05-16 21:51:33.000000 impose-0.4.8/impose/structure/composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-05-16 21:51:33.000000 impose-0.4.8/impose/structure/composite_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7235 2024-05-16 21:51:33.000000 impose-0.4.8/impose/structure/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-16 21:51:33.000000 impose-0.4.8/impose/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:52:00.064837 impose-0.4.8/impose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-16 21:52:00.000000 impose-0.4.8/impose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-16 21:52:00.000000 impose-0.4.8/impose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 21:52:00.000000 impose-0.4.8/impose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-16 21:52:00.000000 impose-0.4.8/impose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 21:52:00.000000 impose-0.4.8/impose.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-16 21:52:00.080837 impose-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-16 21:51:33.000000 impose-0.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:52:00.072837 impose-0.4.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-16 21:51:33.000000 impose-0.4.8/tests/common_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-16 21:51:33.000000 impose-0.4.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:52:00.076837 impose-0.4.8/tests/data/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4464 2024-05-16 21:51:33.000000 impose-0.4.8/tests/data/brillouin-invalid.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     7566 2024-05-16 21:51:33.000000 impose-0.4.8/tests/data/brillouin-wo-signature.impose-session
+-rw-r--r--   0 runner    (1001) docker     (127)   118968 2024-05-16 21:51:33.000000 impose-0.4.8/tests/data/brillouin.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-16 21:51:33.000000 impose-0.4.8/tests/data/brillouin.impose-composite
+-rw-r--r--   0 runner    (1001) docker     (127)     7894 2024-05-16 21:51:33.000000 impose-0.4.8/tests/data/brillouin.impose-session
+-rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-05-16 21:51:33.000000 impose-0.4.8/tests/data/brillouin_cutout.impose-session
+-rw-r--r--   0 runner    (1001) docker     (127)    99622 2024-05-16 21:51:33.000000 impose-0.4.8/tests/data/fmt_brillouin-h5_bmlab-session_2022.zip
+-rw-r--r--   0 runner    (1001) docker     (127)   194328 2024-05-16 21:51:33.000000 impose-0.4.8/tests/data/fmt_brillouin-h5_bmlab-session_2022_2-rep.zip
+-rw-r--r--   0 runner    (1001) docker     (127)   426967 2024-05-16 21:51:33.000000 impose-0.4.8/tests/data/fmt_brillouin-h5_bmlab-session_2022_water.zip
+-rw-r--r--   0 runner    (1001) docker     (127)   881709 2024-05-16 21:51:33.000000 impose-0.4.8/tests/data/fmt_brillouin-h5_bmlab-session_2022_water_2-rep.zip
+-rw-r--r--   0 runner    (1001) docker     (127)   287183 2024-05-16 21:51:33.000000 impose-0.4.8/tests/data/fmt_fl_ometif.zip
+-rw-r--r--   0 runner    (1001) docker     (127)   333519 2024-05-16 21:51:33.000000 impose-0.4.8/tests/data/lsm-fish.zip
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-16 21:51:33.000000 impose-0.4.8/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 21:51:33.000000 impose-0.4.8/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-16 21:51:33.000000 impose-0.4.8/tests/test_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-16 21:51:33.000000 impose-0.4.8/tests/test_flblend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-16 21:51:33.000000 impose-0.4.8/tests/test_fmt_czi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-16 21:51:33.000000 impose-0.4.8/tests/test_fmt_fl_ometif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-16 21:51:33.000000 impose-0.4.8/tests/test_fmt_h5_brillouin_bmlab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-16 21:51:33.000000 impose-0.4.8/tests/test_fmt_h5_brillouin_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12289 2024-05-16 21:51:33.000000 impose-0.4.8/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-05-16 21:51:33.000000 impose-0.4.8/tests/test_gui_collect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-16 21:51:33.000000 impose-0.4.8/tests/test_gui_colocalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9366 2024-05-16 21:51:33.000000 impose-0.4.8/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-05-16 21:51:33.000000 impose-0.4.8/tests/test_structure_composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-16 21:51:33.000000 impose-0.4.8/tests/test_structure_composite_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-16 21:51:33.000000 impose-0.4.8/tests/test_structure_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-16 21:51:33.000000 impose-0.4.8/tests/test_util.py
```

### Comparing `impose-0.4.6/CHANGELOG` & `impose-0.4.8/CHANGELOG`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+0.4.8
+ - maintenance release
+0.4.7
+ - enh: support .ome.tif files (no stacks supported yet)
 0.4.6
  - maintenance release
 0.4.5
  - maintenance release
 0.4.4
  - maintenance release
 0.4.3
```

### Comparing `impose-0.4.6/LICENSE` & `impose-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/PKG-INFO` & `impose-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impose
-Version: 0.4.6
+Version: 0.4.8
 Summary: Fit and superimpose shapes from different imaging modalities
 Home-page: https://github.com/GuckLab/impose
 Maintainer: Paul Müller
 Maintainer-email: dev@craban.de
 License: GPL v3
 Keywords: image analysis,biology,microscopy
 Platform: ALL
```

### Comparing `impose-0.4.6/README.rst` & `impose-0.4.8/README.rst`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/docs/conf.py` & `impose-0.4.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/docs/extensions/github_changelog.py` & `impose-0.4.8/docs/extensions/github_changelog.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/docs/index.rst` & `impose-0.4.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/docs/sec_getting_started.rst` & `impose-0.4.8/docs/sec_getting_started.rst`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/__main__.py` & `impose-0.4.8/impose/__main__.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/_version.py` & `impose-0.4.8/impose/_version.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/data.py` & `impose-0.4.8/impose/data.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/flblend.py` & `impose-0.4.8/impose/flblend.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/formats/__init__.py` & `impose-0.4.8/impose/formats/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # - bf: Bright-Field Microscopy
 # - bm: Brillouin Microscopy
 # - fl: Fluorescence Microscopy
 
 from .fmt_fl_zeiss import load_czi
 from .fmt_bm_bmlab import load_h5
 from .fmt_bf_generic import load_img
+from .fmt_fl_ometif import load_ometif
 
 
 def load(path):
     """Load image data from microscopy files
 
     Parameters
     ----------
@@ -68,11 +69,12 @@
     """Convenience function for getting the signature of a data file"""
     _, meta = load(path)
     return meta["signature"]
 
 
 suffix_dict = {
     ".czi": load_czi,
-    ".png": load_img,
     ".h5": load_h5,
     ".jpg": load_img,
+    ".png": load_img,
+    ".tif": load_ometif,
 }
```

### Comparing `impose-0.4.6/impose/formats/fmt_bf_generic.py` & `impose-0.4.8/impose/formats/fmt_bf_generic.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/formats/fmt_bm_bmlab.py` & `impose-0.4.8/impose/formats/fmt_bm_bmlab.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/formats/fmt_fl_zeiss.py` & `impose-0.4.8/impose/formats/fmt_fl_zeiss.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/geometry/__init__.py` & `impose-0.4.8/impose/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/geometry/mask.py` & `impose-0.4.8/impose/geometry/mask.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/geometry/shapes/base.py` & `impose-0.4.8/impose/geometry/shapes/base.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/geometry/shapes/sh_circle.py` & `impose-0.4.8/impose/geometry/shapes/sh_circle.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/geometry/shapes/sh_ellipse.py` & `impose-0.4.8/impose/geometry/shapes/sh_ellipse.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/geometry/shapes/sh_polygon.py` & `impose-0.4.8/impose/geometry/shapes/sh_polygon.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/geometry/shapes/sh_rectangle.py` & `impose-0.4.8/impose/geometry/shapes/sh_rectangle.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/gui/collect.py` & `impose-0.4.8/impose/gui/collect.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/gui/collect.ui` & `impose-0.4.8/impose/gui/collect.ui`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/gui/collect_pgrois.py` & `impose-0.4.8/impose/gui/collect_pgrois.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/gui/collect_shape_controls.py` & `impose-0.4.8/impose/gui/collect_shape_controls.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/gui/collect_shape_controls.ui` & `impose-0.4.8/impose/gui/collect_shape_controls.ui`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/gui/colocalize.py` & `impose-0.4.8/impose/gui/colocalize.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/gui/colocalize.ui` & `impose-0.4.8/impose/gui/colocalize.ui`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/gui/colocalize_pgrois.py` & `impose-0.4.8/impose/gui/colocalize_pgrois.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/gui/dlg_edit_circle.ui` & `impose-0.4.8/impose/gui/dlg_edit_circle.ui`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/gui/dlg_edit_ellipse.ui` & `impose-0.4.8/impose/gui/dlg_edit_ellipse.ui`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/gui/dlg_edit_polygon.ui` & `impose-0.4.8/impose/gui/dlg_edit_polygon.ui`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/gui/dlg_edit_rectangle.ui` & `impose-0.4.8/impose/gui/dlg_edit_rectangle.ui`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/gui/dlg_edit_shape.py` & `impose-0.4.8/impose/gui/dlg_edit_shape.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/gui/main.py` & `impose-0.4.8/impose/gui/main.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/gui/main.ui` & `impose-0.4.8/impose/gui/main.ui`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/gui/visualize.py` & `impose-0.4.8/impose/gui/visualize.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/gui/visualize.ui` & `impose-0.4.8/impose/gui/visualize.ui`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/gui/widgets/simple_image_view.py` & `impose-0.4.8/impose/gui/widgets/simple_image_view.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/gui/widgets/simple_plot_widget.py` & `impose-0.4.8/impose/gui/widgets/simple_plot_widget.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/gui/widgets/wait_cursor.py` & `impose-0.4.8/impose/gui/widgets/wait_cursor.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/session.py` & `impose-0.4.8/impose/session.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/structure/composite.py` & `impose-0.4.8/impose/structure/composite.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/structure/composite_stack.py` & `impose-0.4.8/impose/structure/composite_stack.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/structure/layer.py` & `impose-0.4.8/impose/structure/layer.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose/util.py` & `impose-0.4.8/impose/util.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/impose.egg-info/PKG-INFO` & `impose-0.4.8/impose.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impose
-Version: 0.4.6
+Version: 0.4.8
 Summary: Fit and superimpose shapes from different imaging modalities
 Home-page: https://github.com/GuckLab/impose
 Maintainer: Paul Müller
 Maintainer-email: dev@craban.de
 License: GPL v3
 Keywords: image analysis,biology,microscopy
 Platform: ALL
```

### Comparing `impose-0.4.6/impose.egg-info/SOURCES.txt` & `impose-0.4.8/impose.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 impose.egg-info/SOURCES.txt
 impose.egg-info/dependency_links.txt
 impose.egg-info/requires.txt
 impose.egg-info/top_level.txt
 impose/formats/__init__.py
 impose/formats/fmt_bf_generic.py
 impose/formats/fmt_bm_bmlab.py
+impose/formats/fmt_fl_ometif.py
 impose/formats/fmt_fl_zeiss.py
 impose/geometry/__init__.py
 impose/geometry/mask.py
 impose/geometry/shapes/__init__.py
 impose/geometry/shapes/base.py
 impose/geometry/shapes/sh_circle.py
 impose/geometry/shapes/sh_ellipse.py
@@ -67,14 +68,15 @@
 tests/common_gui.py
 tests/conftest.py
 tests/helpers.py
 tests/requirements.txt
 tests/test_data_source.py
 tests/test_flblend.py
 tests/test_fmt_czi.py
+tests/test_fmt_fl_ometif.py
 tests/test_fmt_h5_brillouin_bmlab.py
 tests/test_fmt_h5_brillouin_legacy.py
 tests/test_geometry.py
 tests/test_gui_collect.py
 tests/test_gui_colocalize.py
 tests/test_session.py
 tests/test_structure_composite.py
@@ -87,8 +89,9 @@
 tests/data/brillouin.impose-composite
 tests/data/brillouin.impose-session
 tests/data/brillouin_cutout.impose-session
 tests/data/fmt_brillouin-h5_bmlab-session_2022.zip
 tests/data/fmt_brillouin-h5_bmlab-session_2022_2-rep.zip
 tests/data/fmt_brillouin-h5_bmlab-session_2022_water.zip
 tests/data/fmt_brillouin-h5_bmlab-session_2022_water_2-rep.zip
+tests/data/fmt_fl_ometif.zip
 tests/data/lsm-fish.zip
```

### Comparing `impose-0.4.6/setup.py` & `impose-0.4.8/setup.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/tests/common_gui.py` & `impose-0.4.8/tests/common_gui.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/tests/conftest.py` & `impose-0.4.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/tests/data/brillouin-invalid.h5` & `impose-0.4.8/tests/data/brillouin-invalid.h5`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/tests/data/brillouin-wo-signature.impose-session` & `impose-0.4.8/tests/data/brillouin-wo-signature.impose-session`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/tests/data/brillouin.h5` & `impose-0.4.8/tests/data/brillouin.h5`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/tests/data/brillouin.impose-composite` & `impose-0.4.8/tests/data/brillouin.impose-composite`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/tests/data/brillouin.impose-session` & `impose-0.4.8/tests/data/brillouin.impose-session`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/tests/data/brillouin_cutout.impose-session` & `impose-0.4.8/tests/data/brillouin_cutout.impose-session`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/tests/data/fmt_brillouin-h5_bmlab-session_2022.zip` & `impose-0.4.8/tests/data/fmt_brillouin-h5_bmlab-session_2022.zip`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/tests/data/fmt_brillouin-h5_bmlab-session_2022_2-rep.zip` & `impose-0.4.8/tests/data/fmt_brillouin-h5_bmlab-session_2022_2-rep.zip`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/tests/data/fmt_brillouin-h5_bmlab-session_2022_water.zip` & `impose-0.4.8/tests/data/fmt_brillouin-h5_bmlab-session_2022_water.zip`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/tests/data/fmt_brillouin-h5_bmlab-session_2022_water_2-rep.zip` & `impose-0.4.8/tests/data/fmt_brillouin-h5_bmlab-session_2022_water_2-rep.zip`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/tests/data/lsm-fish.zip` & `impose-0.4.8/tests/data/lsm-fish.zip`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/tests/test_data_source.py` & `impose-0.4.8/tests/test_data_source.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/tests/test_flblend.py` & `impose-0.4.8/tests/test_flblend.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/tests/test_fmt_h5_brillouin_bmlab.py` & `impose-0.4.8/tests/test_fmt_h5_brillouin_bmlab.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/tests/test_fmt_h5_brillouin_legacy.py` & `impose-0.4.8/tests/test_fmt_h5_brillouin_legacy.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/tests/test_geometry.py` & `impose-0.4.8/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/tests/test_gui_collect.py` & `impose-0.4.8/tests/test_gui_collect.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/tests/test_session.py` & `impose-0.4.8/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/tests/test_structure_composite.py` & `impose-0.4.8/tests/test_structure_composite.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/tests/test_structure_composite_stack.py` & `impose-0.4.8/tests/test_structure_composite_stack.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/tests/test_structure_layer.py` & `impose-0.4.8/tests/test_structure_layer.py`

 * *Files identical despite different names*

### Comparing `impose-0.4.6/tests/test_util.py` & `impose-0.4.8/tests/test_util.py`

 * *Files identical despite different names*

