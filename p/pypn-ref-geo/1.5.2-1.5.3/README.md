# Comparing `tmp/pypn-ref-geo-1.5.2.tar.gz` & `tmp/pypn_ref_geo-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypn-ref-geo-1.5.2.tar", last modified: Wed Apr 10 05:22:00 2024, max compression
+gzip compressed data, was "pypn_ref_geo-1.5.3.tar", last modified: Thu May 23 15:02:35 2024, max compression
```

## Comparing `pypn-ref-geo-1.5.2.tar` & `pypn_ref_geo-1.5.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:22:00.922731 pypn-ref-geo-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-10 05:22:00.922731 pypn-ref-geo-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      160 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 05:22:00.922731 pypn-ref-geo-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:22:00.914731 pypn-ref-geo-1.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:22:00.922731 pypn-ref-geo-1.5.2/src/pypn_ref_geo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-10 05:22:00.000000 pypn-ref-geo-1.5.2/src/pypn_ref_geo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-10 05:22:00.000000 pypn-ref-geo-1.5.2/src/pypn_ref_geo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 05:22:00.000000 pypn-ref-geo-1.5.2/src/pypn_ref_geo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-10 05:22:00.000000 pypn-ref-geo-1.5.2/src/pypn_ref_geo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-10 05:22:00.000000 pypn-ref-geo-1.5.2/src/pypn_ref_geo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 05:22:00.000000 pypn-ref-geo-1.5.2/src/pypn_ref_geo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:22:00.918731 pypn-ref-geo-1.5.2/src/ref_geo/
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:22:00.918731 pypn-ref-geo-1.5.2/src/ref_geo/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:22:00.918731 pypn-ref-geo-1.5.2/src/ref_geo/migrations/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16369 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/data/ref_geo.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/data/ref_geo_cor.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/data/ref_geo_linear.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/data/ref_geo_point.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:22:00.922731 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/05a0ae652c13_ref_geo_french_regions_1970.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/0dfdbfbccd63_ref_geo_french_municipalities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/3fdaa1805575_ref_geo_french_departments.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/4882d6141a41_add_regions_in_area_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/586613e2faeb_ref_geo_inpn_grids_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/681306b27407_fix_altitude_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/6afe74833ed0_ref_geo.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/795f6ea8ec45_cor_linear_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/7d6e98441e4c_ref_geo_inpn_grids_5.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/bc2fcc772b46_geom_4326.py
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/cb038e76d59c_fix_functions_local_srid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/d02f4563bebe_ref_geo_french_regions.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/dea1645de8c0_ref_geo_point.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/e0ac4c9f5c0a_add_indexes_on_fk_referencing_id_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/ede150d9afd9_ref_geo_inpn_grids_10.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/f22d70b8fcfa_add_areas_types_size_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/f7374cd6e38d_ref_geo_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/fda887e7b578_correct_area_name_for_COM.py
--rw-r--r--   0 runner    (1001) docker     (127)     7369 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     9628 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-10 05:21:56.000000 pypn-ref-geo-1.5.2/src/ref_geo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:02:35.728170 pypn_ref_geo-1.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-23 15:02:35.724170 pypn_ref_geo-1.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      160 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 15:02:35.728170 pypn_ref_geo-1.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:02:35.716170 pypn_ref_geo-1.5.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:02:35.724170 pypn_ref_geo-1.5.3/src/pypn_ref_geo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-23 15:02:35.000000 pypn_ref_geo-1.5.3/src/pypn_ref_geo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-23 15:02:35.000000 pypn_ref_geo-1.5.3/src/pypn_ref_geo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:02:35.000000 pypn_ref_geo-1.5.3/src/pypn_ref_geo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-23 15:02:35.000000 pypn_ref_geo-1.5.3/src/pypn_ref_geo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-23 15:02:35.000000 pypn_ref_geo-1.5.3/src/pypn_ref_geo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 15:02:35.000000 pypn_ref_geo-1.5.3/src/pypn_ref_geo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:02:35.720170 pypn_ref_geo-1.5.3/src/ref_geo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/src/ref_geo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/src/ref_geo/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/src/ref_geo/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:02:35.720170 pypn_ref_geo-1.5.3/src/ref_geo/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/src/ref_geo/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:02:35.720170 pypn_ref_geo-1.5.3/src/ref_geo/migrations/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/src/ref_geo/migrations/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16369 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/src/ref_geo/migrations/data/ref_geo.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/src/ref_geo/migrations/data/ref_geo_cor.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/src/ref_geo/migrations/data/ref_geo_linear.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/src/ref_geo/migrations/data/ref_geo_point.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/src/ref_geo/migrations/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/src/ref_geo/migrations/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:02:35.724170 pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/05a0ae652c13_ref_geo_french_regions_1970.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/0dfdbfbccd63_ref_geo_french_municipalities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/3fdaa1805575_ref_geo_french_departments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/4882d6141a41_add_regions_in_area_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/586613e2faeb_ref_geo_inpn_grids_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/681306b27407_fix_altitude_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/6afe74833ed0_ref_geo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/795f6ea8ec45_cor_linear_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/7d6e98441e4c_ref_geo_inpn_grids_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/bc2fcc772b46_geom_4326.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/cb038e76d59c_fix_functions_local_srid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/d02f4563bebe_ref_geo_french_regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/dea1645de8c0_ref_geo_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/e0ac4c9f5c0a_add_indexes_on_fk_referencing_id_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/ede150d9afd9_ref_geo_inpn_grids_10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/f22d70b8fcfa_add_areas_types_size_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/f7374cd6e38d_ref_geo_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/fda887e7b578_correct_area_name_for_COM.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7369 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/src/ref_geo/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/src/ref_geo/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/src/ref_geo/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-23 15:02:31.000000 pypn_ref_geo-1.5.3/src/ref_geo/utils.py
```

### Comparing `pypn-ref-geo-1.5.2/CHANGELOG.md` & `pypn_ref_geo-1.5.3/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 CHANGELOG
 =========
 
-1.5.2 (2024-09-10)
+1.5.3 (2024-05-23)
+------------------
+
+**🐛 Corrections**
+
+ - Correction de l'intégration des paramètres de type `list` dans la route `/areas` (#26)
+ 
+
+1.5.2 (2024-04-10)
 ------------------
 
 **🚀 Nouveautés**
 
  - Possibilité d'appeler la route `GET/areas` sans retourner les géométries (#22)
 
 1.5.1 (2024-01-29)
```

### Comparing `pypn-ref-geo-1.5.2/LICENSE` & `pypn_ref_geo-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.2/PKG-INFO` & `pypn_ref_geo-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypn-ref-geo
-Version: 1.5.2
+Version: 1.5.3
 Summary: Référentiel géographique
 Home-page: https://github.com/PnX-SI/RefGeo
 Maintainer: Parcs nationaux des Écrins et des Cévennes
 Maintainer-email: geonature@ecrins-parcnational.fr
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -18,15 +18,15 @@
 Requires-Dist: alembic
 Requires-Dist: flask>=3.0
 Requires-Dist: flask-sqlalchemy
 Requires-Dist: flask-marshmallow
 Requires-Dist: python-dotenv
 Requires-Dist: sqlalchemy<2,>=1.4
 Requires-Dist: utils-flask-sqlalchemy>=0.4.1
-Requires-Dist: utils-flask-sqlalchemy-geo>=0.3.1
+Requires-Dist: utils-flask-sqlalchemy-geo>=0.3.2
 Requires-Dist: psycopg2
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-flask; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: jsonschema; extra == "tests"
```

### Comparing `pypn-ref-geo-1.5.2/README.md` & `pypn_ref_geo-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.2/setup.py` & `pypn_ref_geo-1.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.2/src/pypn_ref_geo.egg-info/PKG-INFO` & `pypn_ref_geo-1.5.3/src/pypn_ref_geo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypn-ref-geo
-Version: 1.5.2
+Version: 1.5.3
 Summary: Référentiel géographique
 Home-page: https://github.com/PnX-SI/RefGeo
 Maintainer: Parcs nationaux des Écrins et des Cévennes
 Maintainer-email: geonature@ecrins-parcnational.fr
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -18,15 +18,15 @@
 Requires-Dist: alembic
 Requires-Dist: flask>=3.0
 Requires-Dist: flask-sqlalchemy
 Requires-Dist: flask-marshmallow
 Requires-Dist: python-dotenv
 Requires-Dist: sqlalchemy<2,>=1.4
 Requires-Dist: utils-flask-sqlalchemy>=0.4.1
-Requires-Dist: utils-flask-sqlalchemy-geo>=0.3.1
+Requires-Dist: utils-flask-sqlalchemy-geo>=0.3.2
 Requires-Dist: psycopg2
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-flask; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: jsonschema; extra == "tests"
```

### Comparing `pypn-ref-geo-1.5.2/src/pypn_ref_geo.egg-info/SOURCES.txt` & `pypn_ref_geo-1.5.3/src/pypn_ref_geo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.2/src/ref_geo/__init__.py` & `pypn_ref_geo-1.5.3/src/ref_geo/__init__.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.2/src/ref_geo/commands.py` & `pypn_ref_geo-1.5.3/src/ref_geo/commands.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.2/src/ref_geo/env.py` & `pypn_ref_geo-1.5.3/src/ref_geo/env.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.2/src/ref_geo/migrations/data/ref_geo.sql` & `pypn_ref_geo-1.5.3/src/ref_geo/migrations/data/ref_geo.sql`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.2/src/ref_geo/migrations/data/ref_geo_cor.sql` & `pypn_ref_geo-1.5.3/src/ref_geo/migrations/data/ref_geo_cor.sql`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.2/src/ref_geo/migrations/data/ref_geo_linear.sql` & `pypn_ref_geo-1.5.3/src/ref_geo/migrations/data/ref_geo_linear.sql`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.2/src/ref_geo/migrations/data/ref_geo_point.sql` & `pypn_ref_geo-1.5.3/src/ref_geo/migrations/data/ref_geo_point.sql`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.2/src/ref_geo/migrations/env.py` & `pypn_ref_geo-1.5.3/src/ref_geo/migrations/env.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.2/src/ref_geo/migrations/utils.py` & `pypn_ref_geo-1.5.3/src/ref_geo/migrations/utils.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/05a0ae652c13_ref_geo_french_regions_1970.py` & `pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/05a0ae652c13_ref_geo_french_regions_1970.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/0dfdbfbccd63_ref_geo_french_municipalities.py` & `pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/0dfdbfbccd63_ref_geo_french_municipalities.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/3fdaa1805575_ref_geo_french_departments.py` & `pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/3fdaa1805575_ref_geo_french_departments.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/4882d6141a41_add_regions_in_area_types.py` & `pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/4882d6141a41_add_regions_in_area_types.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/586613e2faeb_ref_geo_inpn_grids_1.py` & `pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/586613e2faeb_ref_geo_inpn_grids_1.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/681306b27407_fix_altitude_trigger.py` & `pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/681306b27407_fix_altitude_trigger.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/6afe74833ed0_ref_geo.py` & `pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/6afe74833ed0_ref_geo.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/795f6ea8ec45_cor_linear_area.py` & `pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/795f6ea8ec45_cor_linear_area.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/7d6e98441e4c_ref_geo_inpn_grids_5.py` & `pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/7d6e98441e4c_ref_geo_inpn_grids_5.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/bc2fcc772b46_geom_4326.py` & `pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/bc2fcc772b46_geom_4326.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/cb038e76d59c_fix_functions_local_srid.py` & `pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/cb038e76d59c_fix_functions_local_srid.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/d02f4563bebe_ref_geo_french_regions.py` & `pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/d02f4563bebe_ref_geo_french_regions.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/dea1645de8c0_ref_geo_point.py` & `pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/dea1645de8c0_ref_geo_point.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/e0ac4c9f5c0a_add_indexes_on_fk_referencing_id_area.py` & `pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/e0ac4c9f5c0a_add_indexes_on_fk_referencing_id_area.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/ede150d9afd9_ref_geo_inpn_grids_10.py` & `pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/ede150d9afd9_ref_geo_inpn_grids_10.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/f22d70b8fcfa_add_areas_types_size_hierarchy.py` & `pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/f22d70b8fcfa_add_areas_types_size_hierarchy.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/f7374cd6e38d_ref_geo_linear.py` & `pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/f7374cd6e38d_ref_geo_linear.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.2/src/ref_geo/migrations/versions/fda887e7b578_correct_area_name_for_COM.py` & `pypn_ref_geo-1.5.3/src/ref_geo/migrations/versions/fda887e7b578_correct_area_name_for_COM.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.2/src/ref_geo/models.py` & `pypn_ref_geo-1.5.3/src/ref_geo/models.py`

 * *Files identical despite different names*

### Comparing `pypn-ref-geo-1.5.2/src/ref_geo/routes.py` & `pypn_ref_geo-1.5.3/src/ref_geo/routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,25 +206,27 @@
             query = query.where(LAreas.enable == True)
         elif enable_param == "false":
             query = query.where(LAreas.enable == False)
     else:
         query = query.where(LAreas.enable == True)
 
     if "id_type" in params:
-        query = query.where(LAreas.id_type.in_(params.getlist("id_type")))
+        # getlist() of request.args does not use the syntax url?param=val1,val2
+        id_type = params.get("id_type").split(",")
+        query = query.where(LAreas.id_type.in_(id_type))
 
     if "type_code" in params:
-        query = query.where(
-            LAreas.area_type.has(BibAreasTypes.type_code.in_(params.getlist("type_code")))
-        )
+        # getlist() of request.args does not use the syntax url?param=val1,val2
+        type_code = params.get("type_code").split(",")
+        query = query.where(LAreas.area_type.has(BibAreasTypes.type_code.in_(type_code)))
 
     if "area_name" in params:
         query = query.where(LAreas.area_name.ilike("%{}%".format(params.get("area_name"))))
 
-    without_geom = params.get("without_geom", False, lambda x: x == "true")
+    without_geom = request.args.get("without_geom", False, lambda x: x == "true")
     if without_geom:
         query = query.options(defer("geom"))
         marsh_params["exclude"] = ["geom"]
 
     limit = int(params.get("limit")[0]) if params.get("limit") else 100
 
     fields = {"area_type.type_code"}
```

### Comparing `pypn-ref-geo-1.5.2/src/ref_geo/schemas.py` & `pypn_ref_geo-1.5.3/src/ref_geo/schemas.py`

 * *Files identical despite different names*

