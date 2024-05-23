# Comparing `tmp/exoplanet-atlas-0.3.0.tar.gz` & `tmp/exoplanet_atlas-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exoplanet-atlas-0.3.0.tar", last modified: Mon Mar 20 19:54:36 2023, max compression
+gzip compressed data, was "exoplanet_atlas-0.3.3.tar", last modified: Thu May 23 06:46:05 2024, max compression
```

## Comparing `exoplanet-atlas-0.3.0.tar` & `exoplanet_atlas-0.3.3.tar`

### file list

```diff
@@ -1,121 +1,82 @@
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-03-20 19:54:36.255981 exoplanet-atlas-0.3.0/
--rw-r--r--   0 zach       (502) staff       (20)      818 2023-03-19 19:25:48.000000 exoplanet-atlas-0.3.0/.gitignore
--rw-r--r--   0 zach       (502) staff       (20)      108 2021-02-08 19:36:42.000000 exoplanet-atlas-0.3.0/.readthedocs.yaml
--rw-r--r--   0 zach       (502) staff       (20)     1086 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/LICENSE
--rw-r--r--   0 zach       (502) staff       (20)       99 2021-02-08 19:36:42.000000 exoplanet-atlas-0.3.0/MANIFEST.in
--rw-r--r--   0 zach       (502) staff       (20)      595 2023-03-20 19:54:36.255834 exoplanet-atlas-0.3.0/PKG-INFO
--rw-r--r--   0 zach       (502) staff       (20)     1921 2021-02-08 19:36:42.000000 exoplanet-atlas-0.3.0/README.md
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-03-20 19:54:36.245898 exoplanet-atlas-0.3.0/docs/
--rw-r--r--   0 zach       (502) staff       (20)      613 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/docs/Makefile
--rw-r--r--   0 zach       (502) staff       (20)      201 2021-02-08 19:36:42.000000 exoplanet-atlas-0.3.0/docs/api.workinprogress
--rw-r--r--   0 zach       (502) staff       (20)     5305 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/docs/conf.py
--rw-r--r--   0 zach       (502) staff       (20)      823 2021-02-08 19:36:42.000000 exoplanet-atlas-0.3.0/docs/index.rst
--rw-r--r--   0 zach       (502) staff       (20)       81 2021-02-08 19:36:42.000000 exoplanet-atlas-0.3.0/docs/requirements.txt
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-03-20 19:54:36.246331 exoplanet-atlas-0.3.0/exoatlas/
--rw-r--r--   0 zach       (502) staff       (20)      170 2021-04-01 20:59:46.000000 exoplanet-atlas-0.3.0/exoatlas/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)     4398 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/imports.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-03-20 19:54:36.246889 exoplanet-atlas-0.3.0/exoatlas/models/
--rw-r--r--   0 zach       (502) staff       (20)       87 2021-02-08 19:36:42.000000 exoplanet-atlas-0.3.0/exoatlas/models/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)     2084 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/models/chen.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-03-20 19:54:36.247003 exoplanet-atlas-0.3.0/exoatlas/models/data/
--rw-r--r--   0 zach       (502) staff       (20)      245 2021-02-08 19:36:42.000000 exoplanet-atlas-0.3.0/exoatlas/models/data/README.txt
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-03-20 19:54:36.247344 exoplanet-atlas-0.3.0/exoatlas/models/data/seager/
--rw-r--r--   0 zach       (502) staff       (20)      157 2021-02-08 19:36:42.000000 exoplanet-atlas-0.3.0/exoatlas/models/data/seager/README.txt
--rw-r--r--   0 zach       (502) staff       (20)      368 2021-02-08 19:36:42.000000 exoplanet-atlas-0.3.0/exoatlas/models/data/seager/gj1214mr_hhe.txt
--rw-r--r--   0 zach       (502) staff       (20)      202 2021-02-08 19:36:42.000000 exoplanet-atlas-0.3.0/exoatlas/models/data/seager/gj1214mr_rock.txt
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-03-20 19:54:36.248519 exoplanet-atlas-0.3.0/exoatlas/models/data/zengandsasselov/
--rw-r--r--   0 zach       (502) staff       (20)     6107 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/models/data/zengandsasselov/MR_100pFe.csv
--rw-r--r--   0 zach       (502) staff       (20)     6126 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/models/data/zengandsasselov/MR_100pH2O.csv
--rw-r--r--   0 zach       (502) staff       (20)     6107 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/models/data/zengandsasselov/MR_100pSi.csv
--rw-r--r--   0 zach       (502) staff       (20)     6124 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/models/data/zengandsasselov/MR_25pSi_75pFe.csv
--rw-r--r--   0 zach       (502) staff       (20)     6107 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/models/data/zengandsasselov/MR_25pSi_75pH2O.csv
--rw-r--r--   0 zach       (502) staff       (20)     6105 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/models/data/zengandsasselov/MR_50pSi_50pFe.csv
--rw-r--r--   0 zach       (502) staff       (20)     6107 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/models/data/zengandsasselov/MR_50pSi_50pH2O.csv
--rw-r--r--   0 zach       (502) staff       (20)     6121 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/models/data/zengandsasselov/MR_75pSi_25pFe.csv
--rw-r--r--   0 zach       (502) staff       (20)      106 2021-02-08 19:36:42.000000 exoplanet-atlas-0.3.0/exoatlas/models/data/zengandsasselov/README.txt
--rw-r--r--   0 zach       (502) staff       (20)     1542 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/models/kopparapu.py
--rw-r--r--   0 zach       (502) staff       (20)     1164 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/models/seager.py
--rw-r--r--   0 zach       (502) staff       (20)      955 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/models/zeng.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-03-20 19:54:36.250076 exoplanet-atlas-0.3.0/exoatlas/populations/
--rw-r--r--   0 zach       (502) staff       (20)    13944 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/populations/Exoplanets.py
--rw-r--r--   0 zach       (502) staff       (20)    50139 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/populations/Population.py
--rw-r--r--   0 zach       (502) staff       (20)     3531 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/populations/SolarSystem.py
--rw-r--r--   0 zach       (502) staff       (20)       62 2021-02-08 19:36:42.000000 exoplanet-atlas-0.3.0/exoatlas/populations/TESS.py
--rw-r--r--   0 zach       (502) staff       (20)     7516 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/populations/TOI.py
--rw-r--r--   0 zach       (502) staff       (20)     3488 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/populations/TOISubsets.py
--rw-r--r--   0 zach       (502) staff       (20)     3351 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/populations/TransitingExoplanets.py
--rw-r--r--   0 zach       (502) staff       (20)     5568 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/populations/TransitingExoplanetsSubsets.py
--rw-r--r--   0 zach       (502) staff       (20)      416 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/populations/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)      716 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/populations/collections.py
--rw-r--r--   0 zach       (502) staff       (20)     2236 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/populations/column_descriptions.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-03-20 19:54:36.250409 exoplanet-atlas-0.3.0/exoatlas/populations/curation/
--rw-r--r--   0 zach       (502) staff       (20)     7741 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/populations/curation/Confirmed.py
--rw-r--r--   0 zach       (502) staff       (20)       26 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/populations/curation/TransitingExoplanets.py
--rw-r--r--   0 zach       (502) staff       (20)        0 2021-02-08 19:36:42.000000 exoplanet-atlas-0.3.0/exoatlas/populations/curation/__init__.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-03-20 19:54:36.250487 exoplanet-atlas-0.3.0/exoatlas/populations/data/
--rw-r--r--   0 zach       (502) staff       (20)      252 2021-02-08 19:36:42.000000 exoplanet-atlas-0.3.0/exoatlas/populations/data/README.txt
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-03-20 19:54:36.250860 exoplanet-atlas-0.3.0/exoatlas/populations/data/exoplanet-archive-columns/
--rw-r--r--   0 zach       (502) staff       (20)      378 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/populations/data/exoplanet-archive-columns/exoarchive-columns-with-errors-and-limits.txt
--rw-r--r--   0 zach       (502) staff       (20)      245 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/populations/data/exoplanet-archive-columns/exoarchive-columns-with-errors.txt
--rw-r--r--   0 zach       (502) staff       (20)      325 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/populations/data/exoplanet-archive-columns/exoarchive-columns-without-errors.txt
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-03-20 19:54:36.250964 exoplanet-atlas-0.3.0/exoatlas/populations/data/solarsystem/
--rw-r--r--   0 zach       (502) staff       (20)      237 2021-02-08 19:36:42.000000 exoplanet-atlas-0.3.0/exoatlas/populations/data/solarsystem/solarsystem.txt
--rw-r--r--   0 zach       (502) staff       (20)     9114 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/populations/downloaders.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-03-20 19:54:36.251404 exoplanet-atlas-0.3.0/exoatlas/populations/needs-revision/
--rw-r--r--   0 zach       (502) staff       (20)      963 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/populations/needs-revision/Custom.py
--rw-r--r--   0 zach       (502) staff       (20)     5070 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/populations/needs-revision/KOI.py
--rw-r--r--   0 zach       (502) staff       (20)     1972 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/populations/needs-revision/PredictedTESS.py
--rw-r--r--   0 zach       (502) staff       (20)     5314 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/populations/needs-revision/TOI-will-table.py
--rw-r--r--   0 zach       (502) staff       (20)     1926 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/populations/summary.py
--rw-r--r--   0 zach       (502) staff       (20)     2734 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/talker.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-03-20 19:54:36.251637 exoplanet-atlas-0.3.0/exoatlas/telescopes/
--rw-r--r--   0 zach       (502) staff       (20)       23 2021-02-08 19:36:42.000000 exoplanet-atlas-0.3.0/exoatlas/telescopes/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)     5940 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/telescopes/buckets.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-03-20 19:54:36.252641 exoplanet-atlas-0.3.0/exoatlas/tests/
--rw-r--r--   0 zach       (502) staff       (20)      268 2021-02-08 19:36:42.000000 exoplanet-atlas-0.3.0/exoatlas/tests/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)     1043 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/tests/test_buckets.py
--rw-r--r--   0 zach       (502) staff       (20)      537 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/tests/test_downloaders.py
--rw-r--r--   0 zach       (502) staff       (20)      335 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/tests/test_imports.py
--rw-r--r--   0 zach       (502) staff       (20)      647 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/tests/test_models.py
--rw-r--r--   0 zach       (502) staff       (20)     3379 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/tests/test_populations.py
--rw-r--r--   0 zach       (502) staff       (20)     2455 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/tests/test_snr.py
--rw-r--r--   0 zach       (502) staff       (20)      597 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/tests/test_uncertainties.py
--rw-r--r--   0 zach       (502) staff       (20)     1345 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/tests/test_visualizations.py
--rw-r--r--   0 zach       (502) staff       (20)      673 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/tests/test_whatsup.py
--rw-r--r--   0 zach       (502) staff       (20)       22 2023-03-20 19:43:34.000000 exoplanet-atlas-0.3.0/exoatlas/version.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-03-20 19:54:36.253396 exoplanet-atlas-0.3.0/exoatlas/visualizations/
--rw-r--r--   0 zach       (502) staff       (20)     4131 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/visualizations/MultiPanel.py
--rw-r--r--   0 zach       (502) staff       (20)      790 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/visualizations/ThumbtackMovie.py
--rw-r--r--   0 zach       (502) staff       (20)    14017 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/visualizations/ThumbtackPlot.py
--rw-r--r--   0 zach       (502) staff       (20)       95 2021-02-08 19:36:42.000000 exoplanet-atlas-0.3.0/exoatlas/visualizations/__init__.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-03-20 19:54:36.253726 exoplanet-atlas-0.3.0/exoatlas/visualizations/axes/
--rw-r--r--   0 zach       (502) staff       (20)       58 2021-02-08 19:36:42.000000 exoplanet-atlas-0.3.0/exoatlas/visualizations/axes/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)     4309 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/visualizations/axes/plottable.py
--rw-r--r--   0 zach       (502) staff       (20)    12987 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/visualizations/axes/preset_plottables.py
--rw-r--r--   0 zach       (502) staff       (20)     5898 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/visualizations/buildable.py
--rw-r--r--   0 zach       (502) staff       (20)     2842 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/visualizations/ink_errorbar.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-03-20 19:54:36.254225 exoplanet-atlas-0.3.0/exoatlas/visualizations/panels/
--rw-r--r--   0 zach       (502) staff       (20)     9712 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/visualizations/panels/BubblePanel.py
--rw-r--r--   0 zach       (502) staff       (20)     7469 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/visualizations/panels/ErrorPanel.py
--rw-r--r--   0 zach       (502) staff       (20)    11982 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/visualizations/panels/Panel.py
--rw-r--r--   0 zach       (502) staff       (20)      103 2021-02-08 19:36:42.000000 exoplanet-atlas-0.3.0/exoatlas/visualizations/panels/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)     9790 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/visualizations/panels/preset_panels.py
--rw-r--r--   0 zach       (502) staff       (20)      858 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/visualizations/tweaks.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-03-20 19:54:36.254834 exoplanet-atlas-0.3.0/exoatlas/whatsup/
--rw-r--r--   0 zach       (502) staff       (20)      164 2021-02-08 19:36:42.000000 exoplanet-atlas-0.3.0/exoatlas/whatsup/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)     2073 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/whatsup/block.py
--rw-r--r--   0 zach       (502) staff       (20)      111 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/whatsup/night.py
--rw-r--r--   0 zach       (502) staff       (20)     6515 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/whatsup/observatory.py
--rw-r--r--   0 zach       (502) staff       (20)    11223 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/whatsup/plan.py
--rw-r--r--   0 zach       (502) staff       (20)     5936 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/exoatlas/whatsup/transit.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-03-20 19:54:36.255450 exoplanet-atlas-0.3.0/exoplanet_atlas.egg-info/
--rw-r--r--   0 zach       (502) staff       (20)      595 2023-03-20 19:54:36.000000 exoplanet-atlas-0.3.0/exoplanet_atlas.egg-info/PKG-INFO
--rw-r--r--   0 zach       (502) staff       (20)     3617 2023-03-20 19:54:36.000000 exoplanet-atlas-0.3.0/exoplanet_atlas.egg-info/SOURCES.txt
--rw-r--r--   0 zach       (502) staff       (20)        1 2023-03-20 19:54:36.000000 exoplanet-atlas-0.3.0/exoplanet_atlas.egg-info/dependency_links.txt
--rw-r--r--   0 zach       (502) staff       (20)        1 2021-02-08 19:36:52.000000 exoplanet-atlas-0.3.0/exoplanet_atlas.egg-info/not-zip-safe
--rw-r--r--   0 zach       (502) staff       (20)      104 2023-03-20 19:54:36.000000 exoplanet-atlas-0.3.0/exoplanet_atlas.egg-info/requires.txt
--rw-r--r--   0 zach       (502) staff       (20)        9 2023-03-20 19:54:36.000000 exoplanet-atlas-0.3.0/exoplanet_atlas.egg-info/top_level.txt
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-03-20 19:54:36.255571 exoplanet-atlas-0.3.0/scripts/
--rw-r--r--   0 zach       (502) staff       (20)     2331 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/scripts/thumbtacks.py
--rw-r--r--   0 zach       (502) staff       (20)       38 2023-03-20 19:54:36.256024 exoplanet-atlas-0.3.0/setup.cfg
--rw-r--r--   0 zach       (502) staff       (20)     3661 2023-03-20 19:43:26.000000 exoplanet-atlas-0.3.0/setup.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-23 06:46:05.430907 exoplanet_atlas-0.3.3/
+-rw-r--r--   0 zach       (502) staff       (20)     1091 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/LICENSE
+-rw-r--r--   0 zach       (502) staff       (20)     1533 2024-05-23 06:46:05.430569 exoplanet_atlas-0.3.3/PKG-INFO
+-rw-r--r--   0 zach       (502) staff       (20)     1921 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/README.md
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-23 06:46:05.408072 exoplanet_atlas-0.3.3/exoatlas/
+-rw-r--r--   0 zach       (502) staff       (20)      179 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)     4483 2024-05-23 06:36:30.000000 exoplanet_atlas-0.3.3/exoatlas/imports.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-23 06:46:05.410150 exoplanet_atlas-0.3.3/exoatlas/models/
+-rw-r--r--   0 zach       (502) staff       (20)       87 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/models/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)     2084 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/models/chen.py
+-rw-r--r--   0 zach       (502) staff       (20)     1541 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/models/kopparapu.py
+-rw-r--r--   0 zach       (502) staff       (20)     1171 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/models/seager.py
+-rw-r--r--   0 zach       (502) staff       (20)      963 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/models/zeng.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-23 06:46:05.415813 exoplanet_atlas-0.3.3/exoatlas/populations/
+-rw-r--r--   0 zach       (502) staff       (20)    13402 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/populations/Exoplanets.py
+-rw-r--r--   0 zach       (502) staff       (20)    51413 2024-05-23 06:36:30.000000 exoplanet_atlas-0.3.3/exoatlas/populations/Population.py
+-rw-r--r--   0 zach       (502) staff       (20)     3598 2024-05-23 06:36:30.000000 exoplanet_atlas-0.3.3/exoatlas/populations/SolarSystem.py
+-rw-r--r--   0 zach       (502) staff       (20)       62 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/populations/TESS.py
+-rw-r--r--   0 zach       (502) staff       (20)     7538 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/populations/TOI.py
+-rw-r--r--   0 zach       (502) staff       (20)     3485 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/populations/TOISubsets.py
+-rw-r--r--   0 zach       (502) staff       (20)     3351 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/populations/TransitingExoplanets.py
+-rw-r--r--   0 zach       (502) staff       (20)     5718 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/populations/TransitingExoplanetsSubsets.py
+-rw-r--r--   0 zach       (502) staff       (20)      416 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/populations/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)      716 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/populations/collections.py
+-rw-r--r--   0 zach       (502) staff       (20)     2258 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/populations/column_descriptions.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-23 06:46:05.416800 exoplanet_atlas-0.3.3/exoatlas/populations/curation/
+-rw-r--r--   0 zach       (502) staff       (20)     7747 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/populations/curation/Confirmed.py
+-rw-r--r--   0 zach       (502) staff       (20)       26 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/populations/curation/TransitingExoplanets.py
+-rw-r--r--   0 zach       (502) staff       (20)        0 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/populations/curation/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)     8991 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/populations/downloaders.py
+-rw-r--r--   0 zach       (502) staff       (20)     1963 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/populations/summary.py
+-rw-r--r--   0 zach       (502) staff       (20)     2735 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/talker.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-23 06:46:05.417321 exoplanet_atlas-0.3.3/exoatlas/telescopes/
+-rw-r--r--   0 zach       (502) staff       (20)       23 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/telescopes/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)     6048 2024-05-23 06:36:30.000000 exoplanet_atlas-0.3.3/exoatlas/telescopes/buckets.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-23 06:46:05.420467 exoplanet_atlas-0.3.3/exoatlas/tests/
+-rw-r--r--   0 zach       (502) staff       (20)      268 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/tests/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)       40 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/tests/setup_tests.py
+-rw-r--r--   0 zach       (502) staff       (20)     1070 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/tests/test_buckets.py
+-rw-r--r--   0 zach       (502) staff       (20)      578 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/tests/test_downloaders.py
+-rw-r--r--   0 zach       (502) staff       (20)      363 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/tests/test_imports.py
+-rw-r--r--   0 zach       (502) staff       (20)      675 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/tests/test_models.py
+-rw-r--r--   0 zach       (502) staff       (20)     3284 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/tests/test_populations.py
+-rw-r--r--   0 zach       (502) staff       (20)     2489 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/tests/test_snr.py
+-rw-r--r--   0 zach       (502) staff       (20)      612 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/tests/test_uncertainties.py
+-rw-r--r--   0 zach       (502) staff       (20)     1390 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/tests/test_visualizations.py
+-rw-r--r--   0 zach       (502) staff       (20)      701 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/tests/test_whatsup.py
+-rw-r--r--   0 zach       (502) staff       (20)       62 2024-05-23 06:36:30.000000 exoplanet_atlas-0.3.3/exoatlas/version.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-23 06:46:05.422507 exoplanet_atlas-0.3.3/exoatlas/visualizations/
+-rw-r--r--   0 zach       (502) staff       (20)     4131 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/visualizations/MultiPanel.py
+-rw-r--r--   0 zach       (502) staff       (20)      790 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/visualizations/ThumbtackMovie.py
+-rw-r--r--   0 zach       (502) staff       (20)    14017 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/visualizations/ThumbtackPlot.py
+-rw-r--r--   0 zach       (502) staff       (20)       95 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/visualizations/__init__.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-23 06:46:05.423253 exoplanet_atlas-0.3.3/exoatlas/visualizations/axes/
+-rw-r--r--   0 zach       (502) staff       (20)       58 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/visualizations/axes/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)     4309 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/visualizations/axes/plottable.py
+-rw-r--r--   0 zach       (502) staff       (20)    13910 2024-05-23 06:36:30.000000 exoplanet_atlas-0.3.3/exoatlas/visualizations/axes/preset_plottables.py
+-rw-r--r--   0 zach       (502) staff       (20)     8240 2024-05-23 06:36:30.000000 exoplanet_atlas-0.3.3/exoatlas/visualizations/buildable.py
+-rw-r--r--   0 zach       (502) staff       (20)     2846 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/visualizations/ink_errorbar.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-23 06:46:05.424922 exoplanet_atlas-0.3.3/exoatlas/visualizations/panels/
+-rw-r--r--   0 zach       (502) staff       (20)     9710 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/visualizations/panels/BubblePanel.py
+-rw-r--r--   0 zach       (502) staff       (20)     7716 2024-05-23 06:36:30.000000 exoplanet_atlas-0.3.3/exoatlas/visualizations/panels/ErrorPanel.py
+-rw-r--r--   0 zach       (502) staff       (20)    12096 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/visualizations/panels/Panel.py
+-rw-r--r--   0 zach       (502) staff       (20)      103 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/visualizations/panels/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)     9782 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/visualizations/panels/preset_panels.py
+-rw-r--r--   0 zach       (502) staff       (20)      858 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/visualizations/tweaks.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-23 06:46:05.427521 exoplanet_atlas-0.3.3/exoatlas/whatsup/
+-rw-r--r--   0 zach       (502) staff       (20)      164 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/whatsup/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)     2073 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/whatsup/block.py
+-rw-r--r--   0 zach       (502) staff       (20)      111 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/whatsup/night.py
+-rw-r--r--   0 zach       (502) staff       (20)     6515 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/whatsup/observatory.py
+-rw-r--r--   0 zach       (502) staff       (20)    11246 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/whatsup/plan.py
+-rw-r--r--   0 zach       (502) staff       (20)     5940 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/whatsup/transit.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-23 06:46:05.429070 exoplanet_atlas-0.3.3/exoplanet_atlas.egg-info/
+-rw-r--r--   0 zach       (502) staff       (20)     1533 2024-05-23 06:46:05.000000 exoplanet_atlas-0.3.3/exoplanet_atlas.egg-info/PKG-INFO
+-rw-r--r--   0 zach       (502) staff       (20)     2288 2024-05-23 06:46:05.000000 exoplanet_atlas-0.3.3/exoplanet_atlas.egg-info/SOURCES.txt
+-rw-r--r--   0 zach       (502) staff       (20)        1 2024-05-23 06:46:05.000000 exoplanet_atlas-0.3.3/exoplanet_atlas.egg-info/dependency_links.txt
+-rw-r--r--   0 zach       (502) staff       (20)        1 2024-05-20 18:33:32.000000 exoplanet_atlas-0.3.3/exoplanet_atlas.egg-info/not-zip-safe
+-rw-r--r--   0 zach       (502) staff       (20)      300 2024-05-23 06:46:05.000000 exoplanet_atlas-0.3.3/exoplanet_atlas.egg-info/requires.txt
+-rw-r--r--   0 zach       (502) staff       (20)        9 2024-05-23 06:46:05.000000 exoplanet_atlas-0.3.3/exoplanet_atlas.egg-info/top_level.txt
+-rw-r--r--   0 zach       (502) staff       (20)       38 2024-05-23 06:46:05.430973 exoplanet_atlas-0.3.3/setup.cfg
+-rw-r--r--   0 zach       (502) staff       (20)     4028 2024-05-23 06:36:30.000000 exoplanet_atlas-0.3.3/setup.py
```

### Comparing `exoplanet-atlas-0.3.0/LICENSE` & `exoplanet_atlas-0.3.3/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2015 Zach Berta-Thompson
+Copyright (c) 2015-2024 Zach Berta-Thompson
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `exoplanet-atlas-0.3.0/README.md` & `exoplanet_atlas-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `exoplanet-atlas-0.3.0/exoatlas/imports.py` & `exoplanet_atlas-0.3.3/exoatlas/imports.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # imports that are need by many exoatlas subsections
-import os, sys, time, shutil, warnings, copy
-from unittest import mock
+import os, sys, time, shutil, warnings, copy, importlib
 from tqdm import tqdm
-import pytest
+
+code_directory = importlib.resources.files(__name__)
+
 
 import numpy as np, matplotlib.pyplot as plt, matplotlib.animation as animation
 from matplotlib.ticker import ScalarFormatter, FormatStrFormatter, LogLocator
 
 
 from astropy.utils.exceptions import AstropyDeprecationWarning
 
@@ -70,31 +71,34 @@
     assert base is not None
 except AssertionError:
     # otherwise put it in the local directory
     cwd = os.getcwd()
     base = os.path.join(cwd, "exoatlas-downloads")
 mkdir(base)
 
+
+def locate_local_data():
+    print("💾 `exoatlas` archive data will be stored in:")
+    print(base)
+
+
 directories = dict(data=os.path.join(base, "data/"))
 for k in directories.keys():
     mkdir(directories[k])
 
 
 def reset_local_data():
     if "y" in input(
         "Are you sure you want to wipe all " "local exoplanet-atlas data files? [y/N]"
     ):
         shutil.rmtree(directories["data"])
         mkdir(directories["data"])
         print(f"Removed all local data from {directories['data']}")
 
 
-from pkg_resources import resource_filename
-
-
 # some kludge for dealing with Python 3 vs 2?
 try:
     FileNotFoundError
 except NameError:
     FileNotFoundError = IOError
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `exoplanet-atlas-0.3.0/exoatlas/models/chen.py` & `exoplanet_atlas-0.3.3/exoatlas/models/chen.py`

 * *Files identical despite different names*

### Comparing `exoplanet-atlas-0.3.0/exoatlas/models/kopparapu.py` & `exoplanet_atlas-0.3.3/exoatlas/models/kopparapu.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Tools for working with the habitable zone definitions
 in Kopparapu et al. (2013).
 """
 
-
 coefficients = {}
 coefficients["recent-venus"] = [1.7753, 1.4316e-4, 2.9875e-9, -7.5702e-12, -1.1635e-15]
 coefficients["runaway-greenhouse"] = [
     1.0512,
     1.3242e-4,
     1.5418e-8,
     -7.9895e-12,
```

### Comparing `exoplanet-atlas-0.3.0/exoatlas/models/seager.py` & `exoplanet_atlas-0.3.3/exoatlas/models/seager.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,17 +13,16 @@
     ----------
     which : str
         Options are 'rock' or 'HHe'
     """
 
     assert (which.lower() == "rock") or (which.lower() == "hhe")
 
-    file = resource_filename(__name__, f"data/seager/gj1214mr_{which}.txt")
-
     # load the values
+    file = os.path.join(code_directory, f"models/data/seager/gj1214mr_{which}.txt")
     m, r = np.transpose(np.loadtxt(file))
 
     # fit a simply polynomial to smooth out the messiness
     fit = np.poly1d(np.polyfit(np.log(m), np.log(r), 5))
 
     # plot over a grid of masses
     mm = np.logspace(np.log10(min(m)), np.log10(max(m)), 1000)
```

### Comparing `exoplanet-atlas-0.3.0/exoatlas/models/zeng.py` & `exoplanet_atlas-0.3.3/exoatlas/models/zeng.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Parameters
     ----------
     which : str
         A string to indicate which model to plot.
 
     """
 
-    file = resource_filename(__name__, f"data/zengandsasselov/MR_{which}.csv")
+    file = os.path.join(code_directory, f"models/data/zengandsasselov/MR_{which}.csv")
 
     # load the values
     m, r = np.transpose(np.loadtxt(file, delimiter=","))
 
     # plot the values
     return plt.plot(m, r, **kw)
```

### Comparing `exoplanet-atlas-0.3.0/exoatlas/populations/Exoplanets.py` & `exoplanet_atlas-0.3.3/exoatlas/populations/Exoplanets.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,28 +50,14 @@
         raw : astropy.table.Table
             A raw, untrimmed, unstandardized table.
         """
 
         # load (or download) the table of composite exoplanet properties
         raw = exoplanets_downloader.get(remake=remake)
 
-        # populate which type of columns are which
-        # populate what kinds of columns are what
-
-        """columns_directory = resource_filename(
-            __name__, "data/exoplanet-archive-columns/"
-        )
-        for k in ["with-errors-and-limits", "with-errors", "without-errors"]:
-            column_names = np.genfromtxt(
-                os.path.join(columns_directory, f"exoarchive-columns-{k}.txt"),
-                str,
-                comments="#",
-            )
-            raw.meta[f"columns-{k}"] = column_names"""
-
         # for debugging, hang on to the raw table as a hidden attribute
         self._raw = raw
 
         return raw
 
     def trim_raw(self, raw):
         """
@@ -86,15 +72,15 @@
         -------
         trimmed : astropy.table.Table
             A raw, trimmed, unstandardized table.
         """
 
         masks = {}
 
-        ok = np.ones(len(raw)).astype(np.bool)
+        ok = np.ones(len(raw)).astype(bool)
         for k in masks:
             ok *= masks[k]
             N = sum(ok == True)
             self.speak(f"{N} planets pass the `{k}` filter")
 
         # trim down the table to just those that are OK
         trimmed = raw[ok]
```

### Comparing `exoplanet-atlas-0.3.0/exoatlas/populations/Population.py` & `exoplanet_atlas-0.3.3/exoatlas/populations/Population.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # general class for exoplanet populations
 from ..imports import *
 from ..telescopes import *
 from ..models import *
 
 import string
 
-basic_columns = ["name", "hostname", "ra", "dec", "distance", "discoverer"]
+basic_columns = ["name", "hostname", "ra", "dec", "distance", "discovery_facility"]
 
 transit_columns = [
     "period",
     "semimajoraxis",
-    "e",
+    "eccentricity",
     "omega",
     "inclination",
-    "transit_epoch",
+    "transit_midpoint",
     "transit_duration",
     "transit_depth",
     "stellar_teff",
     "stellar_mass",
     "stellar_radius",
     "radius",
     "mass",
@@ -1108,15 +1108,15 @@
             depth = (2 * H * Rp / Rs**2).decompose()
 
             dlnm = self.uncertainty("mass") / self.mass
             bad = dlnm > 1 / threshold
             depth[bad] = np.nan
             return depth
 
-    def reflection_signal(self, albedo=1.0):
+    def reflection_signal(self, albedo=0.1):
         """
         What is the reflected light eclipse depth,
         for an albedo of 100%?
         """
         return albedo * 0.25 * (self.radius / self.semimajor_axis).decompose() ** 2
 
     def emission_signal(self, wavelength=5 * u.micron):
@@ -1286,14 +1286,25 @@
         )
 
         # create a telescope unit (mostly to get a default wavelength)
         telescope_unit = define_telescope_unit_by_name(telescope_name, **kw)
 
         return noise, telescope_unit
 
+    def depth_snr(self, telescope_name="JWST", **kw):
+        """
+        What's the approximate S/N for the detection of the planet's transit?
+        """
+
+        noise, telescope_unit = self._get_noise_and_unit(
+            telescope_name=telescope_name, **kw
+        )
+        signal = self.transit_depth
+        return signal / noise
+
     def emission_snr(self, telescope_name="JWST", **kw):
         """
         What's the approximate S/N for the detection of the
         thermal emission eclipse of a planet?
         """
 
         noise, telescope_unit = self._get_noise_and_unit(
@@ -1407,21 +1418,96 @@
 
         maxarea = 1000
         area = self.__dict__[area]
         sizeplot = np.sqrt(area / np.nanmax(area) * maxarea)
 
         plt.scatter(xplot, yplot, linewidth=0, marker="o", markersize=sizeplot)
 
+    def create_table(
+        self,
+        desired_columns=[
+            "name",
+            "radius",
+            "relative_insolation",
+            "stellar_radius",
+            "stellar_teff",
+            "ra",
+            "dec",
+            "distance",
+        ],
+    ):
+        """
+        Create an astropy table based on this population,
+        using a subset of columns, which may include ones
+        that have been calculated as Population properties.
+
+        Parameters
+        ----------
+        desired_columns : list
+            The columns you want to include. Anything that
+            can be accessed via Population.??? can be provided
+            here as a string.
+
+        Returns
+        -------
+        table : astropy.table.Table
+            A table, with those columns, in the same order
+            as the Population itself.
+        """
+        # FIXME! need to add method support for arguments
+
+        # create a dictionary with the desired columns
+        d = {c: getattr(self, c) for c in desired_columns}
+
+        # turn that into an astropy Table
+        t = Table(d)
+
+        return t
+
+    def create_planning_table(
+        self,
+        desired_columns=[
+            "name",
+            "ra",
+            "dec",
+            "period",
+            "transit_midpoint",
+            "transit_duration",
+            "radius",
+            "relative_insolation",
+            "stellar_radius",
+            "stellar_teff",
+            "distance",
+        ],
+    ):
+        """
+        Create an astropy table to help plan transit observations.
+
+        Parameters
+        ----------
+        desired_columns : list
+            The columns you want to include. Anything that
+            can be accessed via Population.??? can be provided
+            here as a string.
+
+        Returns
+        -------
+        table : astropy.table.Table
+            A table, with those columns, in the same order
+            as the Population itself.
+        """
+        return self.create_table(desired_columns=desired_columns)
+
 
 class PredefinedPopulation(Population):
     """
     Population object keeps track of an exoplanet population.
     """
 
-    expiration = 0.00001
+    expiration = 10
 
     def __init__(self, label="exoplanets", remake=False, skip_update=False, **plotkw):
         """
         Initialize a population, by trying the following steps:
                 1) Load a standardized ascii table.
                 2) Ingest a raw table, and standardize it.
 
@@ -1556,48 +1642,7 @@
         Save the standardized table out to a text file
         like ~/exoatlas/standardized-*.txt
         """
 
         # save it as an ascii table for humans to read
         standard.write(self.standard_path, format="ascii.ecsv", overwrite=True)
         self.speak(f"Saved a standardized text table to {self.standard_path}")
-
-    def create_table(
-        self,
-        desired_columns=[
-            "name",
-            "radius",
-            "relative_insolation",
-            "stellar_radius",
-            "stellar_teff",
-            "ra",
-            "dec",
-            "distance",
-        ],
-    ):
-        """
-        Create an astropy table based on this population,
-        using a subset of columns, which may include ones
-        that have been calculated as Population properties.
-
-        Parameters
-        ----------
-        desired_columns : list
-            The columns you want to include. Anything that
-            can be accessed via Population.??? can be provided
-            here as a string.
-
-        Returns
-        -------
-        table : astropy.table.Table
-            A table, with those columns, in the same order
-            as the Population itself.
-        """
-        # FIXME! need to add method support for arguments
-
-        # create a dictionary with the desired columns
-        d = {c: getattr(self, c) for c in desired_columns}
-
-        # turn that into an astropy Table
-        t = Table(d)
-
-        return t
```

### Comparing `exoplanet-atlas-0.3.0/exoatlas/populations/SolarSystem.py` & `exoplanet_atlas-0.3.3/exoatlas/populations/SolarSystem.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from ..imports import *
 from .Population import PredefinedPopulation
 import astropy.units as u
 
 __all__ = ["SolarSystem"]
 
-initial_filename = resource_filename(__name__, "data/solarsystem/solarsystem.txt")
+initial_filename = os.path.join(
+    code_directory, "populations/data/solarsystem/solarsystem.txt"
+)
 
 
 class SolarSystem(PredefinedPopulation):
     """The Solar System, very crudely."""
 
     # the data in the table probably don't need to be updated
     expiration = np.inf
@@ -19,14 +21,15 @@
         """
         PredefinedPopulation.__init__(self, label="Solar System", **kwargs)
         self.color = "cornflowerblue"
         self.zorder = 1e10
         self.s = 80
         self.respond_to_color = False
         self.exact = True
+        self.marker = "s"
 
     def load_raw(self):
         """
         Load the raw table of data for the Solar System.
         """
 
         # load the table of Solar System planets
@@ -60,15 +63,15 @@
         s["stellar_mass"] = 1.0 * u.Msun
         s["stellar_age"] = 4.5 * u.Gyr
 
         # store the period, by default, in day
         s["period"] = (t["period"] * u.year).to(u.day)
 
         # store an eccentricity and longitude of periastron
-        s["e"] = np.nan
+        s["eccentricity"] = np.nan
         s["omega"] = np.nan * u.deg
 
         # hide the stellar magnitudes
         s["Jmag"] = np.nan
         s["Vmag"] = np.nan
 
         # pull out the radius and mass
@@ -92,16 +95,16 @@
         s["rv_semiamplitude"] = np.nan * u.m / u.s
         s["radius_ratio"] = (
             (s["radius"].quantity / s["stellar_radius"].quantity).decompose().value
         )
         s["distance"] = np.nan * u.pc
         s["ra"] = 0.0 * u.deg
         s["dec"] = 0.0 * u.deg
-        s["discoverer"] = "humans"
-        s["transit_epoch"] = np.nan * u.day
+        s["discovery_facility"] = "humans"
+        s["transit_midpoint"] = np.nan * u.day
         s["transit_duration"] = np.nan * u.day
         s["transit_depth"] = (
             s["radius"].quantity / s["stellar_radius"].quantity
         ).decompose() ** 2
         s["transit_b"] = 0.0
         s["inclination"] = 90 * u.deg
```

### Comparing `exoplanet-atlas-0.3.0/exoatlas/populations/TOI.py` & `exoplanet_atlas-0.3.3/exoatlas/populations/TOI.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         with np.errstate(invalid="ignore"):
             # is this a relatively cool star?
             masks["cool"] = raw["Stellar Eff Temp (K)"] < 20000
 
             # is this not a single-transit candidate (without period)?
             masks["notsingle"] = raw["Period (days)"] > 0
 
-        ok = np.ones(len(raw)).astype(np.bool)
+        ok = np.ones(len(raw)).astype(bool)
         for k in masks:
             ok *= masks[k]
             N = sum(ok == True)
             self.speak(f"{N} planets pass the `{k}` filter")
 
         # trim down the table to just those that are OK
         trimmed = raw[ok]
@@ -83,24 +83,24 @@
         s["hostname"] = [f"TOI{toi:.0f}" for toi in t["TOI"]]
 
         s["TIC ID"] = t["TIC ID"]  # maybe remove, carefully?
         s["tic"] = s["TIC ID"]
 
         s["distance"] = t["Stellar Distance (pc)"] * u.pc
         s["distance_uncertainty"] = t["Stellar Distance (pc) err"] * u.pc
-        s["discoverer"] = "TESS"
+        s["discovery_facility"] = "TESS"
 
         s["period"] = t["Period (days)"] * u.day
         s["period_uncertainty"] = t["Period (days) err"] * u.day
 
-        s["e"] = np.nan
+        s["eccentricity"] = np.nan
         s["omega"] = np.nan * u.deg
 
-        s["transit_epoch"] = t["Epoch (BJD)"] * u.day
-        # s['transit_epoch_uncertainty'] = t['Epoch (BJD) err']*u.day
+        s["transit_midpoint"] = t["Epoch (BJD)"] * u.day
+        # s['transit_midpoint_uncertainty'] = t['Epoch (BJD) err']*u.day
 
         s["transit_duration"] = t["Duration (hours)"] * u.hour
         s["transit_duration_uncertainty"] = t["Duration (hours) err"] * u.hour
 
         s["transit_depth"] = t["Depth (ppm)"] / 1e6
         s["transit_depth_uncertainty"] = t["Depth (ppm) err"] / 1e6
```

### Comparing `exoplanet-atlas-0.3.0/exoatlas/populations/TOISubsets.py` & `exoplanet_atlas-0.3.3/exoatlas/populations/TOISubsets.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         # find only those planets that have periods close to each other
         dp = (matched_known.period - matched_toi.period) / matched_known.period
         closeperiod = np.abs(dp) < np.inf  # FIXME -- kludge!0.1
         matched_toi.standard["dp"] = dp
         matched_toi.standard["close"] = closeperiod
 
         # populate a mask with Trues where planets are close to another in space and period
-        wasknown = np.zeros(self.n).astype(np.bool)
+        wasknown = np.zeros(self.n).astype(bool)
         wasknown[i_match[closeperiod]] = True
 
         # weird = (matched_toi.period > 13*u.day)*closeperiod
         # print(matched_toi[weird].standard['name', 'period', 'radius', 'dp', 'close'])
         # print(matched_known[weird].standard['name', 'period', 'radius'])
 
         # return that array
```

### Comparing `exoplanet-atlas-0.3.0/exoatlas/populations/TransitingExoplanets.py` & `exoplanet_atlas-0.3.3/exoatlas/populations/TransitingExoplanets.py`

 * *Files identical despite different names*

### Comparing `exoplanet-atlas-0.3.0/exoatlas/populations/TransitingExoplanetsSubsets.py` & `exoplanet_atlas-0.3.3/exoatlas/populations/TransitingExoplanetsSubsets.py`

 * *Files 13% similar despite different names*

```diff
@@ -33,48 +33,56 @@
 class Kepler(TransitingExoplanetsSubset):
     def __init__(self, **kw):
         TransitingExoplanetsSubset.__init__(
             self, label="Kepler", color="royalblue", zorder=0, **kw
         )
 
     def to_include(self):
-        foundbykepler = (self.discoverer == "Kepler") | (self.discoverer == "K2")
+        foundbykepler = (self.discovery_facility == "Kepler") | (
+            self.discovery_facility == "K2"
+        )
         return foundbykepler
 
 
 class NonKepler(TransitingExoplanetsSubset):
     def __init__(self, **kw):
         TransitingExoplanetsSubset.__init__(
             self, label="Non-Kepler", color="black", zorder=0, **kw
         )
 
     def to_include(self):
-        foundbykepler = (self.discoverer == "Kepler") | (self.discoverer == "K2")
+        foundbykepler = (self.discovery_facility == "Kepler") | (
+            self.discovery_facility == "K2"
+        )
         return foundbykepler == False
 
 
 class TESS(TransitingExoplanetsSubset):
     def __init__(self, **kw):
         TransitingExoplanetsSubset.__init__(
             self, label="TESS", color="orangered", zorder=0, **kw
         )
 
     def to_include(self):
-        foundbytess = self.discoverer == "Transiting Exoplanet Survey Satellite (TESS)"
+        foundbytess = (
+            self.discovery_facility == "Transiting Exoplanet Survey Satellite (TESS)"
+        )
         return foundbytess == True
 
 
 class NonTESS(TransitingExoplanetsSubset):
     def __init__(self, **kw):
         TransitingExoplanetsSubset.__init__(
             self, label="TESS", color="black", zorder=0, **kw
         )
 
     def to_include(self):
-        foundbytess = self.discoverer == "Transiting Exoplanet Survey Satellite (TESS)"
+        foundbytess = (
+            self.discovery_facility == "Transiting Exoplanet Survey Satellite (TESS)"
+        )
         return foundbytess == False
 
 
 space_telescopes = [
     "Transiting Exoplanet Survey Satellite (TESS)",
     "K2",
     "Kepler",
@@ -86,30 +94,30 @@
 class Space(TransitingExoplanetsSubset):
     def __init__(self, **kw):
         TransitingExoplanetsSubset.__init__(
             self, label="Space-based", color="orchid", zorder=0, **kw
         )
 
     def to_include(self):
-        foundfromspace = np.zeros(self.n).astype(np.bool)
+        foundfromspace = np.zeros(self.n).astype(bool)
         for x in space_telescopes:
-            foundfromspace = foundfromspace | (self.discoverer == x)
+            foundfromspace = foundfromspace | (self.discovery_facility == x)
         return foundfromspace
 
 
 class Ground(TransitingExoplanetsSubset):
     def __init__(self, **kw):
         TransitingExoplanetsSubset.__init__(
             self, label="Ground-based", color="black", zorder=0, **kw
         )
 
     def to_include(self):
-        foundfromspace = np.zeros(self.n).astype(np.bool)
+        foundfromspace = np.zeros(self.n).astype(bool)
         for x in space_telescopes:
-            foundfromspace = foundfromspace | (self.discoverer == x)
+            foundfromspace = foundfromspace | (self.discovery_facility == x)
         return foundfromspace == False
 
 
 sigma = 2.5
 
 
 def mass_is_good(pop):
```

### Comparing `exoplanet-atlas-0.3.0/exoatlas/populations/collections.py` & `exoplanet_atlas-0.3.3/exoatlas/populations/collections.py`

 * *Files identical despite different names*

### Comparing `exoplanet-atlas-0.3.0/exoatlas/populations/column_descriptions.py` & `exoplanet_atlas-0.3.3/exoatlas/populations/column_descriptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 column_descriptions = {
     "name": "name of the planet",
     "ra": "Right Ascension of the system",
     "dec": "Declination of the system",
     "distance": "distance to the system",
     "distance_modulus": "apparent magnitude - absolute magnitude",
-    "discoverer": "telescope/project that found this planet",
+    "discovery_facility": "telescope/project that found this planet",
     "stellar_teff": "stellar effective temperature",
     "stellar_mass": "stellar mass",
     "stellar_radius": "stellar radius",
     "stellar_luminosity": "luminosity of the star",
     "stellar_brightness": "photon flux from the star at Earth (a function of wavelength)",
     "period": "orbital period of the planet",
     "semimajoraxis": "the semimajor axis of the planet's orbit",
     "a_over_rs": "scaled orbital distance a/R*",
     "b": "impact parameter b",
-    "e": "eccentricity",
+    "eccentricity": "eccentricity",
     "omega": "argument of periastron",
     "radius": "planet radius",
     "mass": "planet mass",
     "density": "density of the planet",
     "insolation": "bolometric energy flux the planet receives from its star",
     "relative_insolation": "insolation relative to Earth",
     "teq": "equilibrium temperature of the planet (assuming 0 albedo)",
     "surface_gravity": "surface gravity of the planet",
     "scale_height": "scale height of an H2-rich atmosphere",
     "escape_velocity": "escape velocity of the planet",
     "escape_parameter": "ratio of gravitational potential to thermal energy for an H atom",
-    "transit_epoch": "a transit midpoint",
+    "transit_midpoint": "a transit midpoint",
     "transit_duration": "duration of the transit",
     "transit_depth": "fraction of starlight the planet blocks",
     "transit_ar": "(transit-derived) scaled orbital distance a/R*",
     "transit_b": "(transit-derived) impact parameter b",
     "transmission_signal": "transit depth of one scale height of atmosphere",
     "emission_signal": "thermal-emission eclipse depth (a function of wavelength)",
     "reflection_signal": "reflected-light eclipse depth (for an albedo of 1)",
```

### Comparing `exoplanet-atlas-0.3.0/exoatlas/populations/curation/Confirmed.py` & `exoplanet_atlas-0.3.3/exoatlas/populations/curation/Confirmed.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         radius=1.130,
         radius_uncertainty_upper=0.056,
         radius_uncertainty_lower=-0.056,
         stellar_teff=3270.0,
         b=0.38,
         stellar_radius=0.2105,
         stellar_mass=0.181,
-        transit_epoch=2457184.55786,
+        transit_midpoint=2457184.55786,
     )
 
     pop.update_planet("30 Ari Bb", radius=np.nan)
 
     pop.update_planet("HD 17156b", transit_duration=0.1338, a_over_r=23.2, b=0.4)
 
     pop.update_planet("HD 17156b", transit_duration=0.1338, a_over_r=23.2, b=0.477)
@@ -133,15 +133,15 @@
         a_over_r=8.9,
         radius=13.630,
         radius_uncertainty_upper=0.269,
         radius_uncertainty_lower=-0.269,
         mass=369.303,
         mass_uncertainty_upper=18.433,
         mass_uncertainty_lower=-18.433,
-        transit_epoch=2454279.436714,
+        transit_midpoint=2454279.436714,
     )
 
     """ I went through all the planets shown in the Dressing et al. (2015)
         mass-radius diagram to double check the values that are present in the
         NASA Exoplanet Archive."""
 
     # parameters taken from the updates in Demory et al. (2015, *submitted*)
```

### Comparing `exoplanet-atlas-0.3.0/exoatlas/populations/downloaders.py` & `exoplanet_atlas-0.3.3/exoatlas/populations/downloaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,18 +68,14 @@
 
         self.speak(f"Download successful! Saved file to {self.path}")
 
     def add_metadata(self, *args, **kwargs):
         pass
 
 
-# columns_directory = resource_filename(__name__, "data/exoplanet-archive-columns/")
-# "exoacrhive-columns-with-errors-and-limits.txt"
-
-
 class ExoplanetArchiveDownloader(Downloader):
     # define the base of all URLs for to access the archive API
     # base = 'http://exoplanetarchive.ipac.caltech.edu/cgi-bin/nstedAPI/nph-nstedAPI?'
     base = "https://exoplanetarchive.ipac.caltech.edu/TAP/sync?"
 
     # what format do we want for the downloaded table?
     format = "csv"
@@ -114,17 +110,18 @@
         """
         Where should the local copy of this file be stored?
         """
         return os.path.join(directories["data"], f"nea-{self.table}.txt")
 
     def add_metadata(self, table):
         # populate what kinds of columns are what
-        columns_directory = resource_filename(
-            __name__, "data/exoplanet-archive-columns/"
+        columns_directory = os.path.join(
+            code_directory, "populations/data/exoplanet-archive-columns/"
         )
+
         for k in ["with-errors-and-limits", "with-errors", "without-errors"]:
             column_names = np.genfromtxt(
                 os.path.join(columns_directory, f"exoarchive-columns-{k}.txt"),
                 str,
                 comments="#",
             )
             table.meta[f"columns-{k}"] = column_names
```

### Comparing `exoplanet-atlas-0.3.0/exoatlas/populations/summary.py` & `exoplanet_atlas-0.3.3/exoatlas/populations/summary.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,32 +35,35 @@
             cols.append(x)
     cols += quant_cols
 
     # create a grid of histograms
     ncols = 3
     nrows = np.ceil(len(cols) / ncols).astype(np.int)
     scale = 2
-    fi, ax = plt.subplots(nrows, ncols, figsize=(ncols * 2 * scale, nrows * scale))
+    fi, ax = plt.subplots(
+        nrows,
+        ncols,
+        figsize=(ncols * 2 * scale, nrows * scale),
+        constrained_layout=True,
+    )
 
     for i, x in enumerate(cols):
         if x in quant_cols:
             good = np.isfinite(pop.standard[x])
         else:
-            good = np.ones(len(pop.standard)).astype(np.bool)
+            good = np.ones(len(pop.standard)).astype(bool)
         bad = good == False
         badfraction = sum(bad) / len(bad)
 
         plt.sca(ax.flatten()[i])
         plt.hist(pop.standard[x][good], color="black")
         plt.axvspan(*plt.xlim(), 0, badfraction, color="red", alpha=0.5, zorder=-1)
         plt.xlabel(x)
         plt.title(f"{x} lacks {sum(bad)}/{len(bad)} ({badfraction:.0%})")
 
-    plt.tight_layout()
-
 
 def summarize_planet(planets):
     """
     Quick tool to print out everything we need about a planet.
     """
     for p in planets:
         for k in attribute_columns:
```

### Comparing `exoplanet-atlas-0.3.0/exoatlas/talker.py` & `exoplanet_atlas-0.3.3/exoatlas/talker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 If something inherits from Talker, then we can print
 text to the terminal in a relatively standard way.
 """
+
 import textwrap, numpy as np, pprint
 import sys
 
 if sys.version_info[0] < 3:
     input = raw_input
 
 shortcuts = None
```

### Comparing `exoplanet-atlas-0.3.0/exoatlas/telescopes/buckets.py` & `exoplanet_atlas-0.3.3/exoatlas/telescopes/buckets.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     unit.telescope_name = telescope_name
     unit.wavelength = wavelength
     unit.dt = dt
     unit.R = R
     return unit
 
 
-def define_JWST_unit(wavelength=5 * u.micron, **kw):
+def define_JWST_unit(wavelength=5 * u.micron, efficiency=0.5, **kw):
     """
     Create a JWST telescope unit.
 
     Parameters
     ----------
     wavelength : astropy.unit.Quantity
         The wavelength at which it should be calculated.
@@ -73,19 +73,22 @@
         (Ignored if telescope is None.)
 
     dt : astropy.units.quantity.Quantity
         The time over which the telescope exposes.
         (Ignored if telescope is None.)
     """
     return define_telescope_unit(
-        telescope_name="JWST", wavelength=wavelength, area=25 * u.m**2, **kw
+        telescope_name="JWST",
+        wavelength=wavelength,
+        area=efficiency * 25 * u.m**2,
+        **kw,
     )
 
 
-def define_HST_unit(wavelength=1.4 * u.micron, **kw):
+def define_HST_unit(wavelength=1.4 * u.micron, efficiency=0.3, **kw):
     """
     Create a HST telescope unit.
 
     Parameters
     ----------
     wavelength : astropy.unit.Quantity
         The wavelength at which it should be calculated.
@@ -96,15 +99,18 @@
         (Ignored if telescope is None.)
 
     dt : astropy.units.quantity.Quantity
         The time over which the telescope exposes.
         (Ignored if telescope is None.)
     """
     return define_telescope_unit(
-        telescope_name="HST", wavelength=wavelength, area=4.5 * u.m**2, **kw
+        telescope_name="HST",
+        wavelength=wavelength,
+        area=efficiency * 4.5 * u.m**2,
+        **kw,
     )
 
 
 def define_APO_unit(wavelength=0.5 * u.micron, efficiency=0.1, **kw):
     """
     Create an APO telescope unit.
```

### Comparing `exoplanet-atlas-0.3.0/exoatlas/tests/test_buckets.py` & `exoplanet_atlas-0.3.3/exoatlas/tests/test_buckets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from .setup_tests import *
 from exoatlas.imports import *
 from exoatlas import *
 
 
 def test_telescope_units():
     for t in ["Kepler", "TESS", "JWST", "HST"]:
         define_telescope_unit_by_name(t)
```

### Comparing `exoplanet-atlas-0.3.0/exoatlas/tests/test_downloaders.py` & `exoplanet_atlas-0.3.3/exoatlas/tests/test_downloaders.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,25 @@
+from .setup_tests import *
+
 from exoatlas.imports import *
 from exoatlas.populations.downloaders import *
 
 
 def test_exoplanets():
     with mock.patch("builtins.input", return_value=""):
-        return exoplanets.get()
+        exoplanets_downloader.get()
 
 
-def test_composite():
-    with mock.patch("builtins.input", return_value=""):
-        return merged_exoplanets.get()
+# def test_composite():
+#    with mock.patch("builtins.input", return_value=""):
+#        composite_exoplanets_downloader.get()
 
 
-def test_tess():
-    with mock.patch("builtins.input", return_value=""):
-        return toi_exofop.get()
+# def test_tess():
+#    with mock.patch("builtins.input", return_value=""):
+#        toi_exofop.get()
 
 
-if __name__ == "__main__":  # pragma: no cover
+if __name__ == "__main__":  # pragma: no covers
     a = test_exoplanets()
     c = test_composite()
     t = test_tess()
```

### Comparing `exoplanet-atlas-0.3.0/exoatlas/tests/test_models.py` & `exoplanet_atlas-0.3.3/exoatlas/tests/test_models.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from .setup_tests import *
+
 from exoatlas.models import *
 from exoatlas.imports import *
 
 
 def test_seager():
     """
     Test the Seager mass-radius relations.
```

### Comparing `exoplanet-atlas-0.3.0/exoatlas/tests/test_populations.py` & `exoplanet_atlas-0.3.3/exoatlas/tests/test_populations.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,47 @@
+from .setup_tests import *
+
 from exoatlas.imports import *
 from exoatlas.populations import *
 
 
 def test_population():
     """
     Can we make a population from scratch from a table?
     """
 
     fake = Table({x: [0] * 3 for x in attribute_columns}, masked=True)
     p = Population(standard=fake, label="fake")
     p.validate_columns()
-    return p
 
 
 def test_solarsystem():
     """
     Can we make a population of Solar System planets?
     """
     p = SolarSystem()
     p.validate_columns()
-    return p
 
 
 def test_transitingexoplanets():
     """
     Can we make a population of confirmed transiting exoplanets?
     """
     with mock.patch("builtins.input", return_value=""):
         p = TransitingExoplanets()
     p.validate_columns()
-    return p
 
 
 def test_exoplanets():
     """
     Can we make a population of confirmed exoplanets?
     """
     with mock.patch("builtins.input", return_value=""):
         p = Exoplanets()
     p.validate_columns()
-    return p
 
 
 def test_subsets():
     """
     Can we make a population of confirmed Kepler planets?
     """
     with mock.patch("builtins.input", return_value=""):
@@ -58,15 +56,14 @@
 def test_tess():
     """
     Can we make a population of confirmed TESS planets?
     """
     with mock.patch("builtins.input", return_value=""):
         p = TESS()
     p.validate_columns()
-    return p
 
 
 def test_indexing():
     """
     Can we make a population of confirmed transiting exoplanets?
     """
     with mock.patch("builtins.input", return_value=""):
@@ -76,24 +73,23 @@
     a = p[[]]
     b = p[5]
     c = p[0:10]
     with np.errstate(invalid="ignore"):
         d = p[p.stellar_radius < 1.0 * u.Rsun]
     e = p["GJ 1214b"]
     f = p[["GJ 1214b", "LHS 1140b"]]  #'GJ 1132b',
-    g = p[p.discoverer == "Kepler"]
+    g = p[p.discovery_facility == "Kepler"]
     h = p["TRAPPIST-1b"]
     i = p["TRAPPIST-1"]
     j = e + h
     k = f - e
     l = p.create_subset_by_name("GJ1214b")
     m = p.create_subset_by_hostname("GJ1214")
     coordinates = SkyCoord(e.ra, e.dec)
     n = p.create_subset_by_position(coordinates)
-    return a, b, c, d, e, f, g, h, i, j, k, l, m, n
 
 
 def test_table():
     """
     Can we make a custom astropy table out of a Population?
     """
 
@@ -129,12 +125,10 @@
 
     p.emission_signal(wavelength=5 * u.micron)
     p.emission_snr(wavelength=5 * u.micron, telescope_name="JWST")
 
     p.reflection_signal(albedo=0.5)
     p.reflection_snr(albedo=0.5, wavelength=5 * u.micron, telescope_name="JWST")
 
-    return p
-
 
 if __name__ == "__main__":  # pragma: no cover
     outputs = {k.split("_")[-1]: v() for k, v in locals().items() if "test_" in k}
```

### Comparing `exoplanet-atlas-0.3.0/exoatlas/tests/test_snr.py` & `exoplanet_atlas-0.3.3/exoatlas/tests/test_snr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+from .setup_tests import *
+
 from exoatlas import *
 
 
 def test_reflection(telescope_name="JWST", wavelength=1 * u.micron):
     with mock.patch("builtins.input", return_value=""):
         t = TransitingExoplanets()
 
     w = 1 * u.micron
-    fi, ax = plt.subplots(1, 2, figsize=(8, 4))
+    fi, ax = plt.subplots(1, 2, figsize=(8, 4), constrained_layout=True)
     for i, per_transit in enumerate([True, False]):
         BubblePanel(
             xaxis=StellarBrightnessTelescope(
                 wavelength=wavelength, telescope_name=telescope_name
             ),
             yaxis=Reflection(wavelength=w),
             size=ReflectionSNR(
@@ -18,52 +20,49 @@
                 telescope_name=telescope_name,
                 per_transit=per_transit,
             ),
             size_normalization=10,
         ).build(t, ax=ax[i])
         d = {True: "Transit", False: "Hour"}
         plt.title(f"S/N in 1 {d[per_transit]}")
-    plt.tight_layout()
 
 
 def test_emission(telescope_name="JWST", wavelength=5 * u.micron):
     with mock.patch("builtins.input", return_value=""):
         t = TransitingExoplanets()
 
     w = 5 * u.micron
-    fi, ax = plt.subplots(1, 2, figsize=(8, 4))
+    fi, ax = plt.subplots(1, 2, figsize=(8, 4), constrained_layout=True)
     for i, per_transit in enumerate([True, False]):
         BubblePanel(
             xaxis=StellarBrightnessTelescope(
                 wavelength=wavelength, telescope_name=telescope_name
             ),
             yaxis=Emission(wavelength=wavelength),
             size=EmissionSNR(wavelength=wavelength, telescope_name=telescope_name),
             size_normalization=10,
         ).build(t, ax=ax[i])
         d = {True: "Transit", False: "Hour"}
         plt.title(f"S/N in 1 {d[per_transit]}")
-    plt.tight_layout()
 
 
 def test_transmission(telescope_name="JWST", wavelength=5 * u.micron):
     with mock.patch("builtins.input", return_value=""):
         t = TransitingExoplanets()
 
     w = 5 * u.micron
-    fi, ax = plt.subplots(1, 2, figsize=(8, 4))
+    fi, ax = plt.subplots(1, 2, figsize=(8, 4), constrained_layout=True)
     for i, per_transit in enumerate([True, False]):
         BubblePanel(
             xaxis=StellarBrightnessTelescope(
                 wavelength=wavelength, telescope_name=telescope_name
             ),
             yaxis=Transmission(),
             size=TransmissionSNR(wavelength=wavelength, telescope_name=telescope_name),
             size_normalization=10,
         ).build(t, ax=ax[i])
         d = {True: "Transit", False: "Hour"}
         plt.title(f"S/N in 1 {d[per_transit]}")
-    plt.tight_layout()
 
 
 if __name__ == "__main__":
     outputs = {k.split("_")[-1]: v() for k, v in locals().items() if "test_" in k}
```

### Comparing `exoplanet-atlas-0.3.0/exoatlas/tests/test_uncertainties.py` & `exoplanet_atlas-0.3.3/exoatlas/tests/test_uncertainties.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from .setup_tests import *
+
 from exoatlas.imports import *
 from exoatlas.populations import *
 
 
 def test_uncertainties():
     """
     Can we pull out c
@@ -14,12 +16,11 @@
 
     upper, lower = p.uncertainty_lowerupper("radius")
     assert np.all(lower == 0 * u.Rearth)
     assert np.all(upper == 0 * u.Rearth)
 
     bad = p.uncertainty("distance")
     assert np.all(np.isnan(bad))
-    return p
 
 
 if __name__ == "__main__":  # pragma: no cover
     outputs = {k.split("_")[-1]: v() for k, v in locals().items() if "test_" in k}
```

### Comparing `exoplanet-atlas-0.3.0/exoatlas/tests/test_visualizations.py` & `exoplanet_atlas-0.3.3/exoatlas/tests/test_visualizations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+from .setup_tests import *
+
 from exoatlas.imports import *
 
 import exoatlas as ex
 import matplotlib.pyplot as plt
 from exoatlas.visualizations.panels.preset_panels import predefined_panels
 
 
 def test_panels():
     pops = {}
     pops["solarsystem"] = ex.SolarSystem()
     for p in predefined_panels:
+        print(p)
         plt.figure()
         p().build(pops=pops)
         plt.close()
 
 
 def test_panel_types():
     pops = {}
```

### Comparing `exoplanet-atlas-0.3.0/exoatlas/tests/test_whatsup.py` & `exoplanet_atlas-0.3.3/exoatlas/tests/test_whatsup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from .setup_tests import *
+
 from exoatlas.imports import *
 from exoatlas.populations import TransitingExoplanets
 from exoatlas.whatsup import Plan
 
 
 def test_whatsup():
     with mock.patch("builtins.input", return_value=""):
```

### Comparing `exoplanet-atlas-0.3.0/exoatlas/visualizations/MultiPanel.py` & `exoplanet_atlas-0.3.3/exoatlas/visualizations/MultiPanel.py`

 * *Files identical despite different names*

### Comparing `exoplanet-atlas-0.3.0/exoatlas/visualizations/ThumbtackMovie.py` & `exoplanet_atlas-0.3.3/exoatlas/visualizations/ThumbtackMovie.py`

 * *Files identical despite different names*

### Comparing `exoplanet-atlas-0.3.0/exoatlas/visualizations/ThumbtackPlot.py` & `exoplanet_atlas-0.3.3/exoatlas/visualizations/ThumbtackPlot.py`

 * *Files identical despite different names*

### Comparing `exoplanet-atlas-0.3.0/exoatlas/visualizations/axes/plottable.py` & `exoplanet_atlas-0.3.3/exoatlas/visualizations/axes/plottable.py`

 * *Files identical despite different names*

### Comparing `exoplanet-atlas-0.3.0/exoatlas/visualizations/axes/preset_plottables.py` & `exoplanet_atlas-0.3.3/exoatlas/visualizations/axes/preset_plottables.py`

 * *Files 3% similar despite different names*

```diff
@@ -289,14 +289,46 @@
     def value(self):
         """
         What data value to plot?
         """
         return self.panel.pop.stellar_brightness(self.wavelength).to(self.unit)
 
 
+class DepthSNR(StellarBrightnessTelescope):
+    scale = "log"
+    size_normalization = 10
+
+    def __init__(self, **kw):
+        """
+        Initialize S/N for the basic transit depth.
+
+        Parameters
+        ----------
+        wavelength : astropy.units.quantity.Quantity
+            The wavelength at which we want the
+            eclipse depth to be computed.
+        """
+        StellarBrightnessTelescope.__init__(self, **kw)
+        self.kw = kw
+
+    def setup_label(self):
+        """
+        How should this plottable be labled on an axis?
+        """
+        # define the label, based on the wavelength and telescope
+        w = self.wavelength.to(u.micron).value
+        self.label = f"S/N for Transit Depth\nat $\lambda={self.wavelength.to(u.micron).value}\mu m$\n(R={self.R})"
+
+    def value(self):
+        """
+        What data value to plot?
+        """
+        return self.panel.pop.depth_snr(**self.kw)
+
+
 class Transmission(Depth):
     def __init__(self, mu=2.32, threshold=2, **kw):
         """
         Initialize for a particular mean molecular weight.
 
         Parameters
         ----------
@@ -348,36 +380,36 @@
         """
         return self.panel.pop.transmission_snr(
             mu=self.mu, threshold=self.threshold, **self.kw
         )
 
 
 class Reflection(Depth):
-    def __init__(self, albedo=1, **kw):
+    def __init__(self, albedo=0.1, **kw):
         """
         Initialize for a particular albedo.
 
         Parameters
         ----------
         albedo : float
             What fraction of starlight does the planet reflect?
         """
         PlottableAxis.__init__(self, **kw)
         self.albedo = albedo
-        self.label = f"Eclipse Depth\nin Reflected Light\n({albedo:.0%} albedo)"
+        self.label = f"Reflected Light\nEclipse Depth\n({albedo:.0%} albedo)"
 
     def value(self):
         return self.panel.pop.reflection_signal(self.albedo)
 
 
 class ReflectionSNR(StellarBrightnessTelescope):
     scale = "log"
     size_normalization = 10
 
-    def __init__(self, albedo=1, **kw):
+    def __init__(self, albedo=0.1, **kw):
         """
         Initialize for a particular albedo.
 
         Parameters
         ----------
         albedo : float
             What fraction of starlight does the planet reflect?
@@ -388,15 +420,15 @@
 
     def setup_label(self):
         """
         How should this plottable be labled on an axis?
         """
         # define the label, based on the wavelength and telescope
         w = self.wavelength.to(u.micron).value
-        self.label = f"S/N for Eclipse Depth\nin Reflected Light\n({self.albedo:.0%} albedo)\nat $\lambda={w}\mu$m (R={self.R})"
+        self.label = f"S/N for Reflected Light\nEclipse Depth\n({self.albedo:.0%} albedo)\nat $\lambda={w}\mu$m (R={self.R})"
 
     def value(self):
         """
         What data value to plot?
         """
         return self.panel.pop.reflection_snr(albedo=self.albedo, **self.kw)
```

### Comparing `exoplanet-atlas-0.3.0/exoatlas/visualizations/ink_errorbar.py` & `exoplanet_atlas-0.3.3/exoatlas/visualizations/ink_errorbar.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     # calculate Nx4 array of colors
     norm = Normalize(vmin=vmin, vmax=vmax)
     colors = cmap(norm(c))
 
     colors[:, -1] *= alpha
 
     # loop over data points
-    for i in tqdm(i_sorted):
+    for i in i_sorted:  # tqdm()
         # pick this data point's color
         # color = np.array(colors[i]).astype(np.float)
         # assert(len(color) == 4)
 
         # make more transparent, if alpha is <1
         # try:
         #    color[-1] *= alpha[i]
```

### Comparing `exoplanet-atlas-0.3.0/exoatlas/visualizations/panels/BubblePanel.py` & `exoplanet_atlas-0.3.3/exoatlas/visualizations/panels/BubblePanel.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
             default_lim = [None, None]
 
         # if an actual cmap was provided, use it
         if isinstance(cmap, plt.matplotlib.colors.Colormap):
             self.cmap = cmap
         # otherwise, treat the cmap as a string key
         else:
-            self.cmap = plt.matplotlib.cm.get_cmap(cmap)
+            self.cmap = plt.matplotlib.colormaps[cmap]
 
         # make sure the color map limits are set
         self.vmin = vmin or default_lim[0]
         self.vmax = vmax or default_lim[1]
 
         # if a custom normalization is used, reset vmin + vmax
         self.color_normalization = color_normalization
```

### Comparing `exoplanet-atlas-0.3.0/exoatlas/visualizations/panels/ErrorPanel.py` & `exoplanet_atlas-0.3.3/exoatlas/visualizations/panels/ErrorPanel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .Panel import *
+from .BubblePanel import BubblePanel
 from ..ink_errorbar import *
 
 __all__ = ["ErrorPanel"]
 
 
 def remove_unit(x):
     """
@@ -13,15 +14,15 @@
 
     if type(x) == u.quantity.Quantity:
         return x.value
     else:
         return x
 
 
-class ErrorPanel(Panel):
+class ErrorPanel(BubblePanel):
     """
     Error is a general wrapper for making scatter plots
     where planets are represented with 2D error bars, with
     their intensity scaled to some overall visual weight.
     """
 
     @property
@@ -98,14 +99,19 @@
         **kw : dict
             Any extra keywords will be passed on to `errorbar`
         """
 
         # focus attention on that population
         self.point_at(key)
 
+        # do a bubble instead, if requested
+        if getattr(self.pop, "bubble_anyway", False):
+            BubblePanel.plot(self, key=key, ax=ax, labelkw=labelkw, **kw)
+            return
+
         # make sure we're plotting into the appropriate axes
         try:
             plt.sca(self.ax)
         except AttributeError:
             self.setup(ax=ax)
 
         # define the data we're trying to plot
@@ -161,36 +167,36 @@
                 & np.isfinite(yl)
                 & np.isfinite(yu)
                 & np.isfinite(y)
                 & np.isfinite(weights)
             )
 
             n_nouncertainty = sum(ok == False)
-            self.speak(
-                f"skipping {n_nouncertainty} planets that are missing data or uncertainties"
-            )
+            # self.speak(
+            #    f"skipping {n_nouncertainty} planets that are missing data or uncertainties"
+            # )
 
             # kludge to remove those that cross zero
             with np.errstate(invalid="ignore"):
                 ok *= (self.x - xl) > 0
                 ok *= (self.y - yl) > 0
             # FIXME, 5/25/2020: This kludge always useful on
             # logarithmic axes (which are the only that have
             # been defined so far), but at some point we
             # might want to use linear axes too, where we might
             # not want to throw out values that might go
             # negative.
 
             n_consistentwithzero = sum(ok == False) - n_nouncertainty
-            self.speak(
-                f"skipping {n_consistentwithzero} planets that are consistent with zero"
-            )
+            # self.speak(
+            #    f"skipping {n_consistentwithzero} planets that are consistent with zero"
+            # )
 
             if (len(x) > 1) & (self.pop.plotkw.get("ink", True)):
-                self.speak("plotting inked errorbars, this may take a while")
+                # self.speak("plotting inked errorbars, this may take a while")
                 # FIXME, 5/25/2020: We should make the
                 # "invisible" color be something more flexible
                 # than white, in case we're plotting on a dark
                 # background. Remember, things look messy if
                 # we use alpha to do the visual weighting for
                 # these errorbars, because it introduces many
                 # more intersecting lines.
```

### Comparing `exoplanet-atlas-0.3.0/exoatlas/visualizations/panels/Panel.py` & `exoplanet_atlas-0.3.3/exoatlas/visualizations/panels/Panel.py`

 * *Files 2% similar despite different names*

```diff
@@ -346,14 +346,16 @@
         self.ax.set_xlabel(self.xlabel)
         self.ax.set_ylabel(self.ylabel)
 
         # if requested, label the individual planets in the plot
         # for p in self.pops:
         #    self.point_at(p)
         if self.pop.label_planets:
+            if getattr(self.pop, "zorder", None) is not None:
+                labelkw["zorder"] = self.pop.zorder
             self.label_planets(**labelkw)
 
     def remove_xlabel(self):
         """
         Remove the xlabel and xticklabels from this panel.
         """
         plt.setp(self.ax.get_xticklabels(), visible=False)
```

### Comparing `exoplanet-atlas-0.3.0/exoatlas/visualizations/panels/preset_panels.py` & `exoplanet_atlas-0.3.3/exoatlas/visualizations/panels/preset_panels.py`

 * *Files 1% similar despite different names*

```diff
@@ -318,15 +318,15 @@
 
 # class FluxEscape(ErrorPanel):
 class FluxEscape(BubblePanel):
     xaxis = Flux
     yaxis = EscapeVelocity
 
     def plot_constant_lambda(
-        self, alpha=0.5, color="gray", nudge=1, rotation=-4.5, **kw
+        self, alpha=0.5, color="gray", x=0.01, y=100, rotation=-4.5, **kw
     ):
         """
         Plot the escape velocity vs insolation for
         different constant values of the escape parameter.
 
         This assumes the exosphere is at the planet's equilibrium
         temperature, which is is *terrible* approximation. This
@@ -338,16 +338,16 @@
         ----------
         **kw : dict
             Keyword parameters get passed along to plot.
         """
 
         # label one of the lines
         plt.text(
-            0.005,
-            145 * nudge,
+            x,
+            y,
             r"$E_{grav}/E_{thermal}$",
             rotation=rotation,
             fontsize=8,
             color=color,
         )
 
         teq = np.logspace(1, 4) * u.K
```

### Comparing `exoplanet-atlas-0.3.0/exoatlas/visualizations/tweaks.py` & `exoplanet_atlas-0.3.3/exoatlas/visualizations/tweaks.py`

 * *Files identical despite different names*

### Comparing `exoplanet-atlas-0.3.0/exoatlas/whatsup/block.py` & `exoplanet_atlas-0.3.3/exoatlas/whatsup/block.py`

 * *Files identical despite different names*

### Comparing `exoplanet-atlas-0.3.0/exoatlas/whatsup/observatory.py` & `exoplanet_atlas-0.3.3/exoatlas/whatsup/observatory.py`

 * *Files identical despite different names*

### Comparing `exoplanet-atlas-0.3.0/exoatlas/whatsup/plan.py` & `exoplanet_atlas-0.3.3/exoatlas/whatsup/plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         """identify all the transits for all the planets"""
 
         now = midnight
         pop = self.population
 
         # pull out the period and epoch of all the planets
         P = pop.period.to("day")
-        T0 = pop.transit_epoch.to("day")
+        T0 = pop.transit_midpoint.to("day")
         coords = SkyCoord(ra=pop.ra, dec=pop.dec)
 
         # find the closest exact transit epochs
         pop.standard["closest_epoch_number"] = np.round((now - T0) / P)
         pop.standard["closest_epoch_day"] = pop.closest_epoch_number * P + T0
 
         # ask which planets have transits happening tonight/today
@@ -232,15 +232,17 @@
         """
 
         self.speak("plotting transits")
         self.find_transits()
         plt.ioff()
 
         # set up the plotting window (one night at a time)
-        self.figure = plt.figure("upcoming transits", figsize=(15, 6), dpi=200)
+        self.figure = plt.figure(
+            "upcoming transits", figsize=(15, 6), dpi=200, constrained_layout=True
+        )
         self.gs = plt.matplotlib.gridspec.GridSpec(
             2, 1, hspace=0, wspace=0, height_ratios=[0.3, 1.0], bottom=0.35
         )
         self.ax = {}
 
         # an ax to include the names of the planets
         self.ax["transits"] = plt.subplot(self.gs[0])
@@ -270,15 +272,14 @@
             self.observatory.plotSun(jd=self.block.times, ax=self.ax[k])
 
         # set the formatting on the time label
         fmt = plt.matplotlib.dates.DateFormatter("%Y-%m-%d\n%H:%M UT")
         self.ax["airmass"].xaxis.set_major_formatter(fmt)
         f = plt.gcf()
         f.autofmt_xdate(rotation=90)
-        plt.tight_layout()
 
         self.speak("making a movie of transits")
 
         # initialize the animator
         metadata = dict(
             title="Observability from {0}".format(self.observatory.name),
             artist="whatsup",
```

### Comparing `exoplanet-atlas-0.3.0/exoatlas/whatsup/transit.py` & `exoplanet_atlas-0.3.3/exoatlas/whatsup/transit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """define a Transit class, to represent an individual planetary transit"""
+
 from ..imports import *
 
 
 class Transit(Talker):
     """a Transit object is one transit of one (associated) planet"""
 
     def __init__(
@@ -23,15 +24,15 @@
         self.planet = planet
         self.planet._pithy = True
         self.coord = SkyCoord(self.planet.ra, self.planet.dec)
         self.observatory = observatory
 
         # set the midtransit time of this particular transit
         self.midtransit = (
-            planet.period * (i + phasefrommidtransit) + planet.transit_epoch
+            planet.period * (i + phasefrommidtransit) + planet.transit_midpoint
         )[0]
         self.i = i
 
         # how much padding should be on the other side of the transit
         self.buffer = buffer
 
     @property
```

### Comparing `exoplanet-atlas-0.3.0/setup.py` & `exoplanet_atlas-0.3.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -80,21 +80,38 @@
     ],
     # what other packages are required. these must be pip-installable
     install_requires=[
         "numpy>=1.13",
         "matplotlib>=2.0",
         "astropy>=3.2.3",
         "astroquery>=0.3.9",
+        "astroplan>=0.10",
         "rainbow-connection>=0.0.1",
         "PyYAML",
         "tqdm",
         "pytz",
     ],
+    extras_require={
+        "develop": [
+            "pytest",
+            "black",
+            "black[jupyter]",
+            "jupyter",
+            "ipython",
+            "mkdocs",
+            "mkdocs-material",
+            "mkdocstrings",
+            "mkdocstrings-python",
+            "pytkdocs[numpy-style]",
+            "mkdocs-jupyter",
+            "mkdocs-exclude",
+            "twine",
+            "pre-commit",
+        ]
+    },
     # what version of Python is required?
-    python_requires=">=3.6",
-    # packages in `key` will be installed with `pip install pkg-name[key]`
-    extras_require={},
+    python_requires=">=3.8",
     # (I think just leave this set to False)
     zip_safe=False,
     # under what license is this code released?
     license="MIT",
 )
```

