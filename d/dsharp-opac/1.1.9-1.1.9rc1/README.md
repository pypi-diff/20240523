# Comparing `tmp/dsharp_opac-1.1.9.tar.gz` & `tmp/dsharp_opac-1.1.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsharp_opac-1.1.9.tar", last modified: Thu May 23 06:46:40 2024, max compression
+gzip compressed data, was "dsharp_opac-1.1.9rc1.tar", last modified: Thu May 23 06:45:38 2024, max compression
```

## Comparing `dsharp_opac-1.1.9.tar` & `dsharp_opac-1.1.9rc1.tar`

### file list

```diff
@@ -1,109 +1,109 @@
--rw-r--r--   0        0        0      191 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/.gitignore
--rw-r--r--   0        0        0    35140 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/LICENSE
--rw-r--r--   0        0        0      224 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/MANIFEST.in
--rw-r--r--   0        0        0     2190 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/README.md
--rw-r--r--   0        0        0        8 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/apt.txt
--rw-r--r--   0        0        0     2190 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/__init__.py
--rw-r--r--   0        0        0    11792 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/bhmie_fortran.f90
--rw-r--r--   0        0        0     6931 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/bhmie_python.py
--rw-r--r--   0        0        0      414 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/calldraine.f90
--rw-r--r--   0        0        0     2184 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/data/Kataoka2014-Fig2b-1e-5cm.csv
--rw-r--r--   0        0        0     2093 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/data/Kataoka2014-Fig2d-1e-5cm.csv
--rw-r--r--   0        0        0     1301 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/data/andrews2009.dat
--rw-r--r--   0        0        0   803630 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/data/default_opacities.npz
--rw-r--r--   0        0        0   803274 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/data/default_opacities_extrapol.npz
--rw-r--r--   0        0        0   853812 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/data/default_opacities_smooth.npz
--rw-r--r--   0        0        0   803316 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/data/icefree_opacities.npz
--rw-r--r--   0        0        0   853427 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/data/icefree_opacities_smooth.npz
--rw-r--r--   0        0        0     2260 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/data/kappa_D01_T100K_p3.5_amax1mm.csv
--rw-r--r--   0        0        0    15708 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/data/kataoka_mix.lnk
--rw-r--r--   0        0        0      444 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/data/meson.build
--rw-r--r--   0        0        0  2143594 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/data/ricci_compact.npz
--rwxr-xr-x   0        0        0    99640 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/dsharp_opac.py
--rw-r--r--   0        0        0    25142 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/fit_module.f90
--rw-r--r--   0        0        0     1182 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/meson.build
--rw-r--r--   0        0        0      144 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/draine/.gitignore
--rw-r--r--   0        0        0      827 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/draine/links.json
--rw-r--r--   0        0        0      130 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/draine/meson.build
--rw-r--r--   0        0        0        6 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/henning/.gitignore
--rw-r--r--   0        0        0       27 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/henning/meson.build
--rw-r--r--   0        0        0     1058 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/henning/new/links.json
--rw-r--r--   0        0        0      135 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/henning/new/meson.build
--rw-r--r--   0        0        0      599 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/henning/old/links.json
--rw-r--r--   0        0        0      135 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/henning/old/meson.build
--rw-r--r--   0        0        0       45 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/jaeger/.gitignore
--rw-r--r--   0        0        0      425 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/jaeger/links.json
--rw-r--r--   0        0        0      130 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/jaeger/meson.build
--rw-r--r--   0        0        0    75634 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/luca/H2Oice_Warren.dat
--rw-r--r--   0        0        0   132169 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/luca/aC_ACH2_Zubko.dat
--rw-r--r--   0        0        0      180 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/luca/meson.build
--rw-r--r--   0        0        0   132175 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/luca/silicate.dat
--rw-r--r--   0        0        0      199 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/meson.build
--rw-r--r--   0        0        0      580 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-iron-k.csv
--rw-r--r--   0        0        0      568 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-iron-n.csv
--rw-r--r--   0        0        0     7500 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-iron.lnk
--rw-r--r--   0        0        0     1331 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-olivine-k.csv
--rw-r--r--   0        0        0     1078 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-olivine-n.csv
--rw-r--r--   0        0        0     7500 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-olivine.lnk
--rw-r--r--   0        0        0     1656 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-organics-k.csv
--rw-r--r--   0        0        0     1168 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-organics-n.csv
--rw-r--r--   0        0        0     7500 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-organics.lnk
--rw-r--r--   0        0        0     1705 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene-k.csv
--rw-r--r--   0        0        0     1060 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene-n.csv
--rw-r--r--   0        0        0     7500 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene.lnk
--rw-r--r--   0        0        0      666 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-troilite-k.csv
--rw-r--r--   0        0        0      505 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-troilite-n.csv
--rw-r--r--   0        0        0     7500 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-troilite.lnk
--rw-r--r--   0        0        0     2009 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-waterice-k.csv
--rw-r--r--   0        0        0     1425 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-waterice-n.csv
--rw-r--r--   0        0        0     7500 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-waterice.lnk
--rw-r--r--   0        0        0      887 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/make_lnk.py
--rw-r--r--   0        0        0      593 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/meson.build
--rw-r--r--   0        0        0       23 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/preibisch/.gitignore
--rw-r--r--   0        0        0      215 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/preibisch/links.json
--rw-r--r--   0        0        0      133 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/preibisch/meson.build
--rw-r--r--   0        0        0       15 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/segelstein_water/.gitignore
--rw-r--r--   0        0        0      137 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/segelstein_water/links.json
--rw-r--r--   0        0        0      140 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/segelstein_water/meson.build
--rw-r--r--   0        0        0      882 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/testfiles_ricci/beta.dat
--rw-r--r--   0        0        0  2351704 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/testfiles_ricci/d_test_vacuum30.dust
--rw-r--r--   0        0        0    10382 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/testfiles_ricci/dust_opacities.16
--rw-r--r--   0        0        0      509 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/testfiles_ricci/kappa.dat
--rw-r--r--   0        0        0      208 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/testfiles_ricci/meson.build
--rw-r--r--   0        0        0       24 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/warren/.gitignore
--rw-r--r--   0        0        0      122 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/warren/links.json
--rw-r--r--   0        0        0      186 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/warren/meson.build
--rw-r--r--   0        0        0    13224 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/warren/warren_1984.txt
--rw-r--r--   0        0        0     4525 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/warren/warren_1984_all_temps.txt
--rw-r--r--   0        0        0      276 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/zubko+1996/meson.build
--rw-r--r--   0        0        0     1052 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/zubko+1996/zubko_E_ACH2.txt
--rw-r--r--   0        0        0     1097 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/zubko+1996/zubko_E_BE.txt
--rw-r--r--   0        0        0      812 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/zubko+1996/zubko_k_ACH2.txt
--rw-r--r--   0        0        0      731 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/zubko+1996/zubko_k_BE.txt
--rw-r--r--   0        0        0      818 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/zubko+1996/zubko_n_ACH2.txt
--rw-r--r--   0        0        0      750 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/zubko+1996/zubko_n_BE.txt
--rw-r--r--   0        0        0   915276 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/dsharp_opac/optical_constants/zubko+1996/zubko_ocr.pdf
--rw-r--r--   0        0        0      539 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/meson.build
--rw-r--r--   0        0        0    18210 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/notebooks/AppendixB.ipynb
--rw-r--r--   0        0        0     4632 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/notebooks/Figure1.ipynb
--rw-r--r--   0        0        0     1719 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/notebooks/Figure2.ipynb
--rw-r--r--   0        0        0     2339 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/notebooks/Figure3.ipynb
--rw-r--r--   0        0        0     3963 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/notebooks/Figure4.ipynb
--rw-r--r--   0        0        0     6886 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/notebooks/Figure56.ipynb
--rw-r--r--   0        0        0     4105 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/notebooks/Figure7.ipynb
--rw-r--r--   0        0        0    11407 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/notebooks/Figure8.ipynb
--rw-r--r--   0        0        0     3854 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/notebooks/Figure9.ipynb
--rw-r--r--   0        0        0     5933 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/notebooks/aux_functions.py
--rw-r--r--   0        0        0     5917 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/notebooks/dsharp_porosity.ipynb
--rw-r--r--   0        0        0      394 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/notebooks/header.py
--rw-r--r--   0        0        0     1514 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/notebooks/index.ipynb
--rw-r--r--   0        0        0    12688 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/notebooks/opac_widget.py
--rw-r--r--   0        0        0  1816292 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/notebooks/opacity_examples.ipynb
--rw-r--r--   0        0        0   609690 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/notebooks/opacity_package_tests.ipynb
--rw-r--r--   0        0        0    50797 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/notebooks/polarization_fraction.ipynb
--rw-r--r--   0        0        0     8660 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/notebooks/porosity.ipynb
--rw-r--r--   0        0        0     6503 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/notebooks/scattering_phase_functions.ipynb
--rw-r--r--   0        0        0    16618 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/notebooks/smoothed_opacities.ipynb
--rw-r--r--   0        0        0      525 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/pyproject.toml
--rw-r--r--   0        0        0       62 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9/requirements.txt
--rw-r--r--   0        0        0    43126 2024-05-23 06:46:41.344102 dsharp_opac-1.1.9/PKG-INFO
+-rw-r--r--   0        0        0      191 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/.gitignore
+-rw-r--r--   0        0        0    35140 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/LICENSE
+-rw-r--r--   0        0        0      224 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/MANIFEST.in
+-rw-r--r--   0        0        0     2190 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/README.md
+-rw-r--r--   0        0        0        8 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/apt.txt
+-rw-r--r--   0        0        0     2190 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/__init__.py
+-rw-r--r--   0        0        0    11792 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/bhmie_fortran.f90
+-rw-r--r--   0        0        0     6931 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/bhmie_python.py
+-rw-r--r--   0        0        0      414 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/calldraine.f90
+-rw-r--r--   0        0        0     2184 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/data/Kataoka2014-Fig2b-1e-5cm.csv
+-rw-r--r--   0        0        0     2093 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/data/Kataoka2014-Fig2d-1e-5cm.csv
+-rw-r--r--   0        0        0     1301 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/data/andrews2009.dat
+-rw-r--r--   0        0        0   803630 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/data/default_opacities.npz
+-rw-r--r--   0        0        0   803274 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/data/default_opacities_extrapol.npz
+-rw-r--r--   0        0        0   853812 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/data/default_opacities_smooth.npz
+-rw-r--r--   0        0        0   803316 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/data/icefree_opacities.npz
+-rw-r--r--   0        0        0   853427 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/data/icefree_opacities_smooth.npz
+-rw-r--r--   0        0        0     2260 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/data/kappa_D01_T100K_p3.5_amax1mm.csv
+-rw-r--r--   0        0        0    15708 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/data/kataoka_mix.lnk
+-rw-r--r--   0        0        0      444 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/data/meson.build
+-rw-r--r--   0        0        0  2143594 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/data/ricci_compact.npz
+-rwxr-xr-x   0        0        0    99640 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/dsharp_opac.py
+-rw-r--r--   0        0        0    25142 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/fit_module.f90
+-rw-r--r--   0        0        0     1182 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/meson.build
+-rw-r--r--   0        0        0      144 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/draine/.gitignore
+-rw-r--r--   0        0        0      827 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/draine/links.json
+-rw-r--r--   0        0        0      130 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/draine/meson.build
+-rw-r--r--   0        0        0        6 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/henning/.gitignore
+-rw-r--r--   0        0        0       27 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/henning/meson.build
+-rw-r--r--   0        0        0     1058 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/henning/new/links.json
+-rw-r--r--   0        0        0      135 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/henning/new/meson.build
+-rw-r--r--   0        0        0      599 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/henning/old/links.json
+-rw-r--r--   0        0        0      135 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/henning/old/meson.build
+-rw-r--r--   0        0        0       45 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/jaeger/.gitignore
+-rw-r--r--   0        0        0      425 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/jaeger/links.json
+-rw-r--r--   0        0        0      130 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/jaeger/meson.build
+-rw-r--r--   0        0        0    75634 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/luca/H2Oice_Warren.dat
+-rw-r--r--   0        0        0   132169 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/luca/aC_ACH2_Zubko.dat
+-rw-r--r--   0        0        0      180 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/luca/meson.build
+-rw-r--r--   0        0        0   132175 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/luca/silicate.dat
+-rw-r--r--   0        0        0      199 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/meson.build
+-rw-r--r--   0        0        0      580 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-iron-k.csv
+-rw-r--r--   0        0        0      568 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-iron-n.csv
+-rw-r--r--   0        0        0     7500 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-iron.lnk
+-rw-r--r--   0        0        0     1331 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-olivine-k.csv
+-rw-r--r--   0        0        0     1078 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-olivine-n.csv
+-rw-r--r--   0        0        0     7500 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-olivine.lnk
+-rw-r--r--   0        0        0     1656 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-organics-k.csv
+-rw-r--r--   0        0        0     1168 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-organics-n.csv
+-rw-r--r--   0        0        0     7500 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-organics.lnk
+-rw-r--r--   0        0        0     1705 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene-k.csv
+-rw-r--r--   0        0        0     1060 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene-n.csv
+-rw-r--r--   0        0        0     7500 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene.lnk
+-rw-r--r--   0        0        0      666 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-troilite-k.csv
+-rw-r--r--   0        0        0      505 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-troilite-n.csv
+-rw-r--r--   0        0        0     7500 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-troilite.lnk
+-rw-r--r--   0        0        0     2009 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-waterice-k.csv
+-rw-r--r--   0        0        0     1425 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-waterice-n.csv
+-rw-r--r--   0        0        0     7500 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-waterice.lnk
+-rw-r--r--   0        0        0      887 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/make_lnk.py
+-rw-r--r--   0        0        0      593 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/meson.build
+-rw-r--r--   0        0        0       23 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/preibisch/.gitignore
+-rw-r--r--   0        0        0      215 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/preibisch/links.json
+-rw-r--r--   0        0        0      133 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/preibisch/meson.build
+-rw-r--r--   0        0        0       15 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/segelstein_water/.gitignore
+-rw-r--r--   0        0        0      137 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/segelstein_water/links.json
+-rw-r--r--   0        0        0      140 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/segelstein_water/meson.build
+-rw-r--r--   0        0        0      882 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/testfiles_ricci/beta.dat
+-rw-r--r--   0        0        0  2351704 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/testfiles_ricci/d_test_vacuum30.dust
+-rw-r--r--   0        0        0    10382 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/testfiles_ricci/dust_opacities.16
+-rw-r--r--   0        0        0      509 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/testfiles_ricci/kappa.dat
+-rw-r--r--   0        0        0      208 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/testfiles_ricci/meson.build
+-rw-r--r--   0        0        0       24 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/warren/.gitignore
+-rw-r--r--   0        0        0      122 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/warren/links.json
+-rw-r--r--   0        0        0      186 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/warren/meson.build
+-rw-r--r--   0        0        0    13224 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/warren/warren_1984.txt
+-rw-r--r--   0        0        0     4525 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/warren/warren_1984_all_temps.txt
+-rw-r--r--   0        0        0      276 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/zubko+1996/meson.build
+-rw-r--r--   0        0        0     1052 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/zubko+1996/zubko_E_ACH2.txt
+-rw-r--r--   0        0        0     1097 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/zubko+1996/zubko_E_BE.txt
+-rw-r--r--   0        0        0      812 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/zubko+1996/zubko_k_ACH2.txt
+-rw-r--r--   0        0        0      731 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/zubko+1996/zubko_k_BE.txt
+-rw-r--r--   0        0        0      818 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/zubko+1996/zubko_n_ACH2.txt
+-rw-r--r--   0        0        0      750 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/zubko+1996/zubko_n_BE.txt
+-rw-r--r--   0        0        0   915276 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/zubko+1996/zubko_ocr.pdf
+-rw-r--r--   0        0        0      539 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/meson.build
+-rw-r--r--   0        0        0    18210 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/notebooks/AppendixB.ipynb
+-rw-r--r--   0        0        0     4632 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/notebooks/Figure1.ipynb
+-rw-r--r--   0        0        0     1719 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/notebooks/Figure2.ipynb
+-rw-r--r--   0        0        0     2339 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/notebooks/Figure3.ipynb
+-rw-r--r--   0        0        0     3963 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/notebooks/Figure4.ipynb
+-rw-r--r--   0        0        0     6886 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/notebooks/Figure56.ipynb
+-rw-r--r--   0        0        0     4105 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/notebooks/Figure7.ipynb
+-rw-r--r--   0        0        0    11407 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/notebooks/Figure8.ipynb
+-rw-r--r--   0        0        0     3854 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/notebooks/Figure9.ipynb
+-rw-r--r--   0        0        0     5933 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/notebooks/aux_functions.py
+-rw-r--r--   0        0        0     5917 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/notebooks/dsharp_porosity.ipynb
+-rw-r--r--   0        0        0      394 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/notebooks/header.py
+-rw-r--r--   0        0        0     1514 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/notebooks/index.ipynb
+-rw-r--r--   0        0        0    12688 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/notebooks/opac_widget.py
+-rw-r--r--   0        0        0  1816292 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/notebooks/opacity_examples.ipynb
+-rw-r--r--   0        0        0   609690 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/notebooks/opacity_package_tests.ipynb
+-rw-r--r--   0        0        0    50797 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/notebooks/polarization_fraction.ipynb
+-rw-r--r--   0        0        0     8660 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/notebooks/porosity.ipynb
+-rw-r--r--   0        0        0     6503 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/notebooks/scattering_phase_functions.ipynb
+-rw-r--r--   0        0        0    16618 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/notebooks/smoothed_opacities.ipynb
+-rw-r--r--   0        0        0      528 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/pyproject.toml
+-rw-r--r--   0        0        0       62 2024-05-23 06:44:02.000000 dsharp_opac-1.1.9rc1/requirements.txt
+-rw-r--r--   0        0        0    43129 2024-05-23 06:45:39.161219 dsharp_opac-1.1.9rc1/PKG-INFO
```

### Comparing `dsharp_opac-1.1.9/LICENSE` & `dsharp_opac-1.1.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/README.md` & `dsharp_opac-1.1.9rc1/README.md`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/__init__.py` & `dsharp_opac-1.1.9rc1/dsharp_opac/__init__.py`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/bhmie_fortran.f90` & `dsharp_opac-1.1.9rc1/dsharp_opac/bhmie_fortran.f90`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/bhmie_python.py` & `dsharp_opac-1.1.9rc1/dsharp_opac/bhmie_python.py`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/data/Kataoka2014-Fig2b-1e-5cm.csv` & `dsharp_opac-1.1.9rc1/dsharp_opac/data/Kataoka2014-Fig2b-1e-5cm.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/data/Kataoka2014-Fig2d-1e-5cm.csv` & `dsharp_opac-1.1.9rc1/dsharp_opac/data/Kataoka2014-Fig2d-1e-5cm.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/data/andrews2009.dat` & `dsharp_opac-1.1.9rc1/dsharp_opac/data/andrews2009.dat`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/data/default_opacities.npz` & `dsharp_opac-1.1.9rc1/dsharp_opac/data/default_opacities.npz`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/data/default_opacities_extrapol.npz` & `dsharp_opac-1.1.9rc1/dsharp_opac/data/default_opacities_extrapol.npz`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/data/default_opacities_smooth.npz` & `dsharp_opac-1.1.9rc1/dsharp_opac/data/default_opacities_smooth.npz`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/data/icefree_opacities.npz` & `dsharp_opac-1.1.9rc1/dsharp_opac/data/icefree_opacities.npz`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/data/icefree_opacities_smooth.npz` & `dsharp_opac-1.1.9rc1/dsharp_opac/data/icefree_opacities_smooth.npz`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/data/kappa_D01_T100K_p3.5_amax1mm.csv` & `dsharp_opac-1.1.9rc1/dsharp_opac/data/kappa_D01_T100K_p3.5_amax1mm.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/data/kataoka_mix.lnk` & `dsharp_opac-1.1.9rc1/dsharp_opac/data/kataoka_mix.lnk`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/data/ricci_compact.npz` & `dsharp_opac-1.1.9rc1/dsharp_opac/data/ricci_compact.npz`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/dsharp_opac.py` & `dsharp_opac-1.1.9rc1/dsharp_opac/dsharp_opac.py`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/fit_module.f90` & `dsharp_opac-1.1.9rc1/dsharp_opac/fit_module.f90`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/meson.build` & `dsharp_opac-1.1.9rc1/dsharp_opac/meson.build`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/draine/links.json` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/draine/links.json`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/henning/new/links.json` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/henning/new/links.json`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/henning/old/links.json` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/henning/old/links.json`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/luca/H2Oice_Warren.dat` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/luca/H2Oice_Warren.dat`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/luca/aC_ACH2_Zubko.dat` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/luca/aC_ACH2_Zubko.dat`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/luca/silicate.dat` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/luca/silicate.dat`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-iron-k.csv` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-iron-k.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-iron-n.csv` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-iron-n.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-iron.lnk` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-iron.lnk`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-olivine-k.csv` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-olivine-k.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-olivine-n.csv` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-olivine-n.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-olivine.lnk` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-olivine.lnk`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-organics-k.csv` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-organics-k.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-organics-n.csv` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-organics-n.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-organics.lnk` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-organics.lnk`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene-k.csv` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene-k.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene-n.csv` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene-n.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene.lnk` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-orthopyroxene.lnk`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-troilite-k.csv` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-troilite-k.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-troilite.lnk` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-troilite.lnk`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-waterice-k.csv` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-waterice-k.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-waterice-n.csv` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-waterice-n.csv`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/P94-waterice.lnk` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/P94-waterice.lnk`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/make_lnk.py` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/make_lnk.py`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/pollack1994/meson.build` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/pollack1994/meson.build`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/testfiles_ricci/beta.dat` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/testfiles_ricci/beta.dat`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/testfiles_ricci/d_test_vacuum30.dust` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/testfiles_ricci/d_test_vacuum30.dust`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/testfiles_ricci/dust_opacities.16` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/testfiles_ricci/dust_opacities.16`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/warren/warren_1984.txt` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/warren/warren_1984.txt`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/warren/warren_1984_all_temps.txt` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/warren/warren_1984_all_temps.txt`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/zubko+1996/zubko_E_ACH2.txt` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/zubko+1996/zubko_E_ACH2.txt`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/zubko+1996/zubko_E_BE.txt` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/zubko+1996/zubko_E_BE.txt`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/zubko+1996/zubko_k_ACH2.txt` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/zubko+1996/zubko_k_ACH2.txt`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/zubko+1996/zubko_k_BE.txt` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/zubko+1996/zubko_k_BE.txt`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/zubko+1996/zubko_n_ACH2.txt` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/zubko+1996/zubko_n_ACH2.txt`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/zubko+1996/zubko_n_BE.txt` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/zubko+1996/zubko_n_BE.txt`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/dsharp_opac/optical_constants/zubko+1996/zubko_ocr.pdf` & `dsharp_opac-1.1.9rc1/dsharp_opac/optical_constants/zubko+1996/zubko_ocr.pdf`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/meson.build` & `dsharp_opac-1.1.9rc1/meson.build`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/notebooks/AppendixB.ipynb` & `dsharp_opac-1.1.9rc1/notebooks/AppendixB.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/notebooks/Figure1.ipynb` & `dsharp_opac-1.1.9rc1/notebooks/Figure1.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/notebooks/Figure2.ipynb` & `dsharp_opac-1.1.9rc1/notebooks/Figure2.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/notebooks/Figure3.ipynb` & `dsharp_opac-1.1.9rc1/notebooks/Figure3.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/notebooks/Figure4.ipynb` & `dsharp_opac-1.1.9rc1/notebooks/Figure4.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/notebooks/Figure56.ipynb` & `dsharp_opac-1.1.9rc1/notebooks/Figure56.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/notebooks/Figure7.ipynb` & `dsharp_opac-1.1.9rc1/notebooks/Figure7.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/notebooks/Figure8.ipynb` & `dsharp_opac-1.1.9rc1/notebooks/Figure8.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/notebooks/Figure9.ipynb` & `dsharp_opac-1.1.9rc1/notebooks/Figure9.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/notebooks/aux_functions.py` & `dsharp_opac-1.1.9rc1/notebooks/aux_functions.py`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/notebooks/dsharp_porosity.ipynb` & `dsharp_opac-1.1.9rc1/notebooks/dsharp_porosity.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/notebooks/index.ipynb` & `dsharp_opac-1.1.9rc1/notebooks/index.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/notebooks/opac_widget.py` & `dsharp_opac-1.1.9rc1/notebooks/opac_widget.py`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/notebooks/opacity_examples.ipynb` & `dsharp_opac-1.1.9rc1/notebooks/opacity_examples.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/notebooks/opacity_package_tests.ipynb` & `dsharp_opac-1.1.9rc1/notebooks/opacity_package_tests.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/notebooks/polarization_fraction.ipynb` & `dsharp_opac-1.1.9rc1/notebooks/polarization_fraction.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/notebooks/porosity.ipynb` & `dsharp_opac-1.1.9rc1/notebooks/porosity.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/notebooks/scattering_phase_functions.ipynb` & `dsharp_opac-1.1.9rc1/notebooks/scattering_phase_functions.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/notebooks/smoothed_opacities.ipynb` & `dsharp_opac-1.1.9rc1/notebooks/smoothed_opacities.ipynb`

 * *Files identical despite different names*

### Comparing `dsharp_opac-1.1.9/pyproject.toml` & `dsharp_opac-1.1.9rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = 'mesonpy'
 requires = ['meson-python', 'numpy']
 
 [project]
 name = 'dsharp_opac'
-version = '1.1.9'
+version = '1.1.9rc1'
 description = 'python routines to calculate mie opacities'
 readme = { file = 'README.md', content-type = 'text/markdown' }
 authors = [
     { name = "Til Birnstiel & DSHARP collaboration", email = "til.birnstiel@lmu.de" },
 ]
 license = { file = 'LICENSE' }
 dependencies = ['numpy', 'scipy', 'matplotlib', 'astropy', 'mpmath']
```

### Comparing `dsharp_opac-1.1.9/PKG-INFO` & `dsharp_opac-1.1.9rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsharp_opac
-Version: 1.1.9
+Version: 1.1.9rc1
 Summary: python routines to calculate mie opacities
 Author-Email: Til Birnstiel & DSHARP collaboration <til.birnstiel@lmu.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

