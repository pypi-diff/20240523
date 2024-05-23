# Comparing `tmp/flopy-3.6.0.tar.gz` & `tmp/flopy-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flopy-3.6.0.tar", last modified: Thu Feb  8 04:31:11 2024, max compression
+gzip compressed data, was "flopy-3.7.0.tar", last modified: Thu May 23 21:09:22 2024, max compression
```

## Comparing `flopy-3.6.0.tar` & `flopy-3.7.0.tar`

### file list

```diff
@@ -1,373 +1,438 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:31:11.038928 flopy-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-02-08 04:30:02.000000 flopy-3.6.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-02-08 04:30:02.000000 flopy-3.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-08 04:30:02.000000 flopy-3.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-02-08 04:31:11.038928 flopy-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10104 2024-02-08 04:30:02.000000 flopy-3.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:31:10.958927 flopy-3.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-02-08 04:30:02.000000 flopy-3.6.0/docs/PyPI_release.md
--rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-02-08 04:30:02.000000 flopy-3.6.0/docs/make_release.md
--rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-02-08 04:30:02.000000 flopy-3.6.0/docs/mf6_dev_guide.md
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-02-08 04:30:02.000000 flopy-3.6.0/docs/script_examples.md
--rw-r--r--   0 runner    (1001) docker     (127)    18405 2024-02-08 04:30:02.000000 flopy-3.6.0/docs/supported_packages.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:31:10.958927 flopy-3.6.0/flopy/
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/datbase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:31:10.962927 flopy-3.6.0/flopy/discretization/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/discretization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41458 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/discretization/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/discretization/modeltime.py
--rw-r--r--   0 runner    (1001) docker     (127)    64103 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/discretization/structuredgrid.py
--rw-r--r--   0 runner    (1001) docker     (127)    34168 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/discretization/unstructuredgrid.py
--rw-r--r--   0 runner    (1001) docker     (127)    19405 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/discretization/vertexgrid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:31:10.962927 flopy-3.6.0/flopy/export/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/export/longnames.py
--rw-r--r--   0 runner    (1001) docker     (127)     9625 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/export/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    49757 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/export/netcdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    24034 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/export/shapefile_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/export/unitsformat.py
--rw-r--r--   0 runner    (1001) docker     (127)    68462 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/export/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    50445 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/export/vtk.py
--rw-r--r--   0 runner    (1001) docker     (127)    60731 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mbase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:31:10.966927 flopy-3.6.0/flopy/mf6/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:31:10.966927 flopy-3.6.0/flopy/mf6/coordinates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/coordinates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32527 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/coordinates/modeldimensions.py
--rw-r--r--   0 runner    (1001) docker     (127)    26169 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/coordinates/modelgrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/coordinates/simulationtime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:31:10.970927 flopy-3.6.0/flopy/mf6/data/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:31:10.982927 flopy-3.6.0/flopy/mf6/data/dfn/
--rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/common.dfn
--rw-r--r--   0 runner    (1001) docker     (127)    11775 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/exg-gwfgwf.dfn
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/exg-gwfgwt.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     9440 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/exg-gwtgwt.dfn
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/flopy.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwf-api.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwf-buy.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwf-chd.dfn
--rw-r--r--   0 runner    (1001) docker     (127)    22008 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwf-csub.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwf-dis.dfn
--rw-r--r--   0 runner    (1001) docker     (127)    11472 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwf-disu.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwf-disv.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwf-drn.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwf-evt.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwf-evta.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwf-ghb.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwf-gnc.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwf-hfb.dfn
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwf-ic.dfn
--rw-r--r--   0 runner    (1001) docker     (127)    29248 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwf-lak.dfn
--rw-r--r--   0 runner    (1001) docker     (127)    27133 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwf-maw.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwf-mvr.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwf-nam.dfn
--rw-r--r--   0 runner    (1001) docker     (127)    17672 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwf-npf.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwf-oc.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwf-rch.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwf-rcha.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwf-riv.dfn
--rw-r--r--   0 runner    (1001) docker     (127)    30168 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwf-sfr.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwf-sto.dfn
--rw-r--r--   0 runner    (1001) docker     (127)    18062 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwf-uzf.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwf-vsc.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwf-wel.dfn
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwt-adv.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwt-api.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwt-cnc.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwt-dis.dfn
--rw-r--r--   0 runner    (1001) docker     (127)    11472 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwt-disu.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     6161 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwt-disv.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwt-dsp.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwt-fmi.dfn
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwt-ic.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwt-ist.dfn
--rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwt-lkt.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwt-mst.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwt-mvt.dfn
--rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwt-mwt.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwt-nam.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwt-oc.dfn
--rw-r--r--   0 runner    (1001) docker     (127)    12406 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwt-sft.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwt-src.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwt-ssm.dfn
--rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/gwt-uzt.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/sim-nam.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/sim-tdis.dfn
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/sln-ems.dfn
--rw-r--r--   0 runner    (1001) docker     (127)    26330 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/sln-ims.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/utl-ats.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/utl-laktab.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/utl-obs.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/utl-sfrtab.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/utl-spc.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/utl-spca.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/utl-tas.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/utl-ts.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/utl-tvk.dfn
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/dfn/utl-tvs.dfn
--rw-r--r--   0 runner    (1001) docker     (127)    22120 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/mfdata.py
--rw-r--r--   0 runner    (1001) docker     (127)    77255 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/mfdataarray.py
--rw-r--r--   0 runner    (1001) docker     (127)    86506 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/mfdatalist.py
--rw-r--r--   0 runner    (1001) docker     (127)    95673 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/mfdataplist.py
--rw-r--r--   0 runner    (1001) docker     (127)    36169 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/mfdatascalar.py
--rw-r--r--   0 runner    (1001) docker     (127)   121828 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/mfdatastorage.py
--rw-r--r--   0 runner    (1001) docker     (127)    38784 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/mfdatautil.py
--rw-r--r--   0 runner    (1001) docker     (127)   103330 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/mffileaccess.py
--rw-r--r--   0 runner    (1001) docker     (127)    97262 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/data/mfstructure.py
--rw-r--r--   0 runner    (1001) docker     (127)    24263 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/mfbase.py
--rw-r--r--   0 runner    (1001) docker     (127)    73058 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/mfmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)   137455 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/mfpackage.py
--rw-r--r--   0 runner    (1001) docker     (127)    89953 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/mfsimbase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:31:10.998927 flopy-3.6.0/flopy/mf6/modflow/
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfems.py
--rw-r--r--   0 runner    (1001) docker     (127)    10756 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgnc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwfapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwfbuy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13293 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwfchd.py
--rw-r--r--   0 runner    (1001) docker     (127)    41465 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwfcsub.py
--rw-r--r--   0 runner    (1001) docker     (127)     8247 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwfdis.py
--rw-r--r--   0 runner    (1001) docker     (127)    20273 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwfdisu.py
--rw-r--r--   0 runner    (1001) docker     (127)    12083 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwfdisv.py
--rw-r--r--   0 runner    (1001) docker     (127)    15799 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwfdrn.py
--rw-r--r--   0 runner    (1001) docker     (127)    18185 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwfevt.py
--rw-r--r--   0 runner    (1001) docker     (127)    13084 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwfevta.py
--rw-r--r--   0 runner    (1001) docker     (127)    14180 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwfghb.py
--rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwfgnc.py
--rw-r--r--   0 runner    (1001) docker     (127)    19706 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwfgwf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwfgwt.py
--rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwfhfb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwfic.py
--rw-r--r--   0 runner    (1001) docker     (127)    53846 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwflak.py
--rw-r--r--   0 runner    (1001) docker     (127)    46017 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwfmaw.py
--rw-r--r--   0 runner    (1001) docker     (127)    16509 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwfmvr.py
--rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwfnam.py
--rw-r--r--   0 runner    (1001) docker     (127)    26833 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwfnpf.py
--rw-r--r--   0 runner    (1001) docker     (127)    13427 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwfoc.py
--rw-r--r--   0 runner    (1001) docker     (127)    13494 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwfrch.py
--rw-r--r--   0 runner    (1001) docker     (127)    12488 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwfrcha.py
--rw-r--r--   0 runner    (1001) docker     (127)    14508 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwfriv.py
--rw-r--r--   0 runner    (1001) docker     (127)    54922 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwfsfr.py
--rw-r--r--   0 runner    (1001) docker     (127)     8893 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwfsto.py
--rw-r--r--   0 runner    (1001) docker     (127)    35401 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwfuzf.py
--rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwfvsc.py
--rw-r--r--   0 runner    (1001) docker     (127)    16195 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwfwel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwtadv.py
--rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwtapi.py
--rw-r--r--   0 runner    (1001) docker     (127)    12995 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwtcnc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwtdis.py
--rw-r--r--   0 runner    (1001) docker     (127)    20273 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwtdisu.py
--rw-r--r--   0 runner    (1001) docker     (127)    12072 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwtdisv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwtdsp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwtfmi.py
--rw-r--r--   0 runner    (1001) docker     (127)    18434 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwtgwt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwtic.py
--rw-r--r--   0 runner    (1001) docker     (127)    16251 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwtist.py
--rw-r--r--   0 runner    (1001) docker     (127)    26544 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwtlkt.py
--rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwtmst.py
--rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwtmvt.py
--rw-r--r--   0 runner    (1001) docker     (127)    23987 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwtmwt.py
--rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwtnam.py
--rw-r--r--   0 runner    (1001) docker     (127)    13662 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwtoc.py
--rw-r--r--   0 runner    (1001) docker     (127)    26492 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwtsft.py
--rw-r--r--   0 runner    (1001) docker     (127)    12811 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwtsrc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8153 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwtssm.py
--rw-r--r--   0 runner    (1001) docker     (127)    25071 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfgwtuzt.py
--rw-r--r--   0 runner    (1001) docker     (127)    38564 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfims.py
--rw-r--r--   0 runner    (1001) docker     (127)    16482 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfmvr.py
--rw-r--r--   0 runner    (1001) docker     (127)     7802 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfmvt.py
--rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfnam.py
--rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfsimulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mftdis.py
--rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfutlats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfutllaktab.py
--rw-r--r--   0 runner    (1001) docker     (127)     8384 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfutlobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfutlsfrtab.py
--rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfutlspc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfutlspca.py
--rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfutltas.py
--rw-r--r--   0 runner    (1001) docker     (127)    10700 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfutlts.py
--rw-r--r--   0 runner    (1001) docker     (127)    10013 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfutltvk.py
--rw-r--r--   0 runner    (1001) docker     (127)    10231 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/modflow/mfutltvs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:31:11.002927 flopy-3.6.0/flopy/mf6/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13233 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/utils/binaryfile_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19277 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/utils/binarygrid_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    41033 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/utils/createpackages.py
--rw-r--r--   0 runner    (1001) docker     (127)     7863 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/utils/generate_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9891 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/utils/lakpak_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/utils/mfenums.py
--rw-r--r--   0 runner    (1001) docker     (127)    17406 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/utils/mfobservation.py
--rw-r--r--   0 runner    (1001) docker     (127)    16910 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/utils/mfsimlistfile.py
--rw-r--r--   0 runner    (1001) docker     (127)   125552 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/utils/model_splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)    14038 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/utils/output_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/utils/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    27016 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/utils/reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mf6/utils/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:31:11.002927 flopy-3.6.0/flopy/mfusg/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mfusg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mfusg/cln_dtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    19532 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mfusg/mfusg.py
--rw-r--r--   0 runner    (1001) docker     (127)    23150 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mfusg/mfusgbcf.py
--rw-r--r--   0 runner    (1001) docker     (127)    29968 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mfusg/mfusgcln.py
--rw-r--r--   0 runner    (1001) docker     (127)    29664 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mfusg/mfusgdisu.py
--rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mfusg/mfusggnc.py
--rw-r--r--   0 runner    (1001) docker     (127)    30592 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mfusg/mfusglpf.py
--rw-r--r--   0 runner    (1001) docker     (127)    23812 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mfusg/mfusgsms.py
--rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mfusg/mfusgwel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:31:11.014927 flopy-3.6.0/flopy/modflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32157 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mf.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfaddoutsidefile.py
--rw-r--r--   0 runner    (1001) docker     (127)    33169 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfag.py
--rw-r--r--   0 runner    (1001) docker     (127)    11783 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfbas.py
--rw-r--r--   0 runner    (1001) docker     (127)    16595 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfbcf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfbct.py
--rw-r--r--   0 runner    (1001) docker     (127)     8083 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfchd.py
--rw-r--r--   0 runner    (1001) docker     (127)    10163 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfde4.py
--rw-r--r--   0 runner    (1001) docker     (127)    28539 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfdis.py
--rw-r--r--   0 runner    (1001) docker     (127)     9938 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfdrn.py
--rw-r--r--   0 runner    (1001) docker     (127)     9734 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfdrt.py
--rw-r--r--   0 runner    (1001) docker     (127)    14226 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfevt.py
--rw-r--r--   0 runner    (1001) docker     (127)    24555 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mffhb.py
--rw-r--r--   0 runner    (1001) docker     (127)    20089 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfflwob.py
--rw-r--r--   0 runner    (1001) docker     (127)    12417 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfgage.py
--rw-r--r--   0 runner    (1001) docker     (127)     9097 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfghb.py
--rw-r--r--   0 runner    (1001) docker     (127)    14729 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfgmg.py
--rw-r--r--   0 runner    (1001) docker     (127)    13954 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfhfb.py
--rw-r--r--   0 runner    (1001) docker     (127)    23591 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfhob.py
--rw-r--r--   0 runner    (1001) docker     (127)    11728 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfhyd.py
--rw-r--r--   0 runner    (1001) docker     (127)    35397 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mflak.py
--rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mflmt.py
--rw-r--r--   0 runner    (1001) docker     (127)    25740 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mflpf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfmlt.py
--rw-r--r--   0 runner    (1001) docker     (127)    16694 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfmnw1.py
--rw-r--r--   0 runner    (1001) docker     (127)    76685 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfmnw2.py
--rw-r--r--   0 runner    (1001) docker     (127)    11670 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfmnwi.py
--rw-r--r--   0 runner    (1001) docker     (127)    19506 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfnwt.py
--rw-r--r--   0 runner    (1001) docker     (127)    38964 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfoc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11205 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfpar.py
--rw-r--r--   0 runner    (1001) docker     (127)     8996 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfparbc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfpbc.py
--rw-r--r--   0 runner    (1001) docker     (127)    10636 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfpcg.py
--rw-r--r--   0 runner    (1001) docker     (127)    20281 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfpcgn.py
--rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfpks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfpval.py
--rw-r--r--   0 runner    (1001) docker     (127)    18266 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfrch.py
--rw-r--r--   0 runner    (1001) docker     (127)    12098 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfriv.py
--rw-r--r--   0 runner    (1001) docker     (127)   131324 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfsfr2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7749 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfsip.py
--rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfsor.py
--rw-r--r--   0 runner    (1001) docker     (127)    36297 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfstr.py
--rw-r--r--   0 runner    (1001) docker     (127)    31090 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfsub.py
--rw-r--r--   0 runner    (1001) docker     (127)    25418 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfswi2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfswr1.py
--rw-r--r--   0 runner    (1001) docker     (127)    31219 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfswt.py
--rw-r--r--   0 runner    (1001) docker     (127)    20696 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfupw.py
--rw-r--r--   0 runner    (1001) docker     (127)    42721 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfuzf1.py
--rw-r--r--   0 runner    (1001) docker     (127)    12534 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfwel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflow/mfzon.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:31:11.014927 flopy-3.6.0/flopy/modflowlgr/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflowlgr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20724 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modflowlgr/mflgr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:31:11.018928 flopy-3.6.0/flopy/modpath/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modpath/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19382 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modpath/mp6.py
--rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modpath/mp6bas.py
--rw-r--r--   0 runner    (1001) docker     (127)    20043 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modpath/mp6sim.py
--rw-r--r--   0 runner    (1001) docker     (127)    16755 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modpath/mp7.py
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modpath/mp7bas.py
--rw-r--r--   0 runner    (1001) docker     (127)    49791 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modpath/mp7particledata.py
--rw-r--r--   0 runner    (1001) docker     (127)    15320 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modpath/mp7particlegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)    25279 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/modpath/mp7sim.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:31:11.022928 flopy-3.6.0/flopy/mt3d/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mt3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26426 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mt3d/mt.py
--rw-r--r--   0 runner    (1001) docker     (127)    16041 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mt3d/mtadv.py
--rw-r--r--   0 runner    (1001) docker     (127)    39209 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mt3d/mtbtn.py
--rw-r--r--   0 runner    (1001) docker     (127)    12194 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mt3d/mtcts.py
--rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mt3d/mtdsp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mt3d/mtgcg.py
--rw-r--r--   0 runner    (1001) docker     (127)    17714 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mt3d/mtlkt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mt3d/mtphc.py
--rw-r--r--   0 runner    (1001) docker     (127)    27504 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mt3d/mtrct.py
--rw-r--r--   0 runner    (1001) docker     (127)    28812 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mt3d/mtsft.py
--rw-r--r--   0 runner    (1001) docker     (127)    29313 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mt3d/mtssm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mt3d/mttob.py
--rw-r--r--   0 runner    (1001) docker     (127)    27575 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/mt3d/mtuzt.py
--rw-r--r--   0 runner    (1001) docker     (127)    43700 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/pakbase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:31:11.022928 flopy-3.6.0/flopy/pest/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/pest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/pest/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/pest/templatewriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/pest/tplarray.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:31:11.022928 flopy-3.6.0/flopy/plot/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53616 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/plot/crosssection.py
--rw-r--r--   0 runner    (1001) docker     (127)    34645 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/plot/map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:31:11.022928 flopy-3.6.0/flopy/plot/mplstyle/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/plot/mplstyle/usgsmap.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/plot/mplstyle/usgsmap_linux.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/plot/mplstyle/usgsplot.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/plot/mplstyle/usgsplot_linux.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)    94661 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/plot/plotutil.py
--rw-r--r--   0 runner    (1001) docker     (127)    12926 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/plot/styles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:31:11.026928 flopy-3.6.0/flopy/seawat/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/seawat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14845 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/seawat/swt.py
--rw-r--r--   0 runner    (1001) docker     (127)    20286 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/seawat/swtvdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    17335 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/seawat/swtvsc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:31:11.034928 flopy-3.6.0/flopy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    76096 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/binaryfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    32255 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/check.py
--rw-r--r--   0 runner    (1001) docker     (127)    49943 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/crs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/cvfdutil.py
--rw-r--r--   0 runner    (1001) docker     (127)    19903 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/datafile.py
--rw-r--r--   0 runner    (1001) docker     (127)    27819 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/datautil.py
--rw-r--r--   0 runner    (1001) docker     (127)    17734 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/flopy_io.py
--rw-r--r--   0 runner    (1001) docker     (127)    12606 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/formattedfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    24526 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)    15710 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/geospatial_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    26931 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/get_modflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    64842 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/gridgen.py
--rw-r--r--   0 runner    (1001) docker     (127)    86121 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/gridintersect.py
--rw-r--r--   0 runner    (1001) docker     (127)    11797 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/gridutil.py
--rw-r--r--   0 runner    (1001) docker     (127)    18441 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/lgrutil.py
--rw-r--r--   0 runner    (1001) docker     (127)    31770 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/mflistfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    23627 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/mfreadnam.py
--rw-r--r--   0 runner    (1001) docker     (127)    52589 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/modpathfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    18038 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/mtlistfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    20461 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/observationfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    14915 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/optionblock.py
--rw-r--r--   0 runner    (1001) docker     (127)    16371 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/parse_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    28932 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    25173 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/rasters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/recarray_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/sfroutputfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    23617 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/swroutputfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    22638 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/triangle.py
--rw-r--r--   0 runner    (1001) docker     (127)   101771 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/util_array.py
--rw-r--r--   0 runner    (1001) docker     (127)    42972 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/util_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/utils_def.py
--rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/utl_import.py
--rw-r--r--   0 runner    (1001) docker     (127)    13795 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/voronoi.py
--rw-r--r--   0 runner    (1001) docker     (127)   102292 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/utils/zonbud.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-08 04:30:03.000000 flopy-3.6.0/flopy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 04:31:11.034928 flopy-3.6.0/flopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-02-08 04:31:10.000000 flopy-3.6.0/flopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9539 2024-02-08 04:31:10.000000 flopy-3.6.0/flopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-08 04:31:10.000000 flopy-3.6.0/flopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-08 04:31:10.000000 flopy-3.6.0/flopy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-08 04:30:13.000000 flopy-3.6.0/flopy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-02-08 04:31:10.000000 flopy-3.6.0/flopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-08 04:31:10.000000 flopy-3.6.0/flopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-02-08 04:30:03.000000 flopy-3.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-08 04:31:11.038928 flopy-3.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-08 04:30:03.000000 flopy-3.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:22.251649 flopy-3.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-23 21:08:12.000000 flopy-3.7.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-23 21:08:12.000000 flopy-3.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-23 21:08:12.000000 flopy-3.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-05-23 21:09:22.251649 flopy-3.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-05-23 21:08:12.000000 flopy-3.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:22.171648 flopy-3.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-23 21:08:12.000000 flopy-3.7.0/docs/PyPI_release.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9638 2024-05-23 21:08:12.000000 flopy-3.7.0/docs/make_release.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-05-23 21:08:12.000000 flopy-3.7.0/docs/mf6_dev_guide.md
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-23 21:08:12.000000 flopy-3.7.0/docs/script_examples.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18405 2024-05-23 21:08:12.000000 flopy-3.7.0/docs/supported_packages.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:22.171648 flopy-3.7.0/flopy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/datbase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:22.175648 flopy-3.7.0/flopy/discretization/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/discretization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40588 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/discretization/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/discretization/modeltime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65029 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/discretization/structuredgrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34307 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/discretization/unstructuredgrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19405 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/discretization/vertexgrid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:22.175648 flopy-3.7.0/flopy/export/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/export/longnames.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9625 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/export/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49738 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/export/netcdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24034 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/export/shapefile_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/export/unitsformat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68463 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/export/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53155 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/export/vtk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61133 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mbase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:22.175648 flopy-3.7.0/flopy/mf6/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:22.179648 flopy-3.7.0/flopy/mf6/coordinates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/coordinates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32921 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/coordinates/modeldimensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29257 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/coordinates/modelgrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/coordinates/simulationtime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:22.179648 flopy-3.7.0/flopy/mf6/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:22.199648 flopy-3.7.0/flopy/mf6/data/dfn/
+-rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/common.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/exg-gwegwe.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/exg-gwfgwe.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)    12070 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/exg-gwfgwf.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/exg-gwfgwt.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/exg-gwfprt.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     9230 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/exg-gwtgwt.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/flopy.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwe-adv.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwe-cnd.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwe-ctp.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwe-dis.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)    11742 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwe-disu.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwe-disv.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwe-esl.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwe-est.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwe-fmi.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwe-ic.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)    12809 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwe-lke.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwe-mve.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)    11254 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwe-mwe.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwe-nam.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     5861 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwe-oc.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)    12880 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwe-sfe.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwe-ssm.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)    11559 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwe-uze.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwf-api.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwf-buy.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwf-chd.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)    22008 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwf-csub.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwf-dis.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)    11740 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwf-disu.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     6440 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwf-disv.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwf-drn.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwf-evt.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwf-evta.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwf-ghb.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwf-gnc.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwf-hfb.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwf-ic.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)    29248 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwf-lak.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)    27133 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwf-maw.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwf-mvr.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwf-nam.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)    17230 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwf-npf.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwf-oc.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwf-rch.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwf-rcha.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwf-riv.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)    31015 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwf-sfr.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwf-sto.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)    18079 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwf-uzf.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwf-vsc.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwf-wel.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwt-adv.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwt-api.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwt-cnc.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwt-dis.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)    11740 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwt-disu.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwt-disv.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwt-dsp.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwt-fmi.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwt-ic.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwt-ist.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwt-lkt.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwt-mst.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwt-mvt.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwt-mwt.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwt-nam.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwt-oc.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)    12406 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwt-sft.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwt-src.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwt-ssm.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/gwt-uzt.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/prt-dis.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/prt-disv.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/prt-fmi.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/prt-mip.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/prt-nam.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     7740 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/prt-oc.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)    12672 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/prt-prp.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     6288 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/sim-nam.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/sim-tdis.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/sln-ems.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)    26329 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/sln-ims.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/sln-pts.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/utl-ats.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/utl-hpc.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/utl-laktab.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/utl-obs.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/utl-sfrtab.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/utl-spc.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/utl-spca.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/utl-spt.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/utl-spta.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/utl-tas.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/utl-ts.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/utl-tvk.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/dfn/utl-tvs.dfn
+-rw-r--r--   0 runner    (1001) docker     (127)    22815 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/mfdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78097 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/mfdataarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86858 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/mfdatalist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    97666 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/mfdataplist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36414 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/mfdatascalar.py
+-rw-r--r--   0 runner    (1001) docker     (127)   122575 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/mfdatastorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38834 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/mfdatautil.py
+-rw-r--r--   0 runner    (1001) docker     (127)   103578 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/mffileaccess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    97209 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/data/mfstructure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24736 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/mfbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75604 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/mfmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137829 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/mfpackage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92608 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/mfsimbase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:22.215649 flopy-3.7.0/flopy/mf6/modflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfems.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10882 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgnc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgweadv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8622 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwecnd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12970 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwectp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8771 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwedis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20811 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwedisu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12607 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwedisv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12846 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgweesl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgweest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwefmi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18463 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwegwe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgweic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27081 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwelke.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7863 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwemve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24662 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwemwe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwenam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13614 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgweoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27185 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwesfe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwessm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24994 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgweuze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6391 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwfapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9228 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwfbuy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13288 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwfchd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41460 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwfcsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwfdis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20809 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwfdisu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12618 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwfdisv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15794 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwfdrn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18180 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwfevt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13385 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwfevta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14175 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwfghb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10940 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwfgnc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwfgwe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20048 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwfgwf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwfgwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5953 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwfhfb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwfic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53841 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwflak.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46012 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwfmaw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16504 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwfmvr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwfnam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25499 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwfnpf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13422 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwfoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwfprt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13489 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwfrch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12789 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwfrcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14503 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwfriv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56054 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwfsfr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwfsto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35428 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwfuzf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12051 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwfvsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16478 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwfwel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwtadv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6391 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwtapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12990 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwtcnc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8771 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwtdis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20809 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwtdisu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12607 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwtdisv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7875 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwtdsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwtfmi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18197 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwtgwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwtic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16246 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwtist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26539 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwtlkt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8725 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwtmst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7863 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwtmvt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23982 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwtmwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwtnam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13657 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwtoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26487 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwtsft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12806 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwtsrc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8148 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwtssm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25066 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfgwtuzt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38558 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfims.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16477 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfmvr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7797 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfmvt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfnam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfprt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8771 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfprtdis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12607 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfprtdisv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfprtfmi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfprtmip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfprtnam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17554 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfprtoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22988 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfprtprp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12852 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfsimulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mftdis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7979 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfutlats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfutlhpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfutllaktab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfutlobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfutlsfrtab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfutlspc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfutlspca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6703 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfutlspt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfutlspta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7734 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfutltas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfutlts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10008 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfutltvk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10226 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/modflow/mfutltvs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:22.219648 flopy-3.7.0/flopy/mf6/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13234 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/utils/binaryfile_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19594 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/utils/binarygrid_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42622 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/utils/createpackages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7863 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/utils/generate_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9891 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/utils/lakpak_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/utils/mfenums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17409 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/utils/mfobservation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16910 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/utils/mfsimlistfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)   125566 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/utils/model_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13990 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/utils/output_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/utils/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27016 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/utils/reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mf6/utils/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:22.219648 flopy-3.7.0/flopy/mfusg/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mfusg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mfusg/cln_dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19532 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mfusg/mfusg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23150 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mfusg/mfusgbcf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29968 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mfusg/mfusgcln.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29665 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mfusg/mfusgdisu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mfusg/mfusggnc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30592 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mfusg/mfusglpf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23813 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mfusg/mfusgsms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mfusg/mfusgwel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:22.231649 flopy-3.7.0/flopy/modflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32157 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfaddoutsidefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33169 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11784 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfbas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16547 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfbcf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfbct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8083 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfchd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10163 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfde4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28516 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfdis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9914 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfdrn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9710 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfdrt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14226 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfevt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24629 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mffhb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20089 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfflwob.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12417 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfgage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfghb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14729 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfgmg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13954 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfhfb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23591 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfhob.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11728 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfhyd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35423 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mflak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mflmt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25722 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mflpf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfmlt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16694 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfmnw1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76888 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfmnw2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11670 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfmnwi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19506 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfnwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38940 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11205 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfpar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8996 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfparbc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfpbc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10636 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfpcg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20281 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfpcgn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7723 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfpks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfpval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18267 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfrch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfriv.py
+-rw-r--r--   0 runner    (1001) docker     (127)   131302 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfsfr2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7749 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfsip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfsor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36297 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfstr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31090 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25422 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfswi2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfswr1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31219 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfswt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20696 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfupw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42721 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfuzf1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12534 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfwel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflow/mfzon.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:22.231649 flopy-3.7.0/flopy/modflowlgr/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflowlgr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20724 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modflowlgr/mflgr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:22.231649 flopy-3.7.0/flopy/modpath/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modpath/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19382 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modpath/mp6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modpath/mp6bas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20044 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modpath/mp6sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16755 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modpath/mp7.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modpath/mp7bas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52394 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modpath/mp7particledata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15320 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modpath/mp7particlegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25279 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/modpath/mp7sim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:22.235649 flopy-3.7.0/flopy/mt3d/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mt3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26428 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mt3d/mt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16041 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mt3d/mtadv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39175 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mt3d/mtbtn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12194 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mt3d/mtcts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mt3d/mtdsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mt3d/mtgcg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17706 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mt3d/mtlkt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mt3d/mtphc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27504 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mt3d/mtrct.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28804 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mt3d/mtsft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29312 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mt3d/mtssm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mt3d/mttob.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27567 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/mt3d/mtuzt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43700 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/pakbase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:22.235649 flopy-3.7.0/flopy/pest/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/pest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/pest/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/pest/templatewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/pest/tplarray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:22.235649 flopy-3.7.0/flopy/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53717 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/plot/crosssection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34948 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/plot/map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:22.235649 flopy-3.7.0/flopy/plot/mplstyle/
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/plot/mplstyle/usgsmap.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/plot/mplstyle/usgsplot.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)    95471 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/plot/plotutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12731 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/plot/styles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:22.235649 flopy-3.7.0/flopy/seawat/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/seawat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14845 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/seawat/swt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20286 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/seawat/swtvdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17335 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/seawat/swtvsc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:22.243649 flopy-3.7.0/flopy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75539 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/binaryfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32255 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49943 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/crs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11958 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/cvfdutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19907 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/datafile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28526 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/datautil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17674 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/flopy_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12606 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/formattedfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24526 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15710 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/geospatial_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27389 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/get_modflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64827 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/gridgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85957 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/gridintersect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11795 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/gridutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18842 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/lgrutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31770 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/mflistfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23627 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/mfreadnam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33075 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/modpathfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18038 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/mtlistfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20462 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/observationfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15543 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/optionblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16371 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/parse_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/particletrackfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28932 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25174 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/rasters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/recarray_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/sfroutputfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23618 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/swroutputfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22638 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/triangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101773 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/util_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43342 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/util_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/utils_def.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/utl_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13794 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/voronoi.py
+-rw-r--r--   0 runner    (1001) docker     (127)   102254 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/utils/zonbud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-23 21:08:13.000000 flopy-3.7.0/flopy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:09:22.243649 flopy-3.7.0/flopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-05-23 21:09:22.000000 flopy-3.7.0/flopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11499 2024-05-23 21:09:22.000000 flopy-3.7.0/flopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 21:09:22.000000 flopy-3.7.0/flopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-23 21:09:22.000000 flopy-3.7.0/flopy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 21:08:26.000000 flopy-3.7.0/flopy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-23 21:09:22.000000 flopy-3.7.0/flopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 21:09:22.000000 flopy-3.7.0/flopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-23 21:08:13.000000 flopy-3.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 21:09:22.251649 flopy-3.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-23 21:08:13.000000 flopy-3.7.0/setup.py
```

### Comparing `flopy-3.6.0/CITATION.cff` & `flopy-3.7.0/CITATION.cff`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 cff-version: 1.2.0
 message: If you use this software, please cite both the article from preferred-citation,
   references, and the software itself.
 type: software
 title: FloPy
-version: 3.6.0
-date-released: '2024-02-08'
+version: 3.7.0
+date-released: '2024-05-23'
 doi: 10.5066/F7BK19FH
 abstract: A Python package to create, run, and post-process MODFLOW-based models.
 repository-artifact: https://pypi.org/project/flopy
 repository-code: https://github.com/modflowpy/flopy
 license: CC0-1.0
 authors:
 - family-names: Bakker
```

### Comparing `flopy-3.6.0/LICENSE.md` & `flopy-3.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/PKG-INFO` & `flopy-3.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flopy
-Version: 3.6.0
+Version: 3.7.0
 Summary: FloPy is a Python package to create, run, and post-process MODFLOW-based models
 Author-email: FloPy Team <modflow@usgs.gov>
 Maintainer-email: "Joseph D. Hughes" <jdhughes@usgs.gov>
 License: CC0
 Project-URL: Documentation, https://flopy.readthedocs.io
 Project-URL: Release Notes, https://github.com/modflowpy/flopy/blob/develop/docs/version_changes.md
 Project-URL: Bug Tracker, https://github.com/modflowpy/flopy/issues
@@ -25,32 +25,31 @@
 License-File: LICENSE.md
 Requires-Dist: numpy<2.0.0,>=1.15.0
 Requires-Dist: matplotlib>=1.4.0
 Requires-Dist: pandas>=2.0.0
 Provides-Extra: dev
 Requires-Dist: flopy[doc,lint,optional,test]; extra == "dev"
 Provides-Extra: lint
-Requires-Dist: black; extra == "lint"
 Requires-Dist: cffconvert; extra == "lint"
-Requires-Dist: flake8; extra == "lint"
-Requires-Dist: isort; extra == "lint"
-Requires-Dist: pylint; extra == "lint"
+Requires-Dist: ruff; extra == "lint"
 Provides-Extra: test
 Requires-Dist: flopy[lint]; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: flaky; extra == "test"
 Requires-Dist: filelock; extra == "test"
 Requires-Dist: jupyter; extra == "test"
 Requires-Dist: jupytext; extra == "test"
 Requires-Dist: modflow-devtools; extra == "test"
-Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest!=8.1.0; extra == "test"
 Requires-Dist: pytest-benchmark; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-dotenv; extra == "test"
 Requires-Dist: pytest-xdist; extra == "test"
+Requires-Dist: pyzmq>=25.1.2; extra == "test"
+Requires-Dist: syrupy; extra == "test"
 Requires-Dist: virtualenv; extra == "test"
 Provides-Extra: optional
 Requires-Dist: affine; extra == "optional"
 Requires-Dist: descartes; extra == "optional"
 Requires-Dist: fiona; extra == "optional"
 Requires-Dist: geojson; extra == "optional"
 Requires-Dist: geopandas; extra == "optional"
@@ -106,15 +105,15 @@
 
 *Citation for FloPy:*
 
 [Bakker, Mark, Post, Vincent, Langevin, C. D., Hughes, J. D., White, J. T., Starn, J. J. and Fienen, M. N., 2016, Scripting MODFLOW Model Development Using Python and FloPy: Groundwater, v. 54, p. 733–739, doi:10.1111/gwat.12413.](https://doi.org/10.1111/gwat.12413)
 
 *Software/Code citation for FloPy:*
 
-[Bakker, Mark, Post, Vincent, Hughes, J. D., Langevin, C. D., White, J. T., Leaf, A. T., Paulinski, S. R., Bellino, J. C., Morway, E. D., Toews, M. W., Larsen, J. D., Fienen, M. N., Starn, J. J., Brakenhoff, D. A., and Bonelli, W. P., 2024, FloPy v3.6.0: U.S. Geological Survey Software Release, 08 February 2024, https://doi.org/10.5066/F7BK19FH](https://doi.org/10.5066/F7BK19FH)
+[Bakker, Mark, Post, Vincent, Hughes, J. D., Langevin, C. D., White, J. T., Leaf, A. T., Paulinski, S. R., Bellino, J. C., Morway, E. D., Toews, M. W., Larsen, J. D., Fienen, M. N., Starn, J. J., Brakenhoff, D. A., and Bonelli, W. P., 2024, FloPy v3.7.0: U.S. Geological Survey Software Release, 23 May 2024, https://doi.org/10.5066/F7BK19FH](https://doi.org/10.5066/F7BK19FH)
 
 
 Disclaimer
 ----------
 
 This software is provided "as is" and "as-available", and makes no 
 representations or warranties of any kind concerning the software, whether
```

### Comparing `flopy-3.6.0/README.md` & `flopy-3.7.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 <img src="https://raw.githubusercontent.com/modflowpy/flopy/master/examples/images/flopy3.png" alt="flopy3" style="width:50;height:20">
 
-### Version 3.6.0
+### Version 3.7.0
 [![flopy continuous integration](https://github.com/modflowpy/flopy/actions/workflows/commit.yml/badge.svg?branch=develop)](https://github.com/modflowpy/flopy/actions/workflows/commit.yml)
 [![Read the Docs](https://github.com/modflowpy/flopy/actions/workflows/rtd.yml/badge.svg?branch=develop)](https://github.com/modflowpy/flopy/actions/workflows/rtd.yml)
 
 [![codecov](https://codecov.io/gh/modflowpy/flopy/branch/develop/graph/badge.svg)](https://codecov.io/gh/modflowpy/flopy)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/3f44f457aa474a8f83ad60c1842f7be2)](https://www.codacy.com/gh/modflowpy/flopy/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=modflowpy/flopy&amp;utm_campaign=Badge_Grade)
 [![Documentation Status](https://readthedocs.org/projects/flopy/badge/?version=latest)](https://flopy.readthedocs.io/en/latest/?badge=latest)
 
@@ -146,15 +146,15 @@
 
 [Hughes, J.D., Langevin, C.D., Paulinski, S.R., Larsen, J.D. and Brakenhoff, D. (2023), FloPy Workflows for Creating Structured and Unstructured MODFLOW Models. Groundwater. https://doi.org/10.1111/gwat.13327](https://doi.org/10.1111/gwat.13327)
 
 [Bakker, Mark, Post, Vincent, Langevin, C. D., Hughes, J. D., White, J. T., Starn, J. J. and Fienen, M. N., 2016, Scripting MODFLOW Model Development Using Python and FloPy: Groundwater, v. 54, p. 733–739, doi:10.1111/gwat.12413.](https://doi.org/10.1111/gwat.12413)
 
 ##### ***Software/Code citation for FloPy:***
 
-[Bakker, Mark, Post, Vincent, Hughes, J. D., Langevin, C. D., White, J. T., Leaf, A. T., Paulinski, S. R., Bellino, J. C., Morway, E. D., Toews, M. W., Larsen, J. D., Fienen, M. N., Starn, J. J., Brakenhoff, D. A., and Bonelli, W. P., 2024, FloPy v3.6.0: U.S. Geological Survey Software Release, 08 February 2024, https://doi.org/10.5066/F7BK19FH](https://doi.org/10.5066/F7BK19FH)
+[Bakker, Mark, Post, Vincent, Hughes, J. D., Langevin, C. D., White, J. T., Leaf, A. T., Paulinski, S. R., Bellino, J. C., Morway, E. D., Toews, M. W., Larsen, J. D., Fienen, M. N., Starn, J. J., Brakenhoff, D. A., and Bonelli, W. P., 2024, FloPy v3.7.0: U.S. Geological Survey Software Release, 23 May 2024, https://doi.org/10.5066/F7BK19FH](https://doi.org/10.5066/F7BK19FH)
 
 
 Additional FloPy Related Publications
 -----------------------------------------------
 
 [Leaf A.T, and Fienen M. N., 2022, Flopy&mdash;The Python Interface for MODFLOW: Groundwater, v. 60, no. 6, p. 710-712. doi:10.1111/gwat.13259.](https://doi.org/10.1111/gwat.13259)
```

### Comparing `flopy-3.6.0/docs/PyPI_release.md` & `flopy-3.7.0/docs/PyPI_release.md`

 * *Files 9% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 *Citation for FloPy:*
 
 [Bakker, Mark, Post, Vincent, Langevin, C. D., Hughes, J. D., White, J. T., Starn, J. J. and Fienen, M. N., 2016, Scripting MODFLOW Model Development Using Python and FloPy: Groundwater, v. 54, p. 733–739, doi:10.1111/gwat.12413.](https://doi.org/10.1111/gwat.12413)
 
 *Software/Code citation for FloPy:*
 
-[Bakker, Mark, Post, Vincent, Hughes, J. D., Langevin, C. D., White, J. T., Leaf, A. T., Paulinski, S. R., Bellino, J. C., Morway, E. D., Toews, M. W., Larsen, J. D., Fienen, M. N., Starn, J. J., Brakenhoff, D. A., and Bonelli, W. P., 2024, FloPy v3.6.0: U.S. Geological Survey Software Release, 08 February 2024, https://doi.org/10.5066/F7BK19FH](https://doi.org/10.5066/F7BK19FH)
+[Bakker, Mark, Post, Vincent, Hughes, J. D., Langevin, C. D., White, J. T., Leaf, A. T., Paulinski, S. R., Bellino, J. C., Morway, E. D., Toews, M. W., Larsen, J. D., Fienen, M. N., Starn, J. J., Brakenhoff, D. A., and Bonelli, W. P., 2024, FloPy v3.7.0: U.S. Geological Survey Software Release, 23 May 2024, https://doi.org/10.5066/F7BK19FH](https://doi.org/10.5066/F7BK19FH)
 
 
 Disclaimer
 ----------
 
 This software is provided "as is" and "as-available", and makes no 
 representations or warranties of any kind concerning the software, whether
```

### Comparing `flopy-3.6.0/docs/make_release.md` & `flopy-3.7.0/docs/make_release.md`

 * *Files 3% similar despite different names*

```diff
@@ -94,17 +94,15 @@
 
 #### Release from `master` branch
 
 - Run `python scripts/update_version.py -v <semver>` to update the version number stored in `version.txt` and `flopy/version.py`. For an approved release use the `--approve` flag.
 
 - Update MODFLOW 6 dfn files in the repository and MODFLOW 6 package classes by running `python -m flopy.mf6.utils.generate_classes --ref master --no-backup`
 
-- Run `isort` and `black` on the `flopy` module. This can be achieved by running `python scripts/pull_request_prepare.py` from the project root. The commands `isort .` and `black .` can also be run individually instead.
-
-- Use `run_notebooks.py` in the `scripts` directory to rerun all notebooks in `.docs/Notebooks`.
+- Run `ruff check .` and `ruff format .` from the project root.
 
 - Generate a changelog starting from the last release with [git cliff](https://github.com/orhun/git-cliff), for instance: `git cliff --config cliff.toml --unreleased --tag=<release version number>`.
 
 - Prepend the release changelog to the comprehensive changelog file `docs/version_changes.md`.
 
 - Commit changes to the release branch and push the commit to the [`modflowpy/flopy` GitHub repository](https://github.com/modflowpy/flopy) (you must have write permissions on the repo).
 
@@ -117,15 +115,15 @@
 
 #### Reinitialize `develop` branch
 
 1.  Merge the `master` branch into the `develop` branch.
 
 2.  Set the development version as appropriate: `python scripts/update_version.py -v <version>`. The version number must comply with [PEP 440](https://peps.python.org/pep-0440/).
 
-3.  Lint Python files: `python scripts/pull_request_prepare.py`
+3.  Lint and format Python files: `ruff check .` and `ruff format .` from the project root.
 
 4.  Commit and push the updated `develop` branch.
 
 
 #### Publish the release
 
 ##### PyPI
```

### Comparing `flopy-3.6.0/docs/mf6_dev_guide.md` & `flopy-3.7.0/docs/mf6_dev_guide.md`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/docs/script_examples.md` & `flopy-3.7.0/docs/script_examples.md`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/docs/supported_packages.md` & `flopy-3.7.0/docs/supported_packages.md`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/__init__.py` & `flopy-3.7.0/flopy/__init__.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/datbase.py` & `flopy-3.7.0/flopy/datbase.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/discretization/grid.py` & `flopy-3.7.0/flopy/discretization/grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,34 +109,20 @@
     yoffset : float
         y coordinate of the origin point in the spatial reference coordinate
         system
     angrot : float
         rotation angle of model grid, as it is rotated around the origin point
     angrot_radians : float
         rotation angle of model grid, in radians
-    xgrid : ndarray
-        returns numpy meshgrid of x edges in reference frame defined by
-        point_type
-    ygrid : ndarray
-        returns numpy meshgrid of y edges in reference frame defined by
-        point_type
-    zgrid : ndarray
-        returns numpy meshgrid of z edges in reference frame defined by
-        point_type
     xcenters : ndarray
         returns x coordinate of cell centers
     ycenters : ndarray
         returns y coordinate of cell centers
     ycenters : ndarray
         returns z coordinate of cell centers
-    xyzgrid : [ndarray, ndarray, ndarray]
-        returns the location of grid edges of all model cells. if the model
-        grid contains spatial reference information, the grid edges are in the
-        coordinate system provided by the spatial reference information.
-        returns a list of three ndarrays for the x, y, and z coordinates
     xyzcellcenters : [ndarray, ndarray, ndarray]
         returns the cell centers of all model cells in the model grid.  if
         the model grid contains spatial reference information, the cell centers
         are in the coordinate system provided by the spatial reference
         information. otherwise the cell centers are based on a 0,0 location
         for the upper left corner of the model grid. returns a list of three
         ndarrays for the x, y, and z coordinates
@@ -146,18 +132,14 @@
     get_coords(x, y)
         transform point or array of points x, y from model coordinates to
         spatial coordinates
     grid_lines : (point_type=PointType.spatialxyz) : list
         returns the model grid lines in a list.  each line is returned as a
         list containing two tuples in the format [(x1,y1), (x2,y2)] where
         x1,y1 and x2,y2 are the endpoints of the line.
-    xyvertices : (point_type) : ndarray
-        1D array of x and y coordinates of cell vertices for whole grid
-        (single layer) in C-style (row-major) order
-        (same as np.ravel())
 
     See Also
     --------
 
     Notes
     -----
 
@@ -817,15 +799,15 @@
         -------
             list : n-dimensional list of nodes to not plot for each layer
         """
         return [[] for _ in range(nlay)]
 
     def cross_section_adjust_indicies(self, k, cbcnt):
         """
-        Method to get adjusted indicies by layer and confining bed
+        Method to get adjusted indices by layer and confining bed
         for PlotCrossSection plotting
 
         Parameters
         ----------
         k : int
             zero based layer number
         cbcnt : int
@@ -840,16 +822,16 @@
         ncbnn = adjnn - (cbcnt * self.ncpl)
         return k + 1, k + 1, ncbnn
 
     def cross_section_set_contour_arrays(
         self, plotarray, xcenters, head, elev, projpts
     ):
         """
-        Method to set countour array centers for rare instances where
-        matplotlib contouring is prefered over trimesh plotting
+        Method to set contour array centers for rare instances where
+        matplotlib contouring is preferred over trimesh plotting
 
         Parameters
         ----------
         plotarray : np.ndarray
             array of data for contouring
         xcenters : np.ndarray
             xcenters array
```

### Comparing `flopy-3.6.0/flopy/discretization/modeltime.py` & `flopy-3.7.0/flopy/discretization/modeltime.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/discretization/structuredgrid.py` & `flopy-3.7.0/flopy/discretization/structuredgrid.py`

 * *Files 1% similar despite different names*

```diff
@@ -832,15 +832,15 @@
         **kwargs
             k : int
                 layer number
             i : int
                 row number
             j : int
                 column number
-            as_node : bool
+            as_nodes : bool
                 flag to return neighbors as node numbers
             method : str
                 "rook" for shared edge neighbors (default) "queen" for shared
                 vertex neighbors (for flow accumulation calculations)
             reset : bool
                 flag to re-calculate neighbors, default is False
 
@@ -987,38 +987,61 @@
     @property
     def top_botm(self):
         new_top = np.expand_dims(self._top, 0)
         return np.concatenate((new_top, self._botm), axis=0)
 
     def get_cell_vertices(self, *args, **kwargs):
         """
-        Method to get a set of cell vertices for a single cell
-            used in the Shapefile export utilities and plotting code
-        :param node: (int) node number
-        :param i: (int) cell row number
-        :param j: (int) cell column number
+        Get a set of cell vertices for a single cell.
+
+        Parameters
+        ----------
+        node : int, optional
+            Node index, mutually exclusive with i and j
+        i, j : int, optional
+            Row and column index, mutually exclusive with node
+
         Returns
-        ------- list of x,y cell vertices
+        -------
+        list
+            list of tuples with x,y coordinates to cell vertices
+
+        Examples
+        --------
+        >>> import flopy
+        >>> import numpy as np
+        >>> delr, delc = np.array([10.0] * 3), np.array([10.0] * 4)
+        >>> sg = flopy.discretization.StructuredGrid(delr=delr, delc=delc)
+        >>> sg.get_cell_vertices(node=0)
+        [(0.0, 40.0), (10.0, 40.0), (10.0, 30.0), (0.0, 30.0)]
+        >>> sg.get_cell_vertices(3, 0)
+        [(0.0, 10.0), (10.0, 10.0), (10.0, 0.0), (0.0, 0.0)]
         """
-        nn = None
         if kwargs:
-            if "node" in kwargs:
-                nn = kwargs.pop("node")
-            else:
+            if args:
+                raise TypeError(
+                    "mixed positional and keyword arguments not supported"
+                )
+            elif "node" in kwargs:
+                _, i, j = self.get_lrc(kwargs.pop("node"))[0]
+            elif "i" in kwargs and "j" in kwargs:
                 i = kwargs.pop("i")
                 j = kwargs.pop("j")
-
-        if len(args) > 0:
-            if len(args) == 1:
-                nn = args[0]
-            else:
-                i, j = args[0:2]
-
-        if nn is not None:
-            k, i, j = self.get_lrc(nn)[0]
+            if kwargs:
+                unused = ", ".join(kwargs.keys())
+                raise TypeError(f"unused keyword arguments: {unused}")
+        elif len(args) == 0:
+            raise TypeError("expected one or more arguments")
+
+        if len(args) == 1:
+            _, i, j = self.get_lrc(args[0])[0]
+        elif len(args) == 2:
+            i, j = args
+        elif len(args) > 2:
+            raise TypeError("too many arguments")
 
         self._copy_cache = False
         cell_verts = [
             (self.xvertices[i, j], self.yvertices[i, j]),
             (self.xvertices[i, j + 1], self.yvertices[i, j + 1]),
             (self.xvertices[i + 1, j + 1], self.yvertices[i + 1, j + 1]),
             (self.xvertices[i + 1, j], self.yvertices[i + 1, j]),
```

### Comparing `flopy-3.6.0/flopy/discretization/unstructuredgrid.py` & `flopy-3.7.0/flopy/discretization/unstructuredgrid.py`

 * *Files 2% similar despite different names*

```diff
@@ -356,15 +356,15 @@
             return self._cache_dict[cache_index].data
         else:
             return self._cache_dict[cache_index].data_nocopy
 
     @property
     def xyzvertices(self):
         """
-        Method to get model grid verticies
+        Method to get model grid vertices
 
         Returns:
             list of dimension ncpl by nvertices
         """
         cache_index = "xyzgrid"
         if (
             cache_index not in self._cache_dict
@@ -438,15 +438,15 @@
             strt += ncpl
             nodeskip.append(layskip)
 
         return nodeskip
 
     def cross_section_adjust_indicies(self, k, cbcnt):
         """
-        Method to get adjusted indicies by layer and confining bed
+        Method to get adjusted indices by layer and confining bed
         for PlotCrossSection plotting
 
         Parameters
         ----------
         k : int
             zero based model layer
         cbcnt : int
@@ -459,16 +459,16 @@
         """
         return 1, k + 1, 0
 
     def cross_section_set_contour_arrays(
         self, plotarray, xcenters, head, elev, projpts
     ):
         """
-        Method to set countour array centers for rare instances where
-        matplotlib contouring is prefered over trimesh plotting
+        Method to set contour array centers for rare instances where
+        matplotlib contouring is preferred over trimesh plotting
 
         Parameters
         ----------
         plotarray : np.ndarray
             array of data for contouring
         xcenters : np.ndarray
             xcenters array
@@ -1015,21 +1015,25 @@
         -------
             An UnstructuredGrid
         """
 
         with open(file_path) as file:
 
             def split_line():
-                return file.readline().strip().split()
+                return [
+                    head.upper() for head in file.readline().strip().split()
+                ]
 
             header = split_line()
+            while header[0][0] == "#":
+                header = split_line()
             if not (len(header) == 1 and header[0] == "UNSTRUCTURED") or (
                 len(header) == 2 and header == ["UNSTRUCTURED", "GWF"]
             ):
-                raise ValueError(f"Invalid GSF file, no header")
+                raise ValueError("Invalid GSF file, no header")
 
             nnodes = int(split_line()[0])
             verts_declared = int(split_line()[0])
 
             vertices = []
             zverts = []
```

### Comparing `flopy-3.6.0/flopy/discretization/vertexgrid.py` & `flopy-3.7.0/flopy/discretization/vertexgrid.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/export/longnames.py` & `flopy-3.7.0/flopy/export/longnames.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" Human readable long names for netCDF variables. """
+"""Human readable long names for netCDF variables."""
 
 NC_LONG_NAMES = {
     "botm": "Model layer bottom elevations",
     "crs": "Coordinate reference system",
     "delc": "Model grid cell spacing along a column",
     "delr": "Model grid cell spacing along a row",
     "drn_cond": "Drain package conductance",
```

### Comparing `flopy-3.6.0/flopy/export/metadata.py` & `flopy-3.7.0/flopy/export/metadata.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/export/netcdf.py` & `flopy-3.7.0/flopy/export/netcdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         the item is popped from the keys
 
     """
 
     def __init__(self, filename, echo=False):
         self.items = {}
         self.echo = bool(echo)
-        if filename == True:
+        if filename is True:
             self.echo = True
             self.filename = None
         elif filename:
             self.f = open(filename, "w", 0)  # unbuffered
             self.t = datetime.now()
             self.log(f"opening {filename} for logging")
         else:
@@ -383,18 +383,17 @@
                 new_var = self.create_variable(
                     new_vname, attrs, var.dtype, dimensions=var.dimensions
                 )
                 new_var[:] = var[:]
         else:
             for vname, array in other.items():
                 vname_norm = self.normalize_name(vname)
-                assert (
-                    vname_norm in self.nc.variables.keys()
-                ), f"dict var not in self.vars:{vname}-->" + ",".join(
-                    self.nc.variables.keys()
+                assert vname_norm in self.nc.variables.keys(), (
+                    f"dict var not in self.vars:{vname}-->"
+                    + ",".join(self.nc.variables.keys())
                 )
 
                 new_vname = vname_norm + suffix
                 assert new_vname not in self.nc.variables.keys()
                 attrs = self.var_attr_dict[vname_norm].copy()
                 attrs["max"] = np.nanmax(array)
                 attrs["min"] = np.nanmin(array)
@@ -677,15 +676,15 @@
 
         # Check if using newer pyproj version conventions
         if version.parse(pyproj.__version__) < version.parse("2.2"):
             raise ValueError(
                 "The FloPy NetCDF module requires pyproj >= 2.2.0."
             )
 
-        print(f"initialize_geometry::")
+        print("initialize_geometry::")
 
         self.log(f"model crs: {self.model_crs}")
         print(f"model crs: {self.model_crs}")
 
         vmin, vmax = self.model_grid.botm.min(), self.model_grid.top.max()
         if self.z_positive == "down":
             vmin, vmax = vmax, vmin
```

### Comparing `flopy-3.6.0/flopy/export/shapefile_utils.py` & `flopy-3.7.0/flopy/export/shapefile_utils.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/export/unitsformat.py` & `flopy-3.7.0/flopy/export/unitsformat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" unit format strings for netCDF variables. """
+"""unit format strings for netCDF variables."""
 
 NC_UNITS_FORMAT = {
     "2D_cumulative_well_flux": "{0}^3/{1}",
     "3D_cumulative_well_flux": "{0}^3/{1}",
     "al": "{0}/{0}",
     "botm": "{0}",
     "cell_by_cell_flow": "{0}^3/{1}",
```

### Comparing `flopy-3.6.0/flopy/export/utils.py` & `flopy-3.7.0/flopy/export/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,20 +155,20 @@
 ):
     if logger:
         logger.log(f"creating array for {var_name}")
 
     array = np.zeros(
         (len(times), shape3d[0], shape3d[1], shape3d[2]), dtype=np.float32
     )
-    array[:] = np.NaN
+    array[:] = np.nan
 
     if isinstance(out_obj, ZBNetOutput):
         a = np.asarray(out_obj.zone_array, dtype=np.float32)
         if mask_array3d is not None:
-            a[mask_array3d] = np.NaN
+            a[mask_array3d] = np.nan
         for i, _ in enumerate(times):
             array[i, :, :, :] = a
 
     else:
         for i, t in enumerate(times):
             if t in out_obj.recordarray["totim"]:
                 try:
@@ -183,15 +183,15 @@
                     estr = f"error getting data for {nme} at time {t}:{e!s}"
                     if logger:
                         logger.warn(estr)
                     else:
                         print(estr)
                     continue
                 if mask_array3d is not None and a.shape == mask_array3d.shape:
-                    a[mask_array3d] = np.NaN
+                    a[mask_array3d] = np.nan
                 try:
                     array[i, :, :, :] = a.astype(np.float32)
                 except Exception as e:
                     nme = var_name + text.decode().strip().lower()
                     estr = f"error assigning {nme} data to array for time {t}:{e!s}"
                     if logger:
                         logger.warn(estr)
@@ -199,15 +199,15 @@
                         print(estr)
                     continue
 
     if logger:
         logger.log(f"creating array for {var_name}")
 
     for mask_val in mask_vals:
-        array[np.where(array == mask_val)] = np.NaN
+        array[np.where(array == mask_val)] = np.nan
     mx, mn = np.nanmax(array), np.nanmin(array)
     array[np.isnan(array)] = netcdf.FILLVALUE
 
     if isinstance(nc, dict):
         if text:
             var_name = text.decode().strip().lower()
         nc[var_name] = array
@@ -592,15 +592,15 @@
         file path (".nc" for netcdf or ".shp" for shapefile) or NetCDF object or dictionary
     ml : flopy.modflow.mbase.ModelInterface object
         flopy model object
     fmt : str
         output format flag. 'vtk' will export to vtk
     **kwargs : keyword arguments
         modelgrid: flopy.discretization.Grid
-            user supplied modelgrid object which will supercede the built
+            user supplied modelgrid object which will supersede the built
             in modelgrid object
         crs : pyproj.CRS, int, str, optional if `prjfile` is specified
             Coordinate reference system (CRS) for the model grid
             (must be projected; geographic CRS are not supported).
             The value can be anything accepted by
             :meth:`pyproj.CRS.from_user_input() <pyproj.crs.CRS.from_user_input>`,
             such as an authority string (eg "EPSG:26916") or a WKT string.
@@ -683,17 +683,17 @@
     ----------
     f : str or PathLike or NetCdf or dict
         output file path (extension .shp for shapefile or .nc for netcdf) or NetCDF object or dictionary
     pak : flopy.pakbase.Package object
         package to export
     fmt : str
         output format flag. 'vtk' will export to vtk
-    ** kwargs : keword arguments
+    ** kwargs : keyword arguments
         modelgrid: flopy.discretization.Grid
-            user supplied modelgrid object which will supercede the built
+            user supplied modelgrid object which will supersede the built
             in modelgrid object
         crs : pyproj.CRS, int, str, optional if `prjfile` is specified
             Coordinate reference system (CRS) for the model grid
             (must be projected; geographic CRS are not supported).
             The value can be anything accepted by
             :meth:`pyproj.CRS.from_user_input() <pyproj.crs.CRS.from_user_input>`,
             such as an authority string (eg "EPSG:26916") or a WKT string.
@@ -869,15 +869,15 @@
     Parameters
     -----------
     f : str or PathLike or NetCdf
         file path or existing export instance type (NetCdf only for now)
     mfl : MfList instance
     **kwargs : keyword arguments
         modelgrid : flopy.discretization.Grid
-            model grid instance which will supercede the flopy.model.modelgrid
+            model grid instance which will supersede the flopy.model.modelgrid
         crs : pyproj.CRS, int, str, optional if `prjfile` is specified
             Coordinate reference system (CRS) for the model grid
             (must be projected; geographic CRS are not supported).
             The value can be anything accepted by
             :meth:`pyproj.CRS.from_user_input() <pyproj.crs.CRS.from_user_input>`,
             such as an authority string (eg "EPSG:26916") or a WKT string.
         prjfile : str or pathlike, optional if `crs` is specified
@@ -1030,15 +1030,15 @@
     t2d : Transient2d instance
     fmt : str
         output format flag. 'vtk' will export to vtk
     **kwargs : keyword arguments
         min_valid : minimum valid value
         max_valid : maximum valid value
         modelgrid : flopy.discretization.Grid
-            model grid instance which will supercede the flopy.model.modelgrid
+            model grid instance which will supersede the flopy.model.modelgrid
         if fmt is set to 'vtk', parameters of Vtk initializer
 
     """
 
     if not isinstance(t2d, DataInterface):
         err = (
             "transient2d_helper only helps instances that support "
@@ -1078,32 +1078,32 @@
 
         # f.log("getting 4D array for {0}".format(t2d.name_base))
         array = t2d.array
         # f.log("getting 4D array for {0}".format(t2d.name_base))
         with np.errstate(invalid="ignore"):
             if array.dtype not in [int, np.int32, np.int64]:
                 if mask is not None:
-                    array[:, 0, mask] = np.NaN
-                array[array <= min_valid] = np.NaN
-                array[array >= max_valid] = np.NaN
+                    array[:, 0, mask] = np.nan
+                array[array <= min_valid] = np.nan
+                array[array >= max_valid] = np.nan
                 mx, mn = np.nanmax(array), np.nanmin(array)
             else:
                 mx, mn = np.nanmax(array), np.nanmin(array)
                 array[array <= min_valid] = netcdf.FILLVALUE
                 array[array >= max_valid] = netcdf.FILLVALUE
                 # if t2d.model.bas6 is not None:
                 #    array[:, 0, t2d.model.bas6.ibound.array[0] == 0] = \
                 #        f.fillvalue
                 # elif t2d.model.btn is not None:
                 #    array[:, 0, t2d.model.btn.icbund.array[0] == 0] = \
                 #        f.fillvalue
 
         var_name = t2d.name.replace("_", "")
         if isinstance(f, dict):
-            array[array == netcdf.FILLVALUE] = np.NaN
+            array[array == netcdf.FILLVALUE] = np.nan
             f[var_name] = array
             return f
 
         array[np.isnan(array)] = f.fillvalue
         units = "unitless"
 
         if var_name in NC_UNITS_FORMAT:
@@ -1190,15 +1190,15 @@
     u3d : Util3d instance
     fmt : str
         output format flag. 'vtk' will export to vtk
     **kwargs : keyword arguments
         min_valid : minimum valid value
         max_valid : maximum valid value
         modelgrid : flopy.discretization.Grid
-            model grid instance which will supercede the flopy.model.modelgrid
+            model grid instance which will supersede the flopy.model.modelgrid
         if fmt is set to 'vtk', parameters of Vtk initializer
 
     """
 
     assert isinstance(
         u3d, DataInterface
     ), "array3d_export only helps instances that support DataInterface"
@@ -1239,46 +1239,46 @@
         # f.log("getting 3D array for {0}".format(var_name))
         array = u3d.array
 
         # this is for the crappy vcont in bcf6
         # if isinstance(f,NetCdf) and array.shape != f.shape:
         #     f.log("broadcasting 3D array for {0}".format(var_name))
         #     full_array = np.empty(f.shape)
-        #     full_array[:] = np.NaN
+        #     full_array[:] = np.nan
         #     full_array[:array.shape[0]] = array
         #     array = full_array
         #     f.log("broadcasting 3D array for {0}".format(var_name))
         # f.log("getting 3D array for {0}".format(var_name))
         #
         mask = None
         if modelgrid.idomain is not None and "ibound" not in var_name:
             mask = modelgrid.idomain == 0
 
         if mask is not None and array.shape != mask.shape:
             # f.log("broadcasting 3D array for {0}".format(var_name))
             full_array = np.empty(mask.shape)
-            full_array[:] = np.NaN
+            full_array[:] = np.nan
             full_array[: array.shape[0]] = array
             array = full_array
             # f.log("broadcasting 3D array for {0}".format(var_name))
 
         # runtime warning issued in some cases - need to track down cause
         # happens when NaN is already in array
         with np.errstate(invalid="ignore"):
             if array.dtype not in [int, np.int32, np.int64]:
                 # if u3d.model.modelgrid.bas6 is not None and "ibound" not
                 # in var_name:
                 #    array[u3d.model.modelgrid.bas6.ibound.array == 0] =
-                # np.NaN
+                # np.nan
                 # elif u3d.model.btn is not None and 'icbund' not in var_name:
-                #    array[u3d.model.modelgrid.btn.icbund.array == 0] = np.NaN
+                #    array[u3d.model.modelgrid.btn.icbund.array == 0] = np.nan
                 if mask is not None:
-                    array[mask] = np.NaN
-                array[array <= min_valid] = np.NaN
-                array[array >= max_valid] = np.NaN
+                    array[mask] = np.nan
+                array[array <= min_valid] = np.nan
+                array[array >= max_valid] = np.nan
                 mx, mn = np.nanmax(array), np.nanmin(array)
             else:
                 mx, mn = np.nanmax(array), np.nanmin(array)
                 if mask is not None:
                     array[mask] = netcdf.FILLVALUE
                 array[array <= min_valid] = netcdf.FILLVALUE
                 array[array >= max_valid] = netcdf.FILLVALUE
@@ -1368,15 +1368,15 @@
         output format flag. 'vtk' will export to vtk
     verbose : bool
         whether to print verbose output
     **kwargs : keyword arguments
         min_valid : minimum valid value
         max_valid : maximum valid value
         modelgrid : flopy.discretization.Grid
-            model grid instance which will supercede the flopy.model.modelgrid
+            model grid instance which will supersede the flopy.model.modelgrid
         if fmt is set to 'vtk', parameters of Vtk initializer
 
     """
     assert isinstance(
         u2d, DataInterface
     ), "util2d_helper only helps instances that support DataInterface"
     assert len(u2d.array.shape) == 2, "util2d_helper only supports 2D arrays"
@@ -1417,17 +1417,17 @@
         with np.errstate(invalid="ignore"):
             if array.dtype not in [int, np.int32, np.int64]:
                 if (
                     modelgrid.idomain is not None
                     and "ibound" not in u2d.name.lower()
                     and "idomain" not in u2d.name.lower()
                 ):
-                    array[modelgrid.idomain[0, :, :] == 0] = np.NaN
-                array[array <= min_valid] = np.NaN
-                array[array >= max_valid] = np.NaN
+                    array[modelgrid.idomain[0, :, :] == 0] = np.nan
+                array[array <= min_valid] = np.nan
+                array[array >= max_valid] = np.nan
                 mx, mn = np.nanmax(array), np.nanmin(array)
             else:
                 mx, mn = np.nanmax(array), np.nanmin(array)
                 array[array <= min_valid] = netcdf.FILLVALUE
                 array[array >= max_valid] = netcdf.FILLVALUE
                 if (
                     modelgrid.idomain is not None
@@ -1521,17 +1521,17 @@
 
     Parameters
     ----------
     modelgrid : flopy.discretization.StructuredGrid object
         model grid
     filename : str or PathLike
         Path of output file. Export format is determined by
-        file extention.
+        file extension.
         '.asc'  Arc Ascii grid
-        '.tif'  GeoTIFF (requries rasterio package)
+        '.tif'  GeoTIFF (requires rasterio package)
         '.shp'  Shapefile
     a : 2D numpy.ndarray
         Array to export
     nodata : scalar
         Value to assign to np.nan entries (default -9999)
     fieldname : str
         Attribute field name for array values (shapefile export only).
@@ -1920,15 +1920,15 @@
     Contour an array using matplotlib; write shapefile of contours.
 
     Parameters
     ----------
     modelgrid : flopy.discretization.Grid object
         model grid object
     filename : str or PathLike
-        Path of output file with '.shp' extention.
+        Path of output file with '.shp' extension.
     a : 2D numpy array
         Array to contour
     fieldname : str
         gis field name
     interval : float
         interval to calculate levels from
     levels : list
```

### Comparing `flopy-3.6.0/flopy/export/vtk.py` & `flopy-3.7.0/flopy/export/vtk.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import os
 import warnings
 from pathlib import Path
 from typing import Union
 
 import numpy as np
+import pandas as pd
 
 from ..datbase import DataInterface, DataType
 from ..utils import Util3d, import_optional_dependency
 
 warnings.simplefilter("always", DeprecationWarning)
 
 
@@ -95,19 +96,19 @@
     Parameters
     ----------
     model : flopy.ModelInterface object
         any flopy model object, example flopy.modflow.Modflow() object
     modelgrid : flopy.discretization.Grid object
         any flopy modelgrid object, example. VertexGrid
     vertical_exageration : float
-        floating point value to scale vertical exageration of the vtk points
+        floating point value to scale vertical exaggeration of the vtk points
         default is 1.
     binary : bool
         flag that indicates if Vtk will write a binary or text file. Binary
-        is prefered as paraview has a bug (8/4/2021) where is cannot represent
+        is preferred as paraview has a bug (8/4/2021) where is cannot represent
         NaN values from ASCII (non xml) files. In this case no-data values
         are set to 1e+30.
     xml : bool
         flag to write xml based VTK files
     pvd : bool
         boolean flag to write a paraview pvd file for transient data. This
         file maps vtk files to a model time.
@@ -116,15 +117,15 @@
         is False, as paraview has a bug (8/4/2021) where some polyhedrons will
         not properly close when using shared points. If shared_points is True
         file size will be slightly smaller.
     smooth : bool
         boolean flag to interpolate vertex elevations based on shared cell
         elevations. Default is False.
     point_scalars : bool
-        boolen flag to write interpolated data at each point based "shared
+        boolean flag to write interpolated data at each point based "shared
         vertices".
 
     """
 
     def __init__(
         self,
         model=None,
@@ -179,15 +180,15 @@
 
         nvpl = 0
         for iv in self.iverts:
             nvpl += len(iv)
 
         self.nvpl = nvpl
 
-        # method to accomodate DISU grids, do not use modelgrid.ncpl!
+        # method to accommodate DISU grids, do not use modelgrid.ncpl!
         self.ncpl = len(self.iverts)
         if self.nnodes == len(self.iverts):
             self.nlay = 1
         else:
             self.nlay = self.modelgrid.nlay
 
         self._laycbd = self.modelgrid.laycbd
@@ -516,15 +517,15 @@
         from vtk.util import numpy_support
 
         # check if modflow 6 or modflow 2005
         if hasattr(pkg, "hfb_data"):
             mf6 = False
             hfb_data = pkg.hfb_data
         else:
-            # asssume that there is no transient hfb data for now
+            # assume that there is no transient hfb data for now
             hfb_data = pkg.stress_period_data.array[0]
             mf6 = True
 
         points = []
         faces = []
         array = []
         cnt = 0
@@ -787,15 +788,15 @@
         Returns
         -------
         None
         """
         if self.__transient_output_data:
             raise AssertionError(
                 "Transient arrays cannot be mixed with transient output, "
-                "Please create a seperate vtk object for transient package "
+                "Please create a separate vtk object for transient package "
                 "data"
             )
 
         if not self._vtk_geometry_set:
             self._set_vtk_grid_geometry()
 
         k = list(d.keys())[0]
@@ -1075,66 +1076,125 @@
                 if package.name[0] not in selpaklist:
                     continue
 
             self.add_package(package, masked_values)
 
     def add_pathline_points(self, pathlines, timeseries=False):
         """
-        Method to add Modpath output from a pathline or timeseries file
-        to the grid. Colors will be representative of totim.
+        Method to add particle pathlines to the grid, with points
+        colored by travel-time. Supports MODPATH or MODFLOW6 PRT
+        pathline format, or MODPATH timeseries format.
 
         Parameters
         ----------
-        pathlines : np.recarray or list
-            pathlines accepts a numpy recarray of a particle pathline or
-            a list of numpy reccarrays associated with pathlines
-        timeseries : bool
-            method to plot data as a series of vtk timeseries files for
-            animation or as a single static vtk file. Default is false
-        """
-
-        if isinstance(pathlines, (np.recarray, np.ndarray)):
-            pathlines = [pathlines]
+        pathlines : pd.dataframe, np.recarray or list
+            Particle pathlines, either as a single dataframe or recarray
+            or a list of such, separated by particle ID. If pathlines are
+            not provided separately, the dataframe or recarray must have
+            columns: 'time', 'k' & 'particleid' for MODPATH 3, 5, 6 or 7,
+            and 'irpt', 'iprp', 'imdl', and 'trelease' for MODFLOW 6 PRT,
+            so particle pathlines can be distinguished.
+        timeseries : bool, optional
+            Whether to plot data as a series of vtk timeseries files for
+            animation or as a single static vtk file. Default is false.
+        """
+
+        mpx_fields = ["particleid", "time", "k"]
+        prt_fields = ["imdl", "iprp", "irpt", "trelease", "ilay"]
+
+        if isinstance(pathlines, list):
+            if len(pathlines) == 0:
+                return
+            pathlines = [
+                (
+                    pl.to_records(index=False)
+                    if isinstance(pl, pd.DataFrame)
+                    else pl
+                )
+                for pl in pathlines
+            ]
+            fields = pathlines[0].dtype.names
+            arr_fields = {
+                n: pathlines[0].dtype[n]
+                for n in fields
+                if np.issubdtype(pathlines[0].dtype[n], np.number)
+            }
+            if not (
+                all(k in fields for k in mpx_fields)
+                or all(k in fields for k in prt_fields)
+            ):
+                raise ValueError("Unrecognized pathline dtype")
+        elif isinstance(pathlines, (np.recarray, np.ndarray, pd.DataFrame)):
+            if isinstance(pathlines, pd.DataFrame):
+                pathlines = pathlines.to_records(index=False)
+            fields = pathlines.dtype.names
+            arr_fields = {
+                n: pathlines.dtype[n]
+                for n in fields
+                if np.issubdtype(pathlines.dtype[n], np.number)
+            }
+            if all(k in pathlines.dtype.names for k in mpx_fields):
+                pids = np.unique(pathlines.particleid)
+                pathlines = [
+                    pathlines[pathlines.particleid == pid] for pid in pids
+                ]
+            elif all(k in pathlines.dtype.names for k in prt_fields):
+                pls = []
+                for imdl in np.unique(pathlines.imdl):
+                    for iprp in np.unique(pathlines.iprp):
+                        for irpt in np.unique(pathlines.irpt):
+                            pl = pathlines[
+                                (pathlines.imdl == imdl)
+                                & (pathlines.iprp == iprp)
+                                & (pathlines.irpt == irpt)
+                            ]
+                            pls.extend(
+                                [pl[pl.trelease == t] for t in np.unique(pl.t)]
+                            )
+                pathlines = pls
+            else:
+                raise ValueError("Unrecognized pathline dtype")
+        else:
+            raise ValueError(
+                "Unsupported pathline format, expected array, recarray, dataframe, or list"
+            )
 
-        keys = ["particleid", "time"]
         if not timeseries:
-            arrays = {key: [] for key in keys}
+            arrays = {f: [] for f in arr_fields}
             points = []
             lines = []
             for recarray in pathlines:
                 recarray["z"] *= self.vertical_exageration
                 line = []
                 for rec in recarray:
                     t = tuple(rec[["x", "y", "z"]])
                     line.append(t)
                     points.append(t)
-                    for key in keys:
-                        arrays[key].append(rec[key])
+                    for f in arr_fields:
+                        arrays[f].append(rec[f])
                 lines.append(line)
 
             self._set_particle_track_data(points, lines, arrays)
 
         else:
             self.vtk_pathlines = self.__vtk.vtkUnstructuredGrid()
             timeseries_data = {}
             points = {}
             for recarray in pathlines:
                 recarray["z"] *= self.vertical_exageration
                 for rec in recarray:
                     time = rec["time"]
                     if time not in points:
                         points[time] = [tuple(rec[["x", "y", "z"]])]
-                        t = {key: [] for key in keys}
-                        timeseries_data[time] = t
-
+                        timeseries_data[time] = {f: [] for f in arr_fields}
                     else:
                         points[time].append(tuple(rec[["x", "y", "z"]]))
 
-                    for key in keys:
-                        timeseries_data[time][key].append(rec[key])
+                    for f in arr_fields:
+                        timeseries_data[time][f].append(rec[f])
 
             self.__pathline_transient_data = timeseries_data
             self._pathline_points = points
 
     def add_heads(self, hds, kstpkper=None, masked_values=None):
         """
         Method to add head data to a vtk file
@@ -1149,15 +1209,15 @@
         masked_values : list, None
             list of values to set equal to nan
 
         """
         if not self.__transient_output_data and self.__transient_data:
             raise AssertionError(
                 "Head data cannot be mixed with transient package data, "
-                "Please create a seperate vtk object for transient head data"
+                "Please create a separate vtk object for transient head data"
             )
 
         if kstpkper is None:
             kstpkper = hds.get_kstpkper()
         elif isinstance(kstpkper, (list, tuple)):
             if not isinstance(kstpkper[0], (list, tuple)):
                 kstpkper = [kstpkper]
@@ -1199,15 +1259,15 @@
         masked_values : list, None
             list of values to set equal to nan
 
         """
         if not self.__transient_output_data and self.__transient_data:
             raise AssertionError(
                 "Binary data cannot be mixed with transient package data, "
-                "Please create a seperate vtk object for transient head data"
+                "Please create a separate vtk object for transient head data"
             )
 
         records = cbc.get_unique_record_names(decode=True)
         imeth_dict = {
             record: imeth for (record, imeth) in zip(records, cbc.imethlist)
         }
         if text is None:
@@ -1454,15 +1514,15 @@
                             w.SetFileName(str(tf))
                             w.update()
                             cnt += 1
                 else:
                     w.SetFileName(str(foo))
                     w.Update()
 
-        if not type(self.pvd) == bool:
+        if not isinstance(self.pvd, bool):
             if f.suffix not in (".vtk", ".vtu"):
                 pvdfile = f.parent / f"{f.name}.pvd"
             else:
                 pvdfile = f.with_suffix(".pvd")
 
             self.pvd.write(pvdfile)
```

### Comparing `flopy-3.6.0/flopy/mbase.py` & `flopy-3.7.0/flopy/mbase.py`

 * *Files 0% similar despite different names*

```diff
@@ -1503,15 +1503,15 @@
                     "preserve the precision of the parameter data."
                 )
             self.free_format_input = True
 
         if self.verbose:
             print("\nWriting packages:")
 
-        if SelPackList == False:
+        if SelPackList is False:
             for p in self.packagelist:
                 if self.verbose:
                     print("   Package: ", p.name[0])
                 # prevent individual package checks from running after
                 # model-level package check above
                 # otherwise checks are run twice
                 # or the model level check procedure would have to be split up
@@ -1740,14 +1740,15 @@
     silent=False,
     pause=False,
     report=False,
     processors=None,
     normal_msg="normal termination",
     use_async=False,
     cargs=None,
+    custom_print=None,
 ) -> Tuple[bool, List[str]]:
     """
     Run the model using subprocess.Popen, optionally collecting stdout and printing
     timestamped progress. Model workspace, namefile, executable to use, and several
     other options may be configured, and additional command line arguments may also
     be provided.
 
@@ -1778,32 +1779,42 @@
         (Default is 'normal termination')
     use_async : boolean
         Asynchronously read model stdout and report with timestamps. Good for
         models taking a long time to run, not good for models that run quickly.
     cargs : str or list, optional, default None
         Additional command line arguments to pass to the executable.
         (Default is None)
+    custom_print: callable
+        Optional callable for printing. It will replace the builtin print
+        function. This is useful for a shorter print output or integration into
+        other systems such as GUIs.
+        default is None, i.e. use the builtin print
     Returns
     -------
     success : boolean
     buff : list of lines of stdout (empty if report is False)
 
     """
+    if custom_print is not None:
+        print = custom_print
+    else:
+        print = __builtins__["print"]
+
     success = False
     buff = []
 
     # convert normal_msg to a list of lower case str for comparison
     if isinstance(normal_msg, str):
         normal_msg = [normal_msg]
     for idx, s in enumerate(normal_msg):
         normal_msg[idx] = s.lower()
 
     # make sure executable exists
     if exe_name is None:
-        raise ValueError(f"An executable name or path must be provided")
+        raise ValueError("An executable name or path must be provided")
     exe_path = resolve_exe(exe_name)
     if not silent:
         print(
             f"FloPy is using the following executable to run the model: {flopy_io.relpath_safe(exe_path, model_ws)}"
         )
 
     # make sure namefile exists
```

### Comparing `flopy-3.6.0/flopy/mf6/coordinates/modeldimensions.py` & `flopy-3.7.0/flopy/mf6/coordinates/modeldimensions.py`

 * *Files 0% similar despite different names*

```diff
@@ -397,17 +397,29 @@
             self._model_grid = ModelGrid(
                 self.model_name, self.simulation_data, DiscretizationType.DISV
             )
         elif grid_type == DiscretizationType.DISU:
             self._model_grid = UnstructuredModelGrid(
                 self.model_name, self.simulation_data
             )
-        elif grid_type == DiscretizationType.DISL:
+        elif grid_type == DiscretizationType.DISV1D:
             self._model_grid = ModelGrid(
-                self.model_name, self.simulation_data, DiscretizationType.DISL
+                self.model_name,
+                self.simulation_data,
+                DiscretizationType.DISV1D,
+            )
+        elif grid_type == DiscretizationType.DIS2D:
+            self._model_grid = ModelGrid(
+                self.model_name, self.simulation_data, DiscretizationType.DIS2D
+            )
+        elif grid_type == DiscretizationType.DISV2D:
+            self._model_grid = ModelGrid(
+                self.model_name,
+                self.simulation_data,
+                DiscretizationType.DISV2D,
             )
         else:
             self._model_grid = ModelGrid(
                 self.model_name,
                 self.simulation_data,
                 DiscretizationType.UNDEFINED,
             )
@@ -462,17 +474,15 @@
                             num,
                             shape_rule,
                             consistent_shape,
                         ) = self._resolve_data_item_shape(
                             data_item_struct,
                             path=path,
                             repeating_key=repeating_key,
-                        )[
-                            0
-                        ]
+                        )[0]
                         num_cols = num_cols + num
                         shape_consistent = (
                             shape_consistent and consistent_shape
                         )
                 shape_dimensions = [num_rows, num_cols]
             else:
                 for data_item_struct in structure.data_item_structures:
```

### Comparing `flopy-3.6.0/flopy/mf6/coordinates/modelgrid.py` & `flopy-3.7.0/flopy/mf6/coordinates/modelgrid.py`

 * *Files 4% similar despite different names*

```diff
@@ -270,15 +270,15 @@
         del anglex[to_cellid - 1][reverse_con_number]
 
     def _get_connection_number(self, cellid, reverse_connection=False):
         # init
         jas = self._simulation_data.mfdata[
             (self._model_name, "disu8", "connectiondata", "ja")
         ]
-        if reverse_connection == False:
+        if reverse_connection is False:
             connection_list = jas[self._cellid - 1]
             connecting_cellid = cellid
         else:
             connection_list = jas[cellid - 1]
             connecting_cellid = self._cellid
 
         # search
@@ -448,42 +448,64 @@
                 f"disu{structure.get_version_string()}", 0
             )
             is not None
         ):
             return DiscretizationType.DISU
         elif (
             package_recarray.search_data(
-                f"disl{structure.get_version_string()}", 0
+                f"disv1d{structure.get_version_string()}", 0
             )
             is not None
         ):
-            return DiscretizationType.DISL
-
+            return DiscretizationType.DISV1D
+        elif (
+            package_recarray.search_data(
+                f"dis2d{structure.get_version_string()}", 0
+            )
+            is not None
+        ):
+            return DiscretizationType.DIS2D
+        elif (
+            package_recarray.search_data(
+                f"disv2d{structure.get_version_string()}", 0
+            )
+            is not None
+        ):
+            return DiscretizationType.DISV2D
         return DiscretizationType.UNDEFINED
 
     def get_idomain(self):
         if self._grid_type == DiscretizationType.DIS:
             return self._simulation_data.mfdata[
                 (self._model_name, "dis", "griddata", "idomain")
             ].get_data()
         elif self._grid_type == DiscretizationType.DISV:
             return self._simulation_data.mfdata[
                 (self._model_name, "disv", "griddata", "idomain")
             ].get_data()
-        elif self._grid_type == DiscretizationType.DISL:
+        elif self._grid_type == DiscretizationType.DISV1D:
             return self._simulation_data.mfdata[
-                (self._model_name, "disl", "griddata", "idomain")
+                (self._model_name, "disv1d", "griddata", "idomain")
             ].get_data()
         elif self._grid_type == DiscretizationType.DISU:
             return self._simulation_data.mfdata[
                 (self._model_name, "disu", "griddata", "idomain")
             ].get_data()
+        elif self._grid_type == DiscretizationType.DIS2D:
+            return self._simulation_data.mfdata[
+                (self._model_name, "dis2d", "griddata", "idomain")
+            ].get_data()
+        elif self._grid_type == DiscretizationType.DISV2D:
+            return self._simulation_data.mfdata[
+                (self._model_name, "disv2d", "griddata", "idomain")
+            ].get_data()
         except_str = (
-            "ERROR: Grid type {} for model {} not "
-            "recognized.".format(self._grid_type, self._model_name)
+            "ERROR: Grid type {} for model {} not " "recognized.".format(
+                self._grid_type, self._model_name
+            )
         )
         print(except_str)
         raise MFGridException(except_str)
 
     def grid_type(self):
         if self.freeze_grid:
             return self._grid_type
@@ -507,54 +529,66 @@
 
     def get_horizontal_cross_section_dim_arrays(self):
         if self.grid_type() == DiscretizationType.DIS:
             return [
                 np.arange(1, self.num_rows() + 1, 1, np.int32),
                 np.arange(1, self.num_columns() + 1, 1, np.int32),
             ]
-        elif self.grid_type() == DiscretizationType.DISV:
+        elif (
+            self.grid_type() == DiscretizationType.DISV
+            or self.grid_type() == DiscretizationType.DISV2D
+        ):
             return [np.arange(1, self.num_cells_per_layer() + 1, 1, np.int32)]
         elif (
             self.grid_type() == DiscretizationType.DISU
-            or self.grid_type() == DiscretizationType.DISL
+            or self.grid_type() == DiscretizationType.DISV1D
         ):
             except_str = (
                 "ERROR: Can not get horizontal plane arrays for "
-                'model "{}" grid.  DISU and DISL grids do not '
+                'model "{}" grid.  DISU and DISV1D grids do not '
                 "support individual layers.".format(self._model_name)
             )
             print(except_str)
             raise MFGridException(except_str)
 
     def get_model_dim(self):
         if self.grid_type() == DiscretizationType.DIS:
             return [self.num_layers(), self.num_rows(), self.num_columns()]
+        elif self.grid_type() == DiscretizationType.DIS2D:
+            return [self.num_rows(), self.num_columns()]
         elif self.grid_type() == DiscretizationType.DISV:
             return [self.num_layers(), self.num_cells_per_layer()]
         elif (
             self.grid_type() == DiscretizationType.DISU
-            or self.grid_type() == DiscretizationType.DISL
+            or self.grid_type() == DiscretizationType.DISV1D
+            or self.grid_type() == DiscretizationType.DISV2D
         ):
             return [self.num_cells()]
 
     def get_model_dim_arrays(self):
         if self.grid_type() == DiscretizationType.DIS:
             return [
                 np.arange(1, self.num_layers() + 1, 1, np.int32),
                 np.arange(1, self.num_rows() + 1, 1, np.int32),
                 np.arange(1, self.num_columns() + 1, 1, np.int32),
             ]
+        elif self.grid_type() == DiscretizationType.DIS2D:
+            return [
+                np.arange(1, self.num_rows() + 1, 1, np.int32),
+                np.arange(1, self.num_columns() + 1, 1, np.int32),
+            ]
         elif self.grid_type() == DiscretizationType.DISV:
             return [
                 np.arange(1, self.num_layers() + 1, 1, np.int32),
                 np.arange(1, self.num_cells_per_layer() + 1, 1, np.int32),
             ]
         elif (
             self.grid_type() == DiscretizationType.DISU
-            or self.grid_type() == DiscretizationType.DISL
+            or self.grid_type() == DiscretizationType.DISV1D
+            or self.grid_type() == DiscretizationType.DISV2D
         ):
             return [np.arange(1, self.num_cells() + 1, 1, np.int32)]
 
     def get_row_array(self):
         return np.arange(1, self.num_rows() + 1, 1, np.int32)
 
     def get_column_array(self):
@@ -562,75 +596,94 @@
 
     def get_layer_array(self):
         return np.arange(1, self.num_layers() + 1, 1, np.int32)
 
     def get_horizontal_cross_section_dim_names(self):
         if self.grid_type() == DiscretizationType.DIS:
             return ["row", "column"]
-        elif self.grid_type() == DiscretizationType.DISV:
+        elif (
+            self.grid_type() == DiscretizationType.DISV
+            or self.grid_type() == DiscretizationType.DISV2D
+        ):
             return ["layer_cell_num"]
         elif (
             self.grid_type() == DiscretizationType.DISU
-            or self.grid_type() == DiscretizationType.DISL
+            or self.grid_type() == DiscretizationType.DISV1D
         ):
             except_str = (
                 "ERROR: Can not get layer dimension name for model "
                 '"{}" DISU grid. DISU grids do not support '
                 "layers.".format(self._model_name)
             )
             print(except_str)
             raise MFGridException(except_str)
 
     def get_model_dim_names(self):
         if self.grid_type() == DiscretizationType.DIS:
             return ["layer", "row", "column"]
+        elif self.grid_type() == DiscretizationType.DIS2D:
+            return ["row", "column"]
         elif self.grid_type() == DiscretizationType.DISV:
             return ["layer", "layer_cell_num"]
+        elif self.grid_type() == DiscretizationType.DISV2D:
+            return ["cell_num"]
         elif (
             self.grid_type() == DiscretizationType.DISU
-            or self.grid_type() == DiscretizationType.DISL
+            or self.grid_type() == DiscretizationType.DISV1D
         ):
             return ["node"]
 
     def get_num_spatial_coordinates(self):
         grid_type = self.grid_type()
         if grid_type == DiscretizationType.DIS:
             return 3
+        elif grid_type == DiscretizationType.DIS2D:
+            return 2
         elif grid_type == DiscretizationType.DISV:
             return 2
-        elif (
-            grid_type == DiscretizationType.DISU
-            or grid_type == DiscretizationType.DISL
-        ):
+        elif grid_type == DiscretizationType.DISV2D:
+            return 1
+        elif grid_type == DiscretizationType.DISU:
+            return 1
+        elif grid_type == DiscretizationType.DISV1D:
             return 1
+        return 0
 
     def num_rows(self):
-        if self.grid_type() != DiscretizationType.DIS:
+        if self.grid_type() not in [
+            DiscretizationType.DIS,
+            DiscretizationType.DIS2D,
+        ]:
             except_str = (
                 'ERROR: Model "{}" does not have rows.  Can not '
                 "return number of rows.".format(self._model_name)
             )
             print(except_str)
             raise MFGridException(except_str)
 
+        distype = self.grid_type().name.lower()  # dis or dis2d
         return self._simulation_data.mfdata[
-            (self._model_name, "dis", "dimensions", "nrow")
+            (self._model_name, distype, "dimensions", "nrow")
         ].get_data()
 
     def num_columns(self):
-        if self.grid_type() != DiscretizationType.DIS:
+        if self.grid_type() not in [
+            DiscretizationType.DIS,
+            DiscretizationType.DIS2D,
+        ]:
             except_str = (
                 'ERROR: Model "{}" does not have columns.  Can not '
                 "return number of columns.".format(self._model_name)
             )
             print(except_str)
             raise MFGridException(except_str)
 
+        distype = self.grid_type().name.lower()  # dis or dis2d
         return self._simulation_data.mfdata[
-            (self._model_name, "dis", "dimensions", "ncol")
+            (self._model_name, distype, "dimensions", "ncol")
         ].get_data()
 
     def num_connections(self):
         if self.grid_type() == DiscretizationType.DISU:
             return self._simulation_data.mfdata[
                 (self._model_name, "disu", "dimensions", "nja")
             ].get_data()
@@ -646,14 +699,18 @@
     def num_cells_per_layer(self):
         if self.grid_type() == DiscretizationType.DIS:
             return self.num_rows() * self.num_columns()
         elif self.grid_type() == DiscretizationType.DISV:
             return self._simulation_data.mfdata[
                 (self._model_name, "disv", "dimensions", "ncpl")
             ].get_data()
+        elif self.grid_type() == DiscretizationType.DISV2D:
+            return self._simulation_data.mfdata[
+                (self._model_name, "disv", "dimensions", "nodes")
+            ].get_data()
         elif self.grid_type() == DiscretizationType.DISU:
             return self._simulation_data.mfdata[
                 (self._model_name, "disu", "dimensions", "nodes")
             ].get_data()
 
     def num_layers(self):
         if self.grid_type() == DiscretizationType.DIS:
@@ -662,48 +719,62 @@
             ].get_data()
         elif self.grid_type() == DiscretizationType.DISV:
             return self._simulation_data.mfdata[
                 (self._model_name, "disv", "dimensions", "nlay")
             ].get_data()
         elif (
             self.grid_type() == DiscretizationType.DISU
-            or self.grid_type() == DiscretizationType.DISL
+            or self.grid_type() == DiscretizationType.DISV1D
+            or self.grid_type() == DiscretizationType.DIS2D
+            or self.grid_type() == DiscretizationType.DISV2D
         ):
             return None
 
     def num_cells(self):
         if self.grid_type() == DiscretizationType.DIS:
             return self.num_rows() * self.num_columns() * self.num_layers()
+        elif self.grid_type() == DiscretizationType.DIS2D:
+            return self.num_rows() * self.num_columns()
         elif self.grid_type() == DiscretizationType.DISV:
             return self.num_layers() * self.num_cells_per_layer()
         elif self.grid_type() == DiscretizationType.DISU:
             return self._simulation_data.mfdata[
                 (self._model_name, "disu", "dimensions", "nodes")
             ].get_data()
-        elif self.grid_type() == DiscretizationType.DISL:
+        elif self.grid_type() == DiscretizationType.DISV2D:
+            return self._simulation_data.mfdata[
+                (self._model_name, "disv2d", "dimensions", "nodes")
+            ].get_data()
+        elif self.grid_type() == DiscretizationType.DISV1D:
             return self._simulation_data.mfdata[
-                (self._model_name, "disl", "dimensions", "nodes")
+                (self._model_name, "disv1d", "dimensions", "nodes")
             ].get_data()
 
     def get_all_model_cells(self):
         model_cells = []
         if self.grid_type() == DiscretizationType.DIS:
             for layer in range(0, self.num_layers()):
                 for row in range(0, self.num_rows()):
                     for column in range(0, self.num_columns()):
                         model_cells.append((layer + 1, row + 1, column + 1))
             return model_cells
+        elif self.grid_type() == DiscretizationType.DIS2D:
+            for row in range(0, self.num_rows()):
+                for column in range(0, self.num_columns()):
+                    model_cells.append((layer + 1, row + 1, column + 1))
+            return model_cells
         elif self.grid_type() == DiscretizationType.DISV:
             for layer in range(0, self.num_layers()):
                 for layer_cellid in range(0, self.num_rows()):
                     model_cells.append((layer + 1, layer_cellid + 1))
             return model_cells
         elif (
             self.grid_type() == DiscretizationType.DISU
-            or self.grid_type() == DiscretizationType.DISL
+            or self.grid_type() == DiscretizationType.DISV1D
+            or self.grid_type() == DiscretizationType.DISV2D
         ):
             for node in range(0, self.num_cells()):
                 model_cells.append(node + 1)
             return model_cells
 
 
 class UnstructuredModelGrid(ModelGrid):
```

### Comparing `flopy-3.6.0/flopy/mf6/coordinates/simulationtime.py` & `flopy-3.7.0/flopy/mf6/coordinates/simulationtime.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/common.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/common.dfn`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 
 name print_head
 description keyword to indicate that the list of {#1} {#2} will be printed to the listing file for every stress period in which ``HEAD PRINT'' is specified in Output Control.  If there is no Output Control option and PRINT\_{#3} is specified, then {#2} are printed for the last time step of each stress period.
 
 name print_concentration
 description keyword to indicate that the list of {#1} {#2} will be printed to the listing file for every stress period in which ``CONCENTRATION PRINT'' is specified in Output Control.  If there is no Output Control option and PRINT\_{#3} is specified, then {#2} are printed for the last time step of each stress period.
 
+name print_temperature
+description keyword to indicate that the list of {#1} {#2} will be printed to the listing file for every stress period in which ``TEMPERATURE PRINT'' is specified in Output Control.  If there is no Output Control option and PRINT\_{#3} is specified, then {#2} are printed for the last time step of each stress period.
+
 name print_flows
 description keyword to indicate that the list of {#1} flow rates will be printed to the listing file for every stress period time step in which ``BUDGET PRINT'' is specified in Output Control.  If there is no Output Control option and ``PRINT\_FLOWS'' is specified, then flow rates are printed for the last time step of each stress period.
 
 name save_flows
 description keyword to indicate that {#1} flow terms will be written to the file specified with ``BUDGET FILEOUT'' in Output Control.
 
 name timeseriesfile
```

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/exg-gwfgwf.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/exg-gwfgwf.dfn`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 block options
 name auxiliary
 type string
 shape (naux)
 reader urword
 optional true
 longname keyword to specify aux variables
-description an array of auxiliary variable names.  There is no limit on the number of auxiliary variables that can be provided. Most auxiliary variables will not be used by the GWF-GWF Exchange, but they will be available for use by other parts of the program.  If an auxiliary variable with the name ``ANGLDEGX'' is found, then this information will be used as the angle (provided in degrees) between the connection face normal and the x axis, where a value of zero indicates that a normal vector points directly along the positive x axis.  The connection face normal is a normal vector on the cell face shared between the cell in model 1 and the cell in model 2 pointing away from the model 1 cell.  Additional information on ``ANGLDEGX'' is provided in the description of the DISU Package.  If an auxiliary variable with the name ``CDIST'' is found, then this information will be used as the straight-line connection distance, including the vertical component, between the two cell centers.  Both ANGLDEGX and CDIST are required if specific discharge is calculated for either of the groundwater models.
+description an array of auxiliary variable names.  There is no limit on the number of auxiliary variables that can be provided. Most auxiliary variables will not be used by the GWF-GWF Exchange, but they will be available for use by other parts of the program.  If an auxiliary variable with the name ``ANGLDEGX'' is found, then this information will be used as the angle (provided in degrees) between the connection face normal and the x axis, where a value of zero indicates that a normal vector points directly along the positive x axis.  The connection face normal is a normal vector on the cell face shared between the cell in model 1 and the cell in model 2 pointing away from the model 1 cell.  Additional information on ``ANGLDEGX'' and when it is required is provided in the description of the DISU Package.  If an auxiliary variable with the name ``CDIST'' is found, then this information will be used in the calculation of specific discharge within model cells connected by the exchange.  For a horizontal connection, CDIST should be specified as the horizontal distance between the cell centers, and should not include the vertical component.  For vertical connections, CDIST should be specified as the difference in elevation between the two cell centers.  Both ANGLDEGX and CDIST are required if specific discharge is calculated for either of the groundwater models.
+
 
 block options
 name boundnames
 type keyword
 shape
 reader urword
 optional true
@@ -302,14 +303,15 @@
 in_record true
 tagged false
 shape (naux)
 reader urword
 optional true
 longname auxiliary variables
 description represents the values of the auxiliary variables for each GWFGWF Exchange. The values of auxiliary variables must be present for each exchange. The values must be specified in the order of the auxiliary variables specified in the OPTIONS block.
+mf6internal auxvar
 
 block exchangedata
 name boundname
 type string
 shape
 tagged false
 in_record true
```

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/exg-gwtgwt.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/exg-gwegwe.dfn`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# --------------------- exg gwtgwt options ---------------------
+# --------------------- exg gwegwe options ---------------------
 # flopy multi-package
 
 block options
 name gwfmodelname1
 type string
 reader urword
 optional false
 longname keyword to specify name of first corresponding GWF Model
-description keyword to specify name of first corresponding GWF Model.  In the simulation name file, the GWT6-GWT6 entry contains names for GWT Models (exgmnamea and exgmnameb).  The GWT Model with the name exgmnamea must correspond to the GWF Model with the name gwfmodelname1.
+description keyword to specify name of first corresponding GWF Model.  In the simulation name file, the GWE6-GWE6 entry contains names for GWE Models (exgmnamea and exgmnameb).  The GWE Model with the name exgmnamea must correspond to the GWF Model with the name gwfmodelname1.
 
 block options
 name gwfmodelname2
 type string
 reader urword
 optional false
 longname keyword to specify name of second corresponding GWF Model
-description keyword to specify name of second corresponding GWF Model.  In the simulation name file, the GWT6-GWT6 entry contains names for GWT Models (exgmnamea and exgmnameb).  The GWT Model with the name exgmnameb must correspond to the GWF Model with the name gwfmodelname2.
+description keyword to specify name of second corresponding GWF Model.  In the simulation name file, the GWE6-GWE6 entry contains names for GWE Models (exgmnamea and exgmnameb).  The GWE Model with the name exgmnameb must correspond to the GWF Model with the name gwfmodelname2.
 
 block options
 name auxiliary
 type string
 shape (naux)
 reader urword
 optional true
@@ -29,15 +29,15 @@
 block options
 name boundnames
 type keyword
 shape
 reader urword
 optional true
 longname
-description REPLACE boundnames {'{#1}': 'GWT Exchange'}
+description REPLACE boundnames {'{#1}': 'GWE Exchange'}
 
 block options
 name print_input
 type keyword
 reader urword
 optional true
 longname keyword to print input to list file
@@ -68,24 +68,24 @@
 valid upstream central tvd
 reader urword
 optional true
 longname advective scheme
 description scheme used to solve the advection term.  Can be upstream, central, or TVD.  If not specified, upstream weighting is the default weighting scheme.
 
 block options
-name dsp_xt3d_off
+name cnd_xt3d_off
 type keyword
 shape
 reader urword
 optional true
 longname deactivate xt3d
 description deactivate the xt3d method for the dispersive flux and use the faster and less accurate approximation for this exchange.
 
 block options
-name dsp_xt3d_rhs
+name cnd_xt3d_rhs
 type keyword
 shape
 reader urword
 optional true
 longname xt3d on right-hand side
 description add xt3d dispersion terms to right-hand side, when possible, for this exchange.
 
@@ -97,43 +97,43 @@
 reader urword
 tagged true
 optional false
 longname file keyword
 description keyword to specify that an input filename is expected next.
 
 block options
-name mvt_filerecord
-type record mvt6 filein mvt6_filename
+name mve_filerecord
+type record mve6 filein mve6_filename
 shape
 reader urword
 tagged true
 optional true
 longname
 description
 
 block options
-name mvt6
+name mve6
 type keyword
 shape
 in_record true
 reader urword
 tagged true
 optional false
 longname obs keyword
-description keyword to specify that record corresponds to a transport mover file.
+description keyword to specify that record corresponds to an energy transport mover file.
 
 block options
-name mvt6_filename
+name mve6_filename
 type string
 preserve_case true
 in_record true
 tagged false
 reader urword
 optional false
-longname mvt6 input filename
+longname mve6 input filename
 description is the file name of the transport mover input file to apply to this exchange.  Information for the transport mover are provided in the file provided with these keywords.
 
 block options
 name obs_filerecord
 type record obs6 filein obs6_filename
 shape
 reader urword
@@ -158,37 +158,37 @@
 type string
 preserve_case true
 in_record true
 tagged false
 reader urword
 optional false
 longname obs6 input filename
-description is the file name of the observations input file for this exchange. See the ``Observation utility'' section for instructions for preparing observation input files. Table \ref{table:gwt-obstypetable} lists observation type(s) supported by the GWT-GWT package.
+description is the file name of the observations input file for this exchange. See the ``Observation utility'' section for instructions for preparing observation input files. Table \ref{table:gwe-obstypetable} lists observation type(s) supported by the GWE-GWE package.
 
 block options
 name dev_interfacemodel_on
 type keyword
 reader urword
 optional true
 longname activate interface model on exchange
 description activates the interface model mechanism for calculating the coefficients at (and possibly near) the exchange. This keyword should only be used for development purposes.
 mf6internal dev_ifmod_on
 
-# --------------------- exg gwtgwt dimensions ---------------------
+# --------------------- exg gwegwe dimensions ---------------------
 
 block dimensions
 name nexg
 type integer
 reader urword
 optional false
 longname number of exchanges
-description keyword and integer value specifying the number of GWT-GWT exchanges.
+description keyword and integer value specifying the number of GWE-GWE exchanges.
 
 
-# --------------------- exg gwtgwt exchangedata ---------------------
+# --------------------- exg gwegwe exchangedata ---------------------
 
 block exchangedata
 name exchangedata
 type recarray cellidm1 cellidm2 ihc cl1 cl2 hwva aux boundname
 shape (nexg)
 reader urword
 optional false
@@ -262,19 +262,20 @@
 type double precision
 in_record true
 tagged false
 shape (naux)
 reader urword
 optional true
 longname auxiliary variables
-description represents the values of the auxiliary variables for each GWTGWT Exchange. The values of auxiliary variables must be present for each exchange. The values must be specified in the order of the auxiliary variables specified in the OPTIONS block.
+description represents the values of the auxiliary variables for each GWEGWE Exchange. The values of auxiliary variables must be present for each exchange. The values must be specified in the order of the auxiliary variables specified in the OPTIONS block.
+mf6internal auxvar
 
 block exchangedata
 name boundname
 type string
 shape
 tagged false
 in_record true
 reader urword
 optional true
 longname exchange boundname
-description REPLACE boundname {'{#1}': 'GWT Exchange'}
+description REPLACE boundname {'{#1}': 'GWE Exchange'}
```

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwf-api.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwf-api.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwf-buy.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwf-buy.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwf-chd.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwf-chd.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwf-csub.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwf-csub.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwf-dis.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwe-dis.dfn`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# --------------------- gwf dis options ---------------------
+# --------------------- gwe dis options ---------------------
 
 block options
 name length_units
 type string
 reader urword
 optional true
 longname model length units
@@ -36,16 +36,24 @@
 name angrot
 type double precision
 reader urword
 optional true
 longname rotation angle
 description counter-clockwise rotation angle (in degrees) of the lower-left corner of the model grid.  If not specified, then a default value of 0.0 is assigned.  The value for ANGROT does not affect the model simulation, but it is written to the binary grid file so that postprocessors can locate the grid in space.
 
+block options
+name export_array_ascii
+type keyword
+reader urword
+optional true
+mf6internal export_ascii
+longname export array variables to layered ascii files.
+description keyword that specifies input griddata arrays should be written to layered ascii output files.
 
-# --------------------- gwf dis dimensions ---------------------
+# --------------------- gwe dis dimensions ---------------------
 
 block dimensions
 name nlay
 type integer
 reader urword
 optional false
 longname number of layers
@@ -66,15 +74,15 @@
 type integer
 reader urword
 optional false
 longname number of columns
 description is the number of columns in the model grid.
 default_value 2
 
-# --------------------- gwf dis griddata ---------------------
+# --------------------- gwe dis griddata ---------------------
 
 block griddata
 name delr
 type double precision
 shape (ncol)
 reader readarray
 longname spacing along a row
@@ -113,10 +121,10 @@
 name idomain
 type integer
 shape (ncol, nrow, nlay)
 reader readarray
 layered true
 optional true
 longname idomain existence array
-description is an optional array that characterizes the existence status of a cell.  If the IDOMAIN array is not specified, then all model cells exist within the solution.  If the IDOMAIN value for a cell is 0, the cell does not exist in the simulation.  Input and output values will be read and written for the cell, but internal to the program, the cell is excluded from the solution.  If the IDOMAIN value for a cell is 1 or greater, the cell exists in the simulation.  If the IDOMAIN value for a cell is -1, the cell does not exist in the simulation.  Furthermore, the first existing cell above will be connected to the first existing cell below.  This type of cell is referred to as a ``vertical pass through'' cell.
+description is an optional array that characterizes the existence status of a cell.  If the IDOMAIN array is not specified, then all model cells exist within the solution.  If the IDOMAIN value for a cell is 0, the cell does not exist in the simulation.  Input and output values will be read and written for the cell, but internal to the program, the cell is excluded from the solution.  If the IDOMAIN value for a cell is 1, the cell exists in the simulation.  If the IDOMAIN value for a cell is -1, the cell does not exist in the simulation.  Furthermore, the first existing cell above will be connected to the first existing cell below.  This type of cell is referred to as a ``vertical pass through'' cell.
```

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwf-disu.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwf-disu.dfn`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,23 @@
 reader urword
 optional true
 default_value 0.0
 longname vertical length dimension for top and bottom checking
 description checks are performed to ensure that the top of a cell is not higher than the bottom of an overlying cell.  This option can be used to specify the tolerance that is used for checking.  If top of a cell is above the bottom of an overlying cell by a value less than this tolerance, then the program will not terminate with an error.  The default value is zero.  This option should generally not be used.
 mf6internal voffsettol
 
+block options
+name export_array_ascii
+type keyword
+reader urword
+optional true
+mf6internal export_ascii
+longname export array variables to layered ascii files.
+description keyword that specifies input griddata arrays should be written to layered ascii output files.
+
 # --------------------- gwf disu dimensions ---------------------
 
 block dimensions
 name nodes
 type integer
 reader urword
 optional false
@@ -162,15 +171,15 @@
 block connectiondata
 name angldegx
 type double precision
 optional true
 shape (nja)
 reader readarray
 longname angle of face normal to connection
-description is the angle (in degrees) between the horizontal x-axis and the outward normal to the face between a cell and its connecting cells. The angle varies between zero and 360.0 degrees, where zero degrees points in the positive x-axis direction, and 90 degrees points in the positive y-axis direction.  ANGLDEGX is only needed if horizontal anisotropy is specified in the NPF Package, if the XT3D option is used in the NPF Package, or if the SAVE\_SPECIFIC\_DISCHARGE option is specifed in the NPF Package.  ANGLDEGX does not need to be specified if these conditions are not met.  ANGLDEGX is of size NJA; values specified for vertical connections and for the diagonal position are not used.  Note that ANGLDEGX is read in degrees, which is different from MODFLOW-USG, which reads a similar variable (ANGLEX) in radians.
+description is the angle (in degrees) between the horizontal x-axis and the outward normal to the face between a cell and its connecting cells. The angle varies between zero and 360.0 degrees, where zero degrees points in the positive x-axis direction, and 90 degrees points in the positive y-axis direction.  ANGLDEGX is only needed if horizontal anisotropy is specified in the NPF Package, if the XT3D option is used in the NPF Package, or if the SAVE\_SPECIFIC\_DISCHARGE option is specified in the NPF Package.  ANGLDEGX does not need to be specified if these conditions are not met.  ANGLDEGX is of size NJA; values specified for vertical connections and for the diagonal position are not used.  Note that ANGLDEGX is read in degrees, which is different from MODFLOW-USG, which reads a similar variable (ANGLEX) in radians.
 jagged_array iac
 
 # --------------------- gwf disu vertices ---------------------
 
 block vertices
 name vertices
 type recarray iv xv yv
```

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwf-disv.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwf-disv.dfn`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,23 @@
 name angrot
 type double precision
 reader urword
 optional true
 longname rotation angle
 description counter-clockwise rotation angle (in degrees) of the model grid coordinate system relative to a real-world coordinate system.  If not specified, then a default value of 0.0 is assigned.  The value for ANGROT does not affect the model simulation, but it is written to the binary grid file so that postprocessors can locate the grid in space.
 
+block options
+name export_array_ascii
+type keyword
+reader urword
+optional true
+mf6internal export_ascii
+longname export array variables to layered ascii files.
+description keyword that specifies input griddata arrays should be written to layered ascii output files. 
+
 # --------------------- gwf disv dimensions ---------------------
 
 block dimensions
 name nlay
 type integer
 reader urword
 optional false
```

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwf-drn.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwf-drn.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwf-evt.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwf-evt.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwf-evta.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwf-evta.dfn`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 block options
 name readasarrays
 type keyword
 shape
 reader urword
 optional false
 longname use array-based input
-description indicates that array-based input will be used for the Evapotranspiration Package.  This keyword must be specified to use array-based input.
+description indicates that array-based input will be used for the Evapotranspiration Package.  This keyword must be specified to use array-based input.  When READASARRAYS is specified, values must be provided for every cell within a model layer, even those cells that have an IDOMAIN value less than one.  Values assigned to cells with IDOMAIN values less than one are not used and have no effect on simulation results.
 default_value True
 
 block options
 name fixed_cell
 type keyword
 shape
 reader urword
```

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwf-ghb.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwf-ghb.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwf-gnc.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwf-gnc.dfn`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # --------------------- gwf gnc options ---------------------
 # flopy subpackage gnc_filerecord gnc gncdata gncdata
-# flopy parent_name_type parent_model_or_package
+# flopy parent_name_type parent_model_or_package MFModel/MFPackage
 
 block options
 name print_input
 type keyword
 reader urword
 optional true
 longname print input to listing file
```

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwf-hfb.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwf-hfb.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwf-lak.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwf-lak.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwf-maw.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwf-maw.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwf-mvr.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwf-mvr.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwf-nam.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwf-nam.dfn`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 block packages
 name ftype
 in_record true
 type string
 tagged false
 reader urword
 longname package type
-description is the file type, which must be one of the following character values shown in table~\ref{table:ftype}. Ftype may be entered in any combination of uppercase and lowercase.
+description is the file type, which must be one of the following character values shown in table~\ref{table:ftype-gwf}. Ftype may be entered in any combination of uppercase and lowercase.
 
 block packages
 name fname
 in_record true
 type string
 preserve_case true
 tagged false
```

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwf-npf.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwf-npf.dfn`

 * *Files 4% similar despite different names*

```diff
@@ -220,51 +220,33 @@
 in_record true
 reader urword
 optional false
 tagged false
 longname file name of TVK information
 description defines a time-varying hydraulic conductivity (TVK) input file.  Records in the TVK file can be used to change hydraulic conductivity properties at specified times or stress periods.
 
-# dev options
-
 block options
-name dev_no_newton
+name export_array_ascii
 type keyword
 reader urword
 optional true
-longname turn off Newton for unconfined cells
-description turn off Newton for unconfined cells
-mf6internal inewton
+mf6internal export_ascii
+longname export array variables to layered ascii files.
+description keyword that specifies input griddata arrays should be written to layered ascii output files.
 
-block options
-name dev_modflowusg_upstream_weighted_saturation
-type keyword
-reader urword
-optional true
-longname use MODFLOW-USG upstream-weighted saturation approach
-description use MODFLOW-USG upstream-weighted saturation approach
-mf6internal iusgnrhc
+# dev options
 
 block options
-name dev_modflownwt_upstream_weighting
+name dev_no_newton
 type keyword
 reader urword
 optional true
-longname use MODFLOW-NWT approach for upstream weighting
-description use MODFLOW-NWT approach for upstream weighting
-mf6internal inwtupw
-
-block options
-name dev_minimum_saturated_thickness
-type double precision
-reader urword
-optional true
-longname set minimum allowed saturated thickness
-description set minimum allowed saturated thickness
-mf6internal satmin
+longname turn off Newton for unconfined cells
+description turn off Newton for unconfined cells
+mf6internal inewton
 
 block options
 name dev_omega
 type double precision
 reader urword
 optional true
 longname set saturation omega value
```

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwf-oc.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwf-oc.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwf-rch.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwf-rch.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwf-rcha.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwf-rcha.dfn`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 block options
 name readasarrays
 type keyword
 shape
 reader urword
 optional false
 longname use array-based input
-description indicates that array-based input will be used for the Recharge Package.  This keyword must be specified to use array-based input.
+description indicates that array-based input will be used for the Recharge Package.  This keyword must be specified to use array-based input.  When READASARRAYS is specified, values must be provided for every cell within a model layer, even those cells that have an IDOMAIN value less than one.  Values assigned to cells with IDOMAIN values less than one are not used and have no effect on simulation results. 
 default_value True
 
 block options
 name fixed_cell
 type keyword
 shape
 reader urword
@@ -170,15 +170,15 @@
 block period
 name recharge
 type double precision
 shape (ncol*nrow; ncpl)
 reader readarray
 time_series true
 longname recharge rate
-description is the recharge flux rate ($LT^{-1}$).  This rate is multiplied inside the program by the surface area of the cell to calculate the volumetric recharge rate. The recharge array may be defined by a time-array series (see the "Using Time-Array Series in a Package" section).
+description is the recharge flux rate ($LT^{-1}$).  This rate is multiplied inside the program by the surface area of the cell to calculate the volumetric recharge rate. The recharge array may be defined by a time-array series (see the ``Using Time-Array Series in a Package'' section).
 default_value 1.e-3
 
 block period
 name aux
 type double precision
 shape (ncol*nrow; ncpl)
 reader readarray
```

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwf-riv.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwf-riv.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwf-sfr.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwf-sfr.dfn`

 * *Files 1% similar despite different names*

```diff
@@ -423,16 +423,17 @@
 block packagedata
 name rhk
 type double precision
 shape
 tagged false
 in_record true
 reader urword
-longname
-description real value that defines the hydraulic conductivity of the reach streambed. RHK can be any positive value if the reach is not connected to an underlying GWF cell. Otherwise, RHK must be greater than zero.
+time_series true
+longname reach bed hydraulic conductivity
+description real or character value that defines the hydraulic conductivity of the reach streambed. RHK can be any positive value if the reach is not connected to an underlying GWF cell. Otherwise, RHK must be greater than zero. If the Options block includes a TIMESERIESFILE entry (see the ``Time-Variable Input'' section), values can be obtained from a time series by entering the time-series name in place of a numeric value.
 
 block packagedata
 name man
 type string
 shape
 tagged false
 in_record true
@@ -673,33 +674,44 @@
 reader urword
 longname reach number for this entry
 description integer value that defines the feature (reach) number associated with the specified PERIOD data on the line. IFNO must be greater than zero and less than or equal to NREACHES.
 numeric_index true
 
 block period
 name sfrsetting
-type keystring status manning stage inflow rainfall evaporation runoff diversionrecord upstream_fraction cross_sectionrecord auxiliaryrecord
+type keystring status bedk manning stage inflow rainfall evaporation runoff diversionrecord upstream_fraction cross_sectionrecord auxiliaryrecord
 shape
 tagged false
 in_record true
 reader urword
 longname
-description line of information that is parsed into a keyword and values.  Keyword values that can be used to start the SFRSETTING string include: STATUS, MANNING, STAGE, INFLOW, RAINFALL, EVAPORATION, RUNOFF, DIVERSION, UPSTREAM\_FRACTION, and AUXILIARY.
+description line of information that is parsed into a keyword and values.  Keyword values that can be used to start the SFRSETTING string include: STATUS, BEDK, MANNING, STAGE, INFLOW, RAINFALL, EVAPORATION, RUNOFF, DIVERSION, UPSTREAM\_FRACTION, and AUXILIARY.
 
 block period
 name status
 type string
 shape
 tagged true
 in_record true
 reader urword
 longname well status
 description keyword option to define stream reach status.  STATUS can be ACTIVE, INACTIVE, or SIMPLE. The SIMPLE STATUS option simulates streamflow using a user-specified stage for a reach or a stage set to the top of the reach (depth = 0). In cases where the simulated leakage calculated using the specified stage exceeds the sum of inflows to the reach, the stage is set to the top of the reach and leakage is set equal to the sum of inflows. Upstream fractions should be changed using the UPSTREAM\_FRACTION SFRSETTING if the status for one or more reaches is changed to ACTIVE or INACTIVE. For example, if one of two downstream connections for a reach is inactivated, the upstream fraction for the active and inactive downstream reach should be changed to 1.0 and 0.0, respectively, to ensure that the active reach receives all of the downstream outflow from the upstream reach. By default, STATUS is ACTIVE.
 
 block period
+name bedk
+type string
+shape
+tagged true
+in_record true
+reader urword
+time_series true
+longname reach bed hydraulic conductivity
+description real or character value that defines the hydraulic conductivity of the reach streambed. BEDK can be any positive value if the reach is not connected to an underlying GWF cell. Otherwise, BEDK must be greater than zero. If the Options block includes a TIMESERIESFILE entry (see the ``Time-Variable Input'' section), values can be obtained from a time series by entering the time-series name in place of a numeric value.
+
+block period
 name manning
 type string
 shape
 tagged true
 in_record true
 reader urword
 time_series true
```

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwf-sto.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwf-sto.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwf-uzf.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwf-uzf.dfn`

 * *Files 0% similar despite different names*

```diff
@@ -308,14 +308,15 @@
 
 block options
 name simulate_gwseep
 type keyword
 tagged true
 reader urword
 optional true
+deprecated 6.5.0
 longname activate seepage
 description keyword specifying that groundwater discharge (GWSEEP) to land surface will be simulated. Groundwater discharge is nonzero when groundwater head is greater than land surface.  This option is no longer recommended; a better approach is to use the Drain Package with discharge scaling as a way to handle seepage to land surface.  The Drain Package with discharge scaling is described in Chapter 3 of the Supplemental Technical Information. 
 
 block options
 name unsat_etwc
 type keyword
 tagged true
```

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwf-vsc.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwf-vsc.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwf-wel.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwf-wel.dfn`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 block options
 name auto_flow_reduce
 type double precision
 reader urword
 optional true
 longname cell fractional thickness for reduced pumping
-description keyword and real value that defines the fraction of the cell thickness used as an interval for smoothly adjusting negative pumping rates to 0 in cells with head values less than or equal to the bottom of the cell. Negative pumping rates are adjusted to 0 or a smaller negative value when the head in the cell is equal to or less than the calculated interval above the cell bottom. AUTO\_FLOW\_REDUCE is set to 0.1 if the specified value is less than or equal to zero. By default, negative pumping rates are not reduced during a simulation.
+description keyword and real value that defines the fraction of the cell thickness used as an interval for smoothly adjusting negative pumping rates to 0 in cells with head values less than or equal to the bottom of the cell. Negative pumping rates are adjusted to 0 or a smaller negative value when the head in the cell is equal to or less than the calculated interval above the cell bottom. AUTO\_FLOW\_REDUCE is set to 0.1 if the specified value is less than or equal to zero. By default, negative pumping rates are not reduced during a simulation.  This AUTO\_FLOW\_REDUCE option only applies to wells in model cells that are marked as ``convertible'' (ICELLTYPE /= 0) in the Node Property Flow (NPF) input file. Reduction in flow will not occur for wells in cells marked as confined (ICELLTYPE = 0).
 mf6internal flowred
 
 block options
 name afrcsv_filerecord
 type record auto_flow_reduce_csv fileout afrcsvfile
 shape
 reader urword
```

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwt-api.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwt-api.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwt-cnc.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwt-cnc.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwt-dis.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwf-dis.dfn`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# --------------------- gwt dis options ---------------------
+# --------------------- gwf dis options ---------------------
 
 block options
 name length_units
 type string
 reader urword
 optional true
 longname model length units
@@ -36,16 +36,24 @@
 name angrot
 type double precision
 reader urword
 optional true
 longname rotation angle
 description counter-clockwise rotation angle (in degrees) of the lower-left corner of the model grid.  If not specified, then a default value of 0.0 is assigned.  The value for ANGROT does not affect the model simulation, but it is written to the binary grid file so that postprocessors can locate the grid in space.
 
+block options
+name export_array_ascii
+type keyword
+reader urword
+optional true
+mf6internal export_ascii
+longname export array variables to layered ascii files.
+description keyword that specifies input griddata arrays should be written to layered ascii output files.
 
-# --------------------- gwt dis dimensions ---------------------
+# --------------------- gwf dis dimensions ---------------------
 
 block dimensions
 name nlay
 type integer
 reader urword
 optional false
 longname number of layers
@@ -66,15 +74,15 @@
 type integer
 reader urword
 optional false
 longname number of columns
 description is the number of columns in the model grid.
 default_value 2
 
-# --------------------- gwt dis griddata ---------------------
+# --------------------- gwf dis griddata ---------------------
 
 block griddata
 name delr
 type double precision
 shape (ncol)
 reader readarray
 longname spacing along a row
@@ -113,10 +121,10 @@
 name idomain
 type integer
 shape (ncol, nrow, nlay)
 reader readarray
 layered true
 optional true
 longname idomain existence array
-description is an optional array that characterizes the existence status of a cell.  If the IDOMAIN array is not specified, then all model cells exist within the solution.  If the IDOMAIN value for a cell is 0, the cell does not exist in the simulation.  Input and output values will be read and written for the cell, but internal to the program, the cell is excluded from the solution.  If the IDOMAIN value for a cell is 1, the cell exists in the simulation.  If the IDOMAIN value for a cell is -1, the cell does not exist in the simulation.  Furthermore, the first existing cell above will be connected to the first existing cell below.  This type of cell is referred to as a ``vertical pass through'' cell.
+description is an optional array that characterizes the existence status of a cell.  If the IDOMAIN array is not specified, then all model cells exist within the solution.  If the IDOMAIN value for a cell is 0, the cell does not exist in the simulation.  Input and output values will be read and written for the cell, but internal to the program, the cell is excluded from the solution.  If the IDOMAIN value for a cell is 1 or greater, the cell exists in the simulation.  If the IDOMAIN value for a cell is -1, the cell does not exist in the simulation.  Furthermore, the first existing cell above will be connected to the first existing cell below.  This type of cell is referred to as a ``vertical pass through'' cell.
```

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwt-disu.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwe-disu.dfn`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# --------------------- gwt disu options ---------------------
+# --------------------- gwe disu options ---------------------
 
 block options
 name length_units
 type string
 reader urword
 optional true
 longname model length units
@@ -46,15 +46,24 @@
 reader urword
 optional true
 default_value 0.0
 longname vertical length dimension for top and bottom checking
 description checks are performed to ensure that the top of a cell is not higher than the bottom of an overlying cell.  This option can be used to specify the tolerance that is used for checking.  If top of a cell is above the bottom of an overlying cell by a value less than this tolerance, then the program will not terminate with an error.  The default value is zero.  This option should generally not be used.
 mf6internal voffsettol
 
-# --------------------- gwt disu dimensions ---------------------
+block options
+name export_array_ascii
+type keyword
+reader urword
+optional true
+mf6internal export_ascii
+longname export array variables to layered ascii files.
+description keyword that specifies input griddata arrays should be written to layered ascii output files.
+
+# --------------------- gwe disu dimensions ---------------------
 
 block dimensions
 name nodes
 type integer
 reader urword
 optional false
 longname number of layers
@@ -72,15 +81,15 @@
 name nvert
 type integer
 reader urword
 optional true
 longname number of vertices
 description is the total number of (x, y) vertex pairs used to define the plan-view shape of each cell in the model grid.  If NVERT is not specified or is specified as zero, then the VERTICES and CELL2D blocks below are not read.  NVERT and the accompanying VERTICES and CELL2D blocks should be specified for most simulations.  If the XT3D or SAVE\_SPECIFIC\_DISCHARGE options are specified in the NPF Package, then this information is required.
 
-# --------------------- gwt disu griddata ---------------------
+# --------------------- gwe disu griddata ---------------------
 
 block griddata
 name top
 type double precision
 shape (nodes)
 reader readarray
 longname cell top elevation
@@ -108,15 +117,15 @@
 shape (nodes)
 reader readarray
 layered false
 optional true
 longname idomain existence array
 description is an optional array that characterizes the existence status of a cell.  If the IDOMAIN array is not specified, then all model cells exist within the solution.  If the IDOMAIN value for a cell is 0, the cell does not exist in the simulation.  Input and output values will be read and written for the cell, but internal to the program, the cell is excluded from the solution.  If the IDOMAIN value for a cell is 1 or greater, the cell exists in the simulation.  IDOMAIN values of -1 cannot be specified for the DISU Package.
 
-# --------------------- gwt disu connectiondata ---------------------
+# --------------------- gwe disu connectiondata ---------------------
 
 block connectiondata
 name iac
 type integer
 shape (nodes)
 reader readarray
 longname number of cell connections
@@ -124,15 +133,15 @@
 
 block connectiondata
 name ja
 type integer
 shape (nja)
 reader readarray
 longname grid connectivity
-description is a list of cell number (n) followed by its connecting cell numbers (m) for each of the m cells connected to cell n. The number of values to provide for cell n is IAC(n).  This list is sequentially provided for the first to the last cell. The first value in the list must be cell n itself, and the remaining cells must be listed in an increasing order (sorted from lowest number to highest).  Note that the cell and its connections are only supplied for the GWT cells and their connections to the other GWT cells.  Also note that the JA list input may be divided such that every node and its connectivity list can be on a separate line for ease in readability of the file. To further ease readability of the file, the node number of the cell whose connectivity is subsequently listed, may be expressed as a negative number, the sign of which is subsequently converted to positive by the code.
+description is a list of cell number (n) followed by its connecting cell numbers (m) for each of the m cells connected to cell n. The number of values to provide for cell n is IAC(n).  This list is sequentially provided for the first to the last cell. The first value in the list must be cell n itself, and the remaining cells must be listed in an increasing order (sorted from lowest number to highest).  Note that the cell and its connections are only supplied for the GWE cells and their connections to the other GWE cells.  Also note that the JA list input may be divided such that every node and its connectivity list can be on a separate line for ease in readability of the file. To further ease readability of the file, the node number of the cell whose connectivity is subsequently listed, may be expressed as a negative number, the sign of which is subsequently converted to positive by the code.
 numeric_index true
 jagged_array iac
 
 block connectiondata
 name ihc
 type integer
 shape (nja)
@@ -162,25 +171,25 @@
 block connectiondata
 name angldegx
 type double precision
 optional true
 shape (nja)
 reader readarray
 longname angle of face normal to connection
-description is the angle (in degrees) between the horizontal x-axis and the outward normal to the face between a cell and its connecting cells. The angle varies between zero and 360.0 degrees, where zero degrees points in the positive x-axis direction, and 90 degrees points in the positive y-axis direction.  ANGLDEGX is only needed if horizontal anisotropy is specified in the NPF Package, if the XT3D option is used in the NPF Package, or if the SAVE\_SPECIFIC\_DISCHARGE option is specifed in the NPF Package.  ANGLDEGX does not need to be specified if these conditions are not met.  ANGLDEGX is of size NJA; values specified for vertical connections and for the diagonal position are not used.  Note that ANGLDEGX is read in degrees, which is different from MODFLOW-USG, which reads a similar variable (ANGLEX) in radians.
+description is the angle (in degrees) between the horizontal x-axis and the outward normal to the face between a cell and its connecting cells. The angle varies between zero and 360.0 degrees, where zero degrees points in the positive x-axis direction, and 90 degrees points in the positive y-axis direction.  ANGLDEGX is only needed if horizontal anisotropy is specified in the NPF Package, if the XT3D option is used in the NPF Package, or if the SAVE\_SPECIFIC\_DISCHARGE option is specified in the NPF Package.  ANGLDEGX does not need to be specified if these conditions are not met.  ANGLDEGX is of size NJA; values specified for vertical connections and for the diagonal position are not used.  Note that ANGLDEGX is read in degrees, which is different from MODFLOW-USG, which reads a similar variable (ANGLEX) in radians.
 jagged_array iac
 
-# --------------------- gwt disu vertices ---------------------
+# --------------------- gwe disu vertices ---------------------
 
 block vertices
 name vertices
 type recarray iv xv yv
 shape (nvert)
 reader urword
-optional true
+optional false
 longname vertices data
 description
 
 block vertices
 name iv
 type integer
 in_record true
@@ -208,22 +217,22 @@
 tagged false
 reader urword
 optional false
 longname y-coordinate for vertex
 description is the y-coordinate for the vertex.
 
 
-# --------------------- gwt disu cell2d ---------------------
+# --------------------- gwe disu cell2d ---------------------
 
 block cell2d
 name cell2d
 type recarray icell2d xc yc ncvert icvert
 shape (nodes)
 reader urword
-optional true
+optional false
 longname cell2d data
 description
 
 block cell2d
 name icell2d
 type integer
 in_record true
```

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwt-disv.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwt-disv.dfn`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,23 @@
 name angrot
 type double precision
 reader urword
 optional true
 longname rotation angle
 description counter-clockwise rotation angle (in degrees) of the model grid coordinate system relative to a real-world coordinate system.  If not specified, then a default value of 0.0 is assigned.  The value for ANGROT does not affect the model simulation, but it is written to the binary grid file so that postprocessors can locate the grid in space.
 
+block options
+name export_array_ascii
+type keyword
+reader urword
+optional true
+mf6internal export_ascii
+longname export array variables to layered ascii files.
+description keyword that specifies input griddata arrays should be written to layered ascii output files.
+
 # --------------------- gwt disv dimensions ---------------------
 
 block dimensions
 name nlay
 type integer
 reader urword
 optional false
```

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwt-dsp.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwt-dsp.dfn`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,23 @@
 type keyword
 shape
 reader urword
 optional true
 longname xt3d on right-hand side
 description add xt3d terms to right-hand side, when possible.  This option uses less memory, but may require more iterations.
 
+block options
+name export_array_ascii
+type keyword
+reader urword
+optional true
+mf6internal export_ascii
+longname export array variables to layered ascii files.
+description keyword that specifies input griddata arrays should be written to layered ascii output files.
+
 # --------------------- gwt dsp griddata ---------------------
 
 block griddata
 name diffc
 type double precision
 shape (nodes)
 reader readarray
```

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwt-fmi.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwt-fmi.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwt-ist.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwt-ist.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwt-lkt.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwt-lkt.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwt-mst.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwt-mst.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwt-mvt.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwt-mvt.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwt-mwt.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwt-mwt.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwt-nam.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwe-nam.dfn`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# --------------------- gwt nam options ---------------------
+# --------------------- gwe nam options ---------------------
 
 block options
 name list
 type string
 reader urword
 optional true
 preserve_case true
 longname name of listing file
-description is name of the listing file to create for this GWT model.  If not specified, then the name of the list file will be the basename of the GWT model name file and the '.lst' extension.  For example, if the GWT name file is called ``my.model.nam'' then the list file will be called ``my.model.lst''.
+description is name of the listing file to create for this GWE model.  If not specified, then the name of the list file will be the basename of the GWE model name file and the ``.lst'' extension.  For example, if the GWE name file is called ``my.model.nam'' then the list file will be called ``my.model.lst''.
 
 block options
 name print_input
 type keyword
 reader urword
 optional true
 longname print input to listing file
@@ -29,15 +29,15 @@
 name save_flows
 type keyword
 reader urword
 optional true
 longname save flows for all packages to budget file
 description REPLACE save_flows {'{#1}': 'all model package'}
 
-# --------------------- gwt nam packages ---------------------
+# --------------------- gwe nam packages ---------------------
 
 block packages
 name packages
 type recarray ftype fname pname
 reader urword
 optional false
 longname package list
@@ -46,15 +46,15 @@
 block packages
 name ftype
 in_record true
 type string
 tagged false
 reader urword
 longname package type
-description is the file type, which must be one of the following character values shown in table~\ref{table:ftype}. Ftype may be entered in any combination of uppercase and lowercase.
+description is the file type, which must be one of the following character values shown in table~\ref{table:ftype-gwe}. Ftype may be entered in any combination of uppercase and lowercase.
 
 block packages
 name fname
 in_record true
 type string
 preserve_case true
 tagged false
@@ -66,9 +66,9 @@
 name pname
 in_record true
 type string
 tagged false
 reader urword
 optional true
 longname user name for package
-description is the user-defined name for the package. PNAME is restricted to 16 characters.  No spaces are allowed in PNAME.  PNAME character values are read and stored by the program for stress packages only.  These names may be useful for labeling purposes when multiple stress packages of the same type are located within a single GWT Model.  If PNAME is specified for a stress package, then PNAME will be used in the flow budget table in the listing file; it will also be used for the text entry in the cell-by-cell budget file.  PNAME is case insensitive and is stored in all upper case letters.
+description is the user-defined name for the package. PNAME is restricted to 16 characters.  No spaces are allowed in PNAME.  PNAME character values are read and stored by the program for stress packages only.  These names may be useful for labeling purposes when multiple stress packages of the same type are located within a single GWE Model.  If PNAME is specified for a stress package, then PNAME will be used in the flow budget table in the listing file; it will also be used for the text entry in the cell-by-cell budget file.  PNAME is case insensitive and is stored in all upper case letters.
```

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwt-oc.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwt-oc.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwt-sft.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwt-sft.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwt-src.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwt-src.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwt-ssm.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwt-ssm.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/gwt-uzt.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/gwt-uzt.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/sim-nam.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/sim-nam.dfn`

 * *Files 10% similar despite different names*

```diff
@@ -37,14 +37,58 @@
 name print_input
 type keyword
 reader urword
 optional true
 longname print input to listing file
 description keyword to activate printing of simulation input summaries to the simulation list file (mfsim.lst). With this keyword, input summaries will be written for those packages that support newer input data model routines.  Not all packages are supported yet by the newer input data model routines.
 
+block options
+name hpc_filerecord
+type record hpc6 filein hpc6_filename
+shape
+reader urword
+tagged true
+optional true
+longname
+description hpc record
+
+block options
+name hpc6
+type keyword
+shape
+in_record true
+reader urword
+tagged true
+optional false
+longname head keyword
+description keyword to specify that record corresponds to a hpc file.
+
+block options
+name filein
+type keyword
+shape
+in_record true
+reader urword
+tagged true
+optional false
+longname file keyword
+description keyword to specify that an input filename is expected next.
+
+block options
+name hpc6_filename
+type string
+preserve_case true
+in_record true
+reader urword
+optional false
+tagged false
+longname file name of time series information
+description name of input file to define HPC file settings for the HPC package. See the ``HPC File'' section for instructions for preparing HPC input files.
+
+
 # --------------------- sim nam timing ---------------------
 
 block timing
 name tdis6
 preserve_case true
 type string
 reader urword
@@ -167,20 +211,20 @@
 reader urword
 longname solution type and models in the solution
 description is the list of solution types and models in the solution.
 
 block solutiongroup
 name slntype
 type string
-valid ims6
+valid ims6 ems6
 in_record true
 tagged false
 reader urword
 longname type of solution
-description is the type of solution.  The Integrated Model Solution (IMS6) is the only supported option in this version.
+description is the type of solution.  The Integrated Model Solution (IMS6) and Explicit Model Solution (EMS6) are the only supported options in this version.
 
 block solutiongroup
 name slnfname
 type string
 preserve_case true
 in_record true
 tagged false
```

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/sim-tdis.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/sim-tdis.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/sln-ims.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/sln-ims.dfn`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
 
 block nonlinear
 name outer_rclosebnd
 type double precision
 reader urword
 optional true
 deprecated 6.1.1
-description real value defining the residual tolerance for convergence of model packages that solve a separate equation not solved by the IMS linear solver. This value represents the maximum allowable residual between successive outer iterations at any single model package element. An example of a model package that would use OUTER\_RCLOSEBND to evaluate convergence is the SFR package which solves a continuity equation for each reach.  The OUTER\_RCLOSEBND option is deprecated and has no effect on simulation results as of version 6.1.1.  The keyword, OUTER\_RCLOSEBND can be still be specified for backward compatibility with previous versions of MODFLOW 6 but eventually specificiation of OUTER\_RCLOSEBND will cause MODFLOW 6 to terminate with an error.
+description real value defining the residual tolerance for convergence of model packages that solve a separate equation not solved by the IMS linear solver. This value represents the maximum allowable residual between successive outer iterations at any single model package element. An example of a model package that would use OUTER\_RCLOSEBND to evaluate convergence is the SFR package which solves a continuity equation for each reach.  The OUTER\_RCLOSEBND option is deprecated and has no effect on simulation results as of version 6.1.1.  The keyword, OUTER\_RCLOSEBND can be still be specified for backward compatibility with previous versions of MODFLOW 6 but eventually specification of OUTER\_RCLOSEBND will cause MODFLOW 6 to terminate with an error.
 longname boundary package flow residual tolerance
 
 block nonlinear
 name outer_maximum
 type integer
 reader urword
 optional false
```

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/utl-ats.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/utl-ats.dfn`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 name dtadj
 type double precision
 in_record true
 tagged false
 reader urword
 optional false
 longname time step multiplier factor
-description is the time step multiplier factor for this period.  If the number of outer solver iterations are less than the product of the maximum number of outer iterations (OUTER\_MAXIMUM) and ATS\_OUTER\_MAXIMUM\_FRACTION (an optional variable in the IMS input file with a default value of 1/3), then the time step length is multipled by dtadj.  If the number of outer solver iterations are greater than the product of the maximum number of outer iterations and ATS\_OUTER\_MAXIMUM\_FRACTION, then the time step length is divided by dtadj.  dtadj must be zero, one, or greater than one.  If dtadj is zero or one, then it has no effect on the simulation.  A value between 2.0 and 5.0 can be used as an initial estimate.
+description is the time step multiplier factor for this period.  If the number of outer solver iterations are less than the product of the maximum number of outer iterations (OUTER\_MAXIMUM) and ATS\_OUTER\_MAXIMUM\_FRACTION (an optional variable in the IMS input file with a default value of 1/3), then the time step length is multiplied by dtadj.  If the number of outer solver iterations are greater than the product of the maximum number of outer iterations and ATS\_OUTER\_MAXIMUM\_FRACTION, then the time step length is divided by dtadj.  dtadj must be zero, one, or greater than one.  If dtadj is zero or one, then it has no effect on the simulation.  A value between 2.0 and 5.0 can be used as an initial estimate.
 
 block perioddata
 name dtfailadj
 type double precision
 in_record true
 tagged false
 reader urword
```

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/utl-laktab.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/utl-laktab.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/utl-obs.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/utl-obs.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/utl-sfrtab.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/utl-sfrtab.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/utl-spc.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/utl-spc.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/utl-spca.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/utl-spca.dfn`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 block options
 name readasarrays
 type keyword
 shape
 reader urword
 optional false
 longname use array-based input
-description indicates that array-based input will be used for the SPC Package.  This keyword must be specified to use array-based input.
+description indicates that array-based input will be used for the SPC Package.  This keyword must be specified to use array-based input.  When READASARRAYS is specified, values must be provided for every cell within a model layer, even those cells that have an IDOMAIN value less than one.  Values assigned to cells with IDOMAIN values less than one are not used and have no effect on simulation results.
 default_value True
 
 block options
 name print_input
 type keyword
 reader urword
 optional true
```

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/utl-tas.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/utl-tas.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/utl-ts.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/utl-ts.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/utl-tvk.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/utl-tvk.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/dfn/utl-tvs.dfn` & `flopy-3.7.0/flopy/mf6/data/dfn/utl-tvs.dfn`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/data/mfdata.py` & `flopy-3.7.0/flopy/mf6/data/mfdata.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,15 +156,15 @@
         for key in self._data_storage.keys():
             key_dict[key] = True
         return key_dict
 
     def _verify_sp(self, sp_num):
         if self._path[0].lower() == "nam":
             return True
-        if not ("tdis", "dimensions", "nper") in self._simulation_data.mfdata:
+        if ("tdis", "dimensions", "nper") not in self._simulation_data.mfdata:
             raise FlopyException(
                 "Could not find number of stress periods (nper)."
             )
         nper = self._simulation_data.mfdata[("tdis", "dimensions", "nper")]
         if not (sp_num <= nper.get_data()):
             if (
                 self._simulation_data.verbosity_level.value
@@ -265,18 +265,34 @@
         sim_data.mfdata[self._path] = self
         # set up model grid caching
         self._cache_next_grid = False
         self._grid_cached = False
         self._cached_model_grid = None
 
     def __repr__(self):
-        return repr(self._get_storage_obj())
+        if isinstance(self._data_storage, dict):
+            stor_size = len(self._data_storage)
+        else:
+            stor_size = 1
+        if stor_size <= 1:
+            return repr(self._get_storage_obj(first_record=True))
+        else:
+            rpr = repr(self._get_storage_obj(first_record=True))
+            return f"{rpr}...\nand {stor_size - 1} additional data blocks"
 
     def __str__(self):
-        return str(self._get_storage_obj())
+        if isinstance(self._data_storage, dict):
+            stor_size = len(self._data_storage)
+        else:
+            stor_size = 1
+        if stor_size <= 1:
+            return str(self._get_storage_obj(first_record=True))
+        else:
+            st = str(self._get_storage_obj(first_record=True))
+            return f"{st}...\nand {stor_size - 1} additional data blocks"
 
     @property
     def path(self):
         return self._path
 
     @property
     def array(self):
@@ -527,15 +543,15 @@
         return f"{sim_data.indent_string.join(const_format)}{suffix}"
 
     def _get_aux_var_name(self, aux_var_index):
         aux_var_names = self.data_dimensions.package_dim.get_aux_variables()
         # TODO: Verify that this works for multi-dimensional layering
         return aux_var_names[0][aux_var_index[0] + 1]
 
-    def _get_storage_obj(self):
+    def _get_storage_obj(self, first_record=False):
         return self._data_storage
 
 
 class MFMultiDimVar(MFData):
     def __init__(
         self,
         sim_data,
```

### Comparing `flopy-3.6.0/flopy/mf6/data/mfdataarray.py` & `flopy-3.7.0/flopy/mf6/data/mfdataarray.py`

 * *Files 2% similar despite different names*

```diff
@@ -383,16 +383,17 @@
             if (
                 self.data_dimensions.get_model_grid().grid_type()
                 == DiscretizationType.DISU
             ):
                 comment = f"Layered option not available for unstructured grid. {self._path}"
             else:
                 comment = (
-                    'Data "{}" does not support layered option. '
-                    "{}".format(self._data_name, self._path)
+                    'Data "{}" does not support layered option. ' "{}".format(
+                        self._data_name, self._path
+                    )
                 )
             type_, value_, traceback_ = sys.exc_info()
             raise MFDataException(
                 self.structure.get_model(),
                 self.structure.get_package(),
                 self._path,
                 "setting layered data",
@@ -432,16 +433,17 @@
             if (
                 self.data_dimensions.get_model_grid().grid_type()
                 == DiscretizationType.DISU
             ):
                 comment = f"Layered option not available for unstructured grid. {self._path}"
             else:
                 comment = (
-                    'Data "{}" does not support layered option. '
-                    "{}".format(self._data_name, self._path)
+                    'Data "{}" does not support layered option. ' "{}".format(
+                        self._data_name, self._path
+                    )
                 )
             type_, value_, traceback_ = sys.exc_info()
             raise MFDataException(
                 self.structure.get_model(),
                 self.structure.get_package(),
                 self._path,
                 "converting data to layered",
@@ -540,16 +542,15 @@
             try:
                 # store layer's data in external file
                 if (
                     self._simulation_data.verbosity_level.value
                     >= VerbosityLevel.verbose.value
                 ):
                     print(
-                        "Storing {} layer {} to external file {}.."
-                        ".".format(
+                        "Storing {} layer {} to external file {}.." ".".format(
                             self.structure.name,
                             current_layer[0] + 1,
                             file_path,
                         )
                     )
                 factor = storage.layer_storage[current_layer].factor
                 external_data = {
@@ -630,16 +631,15 @@
             try:
                 # store layer's data internally
                 if (
                     self._simulation_data.verbosity_level.value
                     >= VerbosityLevel.verbose.value
                 ):
                     print(
-                        "Storing {} layer {} internally.."
-                        ".".format(
+                        "Storing {} layer {} internally.." ".".format(
                             self.structure.name,
                             current_layer[0] + 1,
                         )
                     )
                 factor = storage.layer_storage[current_layer].factor
                 internal_data = {
                     current_layer[0]: {
@@ -848,15 +848,15 @@
         if isinstance(data_record, dict):
             first_key = list(data_record.keys())[0]
             if isinstance(first_key, int):
                 for layer, record in data_record.items():
                     self._set_data(record, layer=layer, preserve_record=False)
             else:
                 self._set_data(data_record, preserve_record=False)
-        elif type(data_record) == list:
+        elif isinstance(data_record, list):
             for layer, record in enumerate(data_record):
                 self._set_data(record, layer=layer, preserve_record=False)
         else:
             message = (
                 "Unable to set record.  The contents of data_record must be"
                 "a dictionary or a list."
             )
@@ -1213,16 +1213,17 @@
             if layer is None:
                 layer_min = shape_ml.first_index()
                 layer_max = copy.deepcopy(self._layer_shape)
             else:
                 # set layer range
                 if not shape_ml.in_shape(layer):
                     comment = (
-                        'Layer {} for variable "{}" does not exist'
-                        ".".format(layer, self._data_name)
+                        'Layer {} for variable "{}" does not exist' ".".format(
+                            layer, self._data_name
+                        )
                     )
                     type_, value_, traceback_ = sys.exc_info()
                     raise MFDataException(
                         self.structure.get_model(),
                         self.structure.get_package(),
                         self._path,
                         "getting file entry",
@@ -1289,15 +1290,15 @@
                 self._get_file_entry,
                 DataStorageType.internal_array,
                 DataStructureType.ndarray,
                 stress_period=stress_period,
                 data_path=self._path,
             )
 
-    def _get_storage_obj(self):
+    def _get_storage_obj(self, first_record=False):
         return self._data_storage
 
     def _set_storage_obj(self, storage):
         self._data_storage = storage
 
     def _get_file_entry_layer(
         self,
@@ -1783,14 +1784,17 @@
 
     def has_data(self, layer=None):
         if layer is None:
             for sto_key in self._data_storage.keys():
                 self.get_data_prep(sto_key)
                 if super().has_data():
                     return True
+            for val in self.empty_keys.values():
+                if val:
+                    return True
             return False
         else:
             self.get_data_prep(layer)
             return super().has_data()
 
     def get_record(self, key=None):
         """Returns the data record (data and metadata) associated with stress
@@ -1913,15 +1917,19 @@
             # each item in the dictionary is a list for one stress period
             # the dictionary key is the stress period the list is for
             del_keys = []
             for key, list_item in data.items():
                 if list_item is None:
                     self.remove_transient_key(key)
                     del_keys.append(key)
+                    self.empty_keys[key] = False
+                elif isinstance(list_item, list) and len(list_item) == 0:
+                    self.empty_keys[key] = True
                 else:
+                    self.empty_keys[key] = False
                     self._set_data_prep(list_item, key)
                     if is_record:
                         super().set_record(list_item)
                     else:
                         super().set_data(list_item, multiplier, layer)
             for key in del_keys:
                 del data[key]
@@ -1935,15 +1943,19 @@
                     and len(data) > new_key_index
                 ):
                     key = data[new_key_index]
                 else:
                     key = 0
             if data is None:
                 self.remove_transient_key(key)
+            elif isinstance(data, list) and len(data) == 0:
+                # add empty record
+                self.empty_keys[key] = True
             else:
+                self.empty_keys[key] = False
                 self._set_data_prep(data, key)
                 super().set_data(data, multiplier, layer)
 
     def get_file_entry(
         self, key=0, ext_file_action=ExtFileAction.copy_relative_paths
     ):
         """Returns a string containing the data in stress period "key".
@@ -1957,14 +1969,16 @@
 
         Returns
         -------
             file entry : str
 
         """
 
+        if key in self.empty_keys and self.empty_keys[key]:
+            return ""
         self._get_file_entry_prep(key)
         return super().get_file_entry(ext_file_action=ext_file_action)
 
     def load(
         self,
         first_line,
         file_handle,
@@ -2016,15 +2030,19 @@
             )
         else:
             return {}
 
     def _set_storage_obj(self, storage):
         self._data_storage[self._current_key] = storage
 
-    def _get_storage_obj(self):
+    def _get_storage_obj(self, first_record=False):
+        if first_record and isinstance(self._data_storage, dict):
+            for value in self._data_storage.values():
+                return value
+            return None
         if (
             self._current_key is None
             or self._current_key not in self._data_storage
         ):
             return None
         return self._data_storage[self._current_key]
```

### Comparing `flopy-3.6.0/flopy/mf6/data/mfdatalist.py` & `flopy-3.7.0/flopy/mf6/data/mfdatalist.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 
         Parameters
         ----------
         kper : int
             MODFLOW zero-based stress period number to return. (default is
             zero)
         mask : bool
-            return array with np.NaN instead of zero
+            return array with np.nan instead of zero
 
         Returns
         ----------
         out : dict of numpy.ndarrays
             Dictionary of 3-D numpy arrays containing the stress period data
             for a selected stress period. The dictionary keys are the
             MFDataList dtype names for the stress period data."""
@@ -217,16 +217,17 @@
                 # if not empty dataset
                 if data is not None:
                     if (
                         self._simulation_data.verbosity_level.value
                         >= VerbosityLevel.verbose.value
                     ):
                         print(
-                            "Storing {} to external file {}.."
-                            ".".format(self.structure.name, external_file_path)
+                            "Storing {} to external file {}.." ".".format(
+                                self.structure.name, external_file_path
+                            )
                         )
                     external_data = {
                         "filename": external_file_path,
                         "data": data,
                         "binary": binary,
                     }
                     self._set_data(external_data, check_data=check_data)
@@ -708,15 +709,15 @@
                 search_term = search_term.lower()
                 for row in data:
                     col_num = 0
                     for val in row:
                         if (
                             val is not None
                             and val.lower() == search_term
-                            and (col == None or col == col_num)
+                            and (col is None or col == col_num)
                         ):
                             return (row, col)
                         col_num += 1
             return None
         except Exception as ex:
             type_, value_, traceback_ = sys.exc_info()
             if col is None:
@@ -973,15 +974,15 @@
                     not data_item.optional
                     or data_item.name_length < 5
                     or not data_item.is_mname
                     or not storage.in_model
                 ):
                     data_complete_len = len(data_line)
                     if data_complete_len <= index:
-                        if data_item.optional == False:
+                        if data_item.optional is False:
                             message = (
                                 "Not enough data provided "
                                 "for {}. Data for required data "
                                 'item "{}" not '
                                 "found (data path: {})"
                                 ".".format(
                                     self.structure.name,
@@ -1387,15 +1388,15 @@
             self._get_file_entry,
             DataStorageType.internal_array,
             DataStructureType.recarray,
             stress_period=stress_period,
             data_path=self._path,
         )
 
-    def _get_storage_obj(self):
+    def _get_storage_obj(self, first_record=False):
         return self._data_storage
 
     def plot(
         self,
         key=None,
         names=None,
         filename_base=None,
@@ -1740,14 +1741,17 @@
         """Returns whether this MFList has any data associated with it in key
         "key"."""
         if key is None:
             for sto_key in self._data_storage.keys():
                 self.get_data_prep(sto_key)
                 if super().has_data():
                     return True
+            for val in self.empty_keys.values():
+                if val:
+                    return True
             return False
         else:
             self.get_data_prep(key)
             return super().has_data()
 
     def get_record(self, key=None):
         """Returns the data for stress period `key`.  If no key is specified
@@ -2042,15 +2046,19 @@
 
         self._update_record_prep(key)
         super().update_record(record, key_index)
 
     def _new_storage(self, stress_period=0):
         return {}
 
-    def _get_storage_obj(self):
+    def _get_storage_obj(self, first_record=False):
+        if first_record and isinstance(self._data_storage, dict):
+            for value in self._data_storage.values():
+                return value
+            return None
         if (
             self._current_key is None
             or self._current_key not in self._data_storage
         ):
             return None
         return self._data_storage[self._current_key]
```

### Comparing `flopy-3.6.0/flopy/mf6/data/mfdataplist.py` & `flopy-3.7.0/flopy/mf6/data/mfdataplist.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,63 @@
         self.internal_data = None
         self.fname = None
         self.iprn = None
         self.binary = False
         self.data_storage_type = None
         self.modified = False
 
+    def __repr__(self):
+        return self.get_data_str(True)
+
+    def __str__(self):
+        return self.get_data_str(False)
+
+    def _get_header_str(self):
+        header_list = []
+        if self.data_storage_type == DataStorageType.external_file:
+            header_list.append(f"open/close {self.fname}")
+        else:
+            header_list.append("internal")
+        if self.iprn is not None:
+            header_list.append(f"iprn {self.iprn}")
+        if len(header_list) > 0:
+            return ", ".join(header_list)
+        else:
+            return ""
+
+    def get_data_str(self, formal):
+        data_str = ""
+        layer_str = ""
+        if self.data_storage_type == DataStorageType.internal_array:
+            if self.internal_data is not None:
+                header = self._get_header_str()
+                if formal:
+                    data_str = "{}{}{{{}}}\n({})\n".format(
+                        data_str,
+                        layer_str,
+                        header,
+                        repr(self.internal_data),
+                    )
+                else:
+                    data_str = "{}{}{{{}}}\n({})\n".format(
+                        data_str,
+                        layer_str,
+                        header,
+                        str(self.internal_data),
+                    )
+        elif self.data_storage_type == DataStorageType.external_file:
+            header = self._get_header_str()
+            data_str = "{}{}{{{}}}\n({})\n".format(
+                data_str,
+                layer_str,
+                header,
+                "External data not displayed",
+            )
+        return data_str
+
     def get_record(self):
         rec = {}
         if self.internal_data is not None:
             rec["data"] = copy.deepcopy(self.internal_data)
         if self.fname is not None:
             rec["filename"] = self.fname
         if self.iprn is not None:
@@ -722,15 +771,15 @@
                 type_,
                 value_,
                 traceback_,
                 message,
                 self._simulation_data.debug,
             )
 
-        data_storage = self._get_storage()
+        data_storage = self._get_storage_obj()
         if append:
             # append data to existing dataframe
             current_data = self._get_dataframe()
             if current_data is not None:
                 data = pandas.concat([current_data, data])
         if data_storage.data_storage_type == DataStorageType.external_file:
             # store external data until next write
@@ -738,36 +787,36 @@
         else:
             # store data internally
             data_storage.set_internal(data)
             data_storage.modified = True
 
     def has_modified_ext_data(self):
         """check to see if external data has been modified since last read"""
-        data_storage = self._get_storage()
+        data_storage = self._get_storage_obj()
         return (
             data_storage.data_storage_type == DataStorageType.external_file
             and data_storage.internal_data is not None
         )
 
     def binary_ext_data(self):
         """check for binary data"""
-        data_storage = self._get_storage()
+        data_storage = self._get_storage_obj()
         return data_storage.binary
 
     def to_array(self, kper=0, mask=False):
         """Convert stress period boundary condition (MFDataList) data for a
         specified stress period to a 3-D numpy array.
 
         Parameters
         ----------
         kper : int
             MODFLOW zero-based stress period number to return (default is
             zero)
         mask : bool
-            return array with np.NaN instead of zero
+            return array with np.nan instead of zero
 
         Returns
         ----------
         out : dict of numpy.ndarrays
             Dictionary of 3-D numpy arrays containing the stress period data
             for a selected stress period. The dictionary keys are the
             MFDataList dtype names for the stress period data."""
@@ -788,15 +837,15 @@
             autofill : bool
                 Automatically correct data
             check_data : bool
                 Whether to verify the data
 
         """
         if isinstance(record, dict):
-            data_storage = self._get_storage()
+            data_storage = self._get_storage_obj()
             if "filename" in record:
                 data_storage.set_external(record["filename"])
                 if "binary" in record:
                     if (
                         record["binary"]
                         and self.data_dimensions.package_dim.boundnames()
                     ):
@@ -847,17 +896,17 @@
         ----------
             data : list(tuple)
                 Data to append.
 
         """
         try:
             self._resync()
-            if self._get_storage() is None:
+            if self._get_storage_obj() is None:
                 self._data_storage = self._new_storage()
-            data_storage = self._get_storage()
+            data_storage = self._get_storage_obj()
             if (
                 data_storage.data_storage_type
                 == DataStorageType.internal_array
             ):
                 # update internal data
                 MFPandasList.set_data(self, data, append=True)
             elif (
@@ -948,15 +997,15 @@
 
         Parameters
         ----------
             check_data : bool
                 Verify data prior to storing
 
         """
-        storage = self._get_storage()
+        storage = self._get_storage_obj()
         # check if data is already stored external
         if (
             storage is None
             or storage.data_storage_type == DataStorageType.external_file
         ):
             data = self._get_dataframe()
             # if not empty dataset
@@ -995,15 +1044,15 @@
                 Whether to replace an existing external file.
             check_data : bool
                 Verify data prior to storing
 
         """
         # only store data externally (do not subpackage info)
         if self.structure.construct_package is None:
-            storage = self._get_storage()
+            storage = self._get_storage_obj()
             # check if data is already stored external
             if (
                 replace_existing_external
                 or storage is None
                 or storage.data_storage_type == DataStorageType.internal_array
                 or storage.data_storage_type
                 == DataStorageType.internal_constant
@@ -1012,29 +1061,30 @@
                 # if not empty dataset
                 if data is not None:
                     if (
                         self._simulation_data.verbosity_level.value
                         >= VerbosityLevel.verbose.value
                     ):
                         print(
-                            "Storing {} to external file {}.."
-                            ".".format(self.structure.name, external_file_path)
+                            "Storing {} to external file {}.." ".".format(
+                                self.structure.name, external_file_path
+                            )
                         )
                     external_data = {
                         "filename": external_file_path,
                         "data": data,
                         "binary": binary,
                     }
                     MFPandasList.set_record(
                         self, external_data, check_data=check_data
                     )
 
     def external_file_name(self):
         """Returns external file name, or None if this is not external data."""
-        storage = self._get_storage()
+        storage = self._get_storage_obj()
         if storage is None:
             return None
         if (
             storage.data_storage_type == DataStorageType.external_file
             and storage.fname is not None
             and storage.fname != ""
         ):
@@ -1187,23 +1237,23 @@
             self._current_key,
         )
         file_access.write_binary_file(
             self._dataframe_to_recarray(data),
             fd_data_file,
             self._model_or_sim.modeldiscrit,
         )
-        data_storage = self._get_storage()
+        data_storage = self._get_storage_obj()
         data_storage.internal_data = None
 
     def has_data(self, key=None):
         """Returns whether this MFList has any data associated with it."""
         try:
-            if self._get_storage() is None:
+            if self._get_storage_obj() is None:
                 return False
-            return self._get_storage().has_data()
+            return self._get_storage_obj().has_data()
         except Exception as ex:
             type_, value_, traceback_ = sys.exc_info()
             raise MFDataException(
                 self.structure.get_model(),
                 self.structure.get_package(),
                 self._path,
                 "checking for data",
@@ -1277,15 +1327,15 @@
                 Contains information about storing files externally
         Returns
         -------
             more data : bool,
             next data line : str
 
         """
-        data_storage = self._get_storage()
+        data_storage = self._get_storage_obj()
         data_storage.modified = False
         # parse first line to determine if this is internal or external data
         datautil.PyListUtil.reset_delimiter_used()
         arr_line = datautil.PyListUtil.split_data_line(first_line)
         if arr_line and (
             len(arr_line[0]) >= 2 and arr_line[0][:3].upper() == "END"
         ):
@@ -1334,15 +1384,15 @@
             # store internal data
             data_storage.set_internal(pd_data)
         return return_val
 
     def _new_storage(self):
         return {"Data": PandasListStorage()}
 
-    def _get_storage(self):
+    def _get_storage_obj(self, first_record=False):
         return self._data_storage["Data"]
 
     def _get_id_fields(self, data_frame):
         """
         assemble a list of id fields in this dataset
 
         Parameters
@@ -1480,15 +1530,15 @@
         dataframe = self._get_dataframe()
         if dataframe is None:
             return None
         return self._dataframe_to_recarray(dataframe)
 
     def _get_dataframe(self):
         """get and return dataframe for this list data"""
-        data_storage = self._get_storage()
+        data_storage = self._get_storage_obj()
         if data_storage is None or data_storage.data_storage_type is None:
             block_exists = self._block.header_exists(
                 self._current_key, self.path
             )
             if block_exists:
                 self._build_data_header()
                 return pandas.DataFrame(columns=self._header_names)
@@ -1547,17 +1597,17 @@
 
         Returns
         -------
             data_record : dict
 
         """
         try:
-            if self._get_storage() is None:
+            if self._get_storage_obj() is None:
                 return None
-            record = self._get_storage().get_record()
+            record = self._get_storage_obj().get_record()
         except Exception as ex:
             type_, value_, traceback_ = sys.exc_info()
             raise MFDataException(
                 self.structure.get_model(),
                 self.structure.get_package(),
                 self._path,
                 "getting record",
@@ -1646,15 +1696,15 @@
         fd_main
             file descriptor where open/close string should be written (for
             external file data)
         Returns
         -------
             result of pandas to_csv call
         """
-        data_storage = self._get_storage()
+        data_storage = self._get_storage_obj()
         if data_storage is None:
             return ""
         if (
             data_storage.data_storage_type == DataStorageType.external_file
             and fd_main is not None
         ):
             indent = self._simulation_data.indent_string
@@ -1747,15 +1797,15 @@
         gets the file path to the data
 
         Returns
         -------
         file_path : file path to data
 
         """
-        data_storage = self._get_storage()
+        data_storage = self._get_storage_obj()
         if data_storage.fname is None:
             return None
         if self._model_or_sim.type == "model":
             rel_path = self._simulation_data.mfpath.model_relative_path[
                 self._model_or_sim.name
             ]
             fp_relative = data_storage.fname
@@ -1985,19 +2035,19 @@
                 Whether to replace an existing external file.
             check_data : bool
                 Verify data prior to storing
         """
         self._cache_model_grid = True
         for sp in self._data_storage.keys():
             self._current_key = sp
-            storage = self._get_storage()
+            storage = self._get_storage_obj()
             if storage.internal_size == 0:
                 storage.internal_data = self.get_dataframe(sp)
             if storage.internal_size > 0 and (
-                self._get_storage().data_storage_type
+                self._get_storage_obj().data_storage_type
                 != DataStorageType.external_file
                 or replace_existing_external
             ):
                 fname, ext = os.path.splitext(external_file_path)
                 if datautil.DatumUtil.is_int(sp):
                     full_name = f"{fname}_{int(sp) + 1}{ext}"
                 else:
@@ -2023,15 +2073,15 @@
                 Verify data prior to storing
 
         """
         self._cache_model_grid = True
         for sp in self._data_storage.keys():
             self._current_key = sp
             if (
-                self._get_storage().data_storage_type
+                self._get_storage_obj().data_storage_type
                 == DataStorageType.external_file
             ):
                 super().store_internal(
                     check_data,
                 )
         self._cache_model_grid = False
 
@@ -2478,15 +2528,19 @@
 
         self._update_record_prep(key)
         super().update_record(record, key_index)
 
     def _new_storage(self):
         return {}
 
-    def _get_storage(self):
+    def _get_storage_obj(self, first_record=False):
+        if first_record and isinstance(self._data_storage, dict):
+            for value in self._data_storage.values():
+                return value
+            return None
         if (
             self._current_key is None
             or self._current_key not in self._data_storage
         ):
             return None
         return self._data_storage[self._current_key]
```

### Comparing `flopy-3.6.0/flopy/mf6/data/mfdatascalar.py` & `flopy-3.7.0/flopy/mf6/data/mfdatascalar.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,16 +295,15 @@
                         traceback_,
                         comment,
                         self._simulation_data.debug,
                         ex,
                     )
         else:
             message = (
-                "{} of type {} does not support add one "
-                "operation.".format(
+                "{} of type {} does not support add one " "operation.".format(
                     self._data_name, self.structure.get_datum_type()
                 )
             )
             type_, value_, traceback_ = sys.exc_info()
             raise MFDataException(
                 self.structure.get_model(),
                 self.structure.get_package(),
@@ -381,15 +380,15 @@
                     value_,
                     traceback_,
                     None,
                     self._simulation_data.debug,
                     ex,
                 )
         if self.structure.type == DatumType.keyword:
-            if data is not None and data != False:
+            if data is not None and data is not False:
                 # keyword appears alone
                 return "{}{}\n".format(
                     self._simulation_data.indent_string,
                     self.structure.name.upper(),
                 )
             else:
                 return ""
@@ -404,41 +403,42 @@
                     if isinstance(data, list) or isinstance(data, tuple):
                         if len(data) == 1 and (
                             isinstance(data[0], tuple)
                             or isinstance(data[0], list)
                         ):
                             data = data[0]
                         if len(data) > index and (
-                            data[index] is not None and data[index] != False
+                            data[index] is not None
+                            and data[index] is not False
                         ):
                             text_line.append(data_item.name.upper())
                             if (
                                 isinstance(data[index], str)
                                 and data_item.name.upper()
                                 != data[index].upper()
                                 and data[index] != ""
                             ):
                                 # since the data does not match the keyword
                                 # assume the keyword was excluded
                                 index -= 1
                     else:
-                        if data is not None and data != False:
+                        if data is not None and data is not False:
                             text_line.append(data_item.name.upper())
                 else:
                     if data is not None and data != "":
                         if isinstance(data, list) or isinstance(data, tuple):
                             if len(data) > index:
                                 if (
                                     data[index] is not None
-                                    and data[index] != False
+                                    and data[index] is not False
                                 ):
                                     current_data = data[index]
                                 else:
                                     break
-                            elif data_item.optional == True:
+                            elif data_item.optional is True:
                                 break
                             else:
                                 message = (
                                     "Missing expected data. Data "
                                     "size is {}. Index {} not"
                                     "found.".format(len(data), index)
                                 )
@@ -458,15 +458,15 @@
                                 )
 
                         else:
                             current_data = data
                         if data_item.type == DatumType.keyword:
                             if (
                                 current_data is not None
-                                and current_data != False
+                                and current_data is not False
                             ):
                                 if (
                                     isinstance(data[index], str)
                                     and data[index] == "#"
                                 ):
                                     # if data has been commented out,
                                     # keep the comment
@@ -657,15 +657,15 @@
             self.get_file_entry,
             DataStorageType.internal_array,
             DataStructureType.scalar,
             stress_period=stress_period,
             data_path=self._path,
         )
 
-    def _get_storage_obj(self):
+    def _get_storage_obj(self, first_record=False):
         return self._data_storage
 
     def plot(self, filename_base=None, file_extension=None, **kwargs):
         """
         Helper method to plot scalar objects
 
         Parameters:
@@ -907,15 +907,19 @@
         return super().load(
             first_line, file_handle, pre_data_comments, external_file_info
         )
 
     def _new_storage(self, stress_period=0):
         return {}
 
-    def _get_storage_obj(self):
+    def _get_storage_obj(self, first_record=False):
+        if first_record and isinstance(self._data_storage, dict):
+            for value in self._data_storage.values():
+                return value
+            return None
         if (
             self._current_key is None
             or self._current_key not in self._data_storage
         ):
             return None
         return self._data_storage[self._current_key]
```

### Comparing `flopy-3.6.0/flopy/mf6/data/mfdatastorage.py` & `flopy-3.7.0/flopy/mf6/data/mfdatastorage.py`

 * *Files 1% similar despite different names*

```diff
@@ -493,14 +493,30 @@
                 else:
                     if storage.data_const_value is not None:
                         data_str = "{}{}{{{}}}\n".format(
                             data_str,
                             layer_str,
                             self._get_layer_header_str(index),
                         )
+            elif storage.data_storage_type == DataStorageType.external_file:
+                header = self._get_layer_header_str(index)
+                if self.layered:
+                    data_str = "{}{}{{{}}}\n({})\n".format(
+                        data_str,
+                        layer_str,
+                        header,
+                        "External data not displayed",
+                    )
+                else:
+                    data_str = "{}{}{{{}}}\n({})\n".format(
+                        data_str,
+                        layer_str,
+                        header,
+                        "External data not displayed",
+                    )
         return data_str
 
     def _get_layer_header_str(self, layer):
         header_list = []
         if (
             self.layer_storage[layer].data_storage_type
             == DataStorageType.external_file
@@ -1368,24 +1384,24 @@
             if preserve_record:
                 factor = self.layer_storage[layer].factor
                 adjustment = multiplier / factor
                 if adjustment != 1.0:
                     # convert numbers to be multiplied by the original factor
                     data = data * adjustment
             if const:
-                self.layer_storage[layer].data_storage_type = (
-                    DataStorageType.internal_constant
-                )
+                self.layer_storage[
+                    layer
+                ].data_storage_type = DataStorageType.internal_constant
                 self.layer_storage[layer].data_const_value = [
                     mfdatautil.get_first_val(data)
                 ]
             else:
-                self.layer_storage[layer].data_storage_type = (
-                    DataStorageType.internal_array
-                )
+                self.layer_storage[
+                    layer
+                ].data_storage_type = DataStorageType.internal_array
                 try:
                     self.layer_storage[layer].internal_data = np.reshape(
                         data, dimensions
                     )
                 except:
                     message = (
                         'An error occurred when reshaping data "{}" to store. '
@@ -1406,19 +1422,19 @@
                         traceback_,
                         message,
                         self._simulation_data.debug,
                     )
                 data_type = self.data_dimensions.structure.get_datum_type(True)
                 dt = self.layer_storage[layer].internal_data.dtype
                 if dt != data_type:
-                    self.layer_storage[layer].internal_data = (
-                        self.layer_storage[layer].internal_data.astype(
-                            data_type
-                        )
-                    )
+                    self.layer_storage[
+                        layer
+                    ].internal_data = self.layer_storage[
+                        layer
+                    ].internal_data.astype(data_type)
             if not preserve_record:
                 self.layer_storage[layer].factor = multiplier
                 self.layer_storage[layer].iprn = print_format
 
     def _resolve_data_line(self, data, key):
         if len(self._recarray_type_list) > 1:
             # add any missing leading keywords to the beginning of the string
@@ -1798,17 +1814,17 @@
                 # store data externally in file
                 data_size = self.get_data_size(layer_new)
                 data_type = data_dim.structure.data_item_structures[0].type
 
                 if self._calc_data_size(data, 2) == 1 and data_size > 1:
                     # constant data, need to expand
                     self.layer_storage[layer_new].data_const_value = data
-                    self.layer_storage[layer_new].data_storage_type = (
-                        DataStorageType.internal_constant
-                    )
+                    self.layer_storage[
+                        layer_new
+                    ].data_storage_type = DataStorageType.internal_constant
                     data = self._fill_const_layer(layer)
                 elif isinstance(data, list):
                     data = self._to_ndarray(data, layer)
                 if binary:
                     text = self.data_dimensions.structure.name
                     file_access = MFFileAccessArray(
                         self.data_dimensions.structure,
@@ -1857,17 +1873,17 @@
         )
 
     def set_ext_file_attributes(self, layer, file_path, print_format, binary):
         # point to the external file and set flags
         self.layer_storage[layer].fname = file_path
         self.layer_storage[layer].iprn = print_format
         self.layer_storage[layer].binary = binary
-        self.layer_storage[layer].data_storage_type = (
-            DataStorageType.external_file
-        )
+        self.layer_storage[
+            layer
+        ].data_storage_type = DataStorageType.external_file
 
     def point_to_existing_external_file(self, arr_line, layer):
         (
             multiplier,
             print_format,
             binary,
             data_file,
@@ -1992,14 +2008,15 @@
                 )[0]
             else:
                 data_out = file_access.read_text_data_from_file(
                     self.get_data_size(layer),
                     self._data_type,
                     self.get_data_dimensions(layer),
                     layer,
+                    self.layered,
                     read_file,
                 )[0]
             if apply_mult and self.layer_storage[layer].factor is not None:
                 data_out = data_out * self.layer_storage[layer].factor
 
             if store_internal:
                 self.store_internal(data_out, layer)
@@ -2086,16 +2103,17 @@
         struct = self.data_dimensions.structure
         try:
             resolved_shape, shape_rule = self.data_dimensions.get_data_shape(
                 data_item, struct, data_line, repeating_key=current_key
             )
         except Exception as se:
             comment = (
-                'Unable to resolve shape for data "{}" field "{}"'
-                ".".format(struct.name, data_item.name)
+                'Unable to resolve shape for data "{}" field "{}"' ".".format(
+                    struct.name, data_item.name
+                )
             )
             type_, value_, traceback_ = sys.exc_info()
             raise MFDataException(
                 struct.get_model(),
                 struct.get_package(),
                 struct.path,
                 "loading data list from package file",
@@ -2449,14 +2467,15 @@
                 else:
                     data_out = (
                         file_access.read_text_data_from_file(
                             self.get_data_size(layer),
                             np_data_type,
                             self.get_data_dimensions(layer),
                             layer,
+                            self.layered,
                             read_file,
                         )[0]
                         * mult
                     )
                 if (
                     self.layer_storage.get_total_size() == 1
                     or not self.layered
```

### Comparing `flopy-3.6.0/flopy/mf6/data/mfdatautil.py` & `flopy-3.7.0/flopy/mf6/data/mfdatautil.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,14 +74,15 @@
                     False,
                 )
         else:
             try:
                 if isinstance(data, str):
                     # fix any scientific formatting that python can't handle
                     data = data.replace("d", "e")
+                    data = data.replace("D", "e")
                 return float(data)
             except (ValueError, TypeError):
                 try:
                     return float(PyListUtil.clean_numeric(data))
                 except (ValueError, TypeError):
                     message = (
                         'Data "{}" with value "{}" can '
@@ -147,15 +148,15 @@
         list data to convert to array
     model_grid : ModelGrid
         model grid object for data
     kper : int
         MODFLOW zero-based stress period number to return. (default is
         zero)
     mask : bool
-        return array with np.NaN instead of zero
+        return array with np.nan instead of zero
 
     Returns
     ----------
     out : dict of numpy.ndarrays
         Dictionary of 3-D numpy arrays containing the stress period data
         for a selected stress period. The dictionary keys are the
         MFDataList dtype names for the stress period data."""
@@ -188,15 +189,15 @@
             arrays[name] = arr.copy()
 
     if np.isscalar(sarr[0]):
         # if there are no entries for this kper
         if sarr[0] == 0:
             if mask:
                 for name, arr in arrays.items():
-                    arrays[name][:] = np.NaN
+                    arrays[name][:] = np.nan
             return arrays
         else:
             raise Exception("MfList: something bad happened")
 
     for name, arr in arrays.items():
         cnt = np.zeros(shape, dtype=np.float64)
         for sp_rec in sarr:
@@ -206,15 +207,15 @@
                     cnt[rec["cellid"]] += 1.0
         # average keys that should not be added
         if name != "cond" and name != "flux":
             idx = cnt > 0.0
             arr[idx] /= cnt[idx]
         if mask:
             arr = np.ma.masked_where(cnt == 0.0, arr)
-            arr[cnt == 0.0] = np.NaN
+            arr[cnt == 0.0] = np.nan
 
         arrays[name] = arr.copy()
     return arrays
 
 
 def process_open_close_line(
     arr_line, data_dim, data_type, sim_data, store=True
@@ -961,15 +962,15 @@
             nseg=nseg, cellid_expanded=cellid_expanded
         )
         if data_storage.jagged_record:
             comment = (
                 "Data dimensions can not be determined for  "
                 "{}. Data structure may be jagged or may contain "
                 "a keystring. Data type information is therefore "
-                "dependant on the data and can not be retreived "
+                "dependent on the data and can not be retrieved "
                 "prior to the data being loaded"
                 ".".format(data_storage.data_dimensions.structure.name)
             )
             type_, value_, traceback_ = sys.exc_info()
 
             raise MFDataException(
                 data_struct.get_model(),
```

### Comparing `flopy-3.6.0/flopy/mf6/data/mffileaccess.py` & `flopy-3.7.0/flopy/mf6/data/mffileaccess.py`

 * *Files 0% similar despite different names*

```diff
@@ -573,18 +573,25 @@
 
     def read_text_data_from_file(
         self,
         data_size,
         data_type,
         data_dim,
         layer,
+        layered,
         fname=None,
         fd=None,
-        data_item=None,
     ):
+        # determine line size
+        line_size = None
+        if layered:
+            # if the array is layered (meaning a control record for
+            # each layer), then limit line size to number of columns
+            if isinstance(data_dim, list):
+                line_size = data_dim[-1]
         # load variable data from file
         current_size = 0
         if layer is None:
             layer = 0
         close_file = False
         if fd is None:
             close_file = True
@@ -597,22 +604,26 @@
             # indicator is found
             while True:
                 line = fd.readline()
                 arr_line = PyListUtil.split_data_line(line, True)
                 if line == "" or arr_line[0].upper() == "END":
                     break
                 if not MFComment.is_comment(arr_line, True):
+                    if line_size is not None:
+                        arr_line = arr_line[:line_size]
                     data_raw += arr_line
                 else:
                     PyListUtil.reset_delimiter_used()
         else:
             while line != "" and len(data_raw) < data_size:
                 line = fd.readline()
                 arr_line = PyListUtil.split_data_line(line, True)
                 if not MFComment.is_comment(arr_line, True):
+                    if line_size is not None:
+                        arr_line = arr_line[:line_size]
                     data_raw += arr_line
                 else:
                     PyListUtil.reset_delimiter_used()
 
         if len(data_raw) < data_size:
             message = (
                 'Not enough data in file {} for data "{}".  '
@@ -882,14 +893,15 @@
                     True
                 )
                 data_from_file = self.read_text_data_from_file(
                     storage.get_data_size(layer),
                     data_type,
                     storage.get_data_dimensions(layer),
                     layer,
+                    storage.layered,
                     fd=file_handle,
                 )
             except Exception as ex:
                 type_, value_, traceback_ = sys.exc_info()
                 raise MFDataException(
                     self.structure.get_model(),
                     self.structure.get_package(),
@@ -1465,17 +1477,15 @@
                                     arr_line_len,
                                     data_item,
                                     data_index,
                                     None,
                                     current_key,
                                     self._data_line,
                                     False,
-                                )[
-                                    0:2
-                                ]
+                                )[0:2]
                             elif (
                                 data_item.name == "boundname"
                                 and self._data_dimensions.package_dim.boundnames()
                             ):
                                 self._data_line += (
                                     convert_data(
                                         arr_line[data_index],
@@ -1716,17 +1726,15 @@
                                                 not in data_item.keystring_dict
                                             ):
                                                 # look for data key in child records
                                                 found = False
                                                 for (
                                                     key,
                                                     record,
-                                                ) in (
-                                                    data_item.keystring_dict.items()
-                                                ):
+                                                ) in data_item.keystring_dict.items():
                                                     if (
                                                         isinstance(
                                                             record,
                                                             MFDataStructure,
                                                         )
                                                         and len(
                                                             record.data_item_structures
@@ -2046,17 +2054,15 @@
                             0,
                             data_index,
                             var_index,
                             1,
                             current_key,
                             data_line,
                             add_to_last_line,
-                        )[
-                            0:3
-                        ]
+                        )[0:3]
                     else:
                         # read in aux variables
                         (
                             data_index,
                             more_data_expected,
                             data_line,
                         ) = self._append_data_list(
@@ -2066,17 +2072,15 @@
                             arr_line_len,
                             data_index,
                             var_index,
                             0,
                             current_key,
                             data_line,
                             add_to_last_line,
-                        )[
-                            0:3
-                        ]
+                        )[0:3]
         return data_index, data_line, more_data_expected
 
     def _append_data_list(
         self,
         storage,
         data_item,
         arr_line,
@@ -2319,15 +2323,15 @@
         if self.structure.type == DatumType.record:
             index = 0
             for data_item_type in self.structure.get_data_item_types():
                 optional = self.structure.data_item_structures[index].optional
                 if (
                     len(arr_line) <= index + 1
                     or data_item_type[0] != DatumType.keyword
-                    or (index > 0 and optional == True)
+                    or (index > 0 and optional is True)
                 ):
                     break
                 index += 1
             first_type = self.structure.get_data_item_types()[0]
             if first_type[0] == DatumType.keyword:
                 converted_data = [True]
             else:
```

### Comparing `flopy-3.6.0/flopy/mf6/data/mfstructure.py` & `flopy-3.7.0/flopy/mf6/data/mfstructure.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,14 @@
             "sim-tdis",  # dfn completed  tex updated
             "exg-gwfgwf",  # dfn completed  tex updated
             "sln-ims",  # dfn completed  tex updated
             "gwf-nam",  # dfn completed  tex updated
             "gwf-dis",  # dfn completed  tex updated
             "gwf-disv",  # dfn completed  tex updated
             "gwf-disu",  # dfn completed  tex updated
-            "lnf-disl",  # dfn completed  tex updated
             "gwf-ic",  # dfn completed  tex updated
             "gwf-npf",  # dfn completed  tex updated
             "gwf-sto",  # dfn completed  tex updated
             "gwf-hfb",  # dfn completed  tex updated
             "gwf-chd",  # dfn completed  tex updated
             "gwf-wel",  # dfn completed  tex updated
             "gwf-drn",  # dfn completed  tex updated
@@ -1172,19 +1171,19 @@
             if key in self.name.lower():
                 return True
         return False
 
     def is_file_name(self):
         if (
             self.name.lower() in self.file_name_keywords
-            and self.file_name_keywords[self.name.lower()] == True
+            and self.file_name_keywords[self.name.lower()] is True
         ):
             return True
         for key, item in self.contained_keywords.items():
-            if self.name.lower().find(key) != -1 and item == True:
+            if self.name.lower().find(key) != -1 and item is True:
                 return True
         return False
 
     @staticmethod
     def remove_cellid(resolved_shape, cellid_size):
         # remove the cellid size from the shape
         for dimension, index in zip(
@@ -1553,15 +1552,15 @@
     def add_item(self, item, record=False, dfn_list=None):
         item_added = False
         if item.type != DatumType.recarray and (
             (
                 item.type != DatumType.record
                 and item.type != DatumType.repeating_record
             )
-            or record == True
+            or record is True
         ):
             if item.name not in self.expected_data_items:
                 raise StructException(
                     'Could not find data item "{}" in '
                     "expected data items of data structure "
                     "{}.".format(item.name, self.name),
                     self.path,
@@ -2067,15 +2066,15 @@
             if item.type == DatumType.recarray:
                 recarray_list.append(item)
         return recarray_list
 
 
 class MFInputFileStructure:
     """
-    MODFLOW Input File Stucture class.  Loads file
+    MODFLOW Input File Structure class.  Loads file
     structure information for individual input file
     types.
 
 
     Parameters
     ----------
     dfn_file : string
```

### Comparing `flopy-3.6.0/flopy/mf6/mfbase.py` & `flopy-3.7.0/flopy/mf6/mfbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" Base classes for Modflow 6 """
+"""Base classes for Modflow 6"""
 
 import copy
 import inspect
 import os
 import sys
 import traceback
 import warnings
@@ -562,29 +562,32 @@
         if package.filename is not None:
             self.package_filename_dict[package.filename.lower()] = package
         if package.package_type not in self.package_type_dict:
             self.package_type_dict[package.package_type.lower()] = []
         self.package_type_dict[package.package_type.lower()].append(package)
 
     def _remove_package(self, package):
-        self._packagelist.remove(package)
+        if package in self._packagelist:
+            self._packagelist.remove(package)
         if (
             package.package_name is not None
             and package.package_name.lower() in self.package_name_dict
         ):
             del self.package_name_dict[package.package_name.lower()]
         if (
             package.filename is not None
             and package.filename.lower() in self.package_filename_dict
         ):
             del self.package_filename_dict[package.filename.lower()]
-        package_list = self.package_type_dict[package.package_type.lower()]
-        package_list.remove(package)
-        if len(package_list) == 0:
-            del self.package_type_dict[package.package_type.lower()]
+        if package.package_type.lower() in self.package_type_dict:
+            package_list = self.package_type_dict[package.package_type.lower()]
+            if package in package_list:
+                package_list.remove(package)
+            if len(package_list) == 0:
+                del self.package_type_dict[package.package_type.lower()]
 
         # collect keys of items to be removed from main dictionary
         items_to_remove = []
         for key in self.simulation_data.mfdata:
             is_subkey = True
             for pitem, ditem in zip(package.path, key):
                 if pitem != ditem:
@@ -620,59 +623,64 @@
         # fix keys in main dictionary
         for key in items_to_fix:
             new_key = (
                 package.path[:-1] + (new_name,) + key[len(package.path) - 1 :]
             )
             main_dict[new_key] = main_dict.pop(key)
 
-    def get_package(self, name=None):
+    def get_package(self, name=None, type_only=False, name_only=False):
         """
         Finds a package by package name, package key, package type, or partial
         package name. returns either a single package, a list of packages,
         or None.
 
         Parameters
         ----------
         name : str
-            Name of the package, 'RIV', 'LPF', etc.
+            Name or type of the package, 'my-riv-1, 'RIV', 'LPF', etc.
+        type_only : bool
+            Search for package by type only
+        name_only : bool
+            Search for package by name only
 
         Returns
         -------
         pp : Package object
 
         """
         if name is None:
             return self._packagelist[:]
 
         # search for full package name
-        if name.lower() in self.package_name_dict:
+        if name.lower() in self.package_name_dict and not type_only:
             return self.package_name_dict[name.lower()]
 
         # search for package type
-        if name.lower() in self.package_type_dict:
+        if name.lower() in self.package_type_dict and not name_only:
             if len(self.package_type_dict[name.lower()]) == 0:
                 return None
             elif len(self.package_type_dict[name.lower()]) == 1:
                 return self.package_type_dict[name.lower()][0]
             else:
                 return self.package_type_dict[name.lower()]
 
         # search for file name
-        if name.lower() in self.package_filename_dict:
+        if name.lower() in self.package_filename_dict and not type_only:
             return self.package_filename_dict[name.lower()]
 
         # search for partial and case-insensitive package name
-        for pp in self._packagelist:
-            if pp.package_name is not None:
-                # get first package of the type requested
-                package_name = pp.package_name.lower()
-                if len(package_name) > len(name):
-                    package_name = package_name[0 : len(name)]
-                if package_name.lower() == name.lower():
-                    return pp
+        if not type_only:
+            for pp in self._packagelist:
+                if pp.package_name is not None:
+                    # get first package of the type requested
+                    package_name = pp.package_name.lower()
+                    if len(package_name) > len(name):
+                        package_name = package_name[0 : len(name)]
+                    if package_name.lower() == name.lower():
+                        return pp
 
         return None
 
     def register_package(self, package):
         """Base method for registering a package.  Should be overridden."""
         path = (package.package_name,)
         return (path, None)
```

### Comparing `flopy-3.6.0/flopy/mf6/mfmodel.py` & `flopy-3.7.0/flopy/mf6/mfmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,35 +260,41 @@
         Returns
         -------
         modeltime : ModelTime
             FloPy object containing time discretization information for the
             simulation.
 
         """
-        tdis = self.simulation.get_package("tdis")
+        tdis = self.simulation.get_package("tdis", type_only=True)
         period_data = tdis.perioddata.get_data()
 
         # build steady state data
-        sto = self.get_package("sto")
+        sto = self.get_package("sto", type_only=True)
         if sto is None:
             steady = np.full((len(period_data["perlen"])), True, dtype=bool)
         else:
             steady = np.full((len(period_data["perlen"])), False, dtype=bool)
             ss_periods = sto.steady_state.get_active_key_dict()
+            for period, val in ss_periods.items():
+                if val:
+                    ss_periods[period] = sto.steady_state.get_data(period)
             tr_periods = sto.transient.get_active_key_dict()
+            for period, val in tr_periods.items():
+                if val:
+                    tr_periods[period] = sto.transient.get_data(period)
             if ss_periods:
                 last_ss_value = False
                 # loop through steady state array
                 for index, value in enumerate(steady):
                     # resolve if current index is steady state or transient
-                    if index in ss_periods:
+                    if index in ss_periods and ss_periods[index]:
                         last_ss_value = True
-                    elif index in tr_periods:
+                    elif index in tr_periods and tr_periods[index]:
                         last_ss_value = False
-                    if last_ss_value == True:
+                    if last_ss_value is True:
                         steady[index] = True
 
         # build model time
         itmuni = tdis.time_units.get_data()
         start_date_time = tdis.start_date_time.get_data()
         if itmuni is None:
             itmuni = 0
@@ -483,16 +489,16 @@
                 crs=self._modelgrid.crs,
                 xoff=self._modelgrid.xoffset,
                 yoff=self._modelgrid.yoffset,
                 angrot=self._modelgrid.angrot,
                 iac=dis.iac.array,
                 ja=dis.ja.array,
             )
-        elif self.get_grid_type() == DiscretizationType.DISL:
-            dis = self.get_package("disl")
+        elif self.get_grid_type() == DiscretizationType.DISV1D:
+            dis = self.get_package("disv1d")
             if not hasattr(dis, "_init_complete"):
                 if not hasattr(dis, "cell1d"):
                     # disv package has not yet been initialized
                     return self._modelgrid
                 else:
                     # disv package has been partially initialized
                     self._modelgrid = VertexGrid(
@@ -521,14 +527,52 @@
                     idomain=idomain,
                     lenuni=dis.length_units.array,
                     crs=self._modelgrid.crs,
                     xoff=self._modelgrid.xoffset,
                     yoff=self._modelgrid.yoffset,
                     angrot=self._modelgrid.angrot,
                 )
+        elif self.get_grid_type() == DiscretizationType.DISV2D:
+            dis = self.get_package("disv2d")
+            if not hasattr(dis, "_init_complete"):
+                if not hasattr(dis, "cell2d"):
+                    # disv package has not yet been initialized
+                    return self._modelgrid
+                else:
+                    # disv package has been partially initialized
+                    self._modelgrid = VertexGrid(
+                        vertices=dis.vertices.array,
+                        cell2d=dis.cell2d.array,
+                        top=None,
+                        botm=None,
+                        idomain=None,
+                        lenuni=None,
+                        crs=self._modelgrid.crs,
+                        xoff=self._modelgrid.xoffset,
+                        yoff=self._modelgrid.yoffset,
+                        angrot=self._modelgrid.angrot,
+                    )
+            else:
+                botm = dis.botm.array
+                idomain = dis.idomain.array
+                if idomain is None:
+                    force_resync = True
+                    idomain = self._resolve_idomain(idomain, botm)
+                self._modelgrid = VertexGrid(
+                    vertices=dis.vertices.array,
+                    cell2d=dis.cell2d.array,
+                    top=dis.top.array,
+                    botm=botm,
+                    idomain=idomain,
+                    lenuni=dis.length_units.array,
+                    crs=self._modelgrid.crs,
+                    xoff=self._modelgrid.xoffset,
+                    yoff=self._modelgrid.yoffset,
+                    angrot=self._modelgrid.angrot,
+                )
         else:
             return self._modelgrid
 
         if self.get_grid_type() != DiscretizationType.DISV:
             # get coordinate data from dis file
             xorig = dis.xorigin.get_data()
             yorig = dis.yorigin.get_data()
@@ -634,30 +678,33 @@
         None : None
 
         """
         return None
 
     @property
     def output(self):
+        budgetkey = None
+        if self.model_type == "gwt6":
+            budgetkey = "MASS BUDGET FOR ENTIRE MODEL"
         try:
-            return self.oc.output
+            return MF6Output(self.oc, budgetkey=budgetkey)
         except AttributeError:
-            return MF6Output(self)
+            return MF6Output(self, budgetkey=budgetkey)
 
     def export(self, f, **kwargs):
         """Method to export a model to a shapefile or netcdf file
 
         Parameters
         ----------
         f : str
             File name (".nc" for netcdf or ".shp" for shapefile)
             or dictionary of ....
         **kwargs : keyword arguments
             modelgrid: flopy.discretization.Grid
-                User supplied modelgrid object which will supercede the built
+                User supplied modelgrid object which will supersede the built
                 in modelgrid object
             if fmt is set to 'vtk', parameters of Vtk initializer
 
         """
         from ..export import utils
 
         return utils.model_export(f, self, **kwargs)
@@ -783,14 +830,17 @@
             f"disv{vnum}": 1,
             f"disu{vnum}": 1,
         }
         packages_ordered = []
         package_recarray = instance.simulation_data.mfdata[
             (modelname, "nam", "packages", "packages")
         ]
+        if package_recarray.array is None:
+            return instance
+
         for item in package_recarray.get_data():
             if item[0] in priority_packages:
                 packages_ordered.insert(0, (item[0], item[1], item[2]))
             else:
                 packages_ordered.append((item[0], item[1], item[2]))
 
         # load packages
@@ -826,15 +876,15 @@
                 ):
                     print(f"    loading package {ftype}...")
                 # load package
                 instance.load_package(ftype, fname, pname, strict, None)
                 sim_data = simulation.simulation_data
                 if ftype == "dis" and not sim_data.max_columns_user_set:
                     # set column wrap to ncol
-                    dis = instance.get_package("dis")
+                    dis = instance.get_package("dis", type_only=True)
                     if dis is not None and hasattr(dis, "ncol"):
                         sim_data.max_columns_of_data = dis.ncol.get_data()
                         sim_data.max_columns_user_set = False
                         sim_data.max_columns_auto_set = True
         # load referenced packages
         if modelname in instance.simulation_data.referenced_files:
             for ref_file in instance.simulation_data.referenced_files[
@@ -1032,15 +1082,15 @@
                                 fd.write(",stress_period/key")
                         if search_output.data_header is not None:
                             if len(search_output.data_entry_cellids) > 0:
                                 fd.write(",cellid")
                             h_columns = ",".join(search_output.data_header)
                             fd.write(f",{h_columns}\n")
                         else:
-                            fd.write(f",cellid,data\n")
+                            fd.write(",cellid,data\n")
                         # write data found
                         for index, data_entry in enumerate(
                             search_output.data_entries
                         ):
                             if search_output.transient:
                                 sp = search_output.data_entry_stress_period[
                                     index
@@ -1064,15 +1114,15 @@
                                         for i in search_output.data_entry_ids[
                                             index
                                         ]
                                     ]
                                 )
                                 fd.write(f",{output}")
                                 fd.write(self._format_data_entry(data_entry))
-                    fd.write(f"\n")
+                    fd.write("\n")
         return output_by_package
 
     def match_array_cells(
         self, cell_list, data_shape, array_data, key, data_output
     ):
         # loop through list of cells we are searching for
         for cell in cell_list:
@@ -1199,19 +1249,26 @@
                 f"disu{structure.get_version_string()}", 0
             )
             is not None
         ):
             return DiscretizationType.DISU
         elif (
             package_recarray.search_data(
-                f"disl{structure.get_version_string()}", 0
+                f"disv1d{structure.get_version_string()}", 0
+            )
+            is not None
+        ):
+            return DiscretizationType.DISV1D
+        elif (
+            package_recarray.search_data(
+                f"disv2d{structure.get_version_string()}", 0
             )
             is not None
         ):
-            return DiscretizationType.DISL
+            return DiscretizationType.DISV2D
 
         return DiscretizationType.UNDEFINED
 
     def get_ims_package(self):
         """Get the IMS package associated with this model.
 
         Returns
@@ -1238,15 +1295,15 @@
         period_data = tdis.perioddata.get_data()
         index = 0
         pd_len = len(period_data)
         while index < pd_len:
             ss_list.append(True)
             index += 1
 
-        storage = self.get_package("sto")
+        storage = self.get_package("sto", type_only=True)
         if storage is not None:
             tr_keys = storage.transient.get_keys(True)
             ss_keys = storage.steady_state.get_keys(True)
             for key in tr_keys:
                 ss_list[key] = False
                 for ss_list_key in range(key + 1, len(ss_list)):
                     for ss_key in ss_keys:
@@ -1274,15 +1331,15 @@
             if not pp.is_valid():
                 return False
 
         # required packages exist
         for package_struct in self.structure.package_struct_objs.values():
             if (
                 not package_struct.optional
-                and not package_struct.file_type in self.package_type_dict
+                and package_struct.file_type not in self.package_type_dict
             ):
                 return False
 
         return True
 
     def set_model_relative_path(self, model_ws):
         """
```

### Comparing `flopy-3.6.0/flopy/mf6/mfpackage.py` & `flopy-3.7.0/flopy/mf6/mfpackage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1027,14 +1027,21 @@
                             )
                             self._save_comments(arr_line, line, key, comments)
                             if (
                                 result[1] is not None
                                 and result[1][:3].upper() == "END"
                             ):
                                 break
+        else:
+            # block empty, store empty array in block variables
+            empty_arr = []
+            for ds in self.datasets.values():
+                if isinstance(ds, mfdata.MFTransient):
+                    transient_key = block_header.get_transient_key()
+                    ds.set_data(empty_arr, key=transient_key)
         self.loaded = True
         self.is_valid()
 
     def _find_data_by_keyword(self, line, fd, initial_comment):
         first_key = None
         nothing_found = False
         next_line = [True, line]
@@ -1105,15 +1112,15 @@
                             )
                 if first_key is None:
                     first_key = key
                 nothing_found = False
             elif (
                 arr_line[0].lower() == "readasarrays"
                 and self.path[-1].lower() == "options"
-                and self._container_package.structure.read_as_arrays == False
+                and self._container_package.structure.read_as_arrays is False
             ):
                 error_msg = (
                     "ERROR: Attempting to read a ReadAsArrays "
                     "package as a non-ReadAsArrays "
                     "package {}".format(self.path)
                 )
                 raise ReadAsArraysException(error_msg)
@@ -1239,15 +1246,15 @@
                 file_path,
                 dict_package_name,
             )
         )
 
     def _save_comments(self, arr_line, line, key, comments):
         # FIX: Save these comments somewhere in the data set
-        if not key in self.datasets_keyword:
+        if key not in self.datasets_keyword:
             if MFComment.is_comment(key, True):
                 if comments:
                     comments.append("\n")
                 comments.append(arr_line)
 
     def write(self, fd, ext_file_action=ExtFileAction.copy_relative_paths):
         """Writes block to a file object.
@@ -1485,16 +1492,17 @@
                     data_found = True
                 else:
                     if (
                         self._simulation_data.verbosity_level.value
                         >= VerbosityLevel.verbose.value
                     ):
                         print(
-                            "        writing data {} ({}).."
-                            ".".format(dataset.structure.name, transient_key)
+                            "        writing data {} ({}).." ".".format(
+                                dataset.structure.name, transient_key
+                            )
                         )
                     if basic_list:
                         ext_fname = dataset.external_file_name(transient_key)
                         if ext_fname is not None:
                             # if dataset.has_modified_ext_data(transient_key):
                             binary = dataset.binary_ext_data(transient_key)
                             # write block contents to external file
@@ -1579,15 +1587,15 @@
             self._simulation_data.mfdata[pth].write(fd)
 
         # write extra line if comments are off
         if not self._simulation_data.comments_on:
             fd.write("\n")
 
     def is_allowed(self):
-        """Determine if block is valid based on the values of dependant
+        """Determine if block is valid based on the values of dependent
         MODFLOW variables."""
         if self.structure.variable_dependant_path:
             # fill in empty part of the path with the current path
             if len(self.structure.variable_dependant_path) == 3:
                 dependant_var_path = (
                     self.path[0],
                 ) + self.structure.variable_dependant_path
@@ -2092,16 +2100,16 @@
                                         data_index = aux_start_loc + idx
                                         # verify auxiliary value is either
                                         # numeric or time series variable
                                         if (
                                             not datautil.DatumUtil.is_float(
                                                 row[data_index]
                                             )
-                                            and not row[data_index]
-                                            in time_series_name_dict
+                                            and row[data_index]
+                                            not in time_series_name_dict
                                         ):
                                             desc = (
                                                 f"Invalid non-numeric "
                                                 f"value "
                                                 f"'{row[data_index]}' "
                                                 f"in auxiliary data."
                                             )
@@ -2116,16 +2124,16 @@
                         for data in aux_datasets:
                             # verify auxiliary value is either numeric or time
                             # array series variable
                             if isinstance(data, np.ndarray):
                                 val = np.isnan(np.sum(data))
                                 if val:
                                     desc = (
-                                        f"One or more nan values were "
-                                        f"found in auxiliary data."
+                                        "One or more nan values were "
+                                        "found in auxiliary data."
                                     )
                                     chk._add_to_summary(
                                         "Warning",
                                         desc=desc,
                                         package=self.package_name,
                                     )
         return chk
@@ -2161,25 +2169,23 @@
             data_str = f"{data_str}\n"
         if show_data:
             for block in self.blocks.values():
                 if formal:
                     bl_repr = repr(block)
                     if len(bl_repr.strip()) > 0:
                         data_str = (
-                            "{}Block {}\n--------------------\n{}"
-                            "\n".format(
+                            "{}Block {}\n--------------------\n{}" "\n".format(
                                 data_str, block.structure.name, repr(block)
                             )
                         )
                 else:
                     bl_str = str(block)
                     if len(bl_str.strip()) > 0:
                         data_str = (
-                            "{}Block {}\n--------------------\n{}"
-                            "\n".format(
+                            "{}Block {}\n--------------------\n{}" "\n".format(
                                 data_str, block.structure.name, str(block)
                             )
                         )
         return data_str
 
     def _get_pname(self):
         if self.package_name is not None:
@@ -2571,15 +2577,15 @@
         """Builds a child package.  This method is only intended for FloPy
         internal use."""
         if not hasattr(self, pkg_type):
             self.build_child_packages_container(pkg_type, filerecord)
         if data is not None:
             package_group = getattr(self, pkg_type)
             # build child package file name
-            child_path = package_group._next_default_file_path()
+            child_path = package_group.next_default_file_path()
             # create new empty child package
             package_obj = self.package_factory(
                 pkg_type, self.model_or_sim.model_type
             )
             package = package_obj(
                 self, filename=child_path, child_builder_call=True
             )
@@ -2973,15 +2979,15 @@
                             "", self.path, self._simulation_data
                         )
 
                         cur_block.load(
                             block_header_info, fd_input_file, strict
                         )
 
-                        # write post block comment comment
+                        # write post block comment
                         self._simulation_data.mfdata[
                             cur_block.block_headers[-1].blk_post_comment_path
                         ] = self.post_block_comments
 
                         blocks_read += 1
                         if blocks_read >= max_blocks:
                             break
@@ -3377,15 +3383,15 @@
     def __file_path_taken(self, possible_path):
         for package in self._packages:
             # Do case insensitive compare
             if package.filename.lower() == possible_path.lower():
                 return True
         return False
 
-    def _next_default_file_path(self):
+    def next_default_file_path(self):
         possible_path = self.__default_file_path_base(self._cpparent.filename)
         suffix = 0
         while self.__file_path_taken(possible_path):
             possible_path = self.__default_file_path_base(
                 self._cpparent.filename, suffix
             )
             suffix += 1
@@ -3395,15 +3401,15 @@
         if remove_packages:
             # clear out existing packages
             self._remove_packages()
         elif fname is not None:
             self._remove_packages(fname)
         if fname is None:
             # build a file name
-            fname = self._next_default_file_path()
+            fname = self.next_default_file_path()
             package._filename = fname
         # check file record variable
         found = False
         fr_data = self._filerecord.get_data()
         if fr_data is not None:
             for line in fr_data:
                 if line[0] == fname:
@@ -3433,15 +3439,15 @@
         else:
             new_file_record_data.append((new_fname,))
         self._filerecord.set_data(new_file_record_data)
 
     def _append_package(self, package, fname, update_frecord=True):
         if fname is None:
             # build a file name
-            fname = self._next_default_file_path()
+            fname = self.next_default_file_path()
             package._filename = fname
 
         if update_frecord:
             # set file record variable
             file_record = self._filerecord.get_data()
             file_record_data = file_record
             new_file_record_data = []
@@ -3453,15 +3459,16 @@
         for existing_pkg in self._packages:
             if existing_pkg is package:
                 # do not add the same package twice
                 return
         # add the package to the list
         self._packages.append(package)
 
-    def _remove_packages(self, fname=None):
+    def _remove_packages(self, fname=None, only_pop_from_list=False):
         rp_list = []
         for idx, package in enumerate(self._packages):
             if fname is None or package.filename == fname:
-                self._model_or_sim.remove_package(package)
+                if not only_pop_from_list:
+                    self._model_or_sim.remove_package(package)
                 rp_list.append(idx)
         for idx in reversed(rp_list):
             self._packages.pop(idx)
```

### Comparing `flopy-3.6.0/flopy/mf6/mfsimbase.py` & `flopy-3.7.0/flopy/mf6/mfsimbase.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,15 +250,15 @@
         self._sci_note_lower_thres = 0.001
         self.fast_write = True
         self.comments_on = False
         self.auto_set_sizes = True
         self.verify_data = True
         self.debug = False
         self.verbose = True
-        self.verbosity_level = VerbosityLevel.normal
+        self._verbosity_level = VerbosityLevel.normal
         self.max_columns_user_set = False
         self.max_columns_auto_set = False
         self.use_pandas = True
 
         self._update_str_format()
 
         # --- file path ---
@@ -272,14 +272,25 @@
         self.mfdata = SimulationDict(self.mfpath)
 
         # --- temporary variables ---
         # other external files referenced
         self.referenced_files = {}
 
     @property
+    def verbosity_level(self):
+        return self._verbosity_level
+
+    @verbosity_level.setter
+    def verbosity_level(self, val):
+        if isinstance(val, VerbosityLevel):
+            self._verbosity_level = val
+        elif isinstance(val, int):
+            self._verbosity_level = VerbosityLevel(val)
+
+    @property
     def lazy_io(self):
         if not self.auto_set_sizes and not self.verify_data:
             return True
         return False
 
     @lazy_io.setter
     def lazy_io(self, val):
@@ -610,17 +621,17 @@
 
         """
         return self._get_data_str(False)
 
     def _get_data_str(self, formal):
         file_mgt = self.simulation_data.mfpath
         data_str = (
-            "sim_name = {}\nsim_path = {}\nexe_name = "
-            "{}\n"
-            "\n".format(self.name, file_mgt.get_sim_path(), self.exe_name)
+            "sim_name = {}\nsim_path = {}\nexe_name = " "{}\n" "\n".format(
+                self.name, file_mgt.get_sim_path(), self.exe_name
+            )
         )
 
         for package in self._packagelist:
             pk_str = package._get_data_str(formal, False)
             if formal:
                 if len(pk_str.strip()) > 0:
                     data_str = (
@@ -801,14 +812,17 @@
             )
             raise MFDataException(
                 mfdata_except=mfde,
                 model=instance.name,
                 package="nam",
                 message=message,
             )
+        if models is None:
+            return instance
+
         for item in models:
             # resolve model working folder and name file
             path, name_file = os.path.split(item[1])
             model_obj = PackageContainer.model_factory(item[0][:-1].lower())
             # load model
             if verbosity_level.value >= VerbosityLevel.normal.value:
                 print(f"  loading model {item[0].lower()}...")
@@ -1302,14 +1316,34 @@
                         "simulation name file with the solution package "
                         'file "{}".'.format(solution_file.filename)
                     )
                     raise MFDataException(
                         mfdata_except=mfde, package="nam", message=message
                     )
 
+    def _create_package(self, package_type, package_data):
+        if package_data is None:
+            return None
+        if not isinstance(package_data, dict):
+            message = (
+                "Error occurred while creating the solution package "
+                f"{package_type}.  Package data must be provided in a "
+                f"dictionary.  User provided type {type(package_data)}."
+            )
+            raise MFDataException(package=package_type, message=message)
+        # find package - only supporting utl packages for now
+        package_obj = self.package_factory(package_type, "utl")
+        if package_obj is not None:
+            # determine file name
+            if "filename" not in package_data:
+                package_data["filename"] = f"{self.name}.{package_type}"
+            # create package which should automatically register with the
+            # simulation
+            pkg = package_obj(self, **package_data)
+
     @staticmethod
     def _rename_package_group(group_dict, name):
         package_type_count = {}
         # first build an array to avoid key modification errors
         package_array = []
         for package in group_dict.values():
             package_array.append(package)
@@ -1531,15 +1565,15 @@
                 Writes out the simulation in silent mode (verbosity_level = 0)
 
         """
         sim_data = self.simulation_data
         if not sim_data.max_columns_user_set:
             # search for dis packages
             for model in self._models.values():
-                dis = model.get_package("dis")
+                dis = model.get_package("dis", type_only=True)
                 if dis is not None and hasattr(dis, "ncol"):
                     sim_data.max_columns_of_data = dis.ncol.get_data()
                     sim_data.max_columns_user_set = False
                     sim_data.max_columns_auto_set = True
 
         saved_verb_lvl = self.simulation_data.verbosity_level
         if silent:
@@ -1627,14 +1661,15 @@
         silent=None,
         pause=False,
         report=False,
         processors=None,
         normal_msg="normal termination",
         use_async=False,
         cargs=None,
+        custom_print=None,
     ):
         """
         Run the simulation.
 
         Parameters
         ----------
             silent: bool
@@ -1653,14 +1688,19 @@
             use_async : bool
                 Asynchronously read model stdout and report with timestamps.
                 good for models that take long time to run.  not good for
                 models that run really fast
             cargs : str or list of strings
                 Additional command line arguments to pass to the executable.
                 default is None
+            custom_print: callable
+                Optional callbale for printing. It will replace the builtin
+                print function. This is useful for shorter prints or integration
+                into other systems such as GUIs.
+                default is None, i.e. use the builtion print
 
         Returns
         --------
             success : bool
             buff : list of lines of stdout
 
         """
@@ -1679,14 +1719,15 @@
             silent=silent,
             pause=pause,
             report=report,
             processors=processors,
             normal_msg=normal_msg,
             use_async=use_async,
             cargs=cargs,
+            custom_print=custom_print,
         )
 
     def delete_output_files(self):
         """Deletes simulation output files."""
         output_req = binaryfile_utils.MFOutputRequester
         output_file_keys = output_req.getkeys(
             self.simulation_data.mfdata, self.simulation_data.mfpath, False
@@ -1724,14 +1765,25 @@
                 del self._solution_files[package.filename]
                 self._update_solution_group(package.filename)
             if package.filename in self._other_files:
                 del self._other_files[package.filename]
 
             self._remove_package(package)
 
+        # if this is a package referenced from a filerecord, remove filerecord
+        # from name file
+        file_record_name = f"_{package.package_type}_filerecord"
+        if hasattr(self.name_file, file_record_name):
+            file_record = getattr(self.name_file, file_record_name)
+            if isinstance(file_record, mfdata.MFData):
+                file_record.set_data(None)
+            if hasattr(self.name_file, package.package_type):
+                child_pkgs = getattr(self.name_file, package.package_type)
+                child_pkgs._remove_packages(package.filename, True)
+
     @property
     def model_dict(self):
         """
         Return a dictionary of models associated with this simulation.
 
         Returns
         --------
@@ -2097,14 +2149,21 @@
                 # auto generate a unique file name and register it
                 file_name = MFFileMgmt.unique_file_name(
                     package.filename, self._other_files
                 )
                 package.filename = file_name
                 self._other_files[file_name] = package
 
+            # If this package is declared in the namefile options block,
+            # update namefile
+            file_record = f"_{package.package_type}_filerecord"
+            if hasattr(self.name_file, file_record):
+                fr_obj = getattr(self.name_file, file_record)
+                fr_obj.set_data(package.filename)
+
         if package.package_type.lower() in self.structure.package_struct_objs:
             return (
                 path,
                 self.structure.package_struct_objs[
                     package.package_type.lower()
                 ],
             )
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/__init__.py` & `flopy-3.7.0/flopy/mf6/modflow/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,55 @@
 from .mfsimulation import MFSimulation  # isort:skip
 from .mfems import ModflowEms
 from .mfgnc import ModflowGnc
+from .mfgwe import ModflowGwe
+from .mfgweadv import ModflowGweadv
+from .mfgwecnd import ModflowGwecnd
+from .mfgwectp import ModflowGwectp
+from .mfgwedis import ModflowGwedis
+from .mfgwedisu import ModflowGwedisu
+from .mfgwedisv import ModflowGwedisv
+from .mfgweesl import ModflowGweesl
+from .mfgweest import ModflowGweest
+from .mfgwefmi import ModflowGwefmi
+from .mfgwegwe import ModflowGwegwe
+from .mfgweic import ModflowGweic
+from .mfgwelke import ModflowGwelke
+from .mfgwemve import ModflowGwemve
+from .mfgwemwe import ModflowGwemwe
+from .mfgwenam import ModflowGwenam
+from .mfgweoc import ModflowGweoc
+from .mfgwesfe import ModflowGwesfe
+from .mfgwessm import ModflowGwessm
+from .mfgweuze import ModflowGweuze
 from .mfgwf import ModflowGwf
 from .mfgwfapi import ModflowGwfapi
 from .mfgwfbuy import ModflowGwfbuy
 from .mfgwfchd import ModflowGwfchd
 from .mfgwfcsub import ModflowGwfcsub
 from .mfgwfdis import ModflowGwfdis
 from .mfgwfdisu import ModflowGwfdisu
 from .mfgwfdisv import ModflowGwfdisv
 from .mfgwfdrn import ModflowGwfdrn
 from .mfgwfevt import ModflowGwfevt
 from .mfgwfevta import ModflowGwfevta
 from .mfgwfghb import ModflowGwfghb
 from .mfgwfgnc import ModflowGwfgnc
+from .mfgwfgwe import ModflowGwfgwe
 from .mfgwfgwf import ModflowGwfgwf
 from .mfgwfgwt import ModflowGwfgwt
 from .mfgwfhfb import ModflowGwfhfb
 from .mfgwfic import ModflowGwfic
 from .mfgwflak import ModflowGwflak
 from .mfgwfmaw import ModflowGwfmaw
 from .mfgwfmvr import ModflowGwfmvr
 from .mfgwfnam import ModflowGwfnam
 from .mfgwfnpf import ModflowGwfnpf
 from .mfgwfoc import ModflowGwfoc
+from .mfgwfprt import ModflowGwfprt
 from .mfgwfrch import ModflowGwfrch
 from .mfgwfrcha import ModflowGwfrcha
 from .mfgwfriv import ModflowGwfriv
 from .mfgwfsfr import ModflowGwfsfr
 from .mfgwfsto import ModflowGwfsto
 from .mfgwfuzf import ModflowGwfuzf
 from .mfgwfvsc import ModflowGwfvsc
@@ -54,19 +76,31 @@
 from .mfgwtsrc import ModflowGwtsrc
 from .mfgwtssm import ModflowGwtssm
 from .mfgwtuzt import ModflowGwtuzt
 from .mfims import ModflowIms
 from .mfmvr import ModflowMvr
 from .mfmvt import ModflowMvt
 from .mfnam import ModflowNam
+from .mfprt import ModflowPrt
+from .mfprtdis import ModflowPrtdis
+from .mfprtdisv import ModflowPrtdisv
+from .mfprtfmi import ModflowPrtfmi
+from .mfprtmip import ModflowPrtmip
+from .mfprtnam import ModflowPrtnam
+from .mfprtoc import ModflowPrtoc
+from .mfprtprp import ModflowPrtprp
+from .mfpts import ModflowPts
 from .mfsimulation import MFSimulation
 from .mftdis import ModflowTdis
 from .mfutlats import ModflowUtlats
+from .mfutlhpc import ModflowUtlhpc
 from .mfutllaktab import ModflowUtllaktab
 from .mfutlobs import ModflowUtlobs
 from .mfutlsfrtab import ModflowUtlsfrtab
 from .mfutlspc import ModflowUtlspc
 from .mfutlspca import ModflowUtlspca
+from .mfutlspt import ModflowUtlspt
+from .mfutlspta import ModflowUtlspta
 from .mfutltas import ModflowUtltas
 from .mfutlts import ModflowUtlts
 from .mfutltvk import ModflowUtltvk
 from .mfutltvs import ModflowUtltvs
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfems.py` & `flopy-3.7.0/flopy/mf6/modflow/mfems.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 
 
 class ModflowEms(mfpackage.MFPackage):
     """
     ModflowEms defines a ems package.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgnc.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgnc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGnc(mfpackage.MFPackage):
     """
     ModflowGnc defines a gnc package.
 
     Parameters
     ----------
-    simulation : MFSimulation
-        Simulation that this package is a part of. Package is automatically
-        added to simulation when it is initialized.
+    parent_model_or_package : MFModel/MFPackage
+        Parent_model_or_package that this package is a part of. Package is automatically
+        added to parent_model_or_package when it is initialized.
     loading_package : bool
         Do not set this parameter. It is intended for debugging and internal
         processing purposes only.
     print_input : boolean
         * print_input (boolean) keyword to indicate that the list of GNC
           information will be written to the listing file immediately after it
           is read.
@@ -189,28 +189,33 @@
             "in_record true",
             "reader urword",
         ],
     ]
 
     def __init__(
         self,
-        simulation,
+        parent_model_or_package,
         loading_package=False,
         print_input=None,
         print_flows=None,
         explicit=None,
         numgnc=None,
         numalphaj=None,
         gncdata=None,
         filename=None,
         pname=None,
         **kwargs,
     ):
         super().__init__(
-            simulation, "gnc", filename, pname, loading_package, **kwargs
+            parent_model_or_package,
+            "gnc",
+            filename,
+            pname,
+            loading_package,
+            **kwargs,
         )
 
         # set up variables
         self.print_input = self.build_mfdata("print_input", print_input)
         self.print_flows = self.build_mfdata("print_flows", print_flows)
         self.explicit = self.build_mfdata("explicit", explicit)
         self.numgnc = self.build_mfdata("numgnc", numgnc)
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwf.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfmodel
 from ..data.mfdatautil import ArrayTemplateGenerator, ListTemplateGenerator
 
 
 class ModflowGwf(mfmodel.MFModel):
     """
     Modflowgwf defines a gwf model
@@ -48,16 +48,16 @@
     newtonoptions : [under_relaxation]
         * under_relaxation (string) keyword that indicates whether the
           groundwater head in a cell will be under-relaxed when water levels
           fall below the bottom of the model below any given cell. By default,
           Newton-Raphson UNDER_RELAXATION is not applied.
     packages : [ftype, fname, pname]
         * ftype (string) is the file type, which must be one of the following
-          character values shown in table in mf6io.pdf. Ftype may be entered in
-          any combination of uppercase and lowercase.
+          character values shown in table ref{table:ftype-gwf}. Ftype may be
+          entered in any combination of uppercase and lowercase.
         * fname (string) is the name of the file containing the package input.
           The path to the file should be included if the file is not located in
           the folder where the program was run.
         * pname (string) is the user-defined name for the package. PNAME is
           restricted to 16 characters. No spaces are allowed in PNAME. PNAME
           character values are read and stored by the program for stress
           packages only. These names may be useful for labeling purposes when
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwfapi.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwfapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfapi(mfpackage.MFPackage):
     """
     ModflowGwfapi defines a api package within a gwf6 model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwfbuy.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwfbuy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfbuy(mfpackage.MFPackage):
     """
     ModflowGwfbuy defines a buy package within a gwf6 model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwfchd.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwfchd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfchd(mfpackage.MFPackage):
     """
     ModflowGwfchd defines a chd package within a gwf6 model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwfcsub.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwfcsub.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator, ListTemplateGenerator
 
 
 class ModflowGwfcsub(mfpackage.MFPackage):
     """
     ModflowGwfcsub defines a csub package within a gwf6 model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwfdis.py` & `flopy-3.7.0/flopy/mf6/modflow/mfprtdis.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator
 
 
-class ModflowGwfdis(mfpackage.MFPackage):
+class ModflowPrtdis(mfpackage.MFPackage):
     """
-    ModflowGwfdis defines a dis package within a gwf6 model.
+    ModflowPrtdis defines a dis package within a prt6 model.
 
     Parameters
     ----------
     model : MFModel
         Model that this package is a part of. Package is automatically
         added to model when it is initialized.
     loading_package : bool
@@ -38,14 +38,17 @@
           grid in space.
     angrot : double
         * angrot (double) counter-clockwise rotation angle (in degrees) of the
           lower-left corner of the model grid. If not specified, then a default
           value of 0.0 is assigned. The value for ANGROT does not affect the
           model simulation, but it is written to the binary grid file so that
           postprocessors can locate the grid in space.
+    export_array_ascii : boolean
+        * export_array_ascii (boolean) keyword that specifies input griddata
+          arrays should be written to layered ascii output files.
     nlay : integer
         * nlay (integer) is the number of layers in the model grid.
     nrow : integer
         * nrow (integer) is the number of rows in the model grid.
     ncol : integer
         * ncol (integer) is the number of columns in the model grid.
     delr : [double]
@@ -60,38 +63,38 @@
     idomain : [integer]
         * idomain (integer) is an optional array that characterizes the
           existence status of a cell. If the IDOMAIN array is not specified,
           then all model cells exist within the solution. If the IDOMAIN value
           for a cell is 0, the cell does not exist in the simulation. Input and
           output values will be read and written for the cell, but internal to
           the program, the cell is excluded from the solution. If the IDOMAIN
-          value for a cell is 1 or greater, the cell exists in the simulation.
-          If the IDOMAIN value for a cell is -1, the cell does not exist in the
+          value for a cell is 1, the cell exists in the simulation. If the
+          IDOMAIN value for a cell is -1, the cell does not exist in the
           simulation. Furthermore, the first existing cell above will be
           connected to the first existing cell below. This type of cell is
           referred to as a "vertical pass through" cell.
     filename : String
         File name for this package.
     pname : String
         Package name for this package.
     parent_file : MFPackage
         Parent package file that references this package. Only needed for
         utility packages (mfutl*). For example, mfutllaktab package must have
         a mfgwflak package parent_file.
 
     """
 
-    delr = ArrayTemplateGenerator(("gwf6", "dis", "griddata", "delr"))
-    delc = ArrayTemplateGenerator(("gwf6", "dis", "griddata", "delc"))
-    top = ArrayTemplateGenerator(("gwf6", "dis", "griddata", "top"))
-    botm = ArrayTemplateGenerator(("gwf6", "dis", "griddata", "botm"))
-    idomain = ArrayTemplateGenerator(("gwf6", "dis", "griddata", "idomain"))
-    package_abbr = "gwfdis"
+    delr = ArrayTemplateGenerator(("prt6", "dis", "griddata", "delr"))
+    delc = ArrayTemplateGenerator(("prt6", "dis", "griddata", "delc"))
+    top = ArrayTemplateGenerator(("prt6", "dis", "griddata", "top"))
+    botm = ArrayTemplateGenerator(("prt6", "dis", "griddata", "botm"))
+    idomain = ArrayTemplateGenerator(("prt6", "dis", "griddata", "idomain"))
+    package_abbr = "prtdis"
     _package_type = "dis"
-    dfn_file_name = "gwf-dis.dfn"
+    dfn_file_name = "prt-dis.dfn"
 
     dfn = [
         [
             "header",
         ],
         [
             "block options",
@@ -125,14 +128,22 @@
             "block options",
             "name angrot",
             "type double precision",
             "reader urword",
             "optional true",
         ],
         [
+            "block options",
+            "name export_array_ascii",
+            "type keyword",
+            "reader urword",
+            "optional true",
+            "mf6internal export_ascii",
+        ],
+        [
             "block dimensions",
             "name nlay",
             "type integer",
             "reader urword",
             "optional false",
             "default_value 1",
         ],
@@ -201,14 +212,15 @@
         model,
         loading_package=False,
         length_units=None,
         nogrb=None,
         xorigin=None,
         yorigin=None,
         angrot=None,
+        export_array_ascii=None,
         nlay=1,
         nrow=2,
         ncol=2,
         delr=1.0,
         delc=1.0,
         top=1.0,
         botm=0.0,
@@ -223,14 +235,17 @@
 
         # set up variables
         self.length_units = self.build_mfdata("length_units", length_units)
         self.nogrb = self.build_mfdata("nogrb", nogrb)
         self.xorigin = self.build_mfdata("xorigin", xorigin)
         self.yorigin = self.build_mfdata("yorigin", yorigin)
         self.angrot = self.build_mfdata("angrot", angrot)
+        self.export_array_ascii = self.build_mfdata(
+            "export_array_ascii", export_array_ascii
+        )
         self.nlay = self.build_mfdata("nlay", nlay)
         self.nrow = self.build_mfdata("nrow", nrow)
         self.ncol = self.build_mfdata("ncol", ncol)
         self.delr = self.build_mfdata("delr", delr)
         self.delc = self.build_mfdata("delc", delc)
         self.top = self.build_mfdata("top", top)
         self.botm = self.build_mfdata("botm", botm)
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwfdisu.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwfdisu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator, ListTemplateGenerator
 
 
 class ModflowGwfdisu(mfpackage.MFPackage):
     """
     ModflowGwfdisu defines a disu package within a gwf6 model.
@@ -49,14 +49,17 @@
         * vertical_offset_tolerance (double) checks are performed to ensure
           that the top of a cell is not higher than the bottom of an overlying
           cell. This option can be used to specify the tolerance that is used
           for checking. If top of a cell is above the bottom of an overlying
           cell by a value less than this tolerance, then the program will not
           terminate with an error. The default value is zero. This option
           should generally not be used.
+    export_array_ascii : boolean
+        * export_array_ascii (boolean) keyword that specifies input griddata
+          arrays should be written to layered ascii output files.
     nodes : integer
         * nodes (integer) is the number of cells in the model grid.
     nja : integer
         * nja (integer) is the sum of the number of connections and NODES. When
           calculating the total number of connections, the connection between
           cell n and cell m is considered to be different from the connection
           between cell m and cell n. Thus, NJA is equal to the total number of
@@ -138,15 +141,15 @@
         * angldegx (double) is the angle (in degrees) between the horizontal
           x-axis and the outward normal to the face between a cell and its
           connecting cells. The angle varies between zero and 360.0 degrees,
           where zero degrees points in the positive x-axis direction, and 90
           degrees points in the positive y-axis direction. ANGLDEGX is only
           needed if horizontal anisotropy is specified in the NPF Package, if
           the XT3D option is used in the NPF Package, or if the
-          SAVE_SPECIFIC_DISCHARGE option is specifed in the NPF Package.
+          SAVE_SPECIFIC_DISCHARGE option is specified in the NPF Package.
           ANGLDEGX does not need to be specified if these conditions are not
           met. ANGLDEGX is of size NJA; values specified for vertical
           connections and for the diagonal position are not used. Note that
           ANGLDEGX is read in degrees, which is different from MODFLOW-USG,
           which reads a similar variable (ANGLEX) in radians.
     vertices : [iv, xv, yv]
         * iv (integer) is the vertex number. Records in the VERTICES block must
@@ -249,14 +252,22 @@
             "type double precision",
             "reader urword",
             "optional true",
             "default_value 0.0",
             "mf6internal voffsettol",
         ],
         [
+            "block options",
+            "name export_array_ascii",
+            "type keyword",
+            "reader urword",
+            "optional true",
+            "mf6internal export_ascii",
+        ],
+        [
             "block dimensions",
             "name nodes",
             "type integer",
             "reader urword",
             "optional false",
         ],
         [
@@ -452,14 +463,15 @@
         loading_package=False,
         length_units=None,
         nogrb=None,
         xorigin=None,
         yorigin=None,
         angrot=None,
         vertical_offset_tolerance=0.0,
+        export_array_ascii=None,
         nodes=None,
         nja=None,
         nvert=None,
         top=None,
         bot=None,
         area=None,
         idomain=None,
@@ -484,14 +496,17 @@
         self.nogrb = self.build_mfdata("nogrb", nogrb)
         self.xorigin = self.build_mfdata("xorigin", xorigin)
         self.yorigin = self.build_mfdata("yorigin", yorigin)
         self.angrot = self.build_mfdata("angrot", angrot)
         self.vertical_offset_tolerance = self.build_mfdata(
             "vertical_offset_tolerance", vertical_offset_tolerance
         )
+        self.export_array_ascii = self.build_mfdata(
+            "export_array_ascii", export_array_ascii
+        )
         self.nodes = self.build_mfdata("nodes", nodes)
         self.nja = self.build_mfdata("nja", nja)
         self.nvert = self.build_mfdata("nvert", nvert)
         self.top = self.build_mfdata("top", top)
         self.bot = self.build_mfdata("bot", bot)
         self.area = self.build_mfdata("area", area)
         self.idomain = self.build_mfdata("idomain", idomain)
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwfdisv.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwtdisv.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator, ListTemplateGenerator
 
 
-class ModflowGwfdisv(mfpackage.MFPackage):
+class ModflowGwtdisv(mfpackage.MFPackage):
     """
-    ModflowGwfdisv defines a disv package within a gwf6 model.
+    ModflowGwtdisv defines a disv package within a gwt6 model.
 
     Parameters
     ----------
     model : MFModel
         Model that this package is a part of. Package is automatically
         added to model when it is initialized.
     loading_package : bool
@@ -41,14 +41,17 @@
     angrot : double
         * angrot (double) counter-clockwise rotation angle (in degrees) of the
           model grid coordinate system relative to a real-world coordinate
           system. If not specified, then a default value of 0.0 is assigned.
           The value for ANGROT does not affect the model simulation, but it is
           written to the binary grid file so that postprocessors can locate the
           grid in space.
+    export_array_ascii : boolean
+        * export_array_ascii (boolean) keyword that specifies input griddata
+          arrays should be written to layered ascii output files.
     nlay : integer
         * nlay (integer) is the number of layers in the model grid.
     ncpl : integer
         * ncpl (integer) is the number of cells per layer. This is a constant
           value for the grid and it applies to all layers.
     nvert : integer
         * nvert (integer) is the total number of (x, y) vertex pairs used to
@@ -61,16 +64,16 @@
     idomain : [integer]
         * idomain (integer) is an optional array that characterizes the
           existence status of a cell. If the IDOMAIN array is not specified,
           then all model cells exist within the solution. If the IDOMAIN value
           for a cell is 0, the cell does not exist in the simulation. Input and
           output values will be read and written for the cell, but internal to
           the program, the cell is excluded from the solution. If the IDOMAIN
-          value for a cell is 1 or greater, the cell exists in the simulation.
-          If the IDOMAIN value for a cell is -1, the cell does not exist in the
+          value for a cell is 1, the cell exists in the simulation. If the
+          IDOMAIN value for a cell is -1, the cell does not exist in the
           simulation. Furthermore, the first existing cell above will be
           connected to the first existing cell below. This type of cell is
           referred to as a "vertical pass through" cell.
     vertices : [iv, xv, yv]
         * iv (integer) is the vertex number. Records in the VERTICES block must
           be listed in consecutive order from 1 to NVERT. This argument is an
           index variable, which means that it should be treated as zero-based
@@ -104,22 +107,22 @@
     parent_file : MFPackage
         Parent package file that references this package. Only needed for
         utility packages (mfutl*). For example, mfutllaktab package must have
         a mfgwflak package parent_file.
 
     """
 
-    top = ArrayTemplateGenerator(("gwf6", "disv", "griddata", "top"))
-    botm = ArrayTemplateGenerator(("gwf6", "disv", "griddata", "botm"))
-    idomain = ArrayTemplateGenerator(("gwf6", "disv", "griddata", "idomain"))
-    vertices = ListTemplateGenerator(("gwf6", "disv", "vertices", "vertices"))
-    cell2d = ListTemplateGenerator(("gwf6", "disv", "cell2d", "cell2d"))
-    package_abbr = "gwfdisv"
+    top = ArrayTemplateGenerator(("gwt6", "disv", "griddata", "top"))
+    botm = ArrayTemplateGenerator(("gwt6", "disv", "griddata", "botm"))
+    idomain = ArrayTemplateGenerator(("gwt6", "disv", "griddata", "idomain"))
+    vertices = ListTemplateGenerator(("gwt6", "disv", "vertices", "vertices"))
+    cell2d = ListTemplateGenerator(("gwt6", "disv", "cell2d", "cell2d"))
+    package_abbr = "gwtdisv"
     _package_type = "disv"
-    dfn_file_name = "gwf-disv.dfn"
+    dfn_file_name = "gwt-disv.dfn"
 
     dfn = [
         [
             "header",
         ],
         [
             "block options",
@@ -153,14 +156,22 @@
             "block options",
             "name angrot",
             "type double precision",
             "reader urword",
             "optional true",
         ],
         [
+            "block options",
+            "name export_array_ascii",
+            "type keyword",
+            "reader urword",
+            "optional true",
+            "mf6internal export_ascii",
+        ],
+        [
             "block dimensions",
             "name nlay",
             "type integer",
             "reader urword",
             "optional false",
         ],
         [
@@ -300,14 +311,15 @@
         model,
         loading_package=False,
         length_units=None,
         nogrb=None,
         xorigin=None,
         yorigin=None,
         angrot=None,
+        export_array_ascii=None,
         nlay=None,
         ncpl=None,
         nvert=None,
         top=None,
         botm=None,
         idomain=None,
         vertices=None,
@@ -322,14 +334,17 @@
 
         # set up variables
         self.length_units = self.build_mfdata("length_units", length_units)
         self.nogrb = self.build_mfdata("nogrb", nogrb)
         self.xorigin = self.build_mfdata("xorigin", xorigin)
         self.yorigin = self.build_mfdata("yorigin", yorigin)
         self.angrot = self.build_mfdata("angrot", angrot)
+        self.export_array_ascii = self.build_mfdata(
+            "export_array_ascii", export_array_ascii
+        )
         self.nlay = self.build_mfdata("nlay", nlay)
         self.ncpl = self.build_mfdata("ncpl", ncpl)
         self.nvert = self.build_mfdata("nvert", nvert)
         self.top = self.build_mfdata("top", top)
         self.botm = self.build_mfdata("botm", botm)
         self.idomain = self.build_mfdata("idomain", idomain)
         self.vertices = self.build_mfdata("vertices", vertices)
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwfdrn.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwfdrn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfdrn(mfpackage.MFPackage):
     """
     ModflowGwfdrn defines a drn package within a gwf6 model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwfevt.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwfevt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfevt(mfpackage.MFPackage):
     """
     ModflowGwfevt defines a evt package within a gwf6 model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwfevta.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwfevta.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator, ListTemplateGenerator
 
 
 class ModflowGwfevta(mfpackage.MFPackage):
     """
     ModflowGwfevta defines a evta package within a gwf6 model.
@@ -16,15 +16,19 @@
         added to model when it is initialized.
     loading_package : bool
         Do not set this parameter. It is intended for debugging and internal
         processing purposes only.
     readasarrays : boolean
         * readasarrays (boolean) indicates that array-based input will be used
           for the Evapotranspiration Package. This keyword must be specified to
-          use array-based input.
+          use array-based input. When READASARRAYS is specified, values must be
+          provided for every cell within a model layer, even those cells that
+          have an IDOMAIN value less than one. Values assigned to cells with
+          IDOMAIN values less than one are not used and have no effect on
+          simulation results.
     fixed_cell : boolean
         * fixed_cell (boolean) indicates that evapotranspiration will not be
           reassigned to a cell underlying the cell specified in the list if the
           specified cell is inactive.
     auxiliary : [string]
         * auxiliary (string) defines an array of one or more auxiliary variable
           names. There is no limit on the number of auxiliary variables that
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwfghb.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwfghb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfghb(mfpackage.MFPackage):
     """
     ModflowGwfghb defines a ghb package within a gwf6 model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwfgnc.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwfgnc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfgnc(mfpackage.MFPackage):
     """
     ModflowGwfgnc defines a gnc package within a gwf6 model.
 
     Parameters
     ----------
-    model : MFModel
-        Model that this package is a part of. Package is automatically
-        added to model when it is initialized.
+    parent_model_or_package : MFModel/MFPackage
+        Parent_model_or_package that this package is a part of. Package is automatically
+        added to parent_model_or_package when it is initialized.
     loading_package : bool
         Do not set this parameter. It is intended for debugging and internal
         processing purposes only.
     print_input : boolean
         * print_input (boolean) keyword to indicate that the list of GNC
           information will be written to the listing file immediately after it
           is read.
@@ -189,28 +189,33 @@
             "in_record true",
             "reader urword",
         ],
     ]
 
     def __init__(
         self,
-        model,
+        parent_model_or_package,
         loading_package=False,
         print_input=None,
         print_flows=None,
         explicit=None,
         numgnc=None,
         numalphaj=None,
         gncdata=None,
         filename=None,
         pname=None,
         **kwargs,
     ):
         super().__init__(
-            model, "gnc", filename, pname, loading_package, **kwargs
+            parent_model_or_package,
+            "gnc",
+            filename,
+            pname,
+            loading_package,
+            **kwargs,
         )
 
         # set up variables
         self.print_input = self.build_mfdata("print_input", print_input)
         self.print_flows = self.build_mfdata("print_flows", print_flows)
         self.explicit = self.build_mfdata("explicit", explicit)
         self.numgnc = self.build_mfdata("numgnc", numgnc)
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwfgwf.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwfgwf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfgwf(mfpackage.MFPackage):
     """
     ModflowGwfgwf defines a gwfgwf package.
@@ -30,21 +30,25 @@
           they will be available for use by other parts of the program. If an
           auxiliary variable with the name "ANGLDEGX" is found, then this
           information will be used as the angle (provided in degrees) between
           the connection face normal and the x axis, where a value of zero
           indicates that a normal vector points directly along the positive x
           axis. The connection face normal is a normal vector on the cell face
           shared between the cell in model 1 and the cell in model 2 pointing
-          away from the model 1 cell. Additional information on "ANGLDEGX" is
-          provided in the description of the DISU Package. If an auxiliary
-          variable with the name "CDIST" is found, then this information will
-          be used as the straight-line connection distance, including the
-          vertical component, between the two cell centers. Both ANGLDEGX and
-          CDIST are required if specific discharge is calculated for either of
-          the groundwater models.
+          away from the model 1 cell. Additional information on "ANGLDEGX" and
+          when it is required is provided in the description of the DISU
+          Package. If an auxiliary variable with the name "CDIST" is found,
+          then this information will be used in the calculation of specific
+          discharge within model cells connected by the exchange. For a
+          horizontal connection, CDIST should be specified as the horizontal
+          distance between the cell centers, and should not include the
+          vertical component. For vertical connections, CDIST should be
+          specified as the difference in elevation between the two cell
+          centers. Both ANGLDEGX and CDIST are required if specific discharge
+          is calculated for either of the groundwater models.
     boundnames : boolean
         * boundnames (boolean) keyword to indicate that boundary names may be
           provided with the list of GWF Exchange cells.
     print_input : boolean
         * print_input (boolean) keyword to indicate that the list of exchange
           entries will be echoed to the listing file immediately after it is
           read.
@@ -448,14 +452,15 @@
             "name aux",
             "type double precision",
             "in_record true",
             "tagged false",
             "shape (naux)",
             "reader urword",
             "optional true",
+            "mf6internal auxvar",
         ],
         [
             "block exchangedata",
             "name boundname",
             "type string",
             "shape",
             "tagged false",
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwfgwt.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwfprt.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 
 
-class ModflowGwfgwt(mfpackage.MFPackage):
+class ModflowGwfprt(mfpackage.MFPackage):
     """
-    ModflowGwfgwt defines a gwfgwt package.
+    ModflowGwfprt defines a gwfprt package.
 
     Parameters
     ----------
     simulation : MFSimulation
         Simulation that this package is a part of. Package is automatically
         added to simulation when it is initialized.
     loading_package : bool
@@ -29,37 +29,37 @@
     parent_file : MFPackage
         Parent package file that references this package. Only needed for
         utility packages (mfutl*). For example, mfutllaktab package must have
         a mfgwflak package parent_file.
 
     """
 
-    package_abbr = "gwfgwt"
-    _package_type = "gwfgwt"
-    dfn_file_name = "exg-gwfgwt.dfn"
+    package_abbr = "gwfprt"
+    _package_type = "gwfprt"
+    dfn_file_name = "exg-gwfprt.dfn"
 
     dfn = [
         [
             "header",
         ],
     ]
 
     def __init__(
         self,
         simulation,
         loading_package=False,
-        exgtype="GWF6-GWT6",
+        exgtype="GWF6-PRT6",
         exgmnamea=None,
         exgmnameb=None,
         filename=None,
         pname=None,
         **kwargs,
     ):
         super().__init__(
-            simulation, "gwfgwt", filename, pname, loading_package, **kwargs
+            simulation, "gwfprt", filename, pname, loading_package, **kwargs
         )
 
         # set up variables
         self.exgtype = exgtype
 
         self.exgmnamea = exgmnamea
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwfhfb.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwfhfb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfhfb(mfpackage.MFPackage):
     """
     ModflowGwfhfb defines a hfb package within a gwf6 model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwfic.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgweic.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,77 +1,86 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator
 
 
-class ModflowGwfic(mfpackage.MFPackage):
+class ModflowGweic(mfpackage.MFPackage):
     """
-    ModflowGwfic defines a ic package within a gwf6 model.
+    ModflowGweic defines a ic package within a gwe6 model.
 
     Parameters
     ----------
     model : MFModel
         Model that this package is a part of. Package is automatically
         added to model when it is initialized.
     loading_package : bool
         Do not set this parameter. It is intended for debugging and internal
         processing purposes only.
+    export_array_ascii : boolean
+        * export_array_ascii (boolean) keyword that specifies input griddata
+          arrays should be written to layered ascii output files.
     strt : [double]
-        * strt (double) is the initial (starting) head---that is, head at the
-          beginning of the GWF Model simulation. STRT must be specified for all
-          simulations, including steady-state simulations. One value is read
-          for every model cell. For simulations in which the first stress
-          period is steady state, the values used for STRT generally do not
-          affect the simulation (exceptions may occur if cells go dry and (or)
-          rewet). The execution time, however, will be less if STRT includes
-          hydraulic heads that are close to the steady-state solution. A head
-          value lower than the cell bottom can be provided if a cell should
-          start as dry.
+        * strt (double) is the initial (starting) temperature---that is, the
+          temperature at the beginning of the GWE Model simulation. STRT must
+          be specified for all GWE Model simulations. One value is read for
+          every model cell.
     filename : String
         File name for this package.
     pname : String
         Package name for this package.
     parent_file : MFPackage
         Parent package file that references this package. Only needed for
         utility packages (mfutl*). For example, mfutllaktab package must have
         a mfgwflak package parent_file.
 
     """
 
-    strt = ArrayTemplateGenerator(("gwf6", "ic", "griddata", "strt"))
-    package_abbr = "gwfic"
+    strt = ArrayTemplateGenerator(("gwe6", "ic", "griddata", "strt"))
+    package_abbr = "gweic"
     _package_type = "ic"
-    dfn_file_name = "gwf-ic.dfn"
+    dfn_file_name = "gwe-ic.dfn"
 
     dfn = [
         [
             "header",
         ],
         [
+            "block options",
+            "name export_array_ascii",
+            "type keyword",
+            "reader urword",
+            "optional true",
+            "mf6internal export_ascii",
+        ],
+        [
             "block griddata",
             "name strt",
             "type double precision",
             "shape (nodes)",
             "reader readarray",
             "layered true",
-            "default_value 1.0",
+            "default_value 0.0",
         ],
     ]
 
     def __init__(
         self,
         model,
         loading_package=False,
-        strt=1.0,
+        export_array_ascii=None,
+        strt=0.0,
         filename=None,
         pname=None,
         **kwargs,
     ):
         super().__init__(
             model, "ic", filename, pname, loading_package, **kwargs
         )
 
         # set up variables
+        self.export_array_ascii = self.build_mfdata(
+            "export_array_ascii", export_array_ascii
+        )
         self.strt = self.build_mfdata("strt", strt)
         self._init_complete = True
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwflak.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwflak.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwflak(mfpackage.MFPackage):
     """
     ModflowGwflak defines a lak package within a gwf6 model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwfmaw.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwfmaw.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfmaw(mfpackage.MFPackage):
     """
     ModflowGwfmaw defines a maw package within a gwf6 model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwfmvr.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwfmvr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfmvr(mfpackage.MFPackage):
     """
     ModflowGwfmvr defines a mvr package within a gwf6 model. This package
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwfnam.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwfnam.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfnam(mfpackage.MFPackage):
     """
     ModflowGwfnam defines a nam package within a gwf6 model.
@@ -41,16 +41,16 @@
     newtonoptions : [under_relaxation]
         * under_relaxation (string) keyword that indicates whether the
           groundwater head in a cell will be under-relaxed when water levels
           fall below the bottom of the model below any given cell. By default,
           Newton-Raphson UNDER_RELAXATION is not applied.
     packages : [ftype, fname, pname]
         * ftype (string) is the file type, which must be one of the following
-          character values shown in table in mf6io.pdf. Ftype may be entered in
-          any combination of uppercase and lowercase.
+          character values shown in table ref{table:ftype-gwf}. Ftype may be
+          entered in any combination of uppercase and lowercase.
         * fname (string) is the name of the file containing the package input.
           The path to the file should be included if the file is not located in
           the folder where the program was run.
         * pname (string) is the user-defined name for the package. PNAME is
           restricted to 16 characters. No spaces are allowed in PNAME. PNAME
           character values are read and stored by the program for stress
           packages only. These names may be useful for labeling purposes when
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwfnpf.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwfnpf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator, ListTemplateGenerator
 
 
 class ModflowGwfnpf(mfpackage.MFPackage):
     """
     ModflowGwfnpf defines a npf package within a gwf6 model.
@@ -104,25 +104,19 @@
           of K33 divided by K. If this option is specified, then the K33 array
           entered in the NPF Package will be multiplied by K after being read.
     perioddata : {varname:data} or tvk_perioddata data
         * Contains data for the tvk package. Data can be stored in a dictionary
           containing data for the tvk package with variable names as keys and
           package data as values. Data just for the perioddata variable is also
           acceptable. See tvk package documentation for more information.
+    export_array_ascii : boolean
+        * export_array_ascii (boolean) keyword that specifies input griddata
+          arrays should be written to layered ascii output files.
     dev_no_newton : boolean
         * dev_no_newton (boolean) turn off Newton for unconfined cells
-    dev_modflowusg_upstream_weighted_saturation : boolean
-        * dev_modflowusg_upstream_weighted_saturation (boolean) use MODFLOW-USG
-          upstream-weighted saturation approach
-    dev_modflownwt_upstream_weighting : boolean
-        * dev_modflownwt_upstream_weighting (boolean) use MODFLOW-NWT approach
-          for upstream weighting
-    dev_minimum_saturated_thickness : double
-        * dev_minimum_saturated_thickness (double) set minimum allowed
-          saturated thickness
     dev_omega : double
         * dev_omega (double) set saturation omega value
     icelltype : [integer]
         * icelltype (integer) flag for each cell that specifies how saturated
           thickness is treated. 0 means saturated thickness is held constant;
           >0 means saturated thickness varies with computed head when head is
           below the cell top; <0 means saturated thickness varies with computed
@@ -451,43 +445,27 @@
             "in_record true",
             "reader urword",
             "optional false",
             "tagged false",
         ],
         [
             "block options",
-            "name dev_no_newton",
-            "type keyword",
-            "reader urword",
-            "optional true",
-            "mf6internal inewton",
-        ],
-        [
-            "block options",
-            "name dev_modflowusg_upstream_weighted_saturation",
+            "name export_array_ascii",
             "type keyword",
             "reader urword",
             "optional true",
-            "mf6internal iusgnrhc",
+            "mf6internal export_ascii",
         ],
         [
             "block options",
-            "name dev_modflownwt_upstream_weighting",
+            "name dev_no_newton",
             "type keyword",
             "reader urword",
             "optional true",
-            "mf6internal inwtupw",
-        ],
-        [
-            "block options",
-            "name dev_minimum_saturated_thickness",
-            "type double precision",
-            "reader urword",
-            "optional true",
-            "mf6internal satmin",
+            "mf6internal inewton",
         ],
         [
             "block options",
             "name dev_omega",
             "type double precision",
             "reader urword",
             "optional true",
@@ -590,18 +568,16 @@
         rewet_record=None,
         xt3doptions=None,
         save_specific_discharge=None,
         save_saturation=None,
         k22overk=None,
         k33overk=None,
         perioddata=None,
+        export_array_ascii=None,
         dev_no_newton=None,
-        dev_modflowusg_upstream_weighted_saturation=None,
-        dev_modflownwt_upstream_weighting=None,
-        dev_minimum_saturated_thickness=None,
         dev_omega=None,
         icelltype=0,
         k=1.0,
         k22=None,
         k33=None,
         angle1=None,
         angle2=None,
@@ -634,26 +610,18 @@
         )
         self.k22overk = self.build_mfdata("k22overk", k22overk)
         self.k33overk = self.build_mfdata("k33overk", k33overk)
         self._tvk_filerecord = self.build_mfdata("tvk_filerecord", None)
         self._tvk_package = self.build_child_package(
             "tvk", perioddata, "tvk_perioddata", self._tvk_filerecord
         )
-        self.dev_no_newton = self.build_mfdata("dev_no_newton", dev_no_newton)
-        self.dev_modflowusg_upstream_weighted_saturation = self.build_mfdata(
-            "dev_modflowusg_upstream_weighted_saturation",
-            dev_modflowusg_upstream_weighted_saturation,
-        )
-        self.dev_modflownwt_upstream_weighting = self.build_mfdata(
-            "dev_modflownwt_upstream_weighting",
-            dev_modflownwt_upstream_weighting,
-        )
-        self.dev_minimum_saturated_thickness = self.build_mfdata(
-            "dev_minimum_saturated_thickness", dev_minimum_saturated_thickness
+        self.export_array_ascii = self.build_mfdata(
+            "export_array_ascii", export_array_ascii
         )
+        self.dev_no_newton = self.build_mfdata("dev_no_newton", dev_no_newton)
         self.dev_omega = self.build_mfdata("dev_omega", dev_omega)
         self.icelltype = self.build_mfdata("icelltype", icelltype)
         self.k = self.build_mfdata("k", k)
         self.k22 = self.build_mfdata("k22", k22)
         self.k33 = self.build_mfdata("k33", k33)
         self.angle1 = self.build_mfdata("angle1", angle1)
         self.angle2 = self.build_mfdata("angle2", angle2)
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwfoc.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwfoc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfoc(mfpackage.MFPackage):
     """
     ModflowGwfoc defines a oc package within a gwf6 model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwfrch.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwfrch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfrch(mfpackage.MFPackage):
     """
     ModflowGwfrch defines a rch package within a gwf6 model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwfrcha.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwfrcha.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator, ListTemplateGenerator
 
 
 class ModflowGwfrcha(mfpackage.MFPackage):
     """
     ModflowGwfrcha defines a rcha package within a gwf6 model.
@@ -16,15 +16,19 @@
         added to model when it is initialized.
     loading_package : bool
         Do not set this parameter. It is intended for debugging and internal
         processing purposes only.
     readasarrays : boolean
         * readasarrays (boolean) indicates that array-based input will be used
           for the Recharge Package. This keyword must be specified to use
-          array-based input.
+          array-based input. When READASARRAYS is specified, values must be
+          provided for every cell within a model layer, even those cells that
+          have an IDOMAIN value less than one. Values assigned to cells with
+          IDOMAIN values less than one are not used and have no effect on
+          simulation results.
     fixed_cell : boolean
         * fixed_cell (boolean) indicates that recharge will not be reassigned
           to a cell underlying the cell specified in the list if the specified
           cell is inactive.
     auxiliary : [string]
         * auxiliary (string) defines an array of one or more auxiliary variable
           names. There is no limit on the number of auxiliary variables that
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwfriv.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwfriv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfriv(mfpackage.MFPackage):
     """
     ModflowGwfriv defines a riv package within a gwf6 model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwfsfr.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwfsfr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfsfr(mfpackage.MFPackage):
     """
     ModflowGwfsfr defines a sfr package within a gwf6 model.
@@ -167,18 +167,21 @@
         * rgrd (double) real value that defines the stream gradient (slope)
           across the reach. RGRD must be greater than zero.
         * rtp (double) real value that defines the bottom elevation of the
           reach.
         * rbth (double) real value that defines the thickness of the reach
           streambed. RBTH can be any value if the reach is not connected to an
           underlying GWF cell. Otherwise, RBTH must be greater than zero.
-        * rhk (double) real value that defines the hydraulic conductivity of
-          the reach streambed. RHK can be any positive value if the reach is
-          not connected to an underlying GWF cell. Otherwise, RHK must be
-          greater than zero.
+        * rhk (double) real or character value that defines the hydraulic
+          conductivity of the reach streambed. RHK can be any positive value if
+          the reach is not connected to an underlying GWF cell. Otherwise, RHK
+          must be greater than zero. If the Options block includes a
+          TIMESERIESFILE entry (see the "Time-Variable Input" section), values
+          can be obtained from a time series by entering the time-series name
+          in place of a numeric value.
         * man (string) real or character value that defines the Manning's
           roughness coefficient for the reach. MAN must be greater than zero.
           If the Options block includes a TIMESERIESFILE entry (see the "Time-
           Variable Input" section), values can be obtained from a time series
           by entering the time-series name in place of a numeric value.
         * ncon (integer) integer value that defines the number of reaches
           connected to the reach. If a value of zero is specified for NCON an
@@ -306,16 +309,17 @@
           greater than zero and less than or equal to NREACHES. This argument
           is an index variable, which means that it should be treated as zero-
           based when working with FloPy and Python. Flopy will automatically
           subtract one when loading index variables and add one when writing
           index variables.
         * sfrsetting (keystring) line of information that is parsed into a
           keyword and values. Keyword values that can be used to start the
-          SFRSETTING string include: STATUS, MANNING, STAGE, INFLOW, RAINFALL,
-          EVAPORATION, RUNOFF, DIVERSION, UPSTREAM_FRACTION, and AUXILIARY.
+          SFRSETTING string include: STATUS, BEDK, MANNING, STAGE, INFLOW,
+          RAINFALL, EVAPORATION, RUNOFF, DIVERSION, UPSTREAM_FRACTION, and
+          AUXILIARY.
             status : [string]
                 * status (string) keyword option to define stream reach status.
                   STATUS can be ACTIVE, INACTIVE, or SIMPLE. The SIMPLE STATUS
                   option simulates streamflow using a user-specified stage for
                   a reach or a stage set to the top of the reach (depth = 0).
                   In cases where the simulated leakage calculated using the
                   specified stage exceeds the sum of inflows to the reach, the
@@ -325,14 +329,23 @@
                   or more reaches is changed to ACTIVE or INACTIVE. For
                   example, if one of two downstream connections for a reach is
                   inactivated, the upstream fraction for the active and
                   inactive downstream reach should be changed to 1.0 and 0.0,
                   respectively, to ensure that the active reach receives all of
                   the downstream outflow from the upstream reach. By default,
                   STATUS is ACTIVE.
+            bedk : [string]
+                * bedk (string) real or character value that defines the
+                  hydraulic conductivity of the reach streambed. BEDK can be
+                  any positive value if the reach is not connected to an
+                  underlying GWF cell. Otherwise, BEDK must be greater than
+                  zero. If the Options block includes a TIMESERIESFILE entry
+                  (see the "Time-Variable Input" section), values can be
+                  obtained from a time series by entering the time-series name
+                  in place of a numeric value.
             manning : [string]
                 * manning (string) real or character value that defines the
                   Manning's roughness coefficient for the reach. MANNING must
                   be greater than zero. If the Options block includes a
                   TIMESERIESFILE entry (see the "Time-Variable Input" section),
                   values can be obtained from a time series by entering the
                   time-series name in place of a numeric value.
@@ -859,14 +872,15 @@
             "block packagedata",
             "name rhk",
             "type double precision",
             "shape",
             "tagged false",
             "in_record true",
             "reader urword",
+            "time_series true",
         ],
         [
             "block packagedata",
             "name man",
             "type string",
             "shape",
             "tagged false",
@@ -1075,17 +1089,17 @@
             "in_record true",
             "reader urword",
             "numeric_index true",
         ],
         [
             "block period",
             "name sfrsetting",
-            "type keystring status manning stage inflow rainfall evaporation "
-            "runoff diversionrecord upstream_fraction cross_sectionrecord "
-            "auxiliaryrecord",
+            "type keystring status bedk manning stage inflow rainfall "
+            "evaporation runoff diversionrecord upstream_fraction "
+            "cross_sectionrecord auxiliaryrecord",
             "shape",
             "tagged false",
             "in_record true",
             "reader urword",
         ],
         [
             "block period",
@@ -1094,14 +1108,24 @@
             "shape",
             "tagged true",
             "in_record true",
             "reader urword",
         ],
         [
             "block period",
+            "name bedk",
+            "type string",
+            "shape",
+            "tagged true",
+            "in_record true",
+            "reader urword",
+            "time_series true",
+        ],
+        [
+            "block period",
             "name manning",
             "type string",
             "shape",
             "tagged true",
             "in_record true",
             "reader urword",
             "time_series true",
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwfsto.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwfsto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator, ListTemplateGenerator
 
 
 class ModflowGwfsto(mfpackage.MFPackage):
     """
     ModflowGwfsto defines a sto package within a gwf6 model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwfuzf.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwfuzf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfuzf(mfpackage.MFPackage):
     """
     ModflowGwfuzf defines a uzf package within a gwf6 model.
@@ -582,14 +582,15 @@
         [
             "block options",
             "name simulate_gwseep",
             "type keyword",
             "tagged true",
             "reader urword",
             "optional true",
+            "deprecated 6.5.0",
         ],
         [
             "block options",
             "name unsat_etwc",
             "type keyword",
             "tagged true",
             "reader urword",
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwfvsc.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwfvsc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfvsc(mfpackage.MFPackage):
     """
     ModflowGwfvsc defines a vsc package within a gwf6 model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwfwel.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwfwel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwfwel(mfpackage.MFPackage):
     """
     ModflowGwfwel defines a wel package within a gwf6 model.
@@ -55,15 +55,19 @@
           fraction of the cell thickness used as an interval for smoothly
           adjusting negative pumping rates to 0 in cells with head values less
           than or equal to the bottom of the cell. Negative pumping rates are
           adjusted to 0 or a smaller negative value when the head in the cell
           is equal to or less than the calculated interval above the cell
           bottom. AUTO_FLOW_REDUCE is set to 0.1 if the specified value is less
           than or equal to zero. By default, negative pumping rates are not
-          reduced during a simulation.
+          reduced during a simulation. This AUTO_FLOW_REDUCE option only
+          applies to wells in model cells that are marked as "convertible"
+          (ICELLTYPE /= 0) in the Node Property Flow (NPF) input file.
+          Reduction in flow will not occur for wells in cells marked as
+          confined (ICELLTYPE = 0).
     afrcsv_filerecord : [afrcsvfile]
         * afrcsvfile (string) name of the comma-separated value (CSV) output
           file to write information about well extraction rates that have been
           reduced by the program. Entries are only written if the extraction
           rates are reduced.
     timeseries : {varname:data} or timeseries data
         * Contains data for the ts package. Data can be stored in a dictionary
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwt.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfmodel
 from ..data.mfdatautil import ArrayTemplateGenerator, ListTemplateGenerator
 
 
 class ModflowGwt(mfmodel.MFModel):
     """
     Modflowgwt defines a gwt model
@@ -43,16 +43,16 @@
           time step of each stress period.
     save_flows : boolean
         * save_flows (boolean) keyword to indicate that all model package flow
           terms will be written to the file specified with "BUDGET FILEOUT" in
           Output Control.
     packages : [ftype, fname, pname]
         * ftype (string) is the file type, which must be one of the following
-          character values shown in table in mf6io.pdf. Ftype may be entered in
-          any combination of uppercase and lowercase.
+          character values shown in table ref{table:ftype-gwt}. Ftype may be
+          entered in any combination of uppercase and lowercase.
         * fname (string) is the name of the file containing the package input.
           The path to the file should be included if the file is not located in
           the folder where the program was run.
         * pname (string) is the user-defined name for the package. PNAME is
           restricted to 16 characters. No spaces are allowed in PNAME. PNAME
           character values are read and stored by the program for stress
           packages only. These names may be useful for labeling purposes when
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwtadv.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwtadv.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 
 
 class ModflowGwtadv(mfpackage.MFPackage):
     """
     ModflowGwtadv defines a adv package within a gwt6 model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwtapi.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwtapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwtapi(mfpackage.MFPackage):
     """
     ModflowGwtapi defines a api package within a gwt6 model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwtcnc.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwtcnc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwtcnc(mfpackage.MFPackage):
     """
     ModflowGwtcnc defines a cnc package within a gwt6 model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwtdis.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwedis.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator
 
 
-class ModflowGwtdis(mfpackage.MFPackage):
+class ModflowGwedis(mfpackage.MFPackage):
     """
-    ModflowGwtdis defines a dis package within a gwt6 model.
+    ModflowGwedis defines a dis package within a gwe6 model.
 
     Parameters
     ----------
     model : MFModel
         Model that this package is a part of. Package is automatically
         added to model when it is initialized.
     loading_package : bool
@@ -38,14 +38,17 @@
           grid in space.
     angrot : double
         * angrot (double) counter-clockwise rotation angle (in degrees) of the
           lower-left corner of the model grid. If not specified, then a default
           value of 0.0 is assigned. The value for ANGROT does not affect the
           model simulation, but it is written to the binary grid file so that
           postprocessors can locate the grid in space.
+    export_array_ascii : boolean
+        * export_array_ascii (boolean) keyword that specifies input griddata
+          arrays should be written to layered ascii output files.
     nlay : integer
         * nlay (integer) is the number of layers in the model grid.
     nrow : integer
         * nrow (integer) is the number of rows in the model grid.
     ncol : integer
         * ncol (integer) is the number of columns in the model grid.
     delr : [double]
@@ -76,22 +79,22 @@
     parent_file : MFPackage
         Parent package file that references this package. Only needed for
         utility packages (mfutl*). For example, mfutllaktab package must have
         a mfgwflak package parent_file.
 
     """
 
-    delr = ArrayTemplateGenerator(("gwt6", "dis", "griddata", "delr"))
-    delc = ArrayTemplateGenerator(("gwt6", "dis", "griddata", "delc"))
-    top = ArrayTemplateGenerator(("gwt6", "dis", "griddata", "top"))
-    botm = ArrayTemplateGenerator(("gwt6", "dis", "griddata", "botm"))
-    idomain = ArrayTemplateGenerator(("gwt6", "dis", "griddata", "idomain"))
-    package_abbr = "gwtdis"
+    delr = ArrayTemplateGenerator(("gwe6", "dis", "griddata", "delr"))
+    delc = ArrayTemplateGenerator(("gwe6", "dis", "griddata", "delc"))
+    top = ArrayTemplateGenerator(("gwe6", "dis", "griddata", "top"))
+    botm = ArrayTemplateGenerator(("gwe6", "dis", "griddata", "botm"))
+    idomain = ArrayTemplateGenerator(("gwe6", "dis", "griddata", "idomain"))
+    package_abbr = "gwedis"
     _package_type = "dis"
-    dfn_file_name = "gwt-dis.dfn"
+    dfn_file_name = "gwe-dis.dfn"
 
     dfn = [
         [
             "header",
         ],
         [
             "block options",
@@ -125,14 +128,22 @@
             "block options",
             "name angrot",
             "type double precision",
             "reader urword",
             "optional true",
         ],
         [
+            "block options",
+            "name export_array_ascii",
+            "type keyword",
+            "reader urword",
+            "optional true",
+            "mf6internal export_ascii",
+        ],
+        [
             "block dimensions",
             "name nlay",
             "type integer",
             "reader urword",
             "optional false",
             "default_value 1",
         ],
@@ -201,14 +212,15 @@
         model,
         loading_package=False,
         length_units=None,
         nogrb=None,
         xorigin=None,
         yorigin=None,
         angrot=None,
+        export_array_ascii=None,
         nlay=1,
         nrow=2,
         ncol=2,
         delr=1.0,
         delc=1.0,
         top=1.0,
         botm=0.0,
@@ -223,14 +235,17 @@
 
         # set up variables
         self.length_units = self.build_mfdata("length_units", length_units)
         self.nogrb = self.build_mfdata("nogrb", nogrb)
         self.xorigin = self.build_mfdata("xorigin", xorigin)
         self.yorigin = self.build_mfdata("yorigin", yorigin)
         self.angrot = self.build_mfdata("angrot", angrot)
+        self.export_array_ascii = self.build_mfdata(
+            "export_array_ascii", export_array_ascii
+        )
         self.nlay = self.build_mfdata("nlay", nlay)
         self.nrow = self.build_mfdata("nrow", nrow)
         self.ncol = self.build_mfdata("ncol", ncol)
         self.delr = self.build_mfdata("delr", delr)
         self.delc = self.build_mfdata("delc", delc)
         self.top = self.build_mfdata("top", top)
         self.botm = self.build_mfdata("botm", botm)
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwtdisu.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwtdisu.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator, ListTemplateGenerator
 
 
 class ModflowGwtdisu(mfpackage.MFPackage):
     """
     ModflowGwtdisu defines a disu package within a gwt6 model.
@@ -49,14 +49,17 @@
         * vertical_offset_tolerance (double) checks are performed to ensure
           that the top of a cell is not higher than the bottom of an overlying
           cell. This option can be used to specify the tolerance that is used
           for checking. If top of a cell is above the bottom of an overlying
           cell by a value less than this tolerance, then the program will not
           terminate with an error. The default value is zero. This option
           should generally not be used.
+    export_array_ascii : boolean
+        * export_array_ascii (boolean) keyword that specifies input griddata
+          arrays should be written to layered ascii output files.
     nodes : integer
         * nodes (integer) is the number of cells in the model grid.
     nja : integer
         * nja (integer) is the sum of the number of connections and NODES. When
           calculating the total number of connections, the connection between
           cell n and cell m is considered to be different from the connection
           between cell m and cell n. Thus, NJA is equal to the total number of
@@ -138,15 +141,15 @@
         * angldegx (double) is the angle (in degrees) between the horizontal
           x-axis and the outward normal to the face between a cell and its
           connecting cells. The angle varies between zero and 360.0 degrees,
           where zero degrees points in the positive x-axis direction, and 90
           degrees points in the positive y-axis direction. ANGLDEGX is only
           needed if horizontal anisotropy is specified in the NPF Package, if
           the XT3D option is used in the NPF Package, or if the
-          SAVE_SPECIFIC_DISCHARGE option is specifed in the NPF Package.
+          SAVE_SPECIFIC_DISCHARGE option is specified in the NPF Package.
           ANGLDEGX does not need to be specified if these conditions are not
           met. ANGLDEGX is of size NJA; values specified for vertical
           connections and for the diagonal position are not used. Note that
           ANGLDEGX is read in degrees, which is different from MODFLOW-USG,
           which reads a similar variable (ANGLEX) in radians.
     vertices : [iv, xv, yv]
         * iv (integer) is the vertex number. Records in the VERTICES block must
@@ -249,14 +252,22 @@
             "type double precision",
             "reader urword",
             "optional true",
             "default_value 0.0",
             "mf6internal voffsettol",
         ],
         [
+            "block options",
+            "name export_array_ascii",
+            "type keyword",
+            "reader urword",
+            "optional true",
+            "mf6internal export_ascii",
+        ],
+        [
             "block dimensions",
             "name nodes",
             "type integer",
             "reader urword",
             "optional false",
         ],
         [
@@ -452,14 +463,15 @@
         loading_package=False,
         length_units=None,
         nogrb=None,
         xorigin=None,
         yorigin=None,
         angrot=None,
         vertical_offset_tolerance=0.0,
+        export_array_ascii=None,
         nodes=None,
         nja=None,
         nvert=None,
         top=None,
         bot=None,
         area=None,
         idomain=None,
@@ -484,14 +496,17 @@
         self.nogrb = self.build_mfdata("nogrb", nogrb)
         self.xorigin = self.build_mfdata("xorigin", xorigin)
         self.yorigin = self.build_mfdata("yorigin", yorigin)
         self.angrot = self.build_mfdata("angrot", angrot)
         self.vertical_offset_tolerance = self.build_mfdata(
             "vertical_offset_tolerance", vertical_offset_tolerance
         )
+        self.export_array_ascii = self.build_mfdata(
+            "export_array_ascii", export_array_ascii
+        )
         self.nodes = self.build_mfdata("nodes", nodes)
         self.nja = self.build_mfdata("nja", nja)
         self.nvert = self.build_mfdata("nvert", nvert)
         self.top = self.build_mfdata("top", top)
         self.bot = self.build_mfdata("bot", bot)
         self.area = self.build_mfdata("area", area)
         self.idomain = self.build_mfdata("idomain", idomain)
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwtdisv.py` & `flopy-3.7.0/flopy/mf6/modflow/mfprtdisv.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator, ListTemplateGenerator
 
 
-class ModflowGwtdisv(mfpackage.MFPackage):
+class ModflowPrtdisv(mfpackage.MFPackage):
     """
-    ModflowGwtdisv defines a disv package within a gwt6 model.
+    ModflowPrtdisv defines a disv package within a prt6 model.
 
     Parameters
     ----------
     model : MFModel
         Model that this package is a part of. Package is automatically
         added to model when it is initialized.
     loading_package : bool
@@ -41,14 +41,17 @@
     angrot : double
         * angrot (double) counter-clockwise rotation angle (in degrees) of the
           model grid coordinate system relative to a real-world coordinate
           system. If not specified, then a default value of 0.0 is assigned.
           The value for ANGROT does not affect the model simulation, but it is
           written to the binary grid file so that postprocessors can locate the
           grid in space.
+    export_array_ascii : boolean
+        * export_array_ascii (boolean) keyword that specifies input griddata
+          arrays should be written to layered ascii output files.
     nlay : integer
         * nlay (integer) is the number of layers in the model grid.
     ncpl : integer
         * ncpl (integer) is the number of cells per layer. This is a constant
           value for the grid and it applies to all layers.
     nvert : integer
         * nvert (integer) is the total number of (x, y) vertex pairs used to
@@ -104,22 +107,22 @@
     parent_file : MFPackage
         Parent package file that references this package. Only needed for
         utility packages (mfutl*). For example, mfutllaktab package must have
         a mfgwflak package parent_file.
 
     """
 
-    top = ArrayTemplateGenerator(("gwt6", "disv", "griddata", "top"))
-    botm = ArrayTemplateGenerator(("gwt6", "disv", "griddata", "botm"))
-    idomain = ArrayTemplateGenerator(("gwt6", "disv", "griddata", "idomain"))
-    vertices = ListTemplateGenerator(("gwt6", "disv", "vertices", "vertices"))
-    cell2d = ListTemplateGenerator(("gwt6", "disv", "cell2d", "cell2d"))
-    package_abbr = "gwtdisv"
+    top = ArrayTemplateGenerator(("prt6", "disv", "griddata", "top"))
+    botm = ArrayTemplateGenerator(("prt6", "disv", "griddata", "botm"))
+    idomain = ArrayTemplateGenerator(("prt6", "disv", "griddata", "idomain"))
+    vertices = ListTemplateGenerator(("prt6", "disv", "vertices", "vertices"))
+    cell2d = ListTemplateGenerator(("prt6", "disv", "cell2d", "cell2d"))
+    package_abbr = "prtdisv"
     _package_type = "disv"
-    dfn_file_name = "gwt-disv.dfn"
+    dfn_file_name = "prt-disv.dfn"
 
     dfn = [
         [
             "header",
         ],
         [
             "block options",
@@ -153,14 +156,22 @@
             "block options",
             "name angrot",
             "type double precision",
             "reader urword",
             "optional true",
         ],
         [
+            "block options",
+            "name export_array_ascii",
+            "type keyword",
+            "reader urword",
+            "optional true",
+            "mf6internal export_ascii",
+        ],
+        [
             "block dimensions",
             "name nlay",
             "type integer",
             "reader urword",
             "optional false",
         ],
         [
@@ -300,14 +311,15 @@
         model,
         loading_package=False,
         length_units=None,
         nogrb=None,
         xorigin=None,
         yorigin=None,
         angrot=None,
+        export_array_ascii=None,
         nlay=None,
         ncpl=None,
         nvert=None,
         top=None,
         botm=None,
         idomain=None,
         vertices=None,
@@ -322,14 +334,17 @@
 
         # set up variables
         self.length_units = self.build_mfdata("length_units", length_units)
         self.nogrb = self.build_mfdata("nogrb", nogrb)
         self.xorigin = self.build_mfdata("xorigin", xorigin)
         self.yorigin = self.build_mfdata("yorigin", yorigin)
         self.angrot = self.build_mfdata("angrot", angrot)
+        self.export_array_ascii = self.build_mfdata(
+            "export_array_ascii", export_array_ascii
+        )
         self.nlay = self.build_mfdata("nlay", nlay)
         self.ncpl = self.build_mfdata("ncpl", ncpl)
         self.nvert = self.build_mfdata("nvert", nvert)
         self.top = self.build_mfdata("top", top)
         self.botm = self.build_mfdata("botm", botm)
         self.idomain = self.build_mfdata("idomain", idomain)
         self.vertices = self.build_mfdata("vertices", vertices)
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwtdsp.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwtdsp.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator
 
 
 class ModflowGwtdsp(mfpackage.MFPackage):
     """
     ModflowGwtdsp defines a dsp package within a gwt6 model.
@@ -24,14 +24,17 @@
           with the model grid, there is no mechanical dispersion, or when the
           longitudinal and transverse dispersivities are equal. This option may
           also be used to assess the computational demand of the XT3D approach
           by noting the run time differences with and without this option on.
     xt3d_rhs : boolean
         * xt3d_rhs (boolean) add xt3d terms to right-hand side, when possible.
           This option uses less memory, but may require more iterations.
+    export_array_ascii : boolean
+        * export_array_ascii (boolean) keyword that specifies input griddata
+          arrays should be written to layered ascii output files.
     diffc : [double]
         * diffc (double) effective molecular diffusion coefficient.
     alh : [double]
         * alh (double) longitudinal dispersivity in horizontal direction. If
           flow is strictly horizontal, then this is the longitudinal
           dispersivity that will be used. If flow is not strictly horizontal or
           strictly vertical, then the longitudinal dispersivity is a function
@@ -102,14 +105,22 @@
             "name xt3d_rhs",
             "type keyword",
             "shape",
             "reader urword",
             "optional true",
         ],
         [
+            "block options",
+            "name export_array_ascii",
+            "type keyword",
+            "reader urword",
+            "optional true",
+            "mf6internal export_ascii",
+        ],
+        [
             "block griddata",
             "name diffc",
             "type double precision",
             "shape (nodes)",
             "reader readarray",
             "layered true",
             "optional true",
@@ -163,14 +174,15 @@
 
     def __init__(
         self,
         model,
         loading_package=False,
         xt3d_off=None,
         xt3d_rhs=None,
+        export_array_ascii=None,
         diffc=None,
         alh=None,
         alv=None,
         ath1=None,
         ath2=None,
         atv=None,
         filename=None,
@@ -180,14 +192,17 @@
         super().__init__(
             model, "dsp", filename, pname, loading_package, **kwargs
         )
 
         # set up variables
         self.xt3d_off = self.build_mfdata("xt3d_off", xt3d_off)
         self.xt3d_rhs = self.build_mfdata("xt3d_rhs", xt3d_rhs)
+        self.export_array_ascii = self.build_mfdata(
+            "export_array_ascii", export_array_ascii
+        )
         self.diffc = self.build_mfdata("diffc", diffc)
         self.alh = self.build_mfdata("alh", alh)
         self.alv = self.build_mfdata("alv", alv)
         self.ath1 = self.build_mfdata("ath1", ath1)
         self.ath2 = self.build_mfdata("ath2", ath2)
         self.atv = self.build_mfdata("atv", atv)
         self._init_complete = True
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwtfmi.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwtfmi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwtfmi(mfpackage.MFPackage):
     """
     ModflowGwtfmi defines a fmi package within a gwt6 model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwtgwt.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwtgwt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwtgwt(mfpackage.MFPackage):
     """
     ModflowGwtgwt defines a gwtgwt package.
@@ -34,29 +34,25 @@
           corresponding GWF Model. In the simulation name file, the GWT6-GWT6
           entry contains names for GWT Models (exgmnamea and exgmnameb). The
           GWT Model with the name exgmnameb must correspond to the GWF Model
           with the name gwfmodelname2.
     auxiliary : [string]
         * auxiliary (string) an array of auxiliary variable names. There is no
           limit on the number of auxiliary variables that can be provided. Most
-          auxiliary variables will not be used by the GWF-GWF Exchange, but
+          auxiliary variables will not be used by the GWT-GWT Exchange, but
           they will be available for use by other parts of the program. If an
           auxiliary variable with the name "ANGLDEGX" is found, then this
           information will be used as the angle (provided in degrees) between
           the connection face normal and the x axis, where a value of zero
           indicates that a normal vector points directly along the positive x
           axis. The connection face normal is a normal vector on the cell face
           shared between the cell in model 1 and the cell in model 2 pointing
           away from the model 1 cell. Additional information on "ANGLDEGX" is
-          provided in the description of the DISU Package. If an auxiliary
-          variable with the name "CDIST" is found, then this information will
-          be used as the straight-line connection distance, including the
-          vertical component, between the two cell centers. Both ANGLDEGX and
-          CDIST are required if specific discharge is calculated for either of
-          the groundwater models.
+          provided in the description of the DISU Package. ANGLDEGX must be
+          specified if dispersion is simulated in the connected GWT models.
     boundnames : boolean
         * boundnames (boolean) keyword to indicate that boundary names may be
           provided with the list of GWT Exchange cells.
     print_input : boolean
         * print_input (boolean) keyword to indicate that the list of exchange
           entries will be echoed to the listing file immediately after it is
           read.
@@ -408,14 +404,15 @@
             "name aux",
             "type double precision",
             "in_record true",
             "tagged false",
             "shape (naux)",
             "reader urword",
             "optional true",
+            "mf6internal auxvar",
         ],
         [
             "block exchangedata",
             "name boundname",
             "type string",
             "shape",
             "tagged false",
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwtic.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwtic.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator
 
 
 class ModflowGwtic(mfpackage.MFPackage):
     """
     ModflowGwtic defines a ic package within a gwt6 model.
@@ -13,14 +13,17 @@
     ----------
     model : MFModel
         Model that this package is a part of. Package is automatically
         added to model when it is initialized.
     loading_package : bool
         Do not set this parameter. It is intended for debugging and internal
         processing purposes only.
+    export_array_ascii : boolean
+        * export_array_ascii (boolean) keyword that specifies input griddata
+          arrays should be written to layered ascii output files.
     strt : [double]
         * strt (double) is the initial (starting) concentration---that is,
           concentration at the beginning of the GWT Model simulation. STRT must
           be specified for all GWT Model simulations. One value is read for
           every model cell.
     filename : String
         File name for this package.
@@ -39,33 +42,45 @@
     dfn_file_name = "gwt-ic.dfn"
 
     dfn = [
         [
             "header",
         ],
         [
+            "block options",
+            "name export_array_ascii",
+            "type keyword",
+            "reader urword",
+            "optional true",
+            "mf6internal export_ascii",
+        ],
+        [
             "block griddata",
             "name strt",
             "type double precision",
             "shape (nodes)",
             "reader readarray",
             "layered true",
             "default_value 0.0",
         ],
     ]
 
     def __init__(
         self,
         model,
         loading_package=False,
+        export_array_ascii=None,
         strt=0.0,
         filename=None,
         pname=None,
         **kwargs,
     ):
         super().__init__(
             model, "ic", filename, pname, loading_package, **kwargs
         )
 
         # set up variables
+        self.export_array_ascii = self.build_mfdata(
+            "export_array_ascii", export_array_ascii
+        )
         self.strt = self.build_mfdata("strt", strt)
         self._init_complete = True
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwtist.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwtist.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator, ListTemplateGenerator
 
 
 class ModflowGwtist(mfpackage.MFPackage):
     """
     ModflowGwtist defines a ist package within a gwt6 model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwtlkt.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwtlkt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwtlkt(mfpackage.MFPackage):
     """
     ModflowGwtlkt defines a lkt package within a gwt6 model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwtmst.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwtmst.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator
 
 
 class ModflowGwtmst(mfpackage.MFPackage):
     """
     ModflowGwtmst defines a mst package within a gwt6 model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwtmvt.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwtmvt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwtmvt(mfpackage.MFPackage):
     """
     ModflowGwtmvt defines a mvt package within a gwt6 model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwtmwt.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwtmwt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwtmwt(mfpackage.MFPackage):
     """
     ModflowGwtmwt defines a mwt package within a gwt6 model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwtnam.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwtnam.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwtnam(mfpackage.MFPackage):
     """
     ModflowGwtnam defines a nam package within a gwt6 model.
@@ -36,16 +36,16 @@
           time step of each stress period.
     save_flows : boolean
         * save_flows (boolean) keyword to indicate that all model package flow
           terms will be written to the file specified with "BUDGET FILEOUT" in
           Output Control.
     packages : [ftype, fname, pname]
         * ftype (string) is the file type, which must be one of the following
-          character values shown in table in mf6io.pdf. Ftype may be entered in
-          any combination of uppercase and lowercase.
+          character values shown in table ref{table:ftype-gwt}. Ftype may be
+          entered in any combination of uppercase and lowercase.
         * fname (string) is the name of the file containing the package input.
           The path to the file should be included if the file is not located in
           the folder where the program was run.
         * pname (string) is the user-defined name for the package. PNAME is
           restricted to 16 characters. No spaces are allowed in PNAME. PNAME
           character values are read and stored by the program for stress
           packages only. These names may be useful for labeling purposes when
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwtoc.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwtoc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwtoc(mfpackage.MFPackage):
     """
     ModflowGwtoc defines a oc package within a gwt6 model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwtsft.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwtsft.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwtsft(mfpackage.MFPackage):
     """
     ModflowGwtsft defines a sft package within a gwt6 model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwtsrc.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwtsrc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwtsrc(mfpackage.MFPackage):
     """
     ModflowGwtsrc defines a src package within a gwt6 model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwtssm.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwtssm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwtssm(mfpackage.MFPackage):
     """
     ModflowGwtssm defines a ssm package within a gwt6 model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfgwtuzt.py` & `flopy-3.7.0/flopy/mf6/modflow/mfgwtuzt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowGwtuzt(mfpackage.MFPackage):
     """
     ModflowGwtuzt defines a uzt package within a gwt6 model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfims.py` & `flopy-3.7.0/flopy/mf6/modflow/mfims.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowIms(mfpackage.MFPackage):
     """
     ModflowIms defines a ims package.
@@ -124,15 +124,15 @@
           allowable residual between successive outer iterations at any single
           model package element. An example of a model package that would use
           OUTER_RCLOSEBND to evaluate convergence is the SFR package which
           solves a continuity equation for each reach. The OUTER_RCLOSEBND
           option is deprecated and has no effect on simulation results as of
           version 6.1.1. The keyword, OUTER_RCLOSEBND can be still be specified
           for backward compatibility with previous versions of MODFLOW 6 but
-          eventually specificiation of OUTER_RCLOSEBND will cause MODFLOW 6 to
+          eventually specification of OUTER_RCLOSEBND will cause MODFLOW 6 to
           terminate with an error.
     outer_maximum : integer
         * outer_maximum (integer) integer value defining the maximum number of
           outer (nonlinear) iterations -- that is, calls to the solution
           routine. For a linear problem OUTER_MAXIMUM should be 1.
     under_relaxation : string
         * under_relaxation (string) is an optional keyword that defines the
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfmvr.py` & `flopy-3.7.0/flopy/mf6/modflow/mfmvr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowMvr(mfpackage.MFPackage):
     """
     ModflowMvr defines a mvr package. This package can only be used to move
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfmvt.py` & `flopy-3.7.0/flopy/mf6/modflow/mfmvt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowMvt(mfpackage.MFPackage):
     """
     ModflowMvt defines a mvt package.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfnam.py` & `flopy-3.7.0/flopy/mf6/modflow/mfnam.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowNam(mfpackage.MFPackage):
     """
     ModflowNam defines a nam package.
@@ -36,14 +36,19 @@
           printed.
     print_input : boolean
         * print_input (boolean) keyword to activate printing of simulation
           input summaries to the simulation list file (mfsim.lst). With this
           keyword, input summaries will be written for those packages that
           support newer input data model routines. Not all packages are
           supported yet by the newer input data model routines.
+    hpc : {varname:data} or hpc_data data
+        * Contains data for the hpc package. Data can be stored in a dictionary
+          containing data for the hpc package with variable names as keys and
+          package data as values. Data just for the hpc variable is also
+          acceptable. See hpc package documentation for more information.
     tdis6 : string
         * tdis6 (string) is the name of the Temporal Discretization (TDIS)
           Input File.
     models : [mtype, mfname, mname]
         * mtype (string) is the type of model to add to simulation.
         * mfname (string) is the file name of the model name file.
         * mname (string) is the user-assigned name of the model. The model name
@@ -59,15 +64,16 @@
           this exchange.
     mxiter : integer
         * mxiter (integer) is the maximum number of outer iterations for this
           solution group. The default value is 1. If there is only one solution
           in the solution group, then MXITER must be 1.
     solutiongroup : [slntype, slnfname, slnmnames]
         * slntype (string) is the type of solution. The Integrated Model
-          Solution (IMS6) is the only supported option in this version.
+          Solution (IMS6) and Explicit Model Solution (EMS6) are the only
+          supported options in this version.
         * slnfname (string) name of file containing solution input.
         * slnmnames (string) is the array of model names to add to this
           solution. The number of model names is determined by the number of
           model names the user provides on this line.
     filename : String
         File name for this package.
     pname : String
@@ -75,14 +81,17 @@
     parent_file : MFPackage
         Parent package file that references this package. Only needed for
         utility packages (mfutl*). For example, mfutllaktab package must have
         a mfgwflak package parent_file.
 
     """
 
+    hpc_filerecord = ListTemplateGenerator(
+        ("nam", "options", "hpc_filerecord")
+    )
     models = ListTemplateGenerator(("nam", "models", "models"))
     exchanges = ListTemplateGenerator(("nam", "exchanges", "exchanges"))
     solutiongroup = ListTemplateGenerator(
         ("nam", "solutiongroup", "solutiongroup")
     )
     package_abbr = "nam"
     _package_type = "nam"
@@ -125,14 +134,56 @@
             "block options",
             "name print_input",
             "type keyword",
             "reader urword",
             "optional true",
         ],
         [
+            "block options",
+            "name hpc_filerecord",
+            "type record hpc6 filein hpc6_filename",
+            "shape",
+            "reader urword",
+            "tagged true",
+            "optional true",
+            "construct_package hpc",
+            "construct_data hpc_data",
+            "parameter_name hpc",
+        ],
+        [
+            "block options",
+            "name hpc6",
+            "type keyword",
+            "shape",
+            "in_record true",
+            "reader urword",
+            "tagged true",
+            "optional false",
+        ],
+        [
+            "block options",
+            "name filein",
+            "type keyword",
+            "shape",
+            "in_record true",
+            "reader urword",
+            "tagged true",
+            "optional false",
+        ],
+        [
+            "block options",
+            "name hpc6_filename",
+            "type string",
+            "preserve_case true",
+            "in_record true",
+            "reader urword",
+            "optional false",
+            "tagged false",
+        ],
+        [
             "block timing",
             "name tdis6",
             "preserve_case true",
             "type string",
             "reader urword",
             "optional",
         ],
@@ -231,15 +282,15 @@
             "type recarray slntype slnfname slnmnames",
             "reader urword",
         ],
         [
             "block solutiongroup",
             "name slntype",
             "type string",
-            "valid ims6",
+            "valid ims6 ems6",
             "in_record true",
             "tagged false",
             "reader urword",
         ],
         [
             "block solutiongroup",
             "name slnfname",
@@ -286,13 +337,14 @@
         self.continue_ = self.build_mfdata("continue", continue_)
         self.nocheck = self.build_mfdata("nocheck", nocheck)
         self.memory_print_option = self.build_mfdata(
             "memory_print_option", memory_print_option
         )
         self.maxerrors = self.build_mfdata("maxerrors", maxerrors)
         self.print_input = self.build_mfdata("print_input", print_input)
+        self._hpc_filerecord = self.build_mfdata("hpc_filerecord", None)
         self.tdis6 = self.build_mfdata("tdis6", tdis6)
         self.models = self.build_mfdata("models", models)
         self.exchanges = self.build_mfdata("exchanges", exchanges)
         self.mxiter = self.build_mfdata("mxiter", mxiter)
         self.solutiongroup = self.build_mfdata("solutiongroup", solutiongroup)
         self._init_complete = True
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfsimulation.py` & `flopy-3.7.0/flopy/mf6/modflow/mfsimulation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 import os
 from typing import Union
 
 from .. import mfsimbase
 
 
 class MFSimulation(mfsimbase.MFSimulationBase):
@@ -36,14 +36,19 @@
           printed.
     print_input : boolean
         * print_input (boolean) keyword to activate printing of simulation
           input summaries to the simulation list file (mfsim.lst). With this
           keyword, input summaries will be written for those packages that
           support newer input data model routines. Not all packages are
           supported yet by the newer input data model routines.
+    hpc : {varname:data} or hpc_data data
+        * Contains data for the hpc package. Data can be stored in a dictionary
+          containing data for the hpc package with variable names as keys and
+          package data as values. Data just for the hpc variable is also
+          acceptable. See hpc package documentation for more information.
     tdis6 : string
         * tdis6 (string) is the name of the Temporal Discretization (TDIS)
           Input File.
     models : [mtype, mfname, mname]
         * mtype (string) is the type of model to add to simulation.
         * mfname (string) is the file name of the model name file.
         * mname (string) is the user-assigned name of the model. The model name
@@ -59,15 +64,16 @@
           this exchange.
     mxiter : integer
         * mxiter (integer) is the maximum number of outer iterations for this
           solution group. The default value is 1. If there is only one solution
           in the solution group, then MXITER must be 1.
     solutiongroup : [slntype, slnfname, slnmnames]
         * slntype (string) is the type of solution. The Integrated Model
-          Solution (IMS6) is the only supported option in this version.
+          Solution (IMS6) and Explicit Model Solution (EMS6) are the only
+          supported options in this version.
         * slnfname (string) name of file containing solution input.
         * slnmnames (string) is the array of model names to add to this
           solution. The number of model names is determined by the number of
           model names the user provides on this line.
 
     Methods
     -------
@@ -90,14 +96,15 @@
         use_pandas=True,
         lazy_io=False,
         continue_=None,
         nocheck=None,
         memory_print_option=None,
         maxerrors=None,
         print_input=None,
+        hpc_data=None,
     ):
         super().__init__(
             sim_name=sim_name,
             version=version,
             exe_name=exe_name,
             sim_ws=sim_ws,
             verbosity_level=verbosity_level,
@@ -113,14 +120,15 @@
         self.name_file.print_input.set_data(print_input)
 
         self.continue_ = self.name_file.continue_
         self.nocheck = self.name_file.nocheck
         self.memory_print_option = self.name_file.memory_print_option
         self.maxerrors = self.name_file.maxerrors
         self.print_input = self.name_file.print_input
+        self.hpc_data = self._create_package("hpc", hpc_data)
 
     @classmethod
     def load(
         cls,
         sim_name="modflowsim",
         version="mf6",
         exe_name: Union[str, os.PathLike] = "mf6",
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mftdis.py` & `flopy-3.7.0/flopy/mf6/modflow/mftdis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowTdis(mfpackage.MFPackage):
     """
     ModflowTdis defines a tdis package.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfutlats.py` & `flopy-3.7.0/flopy/mf6/modflow/mfutlats.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowUtlats(mfpackage.MFPackage):
     """
     ModflowUtlats defines a ats package within a utl model.
@@ -40,15 +40,15 @@
         * dtmax (double) is the maximum time step length for this period. This
           value must be greater than dtmin.
         * dtadj (double) is the time step multiplier factor for this period. If
           the number of outer solver iterations are less than the product of
           the maximum number of outer iterations (OUTER_MAXIMUM) and
           ATS_OUTER_MAXIMUM_FRACTION (an optional variable in the IMS input
           file with a default value of 1/3), then the time step length is
-          multipled by dtadj. If the number of outer solver iterations are
+          multiplied by dtadj. If the number of outer solver iterations are
           greater than the product of the maximum number of outer iterations
           and ATS_OUTER_MAXIMUM_FRACTION, then the time step length is divided
           by dtadj. dtadj must be zero, one, or greater than one. If dtadj is
           zero or one, then it has no effect on the simulation. A value between
           2.0 and 5.0 can be used as an initial estimate.
         * dtfailadj (double) is the divisor of the time step length when a time
           step fails to converge. If there is solver failure, then the time
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfutllaktab.py` & `flopy-3.7.0/flopy/mf6/modflow/mfutllaktab.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowUtllaktab(mfpackage.MFPackage):
     """
     ModflowUtllaktab defines a laktab package within a utl model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfutlobs.py` & `flopy-3.7.0/flopy/mf6/modflow/mfutlobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowUtlobs(mfpackage.MFPackage):
     """
     ModflowUtlobs defines a obs package within a utl model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfutlsfrtab.py` & `flopy-3.7.0/flopy/mf6/modflow/mfutlsfrtab.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowUtlsfrtab(mfpackage.MFPackage):
     """
     ModflowUtlsfrtab defines a sfrtab package within a utl model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfutlspc.py` & `flopy-3.7.0/flopy/mf6/modflow/mfutlspc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowUtlspc(mfpackage.MFPackage):
     """
     ModflowUtlspc defines a spc package within a utl model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfutlspca.py` & `flopy-3.7.0/flopy/mf6/modflow/mfutlspca.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator, ListTemplateGenerator
 
 
 class ModflowUtlspca(mfpackage.MFPackage):
     """
     ModflowUtlspca defines a spca package within a utl model.
@@ -16,15 +16,19 @@
         added to model when it is initialized.
     loading_package : bool
         Do not set this parameter. It is intended for debugging and internal
         processing purposes only.
     readasarrays : boolean
         * readasarrays (boolean) indicates that array-based input will be used
           for the SPC Package. This keyword must be specified to use array-
-          based input.
+          based input. When READASARRAYS is specified, values must be provided
+          for every cell within a model layer, even those cells that have an
+          IDOMAIN value less than one. Values assigned to cells with IDOMAIN
+          values less than one are not used and have no effect on simulation
+          results.
     print_input : boolean
         * print_input (boolean) keyword to indicate that the list of spc
           information will be written to the listing file immediately after it
           is read.
     timearrayseries : {varname:data} or tas_array data
         * Contains data for the tas package. Data can be stored in a dictionary
           containing data for the tas package with variable names as keys and
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfutltas.py` & `flopy-3.7.0/flopy/mf6/modflow/mfutltas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ArrayTemplateGenerator, ListTemplateGenerator
 
 
 class ModflowUtltas(mfpackage.MFPackage):
     """
     ModflowUtltas defines a tas package within a utl model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfutlts.py` & `flopy-3.7.0/flopy/mf6/modflow/mfutlts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowUtlts(mfpackage.MFPackage):
     """
     ModflowUtlts defines a ts package within a utl model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfutltvk.py` & `flopy-3.7.0/flopy/mf6/modflow/mfutltvk.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowUtltvk(mfpackage.MFPackage):
     """
     ModflowUtltvk defines a tvk package within a utl model.
```

### Comparing `flopy-3.6.0/flopy/mf6/modflow/mfutltvs.py` & `flopy-3.7.0/flopy/mf6/modflow/mfutltvs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DO NOT MODIFY THIS FILE DIRECTLY.  THIS FILE MUST BE CREATED BY
 # mf6/utils/createpackages.py
-# FILE created on February 07, 2024 20:16:08 UTC
+# FILE created on May 23, 2024 14:30:07 UTC
 from .. import mfpackage
 from ..data.mfdatautil import ListTemplateGenerator
 
 
 class ModflowUtltvs(mfpackage.MFPackage):
     """
     ModflowUtltvs defines a tvs package within a utl model.
```

### Comparing `flopy-3.6.0/flopy/mf6/utils/binaryfile_utils.py` & `flopy-3.7.0/flopy/mf6/utils/binaryfile_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,15 +173,15 @@
         if key[-1] == "FLOW-JA-FACE":
             return data
 
         else:
             return data
 
     def _get_binary_file_object(self, path, bintype, key):
-        # simple method that trys to open the binary file object using Flopy
+        # simple method that tries to open the binary file object using Flopy
         if bintype == "CBC":
             try:
                 return bf.CellBudgetFile(path, precision="double")
             except AssertionError:
                 raise AssertionError(f"{self.dataDict[key]} does not exist")
 
         elif bintype == "HDS":
```

### Comparing `flopy-3.6.0/flopy/mf6/utils/binarygrid_util.py` & `flopy-3.7.0/flopy/mf6/utils/binarygrid_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -357,112 +357,115 @@
         """
         Number of layers. None for DISU grids.
 
         Returns
         -------
         nlay : int
         """
-        if self._grid_type in ("DIS", "DISV"):
+        nlay = None
+        if "NLAY" in self._datadict:
             nlay = self._datadict["NLAY"]
-        else:
-            nlay = None
         return nlay
 
     @property
     def nrow(self):
         """
         Number of rows. None for DISV and DISU grids.
 
         Returns
         -------
         nrow : int
         """
-        if self._grid_type == "DIS":
+        nrow = None
+        if "NROW" in self._datadict:
             nrow = self._datadict["NROW"]
-        else:
-            nrow = None
         return nrow
 
     @property
     def ncol(self):
         """
         Number of columns. None for DISV and DISU grids.
 
         Returns
         -------
         ncol : int
         """
-        if self._grid_type == "DIS":
+        ncol = None
+        if "NCOL" in self._datadict:
             ncol = self._datadict["NCOL"]
-        else:
-            ncol = None
         return ncol
 
     @property
     def ncpl(self):
         """
         Number of cells per layer. None for DISU grids.
 
         Returns
         -------
         ncpl : int
         """
-        if self._grid_type == "DISV":
+        ncpl = None
+        if "NCPL" in self._datadict:
             ncpl = self._datadict["NCPL"]
-        if self._grid_type == "DIS":
-            ncpl = self.nrow * self.ncol
-        else:
-            None
         return ncpl
 
     @property
     def ncells(self):
         """
         Number of cells.
 
         Returns
         -------
         ncells : int
         """
-        if self._grid_type in ("DIS", "DISV"):
+        # disu is the only grid that has the number of cells
+        # set to nodes.  All other grids use NCELLS in grb
+        if "NCELLS" in self._datadict:
             ncells = self._datadict["NCELLS"]
-        else:
+        elif "NODES" in self._datadict:
             ncells = self._datadict["NODES"]
+        else:
+            ncells = None
         return ncells
 
     @property
     def nodes(self):
         """
         Number of nodes.
 
         Returns
         -------
         nodes : int
         """
-        if self._grid_type in ("DIS", "DISV"):
-            nodes = self.ncells
-        else:
-            nodes = self._datadict["NODES"]
+        nodes = self.ncells
         return nodes
 
     @property
     def shape(self):
         """
         Shape of the model grid (tuple).
 
         Returns
         -------
         shape : tuple
         """
         if self._grid_type == "DIS":
             shape = (self.nlay, self.nrow, self.ncol)
+        elif self._grid_type == "DIS2D":
+            shape = (self.nrow, self.ncol)
         elif self._grid_type == "DISV":
             shape = (self.nlay, self.ncpl)
-        else:
+        elif self._grid_type == "DISV2D":
+            shape = (self.ncells,)
+        elif self._grid_type == "DISV1D":
+            shape = (self.ncells,)
+        elif self._grid_type == "DISU":
             shape = (self.nodes,)
+        else:
+            shape = None
         return shape
 
     @property
     def xorigin(self):
         """
         x-origin of the model grid. None if not defined in the
         MODFLOW 6 grid file.
@@ -531,60 +534,62 @@
         Cell size in the row direction (y-direction). None if not
         defined in the MODFLOW 6 grid file.
 
         Returns
         -------
         delr : ndarray of floats
         """
-        if self.grid_type == "DIS":
+        delr = None
+        if "DELR" in self._datadict:
             delr = self._datadict["DELR"]
-        else:
-            delr = None
         return delr
 
     @property
     def delc(self):
         """
         Cell size in the column direction (x-direction). None if not
         defined in the MODFLOW 6 grid file.
 
         Returns
         -------
         delc : ndarray of floats
         """
-        if self.grid_type == "DIS":
+        delc = None
+        if "DELC" in self._datadict:
             delc = self._datadict["DELC"]
-        else:
-            delc = None
         return delc
 
     @property
     def top(self):
         """
         Top of the model cells in the upper model layer for DIS and
         DISV grids. Top of the model cells for DISU grids.
 
         Returns
         -------
         top : ndarray of floats
         """
-        return self._datadict["TOP"]
+        top = None
+        if "TOP" in self._datadict:
+            top = self._datadict["TOP"]
+        return top
 
     @property
     def bot(self):
         """
         Bottom of the model cells.
 
         Returns
         -------
         bot : ndarray of floats
         """
-        if self.grid_type in ("DIS", "DISV"):
+        bot = None
+        if "BOTM" in self._datadict:
             bot = self._datadict["BOTM"]
-        else:
+        elif "BOT" in self._datadict:
             bot = self._datadict["BOT"]
         return bot
 
     @property
     def nja(self):
         """
         Number of non-zero entries JA vector array.
@@ -729,12 +734,12 @@
         """
         cell2d data for a DISV grid. None for DIS and DISU grids.
 
         Returns
         -------
         cell2d : list of lists
         """
-        if self._grid_type == "DISV":
+        if self._grid_type in ("DISV", "DISV2D", "DISV1D"):
             vertices, cell2d = self.__build_vertices_cell2d()
         else:
             vertices, cell2d = None, None
         return vertices, cell2d
```

### Comparing `flopy-3.6.0/flopy/mf6/utils/createpackages.py` & `flopy-3.7.0/flopy/mf6/utils/createpackages.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 # flopy parent_name_type parent_package MFPackage
 
 There are three possible types (or combination of them) that can be used for
 "parent package type", MFPackage, MFModel, and MFSimulation. If a package
 supports multiple types of parents (for example, it can be either in the model
 namefile or in a package, like the obs package), include all the types
-supported, seperating each type with a / (MFPackage/MFModel).
+supported, separating each type with a / (MFPackage/MFModel).
 
 To create a new type of model choose a unique three letter model abbreviation
 ("gwf", "gwt", ...). Create a name file dfn with the naming convention
 <model abbr>-nam.dfn. The name file must have only an options and packages
 block (see gwf-nam.dfn as an example). Create a new dfn file for each of the
 packages in your new model, following the naming convention described above.
 
@@ -313,14 +313,15 @@
     path,
     data_type,
     basic_init=False,
     construct_package=None,
     construct_data=None,
     parameter_name=None,
     set_param_list=None,
+    mf_nam=False,
 ):
     if set_param_list is None:
         set_param_list = []
     clean_ds_name = datautil.clean_name(python_name)
     if construct_package is None:
         # add variable initialization lines
         if basic_init:
@@ -335,27 +336,34 @@
             options_param_list.append(f"{clean_ds_name}={default_value}")
         # add to set parameter list
         set_param_list.append(f"{clean_ds_name}={clean_ds_name}")
     else:
         clean_parameter_name = datautil.clean_name(parameter_name)
         # init hidden variable
         init_vars.append(create_init_var(f"_{clean_ds_name}", name, "None"))
-        # init child package
-        init_vars.append(
-            create_package_init_var(
-                clean_parameter_name,
-                construct_package,
-                construct_data,
-                clean_ds_name,
+        if mf_nam:
+            options_param_list.append(
+                [f"{parameter_name}_data=None", parameter_name]
+            )
+        else:
+            # init child package
+            init_vars.append(
+                create_package_init_var(
+                    clean_parameter_name,
+                    construct_package,
+                    construct_data,
+                    clean_ds_name,
+                )
+            )
+            # add to parameter list
+            init_param_list.append(f"{clean_parameter_name}=None")
+            # add to set parameter list
+            set_param_list.append(
+                f"{clean_parameter_name}={clean_parameter_name}"
             )
-        )
-        # add to parameter list
-        init_param_list.append(f"{clean_parameter_name}=None")
-        # add to set parameter list
-        set_param_list.append(f"{clean_parameter_name}={clean_parameter_name}")
 
     package_properties.append(create_property(clean_ds_name))
     doc_string.add_parameter(description, model_parameter=True)
     data_structure_dict[python_name] = 0
     if class_vars is not None:
         gen_type = generator_type(data_type)
         if gen_type != "ScalarTemplateGenerator":
@@ -366,14 +374,16 @@
 
 
 def build_init_string(
     init_string, init_param_list, whitespace="                 "
 ):
     line_chars = len(init_string)
     for index, param in enumerate(init_param_list):
+        if isinstance(param, list):
+            param = param[0]
         if index + 1 < len(init_param_list):
             line_chars += len(param) + 2
         else:
             line_chars += len(param) + 3
         if line_chars > 79:
             if len(param) + len(whitespace) + 1 > 79:
                 # try to break apart at = sign
@@ -457,39 +467,60 @@
     return sim_load, sim_load_c
 
 
 def build_model_init_vars(param_list):
     init_var_list = []
     # build set data calls
     for param in param_list:
-        param_parts = param.split("=")
-        init_var_list.append(
-            f"        self.name_file.{param_parts[0]}.set_data({param_parts[0]})"
-        )
+        if not isinstance(param, list):
+            param_parts = param.split("=")
+            init_var_list.append(
+                f"        self.name_file.{param_parts[0]}.set_data({param_parts[0]})"
+            )
     init_var_list.append("")
     # build attributes
     for param in param_list:
-        param_parts = param.split("=")
-        init_var_list.append(
-            f"        self.{param_parts[0]} = self.name_file.{param_parts[0]}"
-        )
+        if isinstance(param, list):
+            pkg_name = param[1]
+            param_parts = param[0].split("=")
+            init_var_list.append(
+                f"        self.{param_parts[0]} = "
+                f"self._create_package('{pkg_name}', {param_parts[0]})"
+            )
+        else:
+            param_parts = param.split("=")
+            init_var_list.append(
+                f"        self.{param_parts[0]} = self.name_file.{param_parts[0]}"
+            )
 
     return "\n".join(init_var_list)
 
 
 def create_packages():
     indent = "    "
     init_string_def = "    def __init__(self"
 
     # load JSON file
     file_structure = mfstructure.MFStructure(load_from_dfn_files=True)
     sim_struct = file_structure.sim_struct
 
     # assemble package list of buildable packages
     package_list = []
+    for package in sim_struct.utl_struct_objs.values():
+        # add utility packages to list
+        package_list.append(
+            (
+                package,
+                PackageLevel.model_level,
+                "utl",
+                package.dfn_list,
+                package.file_type,
+                package.header,
+            )
+        )
     package_list.append(
         (
             sim_struct.name_file_struct_obj,
             PackageLevel.sim_level,
             "",
             sim_struct.name_file_struct_obj.dfn_list,
             sim_struct.name_file_struct_obj.file_type,
@@ -504,26 +535,14 @@
                 PackageLevel.sim_level,
                 "",
                 package.dfn_list,
                 package.file_type,
                 package.header,
             )
         )
-    for package in sim_struct.utl_struct_objs.values():
-        # add utility packages to list
-        package_list.append(
-            (
-                package,
-                PackageLevel.model_level,
-                "utl",
-                package.dfn_list,
-                package.file_type,
-                package.header,
-            )
-        )
     for model_key, model in sim_struct.model_struct_objs.items():
         package_list.append(
             (
                 model.name_file_struct_obj,
                 PackageLevel.model_level,
                 model_key,
                 model.name_file_struct_obj.dfn_list,
@@ -564,14 +583,15 @@
         package_properties = []
         init_vars = []
         init_param_list = []
         options_param_list = []
         set_param_list = []
         class_vars = []
         template_gens = []
+
         package_abbr = clean_class_string(
             f"{clean_class_string(package[2])}{package[0].file_type}"
         ).lower()
         dfn_string = build_dfn_string(
             package[3], package[5], package_abbr, flopy_dict
         )
         package_name = clean_class_string(
@@ -688,14 +708,28 @@
             )
 
         # loop through all blocks
         for block in package[0].blocks.values():
             for data_structure in block.data_structures.values():
                 # only create one property for each unique data structure name
                 if data_structure.name not in data_structure_dict:
+                    mf_sim = (
+                        "parent_name_type" in package[0].header
+                        and package[0].header["parent_name_type"][1]
+                        == "MFSimulation"
+                    )
+                    mf_nam = package[0].file_type == "nam"
+                    if (
+                        data_structure.construct_package is not None
+                        and not mf_sim
+                        and not mf_nam
+                    ):
+                        c_pkg = data_structure.construct_package
+                    else:
+                        c_pkg = None
                     tg = add_var(
                         init_vars,
                         class_vars,
                         options_param_list,
                         init_param_list,
                         package_properties,
                         doc_string,
@@ -703,18 +737,20 @@
                         data_structure.default_value,
                         data_structure.name,
                         data_structure.python_name,
                         data_structure.get_doc_string(79, indent, indent),
                         data_structure.path,
                         data_structure.get_datatype(),
                         False,
+                        # c_pkg,
                         data_structure.construct_package,
                         data_structure.construct_data,
                         data_structure.parameter_name,
                         set_param_list,
+                        mf_nam,
                     )
                     if tg is not None and tg not in template_gens:
                         template_gens.append(tg)
 
         import_string = "from .. import mfpackage"
         if template_gens:
             import_string += "\nfrom ..data.mfdatautil import "
@@ -822,16 +858,22 @@
         # open new Packages file
         pb_file = open(
             os.path.join(util_path, "..", "modflow", f"mf{package_name}.py"),
             "w",
             newline="\n",
         )
         pb_file.write(package_string)
-
-        if package[0].sub_package and package_abbr != "utltab":
+        if (
+            package[0].sub_package
+            and package_abbr != "utltab"
+            and (
+                "parent_name_type" not in package[0].header
+                or package[0].header["parent_name_type"][1] != "MFSimulation"
+            )
+        ):
             set_param_list.append("filename=filename")
             set_param_list.append("pname=pname")
             set_param_list.append("child_builder_call=True")
             whsp_1 = "                   "
             whsp_2 = "                                    "
 
             file_prefix = package[0].dfn_file_name[0:3]
@@ -840,16 +882,17 @@
                 "class for the Modflow{} class.\n\n    "
                 "Methods\n    ----------"
                 "\n".format(package_name.title(), package_name.title())
             )
 
             # write out child packages class
             chld_cls = (
-                "\n\nclass {}Packages(mfpackage.MFChildPackage"
-                "s):\n".format(package_name.title())
+                "\n\nclass {}Packages(mfpackage.MFChildPackage" "s):\n".format(
+                    package_name.title()
+                )
             )
             chld_var = (
                 f"    package_abbr = "
                 f'"{package_name.title().lower()}packages"\n\n'
             )
             chld_init = "    def initialize(self"
             chld_init = build_init_string(
@@ -1069,15 +1112,15 @@
                 doc_text,
                 init_string_sim,
                 sparent_init_string,
                 init_vars,
                 load_txt,
             )
             sim_file = open(
-                os.path.join(util_path, "..", "modflow", f"mfsimulation.py"),
+                os.path.join(util_path, "..", "modflow", "mfsimulation.py"),
                 "w",
                 newline="\n",
             )
             sim_file.write(package_string)
             sim_file.close()
             init_file_imports.append(
                 "from .mfsimulation import MFSimulation\n"
```

### Comparing `flopy-3.6.0/flopy/mf6/utils/generate_classes.py` & `flopy-3.7.0/flopy/mf6/utils/generate_classes.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/utils/lakpak_utils.py` & `flopy-3.7.0/flopy/mf6/utils/lakpak_utils.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/utils/mfobservation.py` & `flopy-3.7.0/flopy/mf6/utils/mfobservation.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     Class is called by the MFSimulation.SimulationDict() class and is not
     called by the user
 
     Inputs:
     -------
     mfdict: (dict) the sim.simulation_dict.mfdict object for the flopy project
     path: (object) the path object detailing model names and paths
-    key: (tuple, stings) user supplied dictionary key to request observation
+    key: (tuple, strings) user supplied dictionary key to request observation
     utility data
 
     Returns:
     --------\
     self.data: (xarray) array of observations
     """
 
@@ -51,15 +51,15 @@
 class Observations:
     """
     Simple class to extract and view Observation files for Uzf models
     (possibly all obs/hobs)?
 
     Input:
     ------
-    fi = (sting) name of the observation binary output file
+    fi = (string) name of the observation binary output file
 
     Methods:
     --------
     get_data(): (np.array) returns array of observation data
         parameters:
         -----------
         text = (str) specific modflow record name contained in Obs.out file
@@ -193,15 +193,15 @@
     ):
         """
         Creates a pandas dataframe object from the observation data, useful
         backend if the user does not like the x-array format!
 
         Parameters
         ----------
-        keys: (string) sting of dictionary/observation keys separated by comma.
+        keys: (string) string of dictionary/observation keys separated by comma.
               (optional)
         idx: (int) time index location (optional)
         totim: (float) simulation time (optional)
         start_datetime: (string) format is 'dd/mm/yyyy' or
                         'dd/mm/yyyy hh:mm:ss' (optional)
         timeunit: (string) specifies the time unit associated with totim when
                            setting a datetime
```

### Comparing `flopy-3.6.0/flopy/mf6/utils/mfsimlistfile.py` & `flopy-3.7.0/flopy/mf6/utils/mfsimlistfile.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/utils/model_splitter.py` & `flopy-3.7.0/flopy/mf6/utils/model_splitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1406,17 +1406,17 @@
                         new_period["ifno"] = [
                             uzf_remap[i] for i in new_period["ifno"]
                         ]
                         spd[per] = new_period
 
                     mapped_data[mkey]["packagedata"] = new_recarray
                     mapped_data[mkey]["nuzfcells"] = len(new_recarray)
-                    mapped_data[mkey][
-                        "ntrailwaves"
-                    ] = package.ntrailwaves.array
+                    mapped_data[mkey]["ntrailwaves"] = (
+                        package.ntrailwaves.array
+                    )
                     mapped_data[mkey]["nwavesets"] = package.nwavesets.array
                     mapped_data[mkey]["perioddata"] = spd
 
             if self._pkg_mover:
                 for per in range(self._model.nper):
                     if per in self._mover_remaps:
                         self._mover_remaps[per][package.name[0]] = mvr_remap
@@ -2395,15 +2395,15 @@
                             else:
                                 mm_keys[key] = [mdl]
 
                     tmp_models = [new_model1[idx][0] for idx in mm_idx]
                     new_model1[mm_idx] = tmp_models
 
                 cellid2 = recarray.id2
-                conv_idx = np.where((cellid2 != None))[0]
+                conv_idx = np.where((cellid2 is not None))[0]
                 if len(conv_idx) > 0:  # do stuff
                     # need to trap layers...
                     if pkg_type is None:
                         if self._modelgrid.grid_type in (
                             "structured",
                             "vertex",
                         ):
@@ -2452,15 +2452,15 @@
 
                         new_cellid2 = np.full(
                             (len(new_node2),), None, dtype=object
                         )
                         for mkey, model in self._model_dict.items():
                             idx = np.where(new_model2 == mkey)
                             tmp_node = new_node2[idx]
-                            cidx = np.where((tmp_node != None))
+                            cidx = np.where((tmp_node is not None))
                             tmp_cellid = model.modelgrid.get_lrc(
                                 tmp_node[cidx].to_list()
                             )
                             if self._modelgrid.grid_type in (
                                 "structured",
                                 "vertex",
                             ):
@@ -2557,17 +2557,17 @@
 
                     if pkg_type is None:
                         if "continuous" not in mapped_data[mkey]:
                             mapped_data[mkey]["continuous"] = {
                                 ofile: new_recarray
                             }
                         else:
-                            mapped_data[mkey]["continuous"][
-                                ofile
-                            ] = new_recarray
+                            mapped_data[mkey]["continuous"][ofile] = (
+                                new_recarray
+                            )
                     else:
                         if "observations" not in mapped_data:
                             mapped_data["observations"] = {
                                 mkey: {} for mkey in self._model_dict.keys()
                             }
 
                         if "continuous" not in mapped_data[mkey]:
@@ -2659,15 +2659,15 @@
         else:
             new_cellids = [(i,) for i in new_node]
 
         return new_cellids
 
     def _remap_adv_tag(self, mkey, recarray, item, mapper):
         """
-        Method to remap advanced package ids such as SFR's ifno varaible
+        Method to remap advanced package ids such as SFR's ifno variable
 
         Parameters
         ----------
         recarray : np.recarray
         item : str
             variable name to remap
         mapper : dict
@@ -3306,9 +3306,9 @@
         epaks = self._create_exchanges()
 
         return self._new_sim
 
 
 # todo: development notes:
 #   Then set up checks for model splitting
-#       (ex. doesnt parallel a fault, doesnt cut through a lake,
+#       (ex. doesn't parallel a fault, doesn't cut through a lake,
 #       active cells in modelgrid...)
```

### Comparing `flopy-3.6.0/flopy/mf6/utils/output_util.py` & `flopy-3.7.0/flopy/mf6/utils/output_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     Parameters
     ----------
     obj : PackageInterface object
 
     """
 
-    def __init__(self, obj):
+    def __init__(self, obj, budgetkey=None):
         from ..modflow import ModflowGwfoc, ModflowGwtoc, ModflowUtlobs
 
         # set initial observation definitions
         methods = {
             "budget": self.__budget,
             "budgetcsv": self.__budgetcsv,
             "zonebudget": self.__zonebudget,
@@ -35,14 +35,19 @@
             "csv": self.__csv,
             "package_convergence": self.__csv,
         }
         delist = ("ts", "wc")
         self._obj = obj
         self._methods = []
         self._sim_ws = obj.simulation_data.mfpath.get_sim_path()
+        self._budgetkey = (
+            "VOLUME BUDGET FOR ENTIRE MODEL"
+            if budgetkey is None
+            else budgetkey
+        )
         self.__budgetcsv = False
 
         if not isinstance(obj, (PackageInterface, ModelInterface)):
             raise TypeError("Only mf6 PackageInterface types can be used")
 
         # capture the list file for Models and for OC packages
         if isinstance(obj, (ModelInterface, ModflowGwfoc, ModflowGwtoc)):
@@ -122,19 +127,15 @@
                                                 ].array[0][0]
                                                 == "fileout"
                                             ):
                                                 data = [
                                                     [
                                                         obj._simulation_data.mfdata[
                                                             ky
-                                                        ].array[
-                                                            0
-                                                        ][
-                                                            -2
-                                                        ]
+                                                        ].array[0][-2]
                                                     ]
                                                 ]
                                                 break
 
                             if rectype == "package_convergence":
                                 rectype = "csv"
                             attr_name = f"_{rectype}"
@@ -211,15 +212,15 @@
             human readable class representation
         """
         name = self._obj.name
         if isinstance(name, list):
             name = name[0]
         l = [
             f"MF6Output Class for {name}",
-            f"Available output methods include:",
+            "Available output methods include:",
         ]
         l += [f".{m}" for m in self.methods()]
         s = "\n".join(l)
         return s
 
     def methods(self):
         """
@@ -291,15 +292,15 @@
                 pass
 
             zonbud.grb = grb
             return zonbud
 
     def __budgetcsv(self):
         """
-        Convience method to open and return a budget csv object
+        Convenience method to open and return a budget csv object
 
         Returns
         -------
             flopy.utils.CsvFile object
         """
         return self.__csv(budget=True)
 
@@ -382,15 +383,15 @@
         Returns
         -------
             Mf6ListBudget object
         """
         if self._lst is not None:
             try:
                 list_file = os.path.join(self._sim_ws, self._lst)
-                return Mf6ListBudget(list_file)
+                return Mf6ListBudget(list_file, budgetkey=self._budgetkey)
             except (AssertionError, OSError):
                 return None
 
     def __mulitfile_handler(self, f, flist):
         """
         Method to parse multiple output files of the same type
```

### Comparing `flopy-3.6.0/flopy/mf6/utils/postprocessing.py` & `flopy-3.7.0/flopy/mf6/utils/postprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
             elif nlay == 1 and ncol == 1:
                 return 1
             elif nlay == 1 and nrow == 1:
                 return 0
             else:
                 # handle 2D layers/rows case
                 return 1 if ncol == 1 else 0
-        elif d == nrow * ncol:
+        elif d % (nrow * ncol) == 0:
             return 2
         else:
             return 1
 
     # fill right, front and lower face flows
     # (below main diagonal)
     flows = [frf, fff, flf]
```

### Comparing `flopy-3.6.0/flopy/mf6/utils/reference.py` & `flopy-3.7.0/flopy/mf6/utils/reference.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mf6/utils/testutils.py` & `flopy-3.7.0/flopy/mf6/utils/testutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,16 +63,15 @@
             (
                 make_int_tuple(linesp[0:cellid_size]),
                 make_int_tuple(
                     linesp[cellid_size : cellid_size + cellid_size_2]
                 ),
                 make_int_tuple(
                     linesp[
-                        cellid_size
-                        + cellid_size_2 : cellid_size * 2
+                        cellid_size + cellid_size_2 : cellid_size * 2
                         + cellid_size_2
                     ]
                 ),
                 float(linesp[cellid_size * 2 + cellid_size_2]),
             )
         )
     return gncrecarray
```

### Comparing `flopy-3.6.0/flopy/mfusg/cln_dtypes.py` & `flopy-3.7.0/flopy/mfusg/cln_dtypes.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mfusg/mfusg.py` & `flopy-3.7.0/flopy/mfusg/mfusg.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mfusg/mfusgbcf.py` & `flopy-3.7.0/flopy/mfusg/mfusgbcf.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mfusg/mfusgcln.py` & `flopy-3.7.0/flopy/mfusg/mfusgcln.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # pylint: disable=E1101
 """
 Mfusgcln module.
 
 Contains the MfUsgCln class. Note that the user can
 access the MfUsgCln class as `flopy.mfusg.MfUsgCln`.
 
-Compatible with USG-Transport Version 1.7.0. which can be downloade from
+Compatible with USG-Transport Version 1.7.0. which can be download from
 https://www.gsi-net.com/en/software/free-software/modflow-usg.html
 
 Additional information for this MODFLOW package can be found at the `Online
 MODFLOW Guide
 Panday, S., 2021; USG-Transport Version 1.7.0: The Block-Centered Transport
 Process for MODFLOW-USG, GSI Environmental, March, 2021
 
 Panday, Sorab, Langevin, C.D., Niswonger, R.G., Ibaraki, Motomu, and Hughes,
 J.D., 2013, MODFLOW–USG version 1: An unstructured grid version of MODFLOW
 for simulating groundwater flow and tightly coupled processes using a control
 volume finite-difference formulation: U.S. Geological Survey Techniques and
 Methods, book 6, chap. A45, 66 p.
 """
+
 import numpy as np
 
 from ..pakbase import Package
 from ..utils import Util2d
 from ..utils.utils_def import get_open_file_object
 from .cln_dtypes import MfUsgClnDtypes
 from .mfusg import MfUsg, fmt_string
```

### Comparing `flopy-3.6.0/flopy/mfusg/mfusgdisu.py` & `flopy-3.7.0/flopy/mfusg/mfusgdisu.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         between nodes 1 and 2 is at the symmetric location of CL1. The array
         CL12 reads both CL1 and CL2 in the upper and lower triangular
         portions of the matrix respectively. Note that the CL1 and CL2 arrays
         are only supplied for the GWF cell connections and are internally
         expanded if CLN or GNC nodes exist in a simulation.
         (default is None.  cl1 and cl2 must be specified, or cl12 must be
         specified)
-    fahl : float or arry of floats
+    fahl : float or array of floats
         Area of the interface Anm between nodes n and m.
         (default is None.  fahl must be specified.)
     perlen : float or array of floats (nper)
         An array of the stress period lengths.
     nstp : int or array of ints (nper)
         Number of time steps in each stress period (default is 1).
     tsmult : float or array of floats (nper)
```

### Comparing `flopy-3.6.0/flopy/mfusg/mfusggnc.py` & `flopy-3.7.0/flopy/mfusg/mfusggnc.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,15 @@
         if iflalphan == 1:
             dtype.append(("AlphaN", "<f4"))
 
         return np.dtype(dtype)
 
     @staticmethod
     def get_empty(numgnc=0, numalphaj=1, iflalphan=0):
-        """Returns empty GNC recarray of defualt dtype."""
+        """Returns empty GNC recarray of default dtype."""
         # get an empty recarray that corresponds to dtype
         dtype = MfUsgGnc.get_default_dtype(numalphaj, iflalphan)
         return create_empty_recarray(numgnc, dtype, default_value=-1.0e10)
 
     @classmethod
     def load(cls, f, model, pak_type="gnc", ext_unit_dict=None, **kwargs):
         """
```

### Comparing `flopy-3.6.0/flopy/mfusg/mfusglpf.py` & `flopy-3.7.0/flopy/mfusg/mfusglpf.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mfusg/mfusgsms.py` & `flopy-3.7.0/flopy/mfusg/mfusgsms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # pylint: disable=too-many-instance-attributes
 """
 mfusgsms module.  This is the solver for MODFLOW-USG.
 
 Contains the MfUsgSms class. Note that the user can access
 the MfUsgSms class as `flopy.mfusg.MfUsgSms`.
 """
+
 from ..pakbase import Package
 from ..utils.flopy_io import line_parse
 from .mfusg import MfUsg
 
 
 class MfUsgSms(Package):
     """
```

### Comparing `flopy-3.6.0/flopy/mfusg/mfusgwel.py` & `flopy-3.7.0/flopy/mfusg/mfusgwel.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modflow/__init__.py` & `flopy-3.7.0/flopy/modflow/__init__.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modflow/mf.py` & `flopy-3.7.0/flopy/modflow/mf.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modflow/mfag.py` & `flopy-3.7.0/flopy/modflow/mfag.py`

 * *Files 0% similar despite different names*

```diff
@@ -695,15 +695,15 @@
         Method to load the AG package from file
 
         Parameters
         ----------
         f : str
             filename
         model : gsflow.modflow.Modflow object
-            model to attach the ag pacakge to
+            model to attach the ag package to
         nper : int
             number of stress periods in model
         ext_unit_dict : dict, optional
 
         Returns
         -------
             ModflowAg object
```

### Comparing `flopy-3.6.0/flopy/modflow/mfbas.py` & `flopy-3.7.0/flopy/modflow/mfbas.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,15 @@
         """
         Check package data for common errors.
 
         Parameters
         ----------
         f : str or file handle
             String defining file name or file handle for summary file
-            of check method output. If a sting is passed a file handle
+            of check method output. If a string is passed a file handle
             is created. If f is None, check method does not write
             results to a summary file. (default is None)
         verbose : bool
             Boolean flag used to determine if check method results are
             written to the screen
         level : int
             Check method analysis level. If level=0, summary checks are
```

### Comparing `flopy-3.6.0/flopy/modflow/mfbcf.py` & `flopy-3.7.0/flopy/modflow/mfbcf.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,25 +268,23 @@
                     f_bcf.write(f"{self.intercellt[k]:1d}{self.laycon[k]:1d}")
                 else:
                     f_bcf.write(f"0{self.laycon[k]:1d}")
         f_bcf.write("\n")
         f_bcf.write(self.trpy.get_file_entry())
         transient = not dis.steady.all()
         for k in range(nlay):
-            if transient == True:
+            if transient:
                 f_bcf.write(self.sf1[k].get_file_entry())
             if (self.laycon[k] == 0) or (self.laycon[k] == 2):
                 f_bcf.write(self.tran[k].get_file_entry())
             else:
                 f_bcf.write(self.hy[k].get_file_entry())
             if k < nlay - 1:
                 f_bcf.write(self.vcont[k].get_file_entry())
-            if (transient == True) and (
-                (self.laycon[k] == 2) or (self.laycon[k] == 3)
-            ):
+            if transient and ((self.laycon[k] == 2) or (self.laycon[k] == 3)):
                 f_bcf.write(self.sf2[k].get_file_entry())
             if (self.iwdflg != 0) and (
                 (self.laycon[k] == 1) or (self.laycon[k] == 3)
             ):
                 f_bcf.write(self.wetdry[k].get_file_entry())
         f_bcf.close()
```

### Comparing `flopy-3.6.0/flopy/modflow/mfbct.py` & `flopy-3.7.0/flopy/modflow/mfbct.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modflow/mfchd.py` & `flopy-3.7.0/flopy/modflow/mfchd.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modflow/mfde4.py` & `flopy-3.7.0/flopy/modflow/mfde4.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modflow/mfdis.py` & `flopy-3.7.0/flopy/modflow/mfdis.py`

 * *Files 0% similar despite different names*

```diff
@@ -608,17 +608,15 @@
             Check package data for common errors. (default True)
 
         Returns
         -------
         None
 
         """
-        if (
-            check
-        ):  # allows turning off package checks when writing files at model level
+        if check:  # allows turning off package checks when writing files at model level
             self.check(
                 f=f"{self.name[0]}.chk",
                 verbose=self.parent.verbose,
                 level=1,
             )
         # Open file for writing
         f_dis = open(self.fn_path, "w")
@@ -663,15 +661,15 @@
         """
         Check dis package data for zero and negative thicknesses.
 
         Parameters
         ----------
         f : str or file handle
             String defining file name or file handle for summary file
-            of check method output. If a sting is passed a file handle
+            of check method output. If a string is passed a file handle
             is created. If f is None, check method does not write
             results to a summary file. (default is None)
         verbose : bool
             Boolean flag used to determine if check method results are
             written to the screen
         level : int
             Check method analysis level. If level=0, summary checks are
```

### Comparing `flopy-3.6.0/flopy/modflow/mfdrn.py` & `flopy-3.7.0/flopy/modflow/mfdrn.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,17 +219,15 @@
             Check package data for common errors. (default True)
 
         Returns
         -------
         None
 
         """
-        if (
-            check
-        ):  # allows turning off package checks when writing files at model level
+        if check:  # allows turning off package checks when writing files at model level
             self.check(
                 f=f"{self.name[0]}.chk",
                 verbose=self.parent.verbose,
                 level=1,
             )
         f_drn = open(self.fn_path, "w")
         f_drn.write(f"{self.heading}\n")
```

### Comparing `flopy-3.6.0/flopy/modflow/mfdrt.py` & `flopy-3.7.0/flopy/modflow/mfdrt.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,17 +211,15 @@
             Check package data for common errors. (default True)
 
         Returns
         -------
         None
 
         """
-        if (
-            check
-        ):  # allows turning off package checks when writing files at model level
+        if check:  # allows turning off package checks when writing files at model level
             self.check(
                 f=f"{self.name[0]}.chk",
                 verbose=self.parent.verbose,
                 level=1,
             )
         f_drn = open(self.fn_path, "w")
         f_drn.write(f"{self.heading}\n")
```

### Comparing `flopy-3.6.0/flopy/modflow/mfevt.py` & `flopy-3.7.0/flopy/modflow/mfevt.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modflow/mffhb.py` & `flopy-3.7.0/flopy/modflow/mffhb.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,28 +233,30 @@
 
         # assign dataset 7
         self.ds7 = ds7
 
         # perform some simple verification
         if len(self.bdtime) != self.nbdtim:
             raise ValueError(
-                "bdtime has {} entries but requires "
-                "{} entries.".format(len(self.bdtime), self.nbdtim)
+                "bdtime has {} entries but requires " "{} entries.".format(
+                    len(self.bdtime), self.nbdtim
+                )
             )
 
         if self.nflw > 0:
             if self.ds5 is None:
                 raise TypeError(
                     f"dataset 5 is not specified but nflw > 0 ({self.nflw})"
                 )
 
             if self.ds5.shape[0] != self.nflw:
                 raise ValueError(
-                    "dataset 5 has {} rows but requires "
-                    "{} rows.".format(self.ds5.shape[0], self.nflw)
+                    "dataset 5 has {} rows but requires " "{} rows.".format(
+                        self.ds5.shape[0], self.nflw
+                    )
                 )
             nc = self.nbdtim
             if model.structured:
                 nc += 4
             else:
                 nc += 2
             if len(self.ds5.dtype.names) != nc:
@@ -266,16 +268,17 @@
         if self.nhed > 0:
             if self.ds7 is None:
                 raise TypeError(
                     f"dataset 7 is not specified but nhed > 0 ({self.nhed})"
                 )
             if self.ds7.shape[0] != self.nhed:
                 raise ValueError(
-                    "dataset 7 has {} rows but requires "
-                    "{} rows.".format(self.ds7.shape[0], self.nhed)
+                    "dataset 7 has {} rows but requires " "{} rows.".format(
+                        self.ds7.shape[0], self.nhed
+                    )
                 )
             nc = self.nbdtim
             if model.structured:
                 nc += 4
             else:
                 nc += 2
             if len(self.ds7.dtype.names) != nc:
```

### Comparing `flopy-3.6.0/flopy/modflow/mfflwob.py` & `flopy-3.7.0/flopy/modflow/mfflwob.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modflow/mfgage.py` & `flopy-3.7.0/flopy/modflow/mfgage.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modflow/mfghb.py` & `flopy-3.7.0/flopy/modflow/mfghb.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,17 +175,15 @@
             Check package data for common errors. (default True)
 
         Returns
         -------
         None
 
         """
-        if (
-            check
-        ):  # allows turning off package checks when writing files at model level
+        if check:  # allows turning off package checks when writing files at model level
             self.check(
                 f=f"{self.name[0]}.chk",
                 verbose=self.parent.verbose,
                 level=1,
             )
         f_ghb = open(self.fn_path, "w")
         f_ghb.write(f"{self.heading}\n")
```

### Comparing `flopy-3.6.0/flopy/modflow/mfgmg.py` & `flopy-3.7.0/flopy/modflow/mfgmg.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modflow/mfhfb.py` & `flopy-3.7.0/flopy/modflow/mfhfb.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modflow/mfhob.py` & `flopy-3.7.0/flopy/modflow/mfhob.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modflow/mfhyd.py` & `flopy-3.7.0/flopy/modflow/mfhyd.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modflow/mflak.py` & `flopy-3.7.0/flopy/modflow/mflak.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,16 +372,17 @@
                     f"stage_range should be a list or array of size ({nlakes}, 2)"
                 )
 
         self.dis = utils_def.get_dis(model)
         if self.dis.steady[0]:
             if stage_range.shape != (nlakes, 2):
                 raise Exception(
-                    "stages shape should be ({},2) but is only "
-                    "{}.".format(nlakes, stage_range.shape)
+                    "stages shape should be ({},2) but is only " "{}.".format(
+                        nlakes, stage_range.shape
+                    )
                 )
         self.stage_range = stage_range
 
         # tabfile data
         self.tabdata = tabdata
         self.iunit_tab = tab_units
```

### Comparing `flopy-3.6.0/flopy/modflow/mflmt.py` & `flopy-3.7.0/flopy/modflow/mflmt.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modflow/mflpf.py` & `flopy-3.7.0/flopy/modflow/mflpf.py`

 * *Files 2% similar despite different names*

```diff
@@ -367,15 +367,15 @@
         if f is None:
             f = open(self.fn_path, "w")
 
         # Item 0: text
         f.write(f"{self.heading}\n")
 
         # Item 1: IBCFCB, HDRY, NPLPF, <IKCFLAG>, OPTIONS
-        if self.parent.version == "mfusg" and self.parent.structured == False:
+        if self.parent.version == "mfusg" and not self.parent.structured:
             f.write(
                 "{:10d}{:10.6G}{:10d}{:10d} {:s}\n".format(
                     self.ipakcb,
                     self.hdry,
                     self.nplpf,
                     self.ikcflag,
                     self.options,
@@ -401,15 +401,15 @@
             f.write(f"{self.wetfct:10f}{self.iwetit:10d}{self.ihdwet:10d}\n")
         transient = not dis.steady.all()
         for k in range(nlay):
             f.write(self.hk[k].get_file_entry())
             if self.chani[k] <= 0.0:
                 f.write(self.hani[k].get_file_entry())
             f.write(self.vka[k].get_file_entry())
-            if transient == True:
+            if transient:
                 f.write(self.ss[k].get_file_entry())
                 if self.laytyp[k] != 0:
                     f.write(self.sy[k].get_file_entry())
             if dis.laycbd[k] > 0:
                 f.write(self.vkcb[k].get_file_entry())
             if self.laywet[k] != 0 and self.laytyp[k] != 0:
                 f.write(self.wetdry[k].get_file_entry())
@@ -473,15 +473,15 @@
 
         # Item 1: IBCFCB, HDRY, NPLPF - line already read above
         if model.verbose:
             print("   loading IBCFCB, HDRY, NPLPF...")
         t = line_parse(line)
         ipakcb, hdry, nplpf = int(t[0]), float(t[1]), int(t[2])
         item1_len = 3
-        if model.version == "mfusg" and model.structured == False:
+        if model.version == "mfusg" and not model.structured:
             ikcflag = int(t[3])
             item1_len = 4
         # if ipakcb != 0:
         #    model.add_pop_key_list(ipakcb)
         #    ipakcb = 53
         # options
         storagecoefficient = False
```

### Comparing `flopy-3.6.0/flopy/modflow/mfmlt.py` & `flopy-3.7.0/flopy/modflow/mfmlt.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modflow/mfmnw1.py` & `flopy-3.7.0/flopy/modflow/mfmnw1.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modflow/mfmnw2.py` & `flopy-3.7.0/flopy/modflow/mfmnw2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1071,14 +1071,20 @@
                 0: self.get_empty_stress_period_data(
                     0, aux_names=aux, structured=self.structured
                 )
             },
             dtype=self.get_default_spd_dtype(structured=self.structured),
         )
         if stress_period_data is not None:
+            stress_period_data = {
+                per: sp.to_records(index=False)
+                if isinstance(sp, pd.DataFrame)
+                else sp
+                for per, sp in stress_period_data.items()
+            }
             for per, data in stress_period_data.items():
                 spd = ModflowMnw2.get_empty_stress_period_data(
                     len(data), aux_names=aux
                 )
                 names = [n for n in data.dtype.names if n in spd.dtype.names]
                 for n in names:
                     spd[n] = data[n]
@@ -1348,17 +1354,15 @@
             )
             mnw[mnwobj.wellid] = mnwobj
             # master table with all node data
             node_data = np.append(node_data, mnwobj.node_data).view(
                 np.recarray
             )
 
-        stress_period_data = (
-            {}
-        )  # stress period data table for package (flopy convention)
+        stress_period_data = {}  # stress period data table for package (flopy convention)
         itmp = []
         for per in range(0, nper):
             # dataset 3
             itmp_per = int(line_parse(get_next_line(f))[0])
             # dataset4
             # dict might be better here to only load submitted values
             if itmp_per > 0:
```

### Comparing `flopy-3.6.0/flopy/modflow/mfmnwi.py` & `flopy-3.7.0/flopy/modflow/mfmnwi.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modflow/mfnwt.py` & `flopy-3.7.0/flopy/modflow/mfnwt.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modflow/mfoc.py` & `flopy-3.7.0/flopy/modflow/mfoc.py`

 * *Files 1% similar despite different names*

```diff
@@ -488,15 +488,15 @@
 
         Parameters
         ----------
         None
 
         Returns
         -------
-        iubud : integer ot list of integers
+        iubud : integer or list of integers
             Unit number or list of cell-by-cell budget output unit numbers.
             None is returned if ipakcb is less than one for all packages.
 
         Examples
         --------
 
         >>> import flopy
@@ -813,15 +813,15 @@
                 #  from the file based on numericformat
                 break
             # set pointer to current position in the OC file
             ipos = f.tell()
 
         # process each line
         lines = []
-        if numericformat == True:
+        if numericformat:
             for iperoc in range(nper):
                 for itsoc in range(nstp[iperoc]):
                     line = f.readline()
                     lnlst = line.strip().split()
                     incode, ihddfl = int(lnlst[0]), int(lnlst[1])
                     ibudfl, icbcfl = int(lnlst[2]), int(lnlst[3])
                     # new print and save flags are needed if incode is not
@@ -974,15 +974,15 @@
                     # add a empty list if necessary
                     iempty = False
                     if iperoc != iperoc1:
                         iempty = True
                     else:
                         if itsoc != itsoc1:
                             iempty = True
-                    if iempty == True:
+                    if iempty:
                         kperkstp = (iperoc1 - 1, itsoc1 - 1)
                         stress_period_data[kperkstp] = []
                 # dataset 3
                 elif "PRINT" in lnlst[0].upper():
                     lines.append(f"{lnlst[0].lower()} {lnlst[1].lower()}")
                 elif "SAVE" in lnlst[0].upper():
                     lines.append(f"{lnlst[0].lower()} {lnlst[1].lower()}")
@@ -1000,15 +1000,15 @@
                 # add a empty list if necessary
                 iempty = False
                 if iperoc != iperoc1:
                     iempty = True
                 else:
                     if itsoc != itsoc1:
                         iempty = True
-                if iempty == True:
+                if iempty:
                     kperkstp = (iperoc1 - 1, itsoc1 - 1)
                     stress_period_data[kperkstp] = []
 
         if openfile:
             f.close()
 
         # reset unit numbers
```

### Comparing `flopy-3.6.0/flopy/modflow/mfpar.py` & `flopy-3.7.0/flopy/modflow/mfpar.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,15 +302,15 @@
                 except:
                     pv = float(parval)
             # print partyp, parval, nclu, clusters
             if partyp == findkey:
                 for [layer, mltarr, zonarr, izones] in clusters:
                     # print layer, mltarr, zonarr, izones
                     foundlayer = False
-                    if findlayer == None:
+                    if findlayer is None:
                         foundlayer = True
                     else:
                         if layer == (findlayer + 1):
                             foundlayer = True
                     if foundlayer:
                         model.parameter_load = True
                         cluster_data = np.zeros(shape, dtype=dtype)
```

### Comparing `flopy-3.6.0/flopy/modflow/mfparbc.py` & `flopy-3.7.0/flopy/modflow/mfparbc.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modflow/mfpbc.py` & `flopy-3.7.0/flopy/modflow/mfpbc.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modflow/mfpcg.py` & `flopy-3.7.0/flopy/modflow/mfpcg.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modflow/mfpcgn.py` & `flopy-3.7.0/flopy/modflow/mfpcgn.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modflow/mfpks.py` & `flopy-3.7.0/flopy/modflow/mfpks.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,15 @@
         if self.npc > 0:
             f.write(f"RELAX {self.relax}\n")
         if self.npc == 3:
             f.write(f"IFILL {self.ifill}\n")
             f.write(f"DROPTOL {self.droptol}\n")
         f.write(f"HCLOSEPKS {self.hclose}\n")
         f.write(f"RCLOSEPKS {self.rclose}\n")
-        if self.l2norm != None:
+        if self.l2norm is not None:
             if self.l2norm.lower() == "l2norm" or self.l2norm == "1":
                 f.write("L2NORM\n")
             elif self.l2norm.lower() == "rl2norm" or self.l2norm == "2":
                 f.write("RELATIVE-L2NORM\n")
         f.write(f"IPRPKS {self.iprpks}\n")
         f.write(f"MUTPKS {self.mutpks}\n")
         # MPI
```

### Comparing `flopy-3.6.0/flopy/modflow/mfpval.py` & `flopy-3.7.0/flopy/modflow/mfpval.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modflow/mfrch.py` & `flopy-3.7.0/flopy/modflow/mfrch.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
         """
         Check package data for common errors.
 
         Parameters
         ----------
         f : str or file handle
             String defining file name or file handle for summary file
-            of check method output. If a sting is passed a file handle
+            of check method output. If a string is passed a file handle
             is created. If f is None, check method does not write
             results to a summary file. (default is None)
         verbose : bool
             Boolean flag used to determine if check method results are
             written to the screen
         level : int
             Check method analysis level. If level=0, summary checks are
```

### Comparing `flopy-3.6.0/flopy/modflow/mfriv.py` & `flopy-3.7.0/flopy/modflow/mfriv.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 Additional information for this MODFLOW package can be found at the `Online
 MODFLOW Guide
 <https://water.usgs.gov/ogw/modflow/MODFLOW-2005-Guide/riv.html>`_.
 
 """
 
 import numpy as np
+import pandas as pd
 
 from ..pakbase import Package
 from ..utils import MfList
 from ..utils.recarray_utils import create_empty_recarray
 
 
 class ModflowRiv(Package):
@@ -190,17 +191,19 @@
         >>> m.riv.check()
 
         """
         basechk = super().check(verbose=False, checktype=checktype)
         chk = self._get_check(f, verbose, level, checktype)
         chk.summary_array = basechk.summary_array
 
-        for per in self.stress_period_data.data.keys():
-            if isinstance(self.stress_period_data.data[per], np.recarray):
-                spd = self.stress_period_data.data[per]
+        for per, data in self.stress_period_data.data.items():
+            if isinstance(data, (np.recarray, pd.DataFrame)):
+                if isinstance(data, pd.DataFrame):
+                    data = data.to_records(index=False).astype(self.dtype)
+                spd = data
                 inds = (
                     (spd.k, spd.i, spd.j)
                     if self.parent.structured
                     else (spd.node)
                 )
 
                 # check that river stage and bottom are above model cell
```

### Comparing `flopy-3.6.0/flopy/modflow/mfsfr2.py` & `flopy-3.7.0/flopy/modflow/mfsfr2.py`

 * *Files 0% similar despite different names*

```diff
@@ -840,15 +840,15 @@
             if "tabfile" in line.lower():
                 t = line.strip().split()
                 options.tabfiles = True
                 options.numtab = int(t[1])
                 options.maxval = int(t[2])
                 line = f.readline()
 
-            # set varibles to be passed to class args
+            # set variables to be passed to class args
             transroute = options.transroute
             reachinput = options.reachinput
             tabfiles = isinstance(options.tabfiles, np.ndarray)
             numtab = options.numtab if tabfiles else 0
 
         # item 1c
         (
@@ -901,17 +901,15 @@
 
         # items 3 and 4 are skipped (parameters not supported)
         # item 5
         segment_data = {}
         channel_geometry_data = {}
         channel_flow_data = {}
         dataset_5 = {}
-        aux_variables = (
-            {}
-        )  # not sure where the auxiliary variables are supposed to go
+        aux_variables = {}  # not sure where the auxiliary variables are supposed to go
         for i in range(0, nper):
             # Dataset 5
             dataset_5[i] = _get_dataset(f.readline(), [-1, 0, 0, 0])
             itmp = dataset_5[i][0]
             if itmp > 0:
                 # Item 6
                 current = ModflowSfr2.get_empty_segment_data(
@@ -2342,15 +2340,15 @@
         """
         headertxt = "Checking for nan values...\n"
         txt = ""
         passed = False
         isnan = np.any(np.isnan(np.array(self.reach_data.tolist())), axis=1)
         nanreaches = self.reach_data[isnan]
         if np.any(isnan):
-            txt += f"Found {len(nanreaches)} reachs with nans:\n"
+            txt += f"Found {len(nanreaches)} reaches with nans:\n"
             if self.level == 1:
                 txt += _print_rec_array(nanreaches, delimiter=" ")
         for per, sd in self.segment_data.items():
             isnan = np.any(np.isnan(np.array(sd.tolist())), axis=1)
             nansd = sd[isnan]
             if np.any(isnan):
                 txt += (
```

### Comparing `flopy-3.6.0/flopy/modflow/mfsip.py` & `flopy-3.7.0/flopy/modflow/mfsip.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modflow/mfsor.py` & `flopy-3.7.0/flopy/modflow/mfsor.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modflow/mfstr.py` & `flopy-3.7.0/flopy/modflow/mfstr.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modflow/mfsub.py` & `flopy-3.7.0/flopy/modflow/mfsub.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modflow/mfswi2.py` & `flopy-3.7.0/flopy/modflow/mfswi2.py`

 * *Files 0% similar despite different names*

```diff
@@ -415,15 +415,15 @@
                 self.iswizt,
                 self.ipakcb,
                 self.iswiobs,
             )
         )
 
         # write SWI2 options
-        if self.options != None:
+        if self.options is not None:
             for o in self.options:
                 f.write(f" {o}")
         f.write("\n")
 
         # write dataset 2a
         f.write("# Dataset 2a\n")
         f.write(f"{self.nsolver:10d}{self.iprsol:10d}{self.mutsol:10d}\n")
```

### Comparing `flopy-3.6.0/flopy/modflow/mfswr1.py` & `flopy-3.7.0/flopy/modflow/mfswr1.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modflow/mfswt.py` & `flopy-3.7.0/flopy/modflow/mfswt.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modflow/mfupw.py` & `flopy-3.7.0/flopy/modflow/mfupw.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modflow/mfuzf1.py` & `flopy-3.7.0/flopy/modflow/mfuzf1.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modflow/mfwel.py` & `flopy-3.7.0/flopy/modflow/mfwel.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,16 +218,16 @@
                     if name.lower() in option.lower():
                         ladd = False
                         break
                 if ladd:
                     options.append(f"aux {name} ")
 
         if isinstance(self.options, OptionBlock):
-            if not self.options.auxillary:
-                self.options.auxillary = options
+            if not self.options.auxiliary:
+                self.options.auxiliary = options
         else:
             self.options = options
 
         # initialize MfList
         self.stress_period_data = MfList(
             self, stress_period_data, binary=binary
         )
@@ -278,17 +278,17 @@
                 self.options.write_options(f_wel)
 
         line = f" {self.stress_period_data.mxact:9d} {self.ipakcb:9d} "
 
         if isinstance(self.options, OptionBlock):
             if self.options.noprint:
                 line += "NOPRINT "
-            if self.options.auxillary:
+            if self.options.auxiliary:
                 line += " ".join(
-                    [str(aux).upper() for aux in self.options.auxillary]
+                    [str(aux).upper() for aux in self.options.auxiliary]
                 )
 
         else:
             for opt in self.options:
                 line += " " + str(opt)
 
         line += "\n"
```

### Comparing `flopy-3.6.0/flopy/modflow/mfzon.py` & `flopy-3.7.0/flopy/modflow/mfzon.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modflowlgr/mflgr.py` & `flopy-3.7.0/flopy/modflowlgr/mflgr.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modpath/mp6.py` & `flopy-3.7.0/flopy/modpath/mp6.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,15 @@
 
     # function to encapsulate next_ext_unit attribute
     def next_ext_unit(self):
         self.__next_ext_unit += 1
         return self.__next_ext_unit
 
     def getsim(self):
-        if self.__sim == None:
+        if self.__sim is None:
             for p in self.packagelist:
                 if isinstance(p, Modpath6Sim):
                     self.__sim = p
         return self.__sim
 
     def getmf(self):
         return self.__mf
```

### Comparing `flopy-3.6.0/flopy/modpath/mp6bas.py` & `flopy-3.7.0/flopy/modpath/mp6bas.py`

 * *Files 4% similar despite different names*

```diff
@@ -185,38 +185,38 @@
             if self.parent.getmf() is None:
                 raise ValueError(
                     "if modflowmodel is None then laytype must be passed"
                 )
 
             # run though flow packages
             flow_package = self.parent.getmf().get_package("BCF6")
-            if flow_package != None:
+            if flow_package is not None:
                 lc = Util2d(
                     self.parent,
                     (nlay,),
                     np.int32,
                     flow_package.laycon.get_value(),
                     name="bas - laytype",
                     locat=self.unit_number[0],
                 )
                 have_layertype = True
 
             flow_package = self.parent.getmf().get_package("LPF")
-            if flow_package != None and not have_layertype:
+            if flow_package is not None and not have_layertype:
                 lc = Util2d(
                     self.parent,
                     (nlay,),
                     np.int32,
                     flow_package.laytyp.get_value(),
                     name="bas - laytype",
                     locat=self.unit_number[0],
                 )
                 have_layertype = True
             flow_package = self.parent.getmf().get_package("UPW")
-            if flow_package != None and have_layertype:
+            if flow_package is not None and have_layertype:
                 lc = Util2d(
                     self.parent,
                     (nlay,),
                     np.int32,
                     flow_package.laytyp.get_value(),
                     name="bas - laytype",
                     locat=self.unit_number[0],
```

### Comparing `flopy-3.6.0/flopy/modpath/mp6sim.py` & `flopy-3.7.0/flopy/modpath/mp6sim.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,15 @@
         """
         Check package data for common errors.
 
         Parameters
         ----------
         f : str or file handle
             String defining file name or file handle for summary file
-            of check method output. If a sting is passed a file handle
+            of check method output. If a string is passed a file handle
             is created. If f is None, check method does not write
             results to a summary file. (default is None)
         verbose : bool
             Boolean flag used to determine if check method results are
             written to the screen
         level : int
             Check method analysis level. If level=0, summary checks are
```

### Comparing `flopy-3.6.0/flopy/modpath/mp7.py` & `flopy-3.7.0/flopy/modpath/mp7.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modpath/mp7bas.py` & `flopy-3.7.0/flopy/modpath/mp7bas.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modpath/mp7particledata.py` & `flopy-3.7.0/flopy/modpath/mp7particledata.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,36 @@
 """
-mp7particledata module. Contains the ParticleData, CellDataType,
-    FaceDataType, and NodeParticleData classes.
+Support for MODPATH 7 particle release configurations. Contains the
+ParticleData, CellDataType, FaceDataType, and NodeParticleData classes.
 
 
 """
 
+from collections import namedtuple
 from itertools import product
-from typing import Generator, Iterator, Tuple
+from typing import Iterator, Tuple
 
 import numpy as np
 import pandas as pd
 from numpy.lib.recfunctions import unstructured_to_structured
 
 from ..utils.recarray_utils import create_empty_recarray
 
 
+def reversed_product(*iterables, repeat=1):
+    """
+    Like `itertools.product()`, but left-most elements advance first.
+
+    Adapted from https://stackoverflow.com/a/32998481/6514033.
+    """
+
+    for t in product(*reversed(iterables), repeat=repeat):
+        yield tuple(reversed(t))
+
+
 class ParticleData:
     """
     Class to create the most basic particle data type (starting location
     input style 1). Input style 1 is the most general input style and
     provides the most flexibility in customizing starting locations.
 
     Parameters
@@ -324,15 +336,15 @@
         self.particleidoption = particleidoption
         self.locationstyle = locationstyle
         self.dtype = particledata.dtype
         self.particledata = pd.DataFrame.from_records(particledata)
 
     def write(self, f=None):
         """
-        Write the particle data to disk.
+        Write the particle data template to a file.
 
         Parameters
         ----------
         f : fileobject
             Fileobject that is open with write access
         """
         # validate that a valid file object was passed
@@ -359,36 +371,39 @@
             d["id"] += 1
 
         # write the particle data
         fmt = self._fmt_string + "\n"
         for v in d:
             f.write(fmt.format(*v))
 
-    def to_coords(self, grid) -> Iterator[tuple]:
+    def to_coords(self, grid, localz=False) -> Iterator[tuple]:
         """
-        Compute global particle coordinates on the given grid.
+        Compute particle coordinates on the given grid.
 
         Parameters
         ----------
-        grid : The grid on which to locate particle release points.
+        grid : flopy.discretization.grid.Grid
+            The grid on which to locate particle release points.
+        localz : bool, optional
+            Whether to return local z coordinates.
 
         Returns
         -------
             Generates coordinate tuples (x, y, z)
         """
 
         def cvt_xy(p, vs):
             mn, mx = min(vs), max(vs)
             span = mx - mn
             return mn + span * p
 
         if grid.grid_type == "structured":
             if not hasattr(self.particledata, "k"):
                 raise ValueError(
-                    f"Particle representation is not structured but grid is"
+                    "Particle representation is not structured but grid is"
                 )
 
             def cvt_z(p, k, i, j):
                 mn, mx = (
                     grid.botm[k, i, j],
                     grid.top[i, j] if k == 0 else grid.botm[k - 1, i, j],
                 )
@@ -397,21 +412,23 @@
 
             def convert(row) -> Tuple[float, float, float]:
                 verts = grid.get_cell_vertices(row.i, row.j)
                 xs, ys = list(zip(*verts))
                 return [
                     cvt_xy(row.localx, xs),
                     cvt_xy(row.localy, ys),
-                    cvt_z(row.localz, row.k, row.i, row.j),
+                    row.localz
+                    if localz
+                    else cvt_z(row.localz, row.k, row.i, row.j),
                 ]
 
         else:
             if hasattr(self.particledata, "k"):
                 raise ValueError(
-                    f"Particle representation is structured but grid is not"
+                    "Particle representation is structured but grid is not"
                 )
 
             def cvt_z(p, nn):
                 k, j = grid.get_lni([nn])[0]
                 mn, mx = (
                     grid.botm[k, j],
                     grid.top[j] if k == 0 else grid.botm[k - 1, j],
@@ -421,44 +438,47 @@
 
             def convert(row) -> Tuple[float, float, float]:
                 verts = grid.get_cell_vertices(row.node)
                 xs, ys = list(zip(*verts))
                 return [
                     cvt_xy(row.localx, xs),
                     cvt_xy(row.localy, ys),
-                    cvt_z(row.localz, row.node),
+                    row.localz if localz else cvt_z(row.localz, row.node),
                 ]
 
         for t in self.particledata.itertuples():
             yield convert(t)
 
-    def to_prp(self, grid) -> Iterator[tuple]:
+    def to_prp(self, grid, localz=False) -> Iterator[tuple]:
         """
         Convert particle data to PRT particle release point (PRP)
         package data entries for the given grid. A model grid is
         required because MODPATH supports several ways to specify
         particle release locations by cell ID and subdivision info
         or local coordinates, but PRT expects global coordinates.
 
         Parameters
         ----------
-        grid : The grid on which to locate particle release points.
+        grid : flopy.discretization.grid.Grid
+            The grid on which to locate particle release points.
+        localz : bool, optional
+            Whether to return local z coordinates.
 
         Returns
         -------
             Generates PRT particle release point (PRP) package
             data tuples: release point index, k, [i,] j, x, y, z.
             If the grid is not structured, i is omitted and j is
             the within-layer cell index for vertex grids.
         """
 
         for i, (t, c) in enumerate(
             zip(
                 self.particledata.itertuples(index=False),
-                self.to_coords(grid),
+                self.to_coords(grid, localz),
             )
         ):
             row = [i]  # release point index (irpt)
             if "node" in self.particledata:
                 k, j = grid.get_lni([t.node])[0]
                 row.extend([(k, j)])
             else:
@@ -683,16 +703,14 @@
             self.rowdivisions5,
             self.columndivisions5,
             self.rowdivisions6,
             self.columndivisions6,
         )
         f.write(line)
 
-        return
-
 
 class CellDataType:
     """
     Cell data type class to create a MODPATH 7 particle location template for
     input style 2, 3, and 4 in cells (templatesubdivisiontype = 2).
 
     Parameters
@@ -741,23 +759,21 @@
         self.drape = drape
         self.columncelldivisions = columncelldivisions
         self.rowcelldivisions = rowcelldivisions
         self.layercelldivisions = layercelldivisions
 
     def write(self, f=None):
         """
+        Write the cell data template to a file.
 
         Parameters
         ----------
         f : fileobject
             Fileobject that is open with write access
 
-        Returns
-        -------
-
         """
         # validate that a valid file object was passed
         if not hasattr(f, "write"):
             raise ValueError(
                 "{}: cannot write data for template "
                 "without passing a valid file object ({}) "
                 "open for writing".format(self.name, f)
@@ -769,185 +785,244 @@
             self.columncelldivisions,
             self.rowcelldivisions,
             self.layercelldivisions,
         )
         f.write(line)
 
 
-def get_release_points(subdivisiondata, grid, k=None, i=None, j=None, nn=None):
-    if nn is None and (k is None or i is None or j is None):
-        raise ValueError(
-            f"A cell (node) must be specified by indices (for structured grids) or node number (for vertex/unstructured)"
-        )
+Extent = namedtuple(
+    "Extent",
+    [
+        "minx",
+        "maxx",
+        "miny",
+        "maxy",
+        "minz",
+        "maxz",
+        "xspan",
+        "yspan",
+        "zspan",
+    ],
+)
 
-    rpts = []
-    template = [k, i, j] if nn is None else [nn]
 
+def get_extent(grid, k=None, i=None, j=None, nn=None, localz=False) -> Extent:
     # get cell coords and span in each dimension
     if not (k is None or i is None or j is None):
         verts = grid.get_cell_vertices(i, j)
-        minz, maxz = grid.botm[k, i, j], grid.top[i, j]
+        minz, maxz = (0, 1) if localz else (grid.botm[k, i, j], grid.top[i, j])
     elif nn is not None:
         verts = grid.get_cell_vertices(nn)
         if grid.grid_type == "structured":
             k, i, j = grid.get_lrc([nn])[0]
             minz, maxz = (
                 grid.botm[k, i, j],
                 grid.top[i, j] if k == 0 else grid.botm[k - 1, i, j],
             )
         else:
             k, j = grid.get_lni([nn])[0]
             minz, maxz = (
-                grid.botm[k, j],
-                grid.top[j] if k == 0 else grid.botm[k - 1, j],
+                (0, 1)
+                if localz
+                else (
+                    grid.botm[k, j],
+                    grid.top[j] if k == 0 else grid.botm[k - 1, j],
+                )
             )
     else:
         raise ValueError(
-            f"A cell (node) must be specified by indices (for structured grids) or node number (for vertex/unstructured)"
+            "A cell (node) must be specified by indices (for structured grids) or node number (for vertex/unstructured)"
         )
     xs, ys = list(zip(*verts))
     minx, maxx = min(xs), max(xs)
     miny, maxy = min(ys), max(ys)
     xspan = maxx - minx
     yspan = maxy - miny
     zspan = maxz - minz
+    return Extent(minx, maxx, miny, maxy, minz, maxz, xspan, yspan, zspan)
 
-    if isinstance(subdivisiondata, FaceDataType):
-        # x1 (west)
-        if (
-            subdivisiondata.verticaldivisions1 > 0
-            and subdivisiondata.horizontaldivisions1 > 0
-        ):
-            yincr = yspan / subdivisiondata.horizontaldivisions1
-            ylocs = [
-                (miny + (yincr * 0.5) + (yincr * d))
-                for d in range(subdivisiondata.horizontaldivisions1)
-            ]
-            zincr = zspan / subdivisiondata.verticaldivisions1
-            zlocs = [
-                (minz + (zincr * 0.5) + (zincr * d))
-                for d in range(subdivisiondata.verticaldivisions1)
-            ]
-            prod = list(product(*[ylocs, zlocs]))
-            rpts = rpts + [template + [minx, p[0], p[1]] for p in prod]
 
-        # x2 (east)
-        if (
-            subdivisiondata.verticaldivisions2 > 0
-            and subdivisiondata.horizontaldivisions2 > 0
-        ):
-            yincr = yspan / subdivisiondata.horizontaldivisions2
-            ylocs = [
-                (miny + (yincr * 0.5) + (yincr * d))
-                for d in range(subdivisiondata.horizontaldivisions2)
-            ]
-            zincr = zspan / subdivisiondata.verticaldivisions2
-            zlocs = [
-                (minz + (zincr * 0.5) + (zincr * d))
-                for d in range(subdivisiondata.verticaldivisions2)
-            ]
-            prod = list(product(*[ylocs, zlocs]))
-            rpts = rpts + [template + [maxx, p[0], p[1]] for p in prod]
+def get_face_release_points(
+    subdivisiondata, cellid, extent
+) -> Iterator[tuple]:
+    """
+    Get release points for MODPATH 7 input style 2, template
+    subdivision style 1, i.e. face (2D) subdivision, for the
+    given cell with the given extent.
+    """
 
-        # y1 (south)
-        if (
-            subdivisiondata.verticaldivisions3 > 0
-            and subdivisiondata.horizontaldivisions3 > 0
-        ):
-            xincr = xspan / subdivisiondata.horizontaldivisions3
-            xlocs = [
-                (minx + (xincr * 0.5) + (xincr * rd))
-                for rd in range(subdivisiondata.horizontaldivisions3)
-            ]
-            zincr = zspan / subdivisiondata.verticaldivisions3
-            zlocs = [
-                (minz + (zincr * 0.5) + (zincr * d))
-                for d in range(subdivisiondata.verticaldivisions3)
-            ]
-            prod = list(product(*[xlocs, zlocs]))
-            rpts = rpts + [template + [p[0], miny, p[1]] for p in prod]
+    # Product incrementing left elements first, to
+    # match the release point ordering used by MP7
+    product = reversed_product
+
+    # x1 (west)
+    if (
+        subdivisiondata.verticaldivisions1 > 0
+        and subdivisiondata.horizontaldivisions1 > 0
+    ):
+        yincr = extent.yspan / subdivisiondata.horizontaldivisions1
+        ylocs = [
+            (extent.miny + (yincr * 0.5) + (yincr * d))
+            for d in range(subdivisiondata.horizontaldivisions1)
+        ]
+        zincr = extent.zspan / subdivisiondata.verticaldivisions1
+        zlocs = [
+            (extent.minz + (zincr * 0.5) + (zincr * d))
+            for d in range(subdivisiondata.verticaldivisions1)
+        ]
+        for p in product(*[ylocs, zlocs]):
+            yield cellid + [extent.minx, p[0], p[1]]
 
-        # y2 (north)
-        if (
-            subdivisiondata.verticaldivisions4 > 0
-            and subdivisiondata.horizontaldivisions4 > 0
-        ):
-            xincr = xspan / subdivisiondata.horizontaldivisions4
-            xlocs = [
-                (minx + (xincr * 0.5) + (xincr * rd))
-                for rd in range(subdivisiondata.horizontaldivisions4)
-            ]
-            zincr = zspan / subdivisiondata.verticaldivisions4
-            zlocs = [
-                (minz + (zincr * 0.5) + (zincr * d))
-                for d in range(subdivisiondata.verticaldivisions4)
-            ]
-            prod = list(product(*[xlocs, zlocs]))
-            rpts = rpts + [template + [p[0], maxy, p[1]] for p in prod]
+    # x2 (east)
+    if (
+        subdivisiondata.verticaldivisions2 > 0
+        and subdivisiondata.horizontaldivisions2 > 0
+    ):
+        yincr = extent.yspan / subdivisiondata.horizontaldivisions2
+        ylocs = [
+            (extent.miny + (yincr * 0.5) + (yincr * d))
+            for d in range(subdivisiondata.horizontaldivisions2)
+        ]
+        zincr = extent.zspan / subdivisiondata.verticaldivisions2
+        zlocs = [
+            (extent.minz + (zincr * 0.5) + (zincr * d))
+            for d in range(subdivisiondata.verticaldivisions2)
+        ]
+        for p in product(*[ylocs, zlocs]):
+            yield cellid + [extent.maxx, p[0], p[1]]
 
-        # z1 (bottom)
-        if (
-            subdivisiondata.rowdivisions5 > 0
-            and subdivisiondata.columndivisions5 > 0
-        ):
-            xincr = xspan / subdivisiondata.columndivisions5
-            xlocs = [
-                (minx + (xincr * 0.5) + (xincr * rd))
-                for rd in range(subdivisiondata.columndivisions5)
-            ]
-            yincr = yspan / subdivisiondata.rowdivisions5
-            ylocs = [
-                (miny + (yincr * 0.5) + (yincr * rd))
-                for rd in range(subdivisiondata.rowdivisions5)
-            ]
-            prod = list(product(*[xlocs, ylocs]))
-            rpts = rpts + [template + [p[0], p[1], minz] for p in prod]
+    # y1 (south)
+    if (
+        subdivisiondata.verticaldivisions3 > 0
+        and subdivisiondata.horizontaldivisions3 > 0
+    ):
+        xincr = extent.xspan / subdivisiondata.horizontaldivisions3
+        xlocs = [
+            (extent.minx + (xincr * 0.5) + (xincr * rd))
+            for rd in range(subdivisiondata.horizontaldivisions3)
+        ]
+        zincr = extent.zspan / subdivisiondata.verticaldivisions3
+        zlocs = [
+            (extent.minz + (zincr * 0.5) + (zincr * d))
+            for d in range(subdivisiondata.verticaldivisions3)
+        ]
+        for p in product(*[xlocs, zlocs]):
+            yield cellid + [p[0], extent.miny, p[1]]
 
-        # z2 (top)
-        if (
-            subdivisiondata.rowdivisions6 > 0
-            and subdivisiondata.columndivisions6 > 0
-        ):
-            xincr = xspan / subdivisiondata.columndivisions6
-            xlocs = [
-                (minx + (xincr * 0.5) + (xincr * rd))
-                for rd in range(subdivisiondata.columndivisions6)
-            ]
-            yincr = yspan / subdivisiondata.rowdivisions6
-            ylocs = [
-                (miny + (yincr * 0.5) + (yincr * rd))
-                for rd in range(subdivisiondata.rowdivisions6)
-            ]
-            prod = list(product(*[xlocs, ylocs]))
-            rpts = rpts + [template + [p[0], p[1], maxz] for p in prod]
-    elif isinstance(subdivisiondata, CellDataType):
-        xincr = xspan / subdivisiondata.columncelldivisions
+    # y2 (north)
+    if (
+        subdivisiondata.verticaldivisions4 > 0
+        and subdivisiondata.horizontaldivisions4 > 0
+    ):
+        xincr = extent.xspan / subdivisiondata.horizontaldivisions4
         xlocs = [
-            (minx + (xincr * 0.5) + (xincr * rd))
-            for rd in range(subdivisiondata.columncelldivisions)
+            (extent.minx + (xincr * 0.5) + (xincr * rd))
+            for rd in range(subdivisiondata.horizontaldivisions4)
+        ]
+        zincr = extent.zspan / subdivisiondata.verticaldivisions4
+        zlocs = [
+            (extent.minz + (zincr * 0.5) + (zincr * d))
+            for d in range(subdivisiondata.verticaldivisions4)
         ]
-        yincr = yspan / subdivisiondata.rowcelldivisions
+        for p in product(*[xlocs, zlocs]):
+            yield cellid + [p[0], extent.maxy, p[1]]
+
+    # z1 (bottom)
+    if (
+        subdivisiondata.rowdivisions5 > 0
+        and subdivisiondata.columndivisions5 > 0
+    ):
+        xincr = extent.xspan / subdivisiondata.columndivisions5
+        xlocs = [
+            (extent.minx + (xincr * 0.5) + (xincr * rd))
+            for rd in range(subdivisiondata.columndivisions5)
+        ]
+        yincr = extent.yspan / subdivisiondata.rowdivisions5
         ylocs = [
-            (miny + (yincr * 0.5) + (yincr * d))
-            for d in range(subdivisiondata.rowcelldivisions)
+            (extent.miny + (yincr * 0.5) + (yincr * rd))
+            for rd in range(subdivisiondata.rowdivisions5)
         ]
-        zincr = zspan / subdivisiondata.layercelldivisions
-        zlocs = [
-            (minz + (zincr * 0.5) + (zincr * d))
-            for d in range(subdivisiondata.layercelldivisions)
+        for p in product(*[xlocs, ylocs]):
+            yield cellid + [p[0], p[1], extent.minz]
+
+    # z2 (top)
+    if (
+        subdivisiondata.rowdivisions6 > 0
+        and subdivisiondata.columndivisions6 > 0
+    ):
+        xincr = extent.xspan / subdivisiondata.columndivisions6
+        xlocs = [
+            (extent.minx + (xincr * 0.5) + (xincr * rd))
+            for rd in range(subdivisiondata.columndivisions6)
         ]
-        prod = list(product(*[xlocs, ylocs, zlocs]))
-        rpts = rpts + [template + [p[0], p[1], p[2]] for p in prod]
+        yincr = extent.yspan / subdivisiondata.rowdivisions6
+        ylocs = [
+            (extent.miny + (yincr * 0.5) + (yincr * rd))
+            for rd in range(subdivisiondata.rowdivisions6)
+        ]
+        for p in product(*[xlocs, ylocs]):
+            yield cellid + [p[0], p[1], extent.maxz]
+
+
+def get_cell_release_points(
+    subdivisiondata, cellid, extent
+) -> Iterator[tuple]:
+    """
+    Get release points for MODPATH 7 input style 2, template
+    subdivision type 2, i.e. cell (3D) subdivision, for the
+    given cell with the given extent.
+    """
+
+    # Product incrementing left elements first, to
+    # match the release point ordering used by MP7
+    product = reversed_product
+
+    xincr = extent.xspan / subdivisiondata.columncelldivisions
+    xlocs = [
+        (extent.minx + (xincr * 0.5) + (xincr * rd))
+        for rd in range(subdivisiondata.columncelldivisions)
+    ]
+    yincr = extent.yspan / subdivisiondata.rowcelldivisions
+    ylocs = [
+        (extent.miny + (yincr * 0.5) + (yincr * d))
+        for d in range(subdivisiondata.rowcelldivisions)
+    ]
+    zincr = extent.zspan / subdivisiondata.layercelldivisions
+    zlocs = [
+        (extent.minz + (zincr * 0.5) + (zincr * d))
+        for d in range(subdivisiondata.layercelldivisions)
+    ]
+    for p in product(*[xlocs, ylocs, zlocs]):
+        yield cellid + [p[0], p[1], p[2]]
+
+
+def get_release_points(
+    subdivisiondata, grid, k=None, i=None, j=None, nn=None, localz=False
+) -> Iterator[tuple]:
+    """
+    Get MODPATH 7 release point tuples for the given cell.
+    """
+
+    if nn is None and (k is None or i is None or j is None):
+        raise ValueError(
+            "A cell (node) must be specified by indices (for structured grids) or node number (for vertex/unstructured)"
+        )
+
+    cellid = [k, i, j] if nn is None else [nn]
+    extent = get_extent(grid, k, i, j, nn, localz)
+
+    if isinstance(subdivisiondata, FaceDataType):
+        return get_face_release_points(subdivisiondata, cellid, extent)
+    elif isinstance(subdivisiondata, CellDataType):
+        return get_cell_release_points(subdivisiondata, cellid, extent)
     else:
         raise ValueError(
             f"Unsupported subdivision data type: {type(subdivisiondata)}"
         )
 
-    return rpts
-
 
 class LRCParticleData:
     """
     MODPATH 7 particle release location template class for particle input style 2.
     Assigns particles to locations on cell faces (templatesubdivisiontype=1) and/or
     in cells (templatesubdivisiontype=2) for cells specified by (layer, row, column).
 
@@ -975,15 +1050,15 @@
         """
         self.name = "LRCParticleData"
 
         if subdivisiondata is None:
             subdivisiondata = CellDataType()
 
         if lrcregions is None:
-            lrcregions = [[0, 0, 0, 0, 0, 0]]
+            lrcregions = [[[0, 0, 0, 0, 0, 0]]]
 
         if isinstance(subdivisiondata, (CellDataType, FaceDataType)):
             subdivisiondata = [subdivisiondata]
 
         for idx, fd in enumerate(subdivisiondata):
             if not isinstance(fd, (CellDataType, FaceDataType)):
                 raise TypeError(
@@ -1031,36 +1106,33 @@
             if shapel[1] != 6:
                 raise ValueError(
                     "{}: Each lrcregions entry must "
                     "have 6 columns passed lrcregions has "
                     "{} columns".format(self.name, shapel[1])
                 )
 
-        #
         totalcellregioncount = 0
         for lrcregion in lrcregions:
             totalcellregioncount += lrcregion.shape[0]
 
         # assign attributes
         self.particletemplatecount = shape
         self.totalcellregioncount = totalcellregioncount
         self.subdivisiondata = subdivisiondata
         self.lrcregions = lrcregions
 
     def write(self, f=None):
         """
+        Write the layer-row-column particle data template to a file.
 
         Parameters
         ----------
         f : fileobject
             Fileobject that is open with write access
 
-        Returns
-        -------
-
         """
         # validate that a valid file object was passed
         if not hasattr(f, "write"):
             raise ValueError(
                 "{}: cannot write data for template "
                 "without passing a valid file object ({}) "
                 "open for writing".format(self.name, f)
@@ -1082,72 +1154,80 @@
             for row in region:
                 line = ""
                 for lrc in row:
                     line += f"{lrc + 1} "
                 line += "\n"
                 f.write(line)
 
-    def to_coords(self, grid) -> Iterator[tuple]:
+    def to_coords(self, grid, localz=False) -> Iterator[tuple]:
         """
         Compute global particle coordinates on the given grid.
 
         Parameters
         ----------
-        grid : The grid on which to locate particle release points.
+        grid : flopy.discretization.grid.Grid
+            The grid on which to locate particle release points.
+        localz : bool, optional
+            Whether to return local z coordinates.
 
         Returns
         -------
             Generator of coordinate tuples (x, y, z)
         """
 
         for region in self.lrcregions:
             for row in region:
                 mink, mini, minj, maxk, maxi, maxj = row
                 for k in range(mink, maxk + 1):
                     for i in range(mini, maxi + 1):
                         for j in range(minj, maxj + 1):
                             for sd in self.subdivisiondata:
                                 for rpt in get_release_points(
-                                    sd, grid, k, i, j
+                                    sd, grid, k, i, j, localz=localz
                                 ):
-                                    yield (rpt[3], rpt[4], rpt[5])
+                                    yield (*rpt[3:6],)
 
-    def to_prp(self, grid) -> Iterator[tuple]:
+    def to_prp(self, grid, localz=False) -> Iterator[tuple]:
         """
         Convert particle data to PRT particle release point (PRP)
         package data entries for the given grid. A model grid is
         required because MODPATH supports several ways to specify
         particle release locations by cell ID and subdivision info
         or local coordinates, but PRT expects global coordinates.
 
         Parameters
         ----------
-        grid : The grid on which to locate particle release points.
+        grid : flopy.discretization.grid.Grid
+            The grid on which to locate particle release points.
+        localz : bool, optional
+            Whether to return local z coordinates.
 
         Returns
         -------
             Generates PRT particle release point (PRP) package
             data tuples: release point index, k, i, j, x, y, z
         """
 
         if grid.grid_type != "structured":
             raise ValueError(
-                f"Particle representation is structured but grid is not"
+                "Particle representation is structured but grid is not"
             )
 
         irpt_offset = 0
         for region in self.lrcregions:
             for row in region:
                 mink, mini, minj, maxk, maxi, maxj = row
                 for k in range(mink, maxk + 1):
                     for i in range(mini, maxi + 1):
                         for j in range(minj, maxj + 1):
                             for sd in self.subdivisiondata:
                                 for irpt, rpt in enumerate(
-                                    get_release_points(sd, grid, k, i, j)
+                                    get_release_points(
+                                        sd, grid, k, i, j, localz=localz
+                                    )
                                 ):
                                     assert rpt[0] == k
                                     assert rpt[1] == i
                                     assert rpt[2] == j
                                     yield (
                                         irpt_offset + irpt,
                                         k,
@@ -1268,23 +1348,21 @@
         self.particletemplatecount = shape
         self.totalcellcount = totalcellcount
         self.subdivisiondata = subdivisiondata
         self.nodedata = nodes
 
     def write(self, f=None):
         """
+        Write the node particle data template to a file.
 
         Parameters
         ----------
         f : fileobject
             Fileobject that is open with write access
 
-        Returns
-        -------
-
         """
         # validate that a valid file object was passed
         if not hasattr(f, "write"):
             raise ValueError(
                 "{}: cannot write data for template "
                 "without passing a valid file object ({}) "
                 "open for writing".format(self.name, f)
@@ -1310,55 +1388,63 @@
                 if idx > 0:
                     if idx % 10 == 0 or idx == nodes.shape[0] - 1:
                         lineend = True
                 if lineend:
                     line += "\n"
             f.write(line)
 
-    def to_coords(self, grid) -> Iterator[tuple]:
+    def to_coords(self, grid, localz=False) -> Iterator[tuple]:
         """
         Compute global particle coordinates on the given grid.
 
         Parameters
         ----------
-        grid : The grid on which to locate particle release points.
+        grid : flopy.discretization.grid.Grid
+            The grid on which to locate particle release points.
+        localz : bool, optional
+            Whether to return local z coordinates.
 
         Returns
         -------
             Generator of coordinate tuples (x, y, z)
         """
 
         for sd in self.subdivisiondata:
             for nd in self.nodedata:
-                rpts = get_release_points(sd, grid, nn=int(nd[0]))
-                for i, rpt in enumerate(rpts):
-                    yield (rpt[1], rpt[2], rpt[3])
+                for rpt in get_release_points(
+                    sd, grid, nn=int(nd[0]), localz=localz
+                ):
+                    yield (*rpt[1:4],)
 
-    def to_prp(self, grid) -> Iterator[tuple]:
+    def to_prp(self, grid, localz=False) -> Iterator[tuple]:
         """
         Convert particle data to PRT particle release point (PRP)
         package data entries for the given grid. A model grid is
         required because MODPATH supports several ways to specify
         particle release locations by cell ID and subdivision info
         or local coordinates, but PRT expects global coordinates.
 
         Parameters
         ----------
-        grid : The grid on which to locate particle release points.
+        grid : flopy.discretization.grid.Grid
+            The grid on which to locate particle release points.
+        localz : bool, optional
+            Whether to return local z coordinates.
 
         Returns
         -------
             Generator of PRT particle release point (PRP) package
             data tuples: release point index, k, j, x, y, z
         """
 
         for sd in self.subdivisiondata:
             for nd in self.nodedata:
-                rpts = get_release_points(sd, grid, nn=int(nd[0]))
-                for irpt, rpt in enumerate(rpts):
+                for irpt, rpt in enumerate(
+                    get_release_points(sd, grid, nn=int(nd[0]), localz=localz)
+                ):
                     row = [irpt]
                     if grid.grid_type == "structured":
                         k, i, j = grid.get_lrc([rpt[0]])[0]
                         row.extend([k, i, j])
                     else:
                         k, j = grid.get_lni([rpt[0]])[0]
                         row.extend([(k, j)])
```

### Comparing `flopy-3.6.0/flopy/modpath/mp7particlegroup.py` & `flopy-3.7.0/flopy/modpath/mp7particlegroup.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/modpath/mp7sim.py` & `flopy-3.7.0/flopy/modpath/mp7sim.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mt3d/mt.py` & `flopy-3.7.0/flopy/mt3d/mt.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,27 +291,27 @@
         xoff = self._modelgrid.xoffset
         if xoff is None:
             if self._xul is not None:
                 xoff = self._modelgrid._xul_to_xll(self._xul)
             else:
                 xoff = self.mf._modelgrid.xoffset
             if xoff is None:
-                # incase mf._modelgrid.xoffset is not set but mf._xul is
+                # in case mf._modelgrid.xoffset is not set but mf._xul is
                 if self.mf._xul is not None:
                     xoff = self._modelgrid._xul_to_xll(self.mf._xul)
                 else:
                     xoff = 0.0
         yoff = self._modelgrid.yoffset
         if yoff is None:
             if self._yul is not None:
                 yoff = self._modelgrid._yul_to_yll(self._yul)
             else:
                 yoff = self.mf._modelgrid.yoffset
             if yoff is None:
-                # incase mf._modelgrid.yoffset is not set but mf._yul is
+                # in case mf._modelgrid.yoffset is not set but mf._yul is
                 if self.mf._yul is not None:
                     yoff = self._modelgrid._yul_to_yll(self.mf._yul)
                 else:
                     yoff = 0.0
         crs = self._modelgrid.crs
         if crs is None:
             crs = self.mf._modelgrid.crs
```

### Comparing `flopy-3.6.0/flopy/mt3d/mtadv.py` & `flopy-3.7.0/flopy/mt3d/mtadv.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mt3d/mtbtn.py` & `flopy-3.7.0/flopy/mt3d/mtbtn.py`

 * *Files 0% similar despite different names*

```diff
@@ -711,31 +711,31 @@
             )
         )
 
         # A4
         f_btn.write(f"{self.tunit:4s}{self.lunit:4s}{self.munit:4s}\n")
 
         # A5
-        if self.parent.adv != None:
+        if self.parent.adv is not None:
             f_btn.write("T ")
         else:
             f_btn.write("F ")
-        if self.parent.dsp != None:
+        if self.parent.dsp is not None:
             f_btn.write("T ")
         else:
             f_btn.write("F ")
-        if self.parent.ssm != None:
+        if self.parent.ssm is not None:
             f_btn.write("T ")
         else:
             f_btn.write("F ")
-        if self.parent.rct != None:
+        if self.parent.rct is not None:
             f_btn.write("T ")
         else:
             f_btn.write("F ")
-        if self.parent.gcg != None:
+        if self.parent.gcg is not None:
             f_btn.write("T ")
         else:
             f_btn.write("F ")
         f_btn.write("\n")
 
         # A6
         self.laycon.set_fmtin("(40I2)")
@@ -767,18 +767,15 @@
         # A14
         f_btn.write(f"{self.cinact:10.0E}{self.thkmin:10.2E}\n")
 
         # A15
         f_btn.write(
             f"{self.ifmtcn:10d}{self.ifmtnp:10d}{self.ifmtrf:10d}{self.ifmtdp:10d}"
         )
-        if self.savucn == True:
-            ss = "T"
-        else:
-            ss = "F"
+        ss = "T" if self.savucn else "F"
         f_btn.write(f"{ss:>10s}\n")
 
         # A16, A17
         if self.timprs is None:
             f_btn.write(f"{self.nprs:10d}\n")
         else:
             f_btn.write(f"{len(self.timprs):10d}\n")
@@ -805,15 +802,15 @@
                         self.obs[i, 0] + 1,
                         self.obs[i, 1] + 1,
                         self.obs[i, 2] + 1,
                     )
                 )
 
         # A20 CHKMAS, NPRMAS
-        if self.chkmas == True:
+        if self.chkmas:
             ss = "T"
         else:
             ss = "F"
         f_btn.write(f"{ss:>10s}{self.nprmas:10d}\n")
 
         # A21, 22, 23 PERLEN, NSTP, TSMULT
         for t in range(self.nper):
@@ -913,15 +910,15 @@
                 if m_arr[i].upper() == "NOWETDRYPRINT":
                     NoWetDryPrint = True
                 if m_arr[i].upper() == "OMITDRYCELLBUDGET":
                     OmitDryBud = True
                 if m_arr[i].upper() == "ALTWTSORB":
                     AltWTSorb = True
         elif model.verbose:
-            print("   optional keywords not identifed/loaded")
+            print("   optional keywords not identified/loaded")
 
         # A3
         if model.verbose:
             print("   loading NLAY, NROW, NCOL, NPER, NCOMP, MCOMP...")
         if m_arr[0].isdigit() is False:
             line = f.readline()
         nlay = int(line[0:10])
```

### Comparing `flopy-3.6.0/flopy/mt3d/mtcts.py` & `flopy-3.7.0/flopy/mt3d/mtcts.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mt3d/mtdsp.py` & `flopy-3.7.0/flopy/mt3d/mtdsp.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mt3d/mtgcg.py` & `flopy-3.7.0/flopy/mt3d/mtgcg.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mt3d/mtlkt.py` & `flopy-3.7.0/flopy/mt3d/mtlkt.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,15 +254,15 @@
         for s in range(len(self.coldlak)):
             f_lkt.write(self.coldlak[s].get_file_entry())
 
         # Items 3-4
         # (Loop through each stress period and write LKT information)
         nper = self.parent.nper
         for kper in range(nper):
-            if f_lkt.closed == True:
+            if f_lkt.closed:
                 f_lkt = open(f_lkt.name, "a")
 
             # List of concentrations associated with fluxes in/out of lake
             # (Evap, precip, specified runoff into the lake, specified
             # withdrawal directly from the lake
             if self.lk_stress_period_data is not None:
                 self.lk_stress_period_data.write_transient(
```

### Comparing `flopy-3.6.0/flopy/mt3d/mtphc.py` & `flopy-3.7.0/flopy/mt3d/mtphc.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mt3d/mtrct.py` & `flopy-3.7.0/flopy/mt3d/mtrct.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mt3d/mtsft.py` & `flopy-3.7.0/flopy/mt3d/mtsft.py`

 * *Files 0% similar despite different names*

```diff
@@ -427,15 +427,15 @@
                 )
                 f.write(line)
 
         # Items 7, 8
         # Loop through each stress period and assign source & sink concentrations to stream features
         nper = self.parent.nper
         for kper in range(nper):
-            if f.closed == True:
+            if f.closed:
                 f = open(f.name, "a")
 
             # List of concentrations associated with various boundaries
             # interacting with the stream network.
             if self.sf_stress_period_data is not None:
                 self.sf_stress_period_data.write_transient(f, single_per=kper)
             else:
```

### Comparing `flopy-3.6.0/flopy/mt3d/mtssm.py` & `flopy-3.7.0/flopy/mt3d/mtssm.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,17 +250,17 @@
                         )
                     self.mxss = max(self.mxss, mxss_kper)
 
             if isinstance(self.parent.btn.icbund, np.ndarray):
                 self.mxss += (self.parent.btn.icbund < 0).sum()
 
             for p in self.__SsmPackages:
-                if (p.label == "BAS6") and (p.instance != None):
+                if (p.label == "BAS6") and (p.instance is not None):
                     self.mxss += (p.instance.ibound.array < 0).sum()
-                elif p.instance != None:
+                elif p.instance is not None:
                     self.mxss += p.instance._ncells()
         else:
             self.mxss = mxss
 
         # Note: list is used for multi-species, NOT for stress periods!
         self.crch = None
         try:
@@ -450,15 +450,15 @@
         f_ssm.write(" F F F F F F F F F F\n")
 
         f_ssm.write(f"{self.mxss:10d}\n")
 
         # Loop through each stress period and write ssm information
         nper = self.parent.nper
         for kper in range(nper):
-            if f_ssm.closed == True:
+            if f_ssm.closed:
                 f_ssm = open(f_ssm.name, "a")
 
             # Distributed sources and sinks (Recharge and Evapotranspiration)
             if self.crch is not None:
                 # If any species need to be written, then all need to be
                 # written
                 incrch = -1
@@ -490,15 +490,15 @@
                         file_entry = u2d.get_file_entry()
                         f_ssm.write(file_entry)
 
             # List of sources
             if self.stress_period_data is not None:
                 self.stress_period_data.write_transient(f_ssm, single_per=kper)
             else:
-                f_ssm.write(f"0\n")
+                f_ssm.write("0\n")
 
         f_ssm.close()
         return
 
     @classmethod
     def load(
         cls,
```

### Comparing `flopy-3.6.0/flopy/mt3d/mttob.py` & `flopy-3.7.0/flopy/mt3d/mttob.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/mt3d/mtuzt.py` & `flopy-3.7.0/flopy/mt3d/mtuzt.py`

 * *Files 0% similar despite different names*

```diff
@@ -335,15 +335,15 @@
         # Item 3
         f_uzt.write(self.iuzfbnd.get_file_entry())
 
         # Items 4-9
         # (Loop through each stress period and write uzt information)
         nper = self.parent.nper
         for kper in range(nper):
-            if f_uzt.closed == True:
+            if f_uzt.closed:
                 f_uzt = open(f_uzt.name, "a")
 
             # Concentrations associated with distributed stresses (Infil, ET)
             if self.cuzinf is not None:
                 # If any species needs to be written, then all need to be
                 # written
                 incuzinf = -1
```

### Comparing `flopy-3.6.0/flopy/pakbase.py` & `flopy-3.7.0/flopy/pakbase.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,24 +206,24 @@
         }
         kparams = {}
         vka_param = None
         for kp, name in kparams_all.items():
             if kp in self.__dict__:
                 kparams[kp] = name
         if "hk" in self.__dict__:
-            if self.hk.shape[1] == None:
+            if self.hk.shape[1] is None:
                 hk = np.asarray(
                     [a.array.flatten() for a in self.hk], dtype=object
                 )
             else:
                 hk = self.hk.array.copy()
         else:
             hk = self.k.array.copy()
         if "vka" in self.__dict__ and self.layvka.sum() > 0:
-            if self.vka.shape[1] == None:
+            if self.vka.shape[1] is None:
                 vka = np.asarray(
                     [a.array.flatten() for a in self.vka], dtype=object
                 )
             else:
                 vka = self.vka.array
             vka_param = kparams.pop("vka")
         elif "k33" in self.__dict__:
@@ -292,15 +292,15 @@
         """
         Check package data for common errors.
 
         Parameters
         ----------
         f : str or file handle
             String defining file name or file handle for summary file
-            of check method output. If a sting is passed a file handle
+            of check method output. If a string is passed a file handle
             is created. If f is None, check method does not write
             results to a summary file. (default is None)
         verbose : bool
             Boolean flag used to determine if check method results are
             written to the screen
         level : int
             Check method analysis level. If level=0, summary checks are
@@ -505,15 +505,15 @@
 
         return
 
     def __repr__(self):
         s = self.__doc__
         exclude_attributes = ["extension", "heading", "name", "parent", "url"]
         for attr, value in sorted(self.__dict__.items()):
-            if not (attr in exclude_attributes):
+            if attr not in exclude_attributes:
                 if isinstance(value, list):
                     if len(value) == 1:
                         s += f" {attr} = {value[0]!s}\n"
                     else:
                         s += f" {attr} (list, items = {len(value)})\n"
                 elif isinstance(value, np.ndarray):
                     s += f" {attr} (array, shape = {str(value.shape)[1:-1]})\n"
@@ -738,15 +738,15 @@
         for field_name, field_type in zip(field_names, field_types):
             newdtypes.append((str(field_name), field_type))
         return np.dtype(newdtypes)
 
     @staticmethod
     def _get_sfac_columns():
         """
-        This should be overriden for individual packages that support an
+        This should be overridden for individual packages that support an
         sfac multiplier for individual list columns
 
         """
         return []
 
     def _confined_layer_check(self, chk):
         # check for confined layers above convertible layers
@@ -998,23 +998,23 @@
                     if toption.lower() == "autoflowreduce":
                         options.append(toption.lower())
                     elif toption.lower() == "iunitafr":
                         options.append(f"{toption.lower()} {t[it+1]}")
                         it += 1
                 it += 1
 
-        # add auxillary information to nwt options
+        # add auxiliary information to nwt options
         if nwt_options is not None:
             if options:
                 if options[0] == "noprint":
                     nwt_options.noprint = True
                     if len(options) > 1:
-                        nwt_options.auxillary = options[1:]
+                        nwt_options.auxiliary = options[1:]
                 else:
-                    nwt_options.auxillary = options
+                    nwt_options.auxiliary = options
 
             options = nwt_options
 
         # set partype
         #  and read phiramp for modflow-nwt well package
         partype = ["cond"]
         if "modflowwel" in pak_type_str:
@@ -1030,17 +1030,17 @@
                     nwt_options = OptionBlock(
                         line.lower().strip(), pak_type, block=False
                     )
                     if options:
                         if options[0] == "noprint":
                             nwt_options.noprint = True
                             if len(options) > 1:
-                                nwt_options.auxillary = options[1:]
+                                nwt_options.auxiliary = options[1:]
                         else:
-                            nwt_options.auxillary = options
+                            nwt_options.auxiliary = options
 
                     options = nwt_options
                 else:
                     f.seek(ipos)
         elif "flopy.modflow.mfchd.modflowchd".lower() in pak_type_str:
             partype = ["shead", "ehead"]
```

### Comparing `flopy-3.6.0/flopy/pest/params.py` & `flopy-3.7.0/flopy/pest/params.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/pest/templatewriter.py` & `flopy-3.7.0/flopy/pest/templatewriter.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,13 +83,13 @@
                 tpla.add_parameter(p)
 
             # Write the file
             paktpl.heading = "ptf ~\n" + paktpl.heading
             paktpl.fn_path += ".tpl"
             paktpl.write_file(
                 check=False
-            )  # fot now, turn off checks for template files
+            )  # for now, turn off checks for template files
 
             # Destroy the template version of the package
             paktpl = None
 
         return
```

### Comparing `flopy-3.6.0/flopy/pest/tplarray.py` & `flopy-3.7.0/flopy/pest/tplarray.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/plot/crosssection.py` & `flopy-3.7.0/flopy/plot/crosssection.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,15 +137,15 @@
                     (xcenter[int(line[onkey])], yedge[0] + eps),
                     (xcenter[int(line[onkey])], yedge[-1] - eps),
                 ]
         else:
             ln = line[onkey]
 
             if not PlotCrossSection._is_valid(ln):
-                raise ValueError(f"Invalid line representation")
+                raise ValueError("Invalid line representation")
 
             gu = GeoSpatialUtil(ln, shapetype="linestring")
             verts = gu.points
             xp = []
             yp = []
             for [v1, v2] in verts:
                 xp.append(v1)
@@ -261,16 +261,15 @@
 
         if model is None:
             self._masked_values = [1e30, -1e30]
         else:
             self._masked_values = [model.hnoflo, model.hdry]
 
         # Set axis limits
-        self.ax.set_xlim(self.extent[0], self.extent[1])
-        self.ax.set_ylim(self.extent[2], self.extent[3])
+        self._set_axes_limits(self.ax)
 
     @staticmethod
     def _is_valid(line):
         shapely_geo = import_optional_dependency("shapely.geometry")
 
         if isinstance(
             line,
@@ -353,14 +352,33 @@
         xmax = np.max(xpts)
 
         ymin = np.min(self.elev)
         ymax = np.max(self.elev)
 
         return xmin, xmax, ymin, ymax
 
+    def _set_axes_limits(self, ax):
+        """
+        Internal method to set axes limits
+
+        Parameters
+        ----------
+        ax : matplotlib.pyplot axis
+            The plot axis
+
+        Returns
+        -------
+        ax : matplotlib.pyplot axis object
+
+        """
+        if ax.get_autoscale_on():
+            ax.set_xlim(self.extent[0], self.extent[1])
+            ax.set_ylim(self.extent[2], self.extent[3])
+        return ax
+
     def plot_array(self, a, masked_values=None, head=None, **kwargs):
         """
         Plot a three-dimensional array as a patch collection.
 
         Parameters
         ----------
         a : numpy.ndarray
@@ -398,16 +416,15 @@
             projpts = self.set_zpts(np.ravel(head))
         else:
             projpts = None
 
         pc = self.get_grid_patch_collection(a, projpts, **kwargs)
         if pc is not None:
             ax.add_collection(pc)
-            ax.set_xlim(self.extent[0], self.extent[1])
-            ax.set_ylim(self.extent[2], self.extent[3])
+            ax = self._set_axes_limits(ax)
 
         return pc
 
     def plot_surface(self, a, masked_values=None, **kwargs):
         """
         Plot a two- or three-dimensional array as line(s).
 
@@ -460,16 +477,15 @@
                 continue
             else:
                 line = ax.plot(
                     d[cell], [a[cell], a[cell]], color=color, **kwargs
                 )
                 surface.append(line)
 
-        ax.set_xlim(self.extent[0], self.extent[1])
-        ax.set_ylim(self.extent[2], self.extent[3])
+        ax = self._set_axes_limits(ax)
 
         return surface
 
     def plot_fill_between(
         self,
         a,
         colors=("blue", "red"),
@@ -519,16 +535,15 @@
             projpts = self.projpts
 
         pc = self.get_grid_patch_collection(
             a, projpts, fill_between=True, **kwargs
         )
         if pc is not None:
             ax.add_collection(pc)
-            ax.set_xlim(self.extent[0], self.extent[1])
-            ax.set_ylim(self.extent[2], self.extent[3])
+            ax = self._set_axes_limits(ax)
 
         return pc
 
     def contour_array(self, a, masked_values=None, head=None, **kwargs):
         """
         Contour a two-dimensional array.
 
@@ -655,16 +670,15 @@
                 contour_set = ax.tricontourf(triang, plotarray, **kwargs)
             else:
                 contour_set = ax.tricontour(triang, plotarray, **kwargs)
 
             if plot_triplot:
                 ax.triplot(triang, color="black", marker="o", lw=0.75)
 
-        ax.set_xlim(self.extent[0], self.extent[1])
-        ax.set_ylim(self.extent[2], self.extent[3])
+        ax = self._set_axes_limits(ax)
 
         return contour_set
 
     def plot_inactive(self, ibound=None, color_noflow="black", **kwargs):
         """
         Make a plot of inactive cells.  If not specified, then pull ibound
         from the self.ml
@@ -1545,15 +1559,15 @@
         ----------
         plotarray : numpy.ndarray
             One-dimensional array to attach to the Patch Collection.
         projpts : dict
             dictionary defined by node number which contains model
             patch vertices.
         fill_between : bool
-            flag to create polygons that mimick the matplotlib fill between
+            flag to create polygons that mimic the matplotlib fill between
             method. Only used by the plot_fill_between method.
         **kwargs : dictionary
             keyword arguments passed to matplotlib.collections.PatchCollection
 
         Returns
         -------
         patches : matplotlib.collections.PatchCollection
```

### Comparing `flopy-3.6.0/flopy/plot/map.py` & `flopy-3.7.0/flopy/plot/map.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,14 +78,33 @@
 
     @property
     def extent(self):
         if self._extent is None:
             self._extent = self.mg.extent
         return self._extent
 
+    def _set_axes_limits(self, ax):
+        """
+        Internal method to set axes limits
+
+        Parameters
+        ----------
+        ax : matplotlib.pyplot axis
+            The plot axis
+
+        Returns
+        -------
+        ax : matplotlib.pyplot axis object
+
+        """
+        if ax.get_autoscale_on():
+            ax.set_xlim(self.extent[0], self.extent[1])
+            ax.set_ylim(self.extent[2], self.extent[3])
+        return ax
+
     def plot_array(self, a, masked_values=None, **kwargs):
         """
         Plot an array.  If the array is three-dimensional, then the method
         will plot the layer tied to this class (self.layer).
 
         Parameters
         ----------
@@ -148,16 +167,15 @@
 
         # set matplotlib kwargs
         collection.set_clim(vmin=vmin, vmax=vmax)
         collection.set(**kwargs)
         ax.add_collection(collection)
 
         # set limits
-        ax.set_xlim(self.extent[0], self.extent[1])
-        ax.set_ylim(self.extent[2], self.extent[3])
+        ax = self._set_axes_limits(ax)
         return collection
 
     def contour_array(self, a, masked_values=None, tri_mask=False, **kwargs):
         """
         Contour an array on the grid. By default the top layer
         is contoured. To select a different layer, specify the
         layer in the class constructor.
@@ -301,16 +319,15 @@
                 if filled
                 else ax.tricontour(triang, plotarray.flatten(), **kwargs)
             )
 
             if plot_triplot:
                 ax.triplot(triang, color="black", marker="o", lw=0.75)
 
-        ax.set_xlim(self.extent[0], self.extent[1])
-        ax.set_ylim(self.extent[2], self.extent[3])
+        ax = self._set_axes_limits(ax)
 
         return contour_set
 
     def plot_inactive(self, ibound=None, color_noflow="black", **kwargs):
         """
         Make a plot of inactive cells.  If not specified, then pull ibound
         from the self.ml
@@ -419,16 +436,15 @@
         grid_lines = self.mg.grid_lines
         if isinstance(grid_lines, dict):
             grid_lines = grid_lines[self.layer]
 
         collection = LineCollection(grid_lines, colors=colors, **kwargs)
 
         ax.add_collection(collection)
-        ax.set_xlim(self.extent[0], self.extent[1])
-        ax.set_ylim(self.extent[2], self.extent[3])
+        ax = self._set_axes_limits(ax)
         return collection
 
     def plot_bc(
         self,
         name=None,
         package=None,
         kper=0,
@@ -601,14 +617,15 @@
 
         Returns
         -------
             matplotlib.Collection object
         """
         ax = kwargs.pop("ax", self.ax)
         patch_collection = plotutil.plot_shapefile(obj, ax, **kwargs)
+        ax = self._set_axes_limits(ax)
         return patch_collection
 
     def plot_vector(
         self,
         vx,
         vy,
         istep=1,
@@ -697,14 +714,15 @@
         u[ib == 0] = np.nan
         v[ib == 0] = np.nan
 
         # rotate and plot, offsets must be zero since
         # these are vectors not locations
         urot, vrot = geometry.rotate(u, v, 0.0, 0.0, self.mg.angrot_radians)
         quiver = ax.quiver(x, y, urot, vrot, pivot=pivot, **kwargs)
+        ax = self._set_axes_limits(ax)
         return quiver
 
     def plot_pathline(self, pl, travel_time=None, **kwargs):
         """
         Plot particle pathlines. Compatible with MODFLOW 6 PRT particle track
         data format, or MODPATH 6 or 7 pathline data format.
 
@@ -841,17 +859,15 @@
                     lw=0,
                     marker=marker,
                     color=markercolor,
                     ms=markersize,
                 )
 
         # set axis limits
-        ax.set_xlim(self.extent[0], self.extent[1])
-        ax.set_ylim(self.extent[2], self.extent[3])
-
+        ax = self._set_axes_limits(ax)
         return lc
 
     def plot_timeseries(self, ts, travel_time=None, **kwargs):
         """
         Plot MODPATH 6 or 7 timeseries. Incompatible with MODFLOW 6 PRT.
 
         Parameters
@@ -985,8 +1001,10 @@
             c = tep["time"] - tep["time0"]
             sp = ax.scatter(arr[:, 0], arr[:, 1], c=c, s=s, **kwargs)
 
         # add a colorbar for travel times
         if createcb:
             cb = plt.colorbar(sp, ax=ax, shrink=shrink)
             cb.set_label(colorbar_label)
+
+        ax = self._set_axes_limits(ax)
         return sp
```

### Comparing `flopy-3.6.0/flopy/plot/mplstyle/usgsmap.mplstyle` & `flopy-3.7.0/flopy/plot/mplstyle/usgsplot.mplstyle`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 font.family: sans-serif
-font.sans-serif: Arial
+font.sans-serif: Arial, Liberation Sans, DejaVu Sans
 font.size: 7
 axes.labelsize: 9
 axes.titlesize: 9
 axes.linewidth: 0.5
-xtick.labelsize: 7
+xtick.labelsize: 8
 xtick.top: True
 xtick.bottom: True
 xtick.major.size: 7.2
 xtick.minor.size: 3.6
 xtick.major.width: 0.5
 xtick.minor.width: 0.5
 xtick.direction: in
-ytick.labelsize: 7
+ytick.labelsize: 8
 ytick.left: True
 ytick.right: True
 ytick.major.size: 7.2
 ytick.minor.size: 3.6
 ytick.major.width: 0.5
 ytick.minor.width: 0.5
 ytick.direction: in
```

### Comparing `flopy-3.6.0/flopy/plot/mplstyle/usgsmap_linux.mplstyle` & `flopy-3.7.0/flopy/plot/mplstyle/usgsmap.mplstyle`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 font.family: sans-serif
-font.sans-serif: Liberation Sans
+font.sans-serif: Arial, Liberation Sans, DejaVu Sans
 font.size: 7
 axes.labelsize: 9
 axes.titlesize: 9
 axes.linewidth: 0.5
 xtick.labelsize: 7
 xtick.top: True
 xtick.bottom: True
```

### Comparing `flopy-3.6.0/flopy/plot/plotutil.py` & `flopy-3.7.0/flopy/plot/plotutil.py`

 * *Files 1% similar despite different names*

```diff
@@ -1322,15 +1322,15 @@
             plt.close("all")
 
         return axes
 
     @staticmethod
     def _set_layer_range(mflay, maxlay):
         """
-        Re-usable method to check for mflay and set
+        Reusable method to check for mflay and set
         the range of plottable layers
 
         Parameters
         ----------
         mflay : int
             zero based layer number
         maxlay : int
@@ -1568,15 +1568,15 @@
     plotting helper functions
     """
 
     @staticmethod
     def line_intersect_grid(ptsin, xgrid, ygrid):
         """
         Uses cross product method to find which cells intersect with the
-        line and then uses the parameterized line equation to caluculate
+        line and then uses the parameterized line equation to calculate
         intersection x, y vertex points. Should be quite fast for large model
         grids!
 
         Parameters
         ----------
         pts : list
             list of tuple line vertex pairs (ex. [(1, 0), (10, 0)]
@@ -2596,107 +2596,155 @@
             )
     else:
         tep = ep.copy()
 
     return tep, istart, xp, yp
 
 
-# define minimum expected fields
-_mp7_pathline_fields = ["x", "y", "z", "time", "k", "particleid"]
-_prt_pathline_fields = [
-    "x",
-    "y",
-    "z",
-    "t",
-    "trelease",
-    "imdl",
-    "iprp",
-    "irpt",
-    "ilay",
-]
+PRT_PATHLINE_DTYPE = np.dtype(
+    [
+        ("kper", np.int32),
+        ("kstp", np.int32),
+        ("imdl", np.int32),
+        ("iprp", np.int32),
+        ("irpt", np.int32),
+        ("ilay", np.int32),
+        ("icell", np.int32),
+        ("izone", np.int32),
+        ("istatus", np.int32),
+        ("ireason", np.int32),
+        ("trelease", np.float32),
+        ("t", np.float32),
+        ("x", np.float32),
+        ("y", np.float32),
+        ("z", np.float32),
+        ("name", np.str_),
+    ]
+)
+MP7_PATHLINE_DTYPE = np.dtype(
+    [
+        ("particleid", np.int32),  # same as sequencenumber
+        ("particlegroup", np.int32),
+        (
+            "sequencenumber",
+            np.int32,
+        ),  # mp7 sequencenumber (globally unique auto-generated ID)
+        (
+            "particleidloc",
+            np.int32,
+        ),  # mp7 particle ID (unique within a group, user-assigned or autogenerated)
+        ("time", np.float32),
+        ("x", np.float32),
+        ("y", np.float32),
+        ("z", np.float32),
+        ("k", np.int32),
+        ("node", np.int32),
+        ("xloc", np.float32),
+        ("yloc", np.float32),
+        ("zloc", np.float32),
+        ("stressperiod", np.int32),
+        ("timestep", np.int32),
+    ]
+)
+MP7_ENDPOINT_DTYPE = np.dtype(
+    [
+        (
+            "particleid",
+            np.int32,
+        ),  # mp7 sequencenumber (globally unique auto-generated ID)
+        ("particlegroup", np.int32),
+        (
+            "particleidloc",
+            np.int32,
+        ),  # mp7 particle ID (unique within a group, user-assigned or autogenerated)
+        ("status", np.int32),
+        ("time0", np.float32),
+        ("time", np.float32),
+        ("node0", np.int32),
+        ("k0", np.int32),
+        ("xloc0", np.float32),
+        ("yloc0", np.float32),
+        ("zloc0", np.float32),
+        ("x0", np.float32),
+        ("y0", np.float32),
+        ("z0", np.float32),
+        ("zone0", np.int32),
+        ("initialcellface", np.int32),
+        ("node", np.int32),
+        ("k", np.int32),
+        ("xloc", np.float32),
+        ("yloc", np.float32),
+        ("zloc", np.float32),
+        ("x", np.float32),
+        ("y", np.float32),
+        ("z", np.float32),
+        ("zone", np.int32),
+        ("cellface", np.int32),
+    ]
+)
 
 
 def to_mp7_pathlines(
-    data: Union[np.recarray, pd.DataFrame]
+    data: Union[np.recarray, pd.DataFrame],
 ) -> Union[np.recarray, pd.DataFrame]:
     """
     Convert MODFLOW 6 PRT pathline data to MODPATH 7 pathline format.
 
     Parameters
     ----------
     data : np.recarray or pd.DataFrame
         MODFLOW 6 PRT pathline data
 
     Returns
     -------
     np.recarray or pd.DataFrame (consistent with input type)
     """
 
+    from flopy.utils.particletrackfile import MIN_PARTICLE_TRACK_DTYPE
+
     # determine return type
     ret_type = type(data)
 
     # convert to dataframe if needed
     if not isinstance(data, pd.DataFrame):
         data = pd.DataFrame(data)
 
     # check format
     dt = data.dtypes
     if not (
-        all(n in dt for n in _mp7_pathline_fields)
-        or all(n in dt for n in _prt_pathline_fields)
+        all(n in dt for n in MIN_PARTICLE_TRACK_DTYPE.names)
+        or all(n in dt for n in PRT_PATHLINE_DTYPE.names)
     ):
         raise ValueError(
-            "Pathline data must contain all of the following columns: "
-            f"{_mp7_pathline_fields} for MODPATH 7, or "
-            f"{_prt_pathline_fields} for MODFLOW 6 PRT"
+            "Pathline data must contain the following fields: "
+            f"{MIN_PARTICLE_TRACK_DTYPE.names} for MODPATH 7, or "
+            f"{PRT_PATHLINE_DTYPE.names} for MODFLOW 6 PRT"
         )
 
     # return early if already in MP7 format
     if "t" not in dt:
         return (
             data if ret_type == pd.DataFrame else data.to_records(index=False)
         )
 
+    # return early if empty
+    if data.empty:
+        ret = np.recarray((0,), dtype=MP7_PATHLINE_DTYPE)
+        return pd.DataFrame(ret) if ret_type == pd.DataFrame else ret
+
     # assign a unique particle index column incrementing an integer
     # for each unique combination of irpt, iprp, imdl, and trelease
     data = data.sort_values(["imdl", "iprp", "irpt", "trelease"])
     particles = data.groupby(["imdl", "iprp", "irpt", "trelease"])
     seqn_key = "sequencenumber"
     data[seqn_key] = particles.ngroup()
 
     # convert to recarray
     data = data.to_records(index=False)
 
-    # define mp7 dtype
-    mp7_dtypes = np.dtype(
-        [
-            ("particleid", np.int32),  # same as sequencenumber
-            ("particlegroup", np.int32),
-            (
-                seqn_key,
-                np.int32,
-            ),  # mp7 sequencenumber (globally unique auto-generated ID)
-            (
-                "particleidloc",
-                np.int32,
-            ),  # mp7 particle ID (unique within a group, user-assigned or autogenerated)
-            ("time", np.float32),
-            ("x", np.float32),
-            ("y", np.float32),
-            ("z", np.float32),
-            ("k", np.int32),
-            ("node", np.int32),
-            ("xloc", np.float32),
-            ("yloc", np.float32),
-            ("zloc", np.float32),
-            ("stressperiod", np.int32),
-            ("timestep", np.int32),
-        ]
-    )
-
     # build mp7 format recarray
     ret = np.core.records.fromarrays(
         [
             data[seqn_key],
             data["iprp"],
             data[seqn_key],
             data["irpt"],
@@ -2709,43 +2757,66 @@
             # todo local coords (xloc, yloc, zloc)
             np.zeros(data.shape[0]),
             np.zeros(data.shape[0]),
             np.zeros(data.shape[0]),
             data["kper"],
             data["kstp"],
         ],
-        dtype=mp7_dtypes,
+        dtype=MP7_PATHLINE_DTYPE,
     )
 
     return pd.DataFrame(ret) if ret_type == pd.DataFrame else ret
 
 
 def to_mp7_endpoints(
-    data: Union[np.recarray, pd.DataFrame]
+    data: Union[np.recarray, pd.DataFrame],
 ) -> Union[np.recarray, pd.DataFrame]:
     """
     Convert MODFLOW 6 PRT pathline data to MODPATH 7 endpoint format.
 
     Parameters
     ----------
     data : np.recarray or pd.DataFrame
         MODFLOW 6 PRT pathline data
 
     Returns
     -------
     np.recarray or pd.DataFrame (consistent with input type)
     """
 
+    from flopy.utils.particletrackfile import MIN_PARTICLE_TRACK_DTYPE
+
     # determine return type
     ret_type = type(data)
 
     # convert to dataframe if needed
     if isinstance(data, np.recarray):
         data = pd.DataFrame(data)
 
+    # check format
+    dt = data.dtypes
+    if all(n in dt for n in MP7_ENDPOINT_DTYPE.names):
+        return (
+            data if ret_type == pd.DataFrame else data.to_records(index=False)
+        )
+    if not (
+        all(n in dt for n in MIN_PARTICLE_TRACK_DTYPE.names)
+        or all(n in dt for n in PRT_PATHLINE_DTYPE.names)
+    ):
+        raise ValueError(
+            "Pathline data must contain the following fields: "
+            f"{MIN_PARTICLE_TRACK_DTYPE.names} for MODPATH 7, or "
+            f"{PRT_PATHLINE_DTYPE.names} for MODFLOW 6 PRT"
+        )
+
+    # return early if empty
+    if data.empty:
+        ret = np.recarray((0,), dtype=MP7_ENDPOINT_DTYPE)
+        return pd.DataFrame(ret) if ret_type == pd.DataFrame else ret
+
     # assign a unique particle index column incrementing an integer
     # for each unique combination of irpt, iprp, imdl, and trelease
     data = data.sort_values(["imdl", "iprp", "irpt", "trelease"])
     particles = data.groupby(["imdl", "iprp", "irpt", "trelease"])
     seqn_key = "sequencenumber"
     data[seqn_key] = particles.ngroup()
 
@@ -2775,52 +2846,14 @@
     ]
     for fl, fr in pairings:
         endpts[fl] = np.select(conditions, startpts[fr].to_numpy())
 
     # convert to recarray
     endpts = endpts.to_records(index=False)
 
-    # define mp7 dtype
-    mp7_dtype = np.dtype(
-        [
-            (
-                "particleid",
-                np.int32,
-            ),  # mp7 sequencenumber (globally unique auto-generated ID)
-            ("particlegroup", np.int32),
-            (
-                "particleidloc",
-                np.int32,
-            ),  # mp7 particle ID (unique within a group, user-assigned or autogenerated)
-            ("status", np.int32),
-            ("time0", np.float32),
-            ("time", np.float32),
-            ("node0", np.int32),
-            ("k0", np.int32),
-            ("xloc0", np.float32),
-            ("yloc0", np.float32),
-            ("zloc0", np.float32),
-            ("x0", np.float32),
-            ("y0", np.float32),
-            ("z0", np.float32),
-            ("zone0", np.int32),
-            ("initialcellface", np.int32),
-            ("node", np.int32),
-            ("k", np.int32),
-            ("xloc", np.float32),
-            ("yloc", np.float32),
-            ("zloc", np.float32),
-            ("x", np.float32),
-            ("y", np.float32),
-            ("z", np.float32),
-            ("zone", np.int32),
-            ("cellface", np.int32),
-        ]
-    )
-
     # build mp7 format recarray
     ret = np.core.records.fromarrays(
         [
             endpts["sequencenumber"],
             endpts["iprp"],
             endpts["irpt"],
             endpts["istatus"],
@@ -2845,22 +2878,22 @@
             np.zeros(endpts.shape[0]),
             endpts["x"],
             endpts["y"],
             endpts["z"],
             endpts["izone"],
             np.zeros(endpts.shape[0]),  # todo cell face?
         ],
-        dtype=mp7_dtype,
+        dtype=MP7_ENDPOINT_DTYPE,
     )
 
     return pd.DataFrame(ret) if ret_type == pd.DataFrame else ret
 
 
 def to_prt_pathlines(
-    data: Union[np.recarray, pd.DataFrame]
+    data: Union[np.recarray, pd.DataFrame],
 ) -> Union[np.recarray, pd.DataFrame]:
     """
     Convert MODPATH 7 pathline or endpoint data to MODFLOW 6 PRT pathline format.
 
     Parameters
     ----------
     data : np.recarray or pd.DataFrame
@@ -2877,54 +2910,37 @@
     # convert to dataframe if needed
     if isinstance(data, np.recarray):
         data = pd.DataFrame(data)
 
     # check format
     dt = data.dtypes
     if not (
-        all(n in dt for n in _mp7_pathline_fields)
-        or all(n in dt for n in _prt_pathline_fields)
+        all(n in dt for n in MP7_PATHLINE_DTYPE.names)
+        or all(n in dt for n in PRT_PATHLINE_DTYPE.names)
     ):
         raise ValueError(
-            "Pathline data must contain all of the following columns: "
-            f"{_mp7_pathline_fields} for MODPATH 7, or "
-            f"{_prt_pathline_fields} for MODFLOW 6 PRT"
+            "Pathline data must contain the following fields: "
+            f"{MP7_PATHLINE_DTYPE.names} for MODPATH 7, or "
+            f"{PRT_PATHLINE_DTYPE.names} for MODFLOW 6 PRT"
         )
 
     # return early if already in PRT format
     if "t" in dt:
         return (
             data if ret_type == pd.DataFrame else data.to_records(index=False)
         )
 
+    # return early if empty
+    if data.empty:
+        ret = np.recarray((0,), dtype=PRT_PATHLINE_DTYPE)
+        return pd.DataFrame(ret) if ret_type == pd.DataFrame else ret
+
     # convert to recarray
     data = data.to_records(index=False)
 
-    # define prt dtype
-    prt_dtypes = np.dtype(
-        [
-            ("kper", np.int32),
-            ("kstp", np.int32),
-            ("imdl", np.int32),
-            ("iprp", np.int32),
-            ("irpt", np.int32),
-            ("ilay", np.int32),
-            ("icell", np.int32),
-            ("izone", np.int32),
-            ("istatus", np.int32),
-            ("ireason", np.int32),
-            ("trelease", np.float32),
-            ("t", np.float32),
-            ("x", np.float32),
-            ("y", np.float32),
-            ("z", np.float32),
-            ("name", str),
-        ]
-    )
-
     # build prt format recarray
     ret = np.core.records.fromarrays(
         [
             data["stressperiod"],
             data["timestep"],
             np.zeros(data.shape[0]),
             data["particlegroup"],
@@ -2935,13 +2951,18 @@
             np.zeros(data.shape[0]),  # todo istatus?
             np.zeros(data.shape[0]),  # todo ireason?
             np.zeros(data.shape[0]),  # todo trelease?
             data["time"],
             data["x"],
             data["y"],
             data["z"],
-            np.zeros(data.shape[0]),
+            np.zeros(data.shape[0], str),
         ],
-        dtype=prt_dtypes,
+        dtype=PRT_PATHLINE_DTYPE,
     )
 
-    return pd.DataFrame(ret) if ret_type == pd.DataFrame else ret
+    if ret_type == pd.DataFrame:
+        df = pd.DataFrame(ret)
+        df.name = df.name.astype(pd.StringDtype())
+        return df
+    else:
+        return ret
```

### Comparing `flopy-3.6.0/flopy/plot/styles.py` & `flopy-3.7.0/flopy/plot/styles.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,14 @@
     accessed using the plt.style.context() method.
 
     """
 
     _ws = os.path.abspath(os.path.dirname(__file__))
     _map_style = os.path.join(_ws, "mplstyle", "usgsmap.mplstyle")
     _plot_style = os.path.join(_ws, "mplstyle", "usgsplot.mplstyle")
-    if platform.system() == "linux":
-        _map_style = os.path.join(_ws, "mplstyle", "usgsmap_linux.mplstyle")
-        _plot_style = os.path.join(_ws, "mplstyle", "usgsplot_linux.mplstyle")
 
     @classmethod
     def USGSMap(cls):
         return plt.style.context(styles._map_style)
 
     @classmethod
     def USGSPlot(cls):
@@ -78,15 +75,15 @@
         x : float
             location of the heading in the x-direction in normalized plot
             dimensions ranging from 0 to 1 (default is 0.00)
         y : float
             location of the heading in the y-direction in normalized plot
             dimensions ranging from 0 to 1 (default is 1.01)
         idx : int
-            index for programatically generating the heading letter when letter
+            index for programmatically generating the heading letter when letter
             is None and idx is not None. idx = 0 will generate A
             (default is None)
 
         Returns
         -------
         text : object
             matplotlib text object
```

### Comparing `flopy-3.6.0/flopy/seawat/swt.py` & `flopy-3.7.0/flopy/seawat/swt.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/seawat/swtvdf.py` & `flopy-3.7.0/flopy/seawat/swtvdf.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/seawat/swtvsc.py` & `flopy-3.7.0/flopy/seawat/swtvsc.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/utils/binaryfile.py` & `flopy-3.7.0/flopy/utils/binaryfile.py`

 * *Files 3% similar despite different names*

```diff
@@ -1009,15 +1009,16 @@
         self.times = []
         self.kstpkper = []
         self.recordarray = []
         self.iposheader = []
         self.iposarray = []
         self.textlist = []
         self.imethlist = []
-        self.paknamlist = []
+        self.paknamlist_from = []
+        self.paknamlist_to = []
         self.nrecords = 0
         self.compact = True  # compact budget file flag
 
         self.dis = None
         self.modelgrid = None
         if "model" in kwargs.keys():
             self.model = kwargs.pop("model")
@@ -1075,20 +1076,21 @@
         self.times = []
         self.kstpkper = []
         self.recordarray = []
         self.iposheader = []
         self.iposarray = []
         self.textlist = []
         self.imethlist = []
-        self.paknamlist = []
+        self.paknamlist_from = []
+        self.paknamlist_to = []
         self.nrecords = 0
 
     def _set_precision(self, precision="single"):
         """
-        Method to set the budget precsion from a CBC file. Enables
+        Method to set the budget precision from a CBC file. Enables
         Auto precision code to work
 
         Parameters
         ----------
         precision : str
             budget file precision (accepts 'single' or 'double')
         """
@@ -1215,16 +1217,18 @@
                             if t.upper() not in asciiset:
                                 raise Exception()
 
                 except:
                     raise BudgetIndexError("Improper precision")
                 self.textlist.append(header["text"])
                 self.imethlist.append(header["imeth"])
-            if header["paknam"] not in self.paknamlist:
-                self.paknamlist.append(header["paknam"])
+            if header["paknam"] not in self.paknamlist_from:
+                self.paknamlist_from.append(header["paknam"])
+            if header["paknam2"] not in self.paknamlist_to:
+                self.paknamlist_to.append(header["paknam2"])
             ipos = self.file.tell()
 
             if self.verbose:
                 for itxt in [
                     "kstp",
                     "kper",
                     "text",
@@ -1386,27 +1390,27 @@
                     text16 = t
                     break
             if text16 is None:
                 errmsg = "The specified text string is not in the budget file."
                 raise Exception(errmsg)
         return text16
 
-    def _find_paknam(self, paknam):
+    def _find_paknam(self, paknam, to=False):
         """
         Determine if selected record name is in budget file
 
         """
         # check and make sure that text is in file
         paknam16 = None
         if paknam is not None:
             if isinstance(paknam, bytes):
                 tpaknam = paknam.decode()
             else:
                 tpaknam = paknam
-            for t in self._unique_package_names():
+            for t in self._unique_package_names(to):
                 if tpaknam.upper() in t.decode():
                     paknam16 = t
                     break
             if paknam16 is None:
                 raise Exception(
                     "The specified package name string is not "
                     "in the budget file."
@@ -1429,19 +1433,19 @@
         print("RECORD           IMETH")
         print(22 * "-")
         for rec, imeth in zip(self.textlist, self.imethlist):
             if isinstance(rec, bytes):
                 rec = rec.decode()
             print(f"{rec.strip():16} {imeth:5d}")
 
-    def list_unique_packages(self):
+    def list_unique_packages(self, to=False):
         """
         Print a list of unique package names
         """
-        for rec in self._unique_package_names():
+        for rec in self._unique_package_names(to):
             if isinstance(rec, bytes):
                 rec = rec.decode()
             print(rec)
 
     def get_unique_record_names(self, decode=False):
         """
         Get a list of unique record names in the file
@@ -1463,50 +1467,51 @@
                 if isinstance(text, bytes):
                     text = text.decode()
                 names.append(text)
         else:
             names = self.textlist
         return names
 
-    def get_unique_package_names(self, decode=False):
+    def get_unique_package_names(self, decode=False, to=False):
         """
         Get a list of unique package names in the file
 
         Parameters
         ----------
         decode : bool
             Optional boolean used to decode byte strings (default is False).
 
         Returns
         ----------
         names : list of strings
             List of unique package names in the binary file.
 
         """
+
         if decode:
             names = []
-            for text in self.paknamlist:
+            for text in self._unique_package_names(to):
                 if isinstance(text, bytes):
                     text = text.decode()
                 names.append(text)
         else:
-            names = self.paknamlist
+            names = self._unique_package_names(to)
         return names
 
-    def _unique_package_names(self):
+    def _unique_package_names(self, to=False):
         """
         Get a list of unique package names in the file
 
         Returns
         ----------
         out : list of strings
             List of unique package names in the binary file.
 
         """
-        return self.paknamlist
+        return self.paknamlist_to if to else self.paknamlist_from
 
     def get_kstpkper(self):
         """
         Get a list of unique tuples (stress period, time step) in the file.
         Indices are 0-based, use the `kstpkper` attribute for 1-based.
 
         Returns
@@ -1573,14 +1578,15 @@
     def get_data(
         self,
         idx=None,
         kstpkper=None,
         totim=None,
         text=None,
         paknam=None,
+        paknam2=None,
         full3D=False,
     ) -> Union[List, np.ndarray]:
         """
         Get data from the binary budget file.
 
         Parameters
         ----------
@@ -1590,14 +1596,22 @@
             A tuple containing the time step and stress period (kstp, kper).
             The kstp and kper values are zero based.
         totim : float
             The simulation time.
         text : str
             The text identifier for the record.  Examples include
             'RIVER LEAKAGE', 'STORAGE', 'FLOW RIGHT FACE', etc.
+        paknam : str
+            The `from` package name for the record.
+        paknam2 : str
+            The `to` package name for the record.  This argument can be
+            useful for MODFLOW 6 budget files if multiple packages of
+            the same type are specified.  The paknam2 argument can be
+            specified as the package name (not the package type) in
+            order to retrieve budget data for a specific named package.
         full3D : boolean
             If true, then return the record as a three dimensional numpy
             array, even for those list-style records written as part of a
             'COMPACT BUDGET' MODFLOW budget file.  (Default is False.)
 
         Returns
         ----------
@@ -1619,104 +1633,79 @@
         --------
 
         """
         # trap for totim error
         if totim is not None:
             if len(self.times) == 0:
                 errmsg = """This is an older style budget file that
-                         does not have times in it.  Use the MODFLOW 
-                         compact budget format if you want to work with 
+                         does not have times in it.  Use the MODFLOW
+                         compact budget format if you want to work with
                          times.  Or you may access this file using the
                          kstp and kper arguments or the idx argument."""
                 raise Exception(errmsg)
 
         # check and make sure that text is in file
         text16 = None
         if text is not None:
             text16 = self._find_text(text)
         paknam16 = None
         if paknam is not None:
             paknam16 = self._find_paknam(paknam)
-
+        paknam16_2 = None
+        if paknam2 is not None:
+            paknam16_2 = self._find_paknam(paknam2, to=True)
+
+        # build the selection mask
+        select_indices = np.array([True] * len(self.recordarray))
+        selected = False
+        if idx is not None:
+            select_indices[idx] = False
+            select_indices = ~select_indices
+            selected = True
         if kstpkper is not None:
             kstp1 = kstpkper[0] + 1
             kper1 = kstpkper[1] + 1
-            if text is None and paknam is None:
-                select_indices = np.where(
-                    (self.recordarray["kstp"] == kstp1)
-                    & (self.recordarray["kper"] == kper1)
-                )
-            else:
-                if paknam is None and text is not None:
-                    select_indices = np.where(
-                        (self.recordarray["kstp"] == kstp1)
-                        & (self.recordarray["kper"] == kper1)
-                        & (self.recordarray["text"] == text16)
-                    )
-                elif text is None and paknam is not None:
-                    select_indices = np.where(
-                        (self.recordarray["kstp"] == kstp1)
-                        & (self.recordarray["kper"] == kper1)
-                        & (self.recordarray["paknam"] == paknam16)
-                    )
-                else:
-                    select_indices = np.where(
-                        (self.recordarray["kstp"] == kstp1)
-                        & (self.recordarray["kper"] == kper1)
-                        & (self.recordarray["text"] == text16)
-                        & (self.recordarray["paknam"] == paknam16)
-                    )
-
-        elif totim is not None:
-            if text is None and paknam is None:
-                select_indices = np.where(self.recordarray["totim"] == totim)
-            else:
-                if paknam is None and text is not None:
-                    select_indices = np.where(
-                        (self.recordarray["totim"] == totim)
-                        & (self.recordarray["text"] == text16)
-                    )
-                elif text is None and paknam is not None:
-                    select_indices = np.where(
-                        (self.recordarray["totim"] == totim)
-                        & (self.recordarray["paknam"] == paknam16)
-                    )
-                else:
-                    select_indices = np.where(
-                        (self.recordarray["totim"] == totim)
-                        & (self.recordarray["text"] == text16)
-                        & (self.recordarray["paknam"] == paknam16)
-                    )
-
-        # allow for idx to be a list or a scalar
-        elif idx is not None:
-            if isinstance(idx, list):
-                select_indices = idx
-            else:
-                select_indices = [idx]
-
-        # case where only text is entered
-        elif text is not None:
-            select_indices = np.where(self.recordarray["text"] == text16)
+            select_indices = select_indices & (
+                self.recordarray["kstp"] == kstp1
+            )
+            select_indices = select_indices & (
+                self.recordarray["kper"] == kper1
+            )
+            selected = True
+        if text16 is not None:
+            select_indices = select_indices & (
+                self.recordarray["text"] == text16
+            )
+            selected = True
+        if paknam16 is not None:
+            select_indices = select_indices & (
+                self.recordarray["paknam"] == paknam16
+            )
+            selected = True
+        if paknam16_2 is not None:
+            select_indices = select_indices & (
+                self.recordarray["paknam2"] == paknam16_2
+            )
+            selected = True
+        if totim is not None:
+            select_indices = select_indices & np.isclose(
+                self.recordarray["totim"], totim
+            )
+            selected = True
 
-        else:
+        if not selected:
             raise TypeError(
                 "get_data() missing 1 required argument: 'kstpkper', 'totim', "
                 "'idx', or 'text'"
             )
-
-        # build and return the record list
-        if isinstance(select_indices, tuple):
-            select_indices = select_indices[0]
-        recordlist = []
-        for idx in select_indices:
-            rec = self.get_record(idx, full3D=full3D)
-            recordlist.append(rec)
-
-        return recordlist
+        return [
+            self.get_record(idx, full3D=full3D)
+            for idx, t in enumerate(select_indices)
+            if t
+        ]
 
     def get_ts(self, idx, text=None, times=None):
         """
         Get a time series from the binary budget file.
 
         Parameters
         ----------
```

### Comparing `flopy-3.6.0/flopy/utils/check.py` & `flopy-3.7.0/flopy/utils/check.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/utils/compare.py` & `flopy-3.7.0/flopy/utils/compare.py`

 * *Files 0% similar despite different names*

```diff
@@ -560,15 +560,15 @@
 
     # Get head info for namefile1
     hfpth1 = None
     status1 = dbs
     if files1 is None:
         # Get oc info, and return if OC not included in models
         ocf1 = get_entries_from_namefile(namefile1, "OC")
-        if not any(ocf1) is None:
+        if any(ocf1) is not None:
             return True
 
         hu1, hfpth1, du1, _ = ModflowOc.get_ocoutput_units(ocf1[0][0])
         if text.lower() == "head":
             iut = hu1
         elif text.lower() == "drawdown":
             iut = du1
```

### Comparing `flopy-3.6.0/flopy/utils/crs.py` & `flopy-3.7.0/flopy/utils/crs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""Utilities related to coordinate reference system handling.
-"""
+"""Utilities related to coordinate reference system handling."""
 
 import warnings
 from pathlib import Path
 
 from ..utils import import_optional_dependency
 
 
@@ -20,15 +19,15 @@
         The value can be anything accepted by
         :meth:`pyproj.CRS.from_user_input() <pyproj.crs.CRS.from_user_input>`,
         such as an authority string (eg "EPSG:26916") or a WKT string.
 
     Returns
     -------
     pyproj.CRS instance
-        CRS instance initiallized with the name
+        CRS instance initialized with the name
         and authority code (e.g. "epsg:5070") produced by
         :meth:`pyproj.crs.CRS.to_authority`
 
     Notes
     -----
     :meth:`pyproj.crs.CRS.to_authority` will return None if a matching
     authority name and code can't be found. In this case,
```

### Comparing `flopy-3.6.0/flopy/utils/cvfdutil.py` & `flopy-3.7.0/flopy/utils/cvfdutil.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,27 @@
 import numpy as np
+import pandas as pd
+
+from .utl_import import import_optional_dependency
 
 
 def area_of_polygon(x, y):
-    """Calculates the signed area of an arbitrary polygon given its vertices
-    https://stackoverflow.com/a/4682656/ (Joe Kington)
-    http://softsurfer.com/Archive/algorithm_0101/algorithm_0101.htm#2D%20Polygons
-    """
-    area = 0.0
-    for i in range(-1, len(x) - 1):
-        area += x[i] * (y[i + 1] - y[i - 1])
-    return area / 2.0
+    shapely = import_optional_dependency("shapely")
+    from shapely.geometry import Polygon
+
+    pgon = Polygon(zip(x, y))
+    return pgon.area
 
 
 def centroid_of_polygon(points):
-    """
-    https://stackoverflow.com/a/14115494/ (mgamba)
-    """
-    import itertools as IT
+    shapely = import_optional_dependency("shapely")
+    from shapely.geometry import Polygon
 
-    area = area_of_polygon(*zip(*points))
-    result_x = 0
-    result_y = 0
-    N = len(points)
-    points = IT.cycle(points)
-    x1, y1 = next(points)
-    for i in range(N):
-        x0, y0 = x1, y1
-        x1, y1 = next(points)
-        cross = (x0 * y1) - (x1 * y0)
-        result_x += (x0 + x1) * cross
-        result_y += (y0 + y1) * cross
-    result_x /= area * 6.0
-    result_y /= area * 6.0
-    return (result_x, result_y)
+    pgon = Polygon(points)
+    return pgon.centroid.x, pgon.centroid.y
 
 
 class Point:
     def __init__(self, x, y):
         self.x = x
         self.y = y
         return
@@ -127,14 +112,15 @@
 
 
 def to_cvfd(
     vertdict,
     nodestart=None,
     nodestop=None,
     skip_hanging_node_check=False,
+    duplicate_decimals=9,
     verbose=False,
 ):
     """
     Convert a vertex dictionary into verts and iverts
 
     Parameters
     ----------
@@ -147,14 +133,19 @@
     nodestop : int
         ending node number up to but not including. (default is len(vertdict))
 
     skip_hanging_node_check : bool
         skip the hanging node check.  this may only be necessary for quad-based
         grid refinement. (default is False)
 
+    duplicate_decimals : int
+        decimals to round duplicate vertex checks.  GRIDGEN can occasionally
+        produce very-nearly overlapping vertices, this can be used to change
+        the sensitivity for filtering out duplicates. (default is 9)
+
     verbose : bool
         print messages to the screen. (default is False)
 
     Returns
     -------
     verts : ndarray
         array of x, y vertices
@@ -188,15 +179,18 @@
         points = vertdict[icell]
         nvertstart += len(points)
         xc, yc = centroid_of_polygon(points)
         xcyc[icell, 0] = xc
         xcyc[icell, 1] = yc
         ivertlist = []
         for p in points:
-            pt = tuple(p)
+            pt = (
+                round(p[0], duplicate_decimals),
+                round(p[1], duplicate_decimals),
+            )
             if pt in vertexdict:
                 ivert = vertexdict[pt]
             else:
                 vertexdict[pt] = iv
                 ivert = iv
                 iv += 1
             ivertlist.append(ivert)
```

### Comparing `flopy-3.6.0/flopy/utils/datafile.py` & `flopy-3.7.0/flopy/utils/datafile.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,15 +270,15 @@
         """
 
         plotarray = np.atleast_3d(
             self.get_data(
                 kstpkper=kstpkper, totim=totim, mflay=mflay
             ).transpose()
         ).transpose()
-        if mflay != None:
+        if mflay is not None:
             attrib_dict = {f"{attrib_name}{mflay}": plotarray[0, :, :]}
         else:
             attrib_dict = {}
             for k in range(plotarray.shape[0]):
                 name = f"{attrib_name}{k}"
                 attrib_dict[name] = plotarray[k]
```

### Comparing `flopy-3.6.0/flopy/utils/datautil.py` & `flopy-3.7.0/flopy/utils/datautil.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,32 +50,40 @@
         if item_abs > max_size:
             max_size = item_abs
     return max_size
 
 
 class DatumUtil:
     @staticmethod
-    def is_int(str):
-        try:
-            int(str)
-            return True
-        except TypeError:
-            return False
-        except ValueError:
-            return False
+    def is_int(v):
+        if isinstance(v, np.ndarray):
+            try:
+                int(v.item())
+            except ValueError:
+                return False
+        else:
+            try:
+                int(v)
+                return True
+            except (TypeError, ValueError):
+                return False
 
     @staticmethod
-    def is_float(str):
-        try:
-            float(str)
-            return True
-        except TypeError:
-            return False
-        except ValueError:
-            return False
+    def is_float(v):
+        if isinstance(v, np.ndarray):
+            try:
+                float(v.item())
+            except ValueError:
+                return False
+        else:
+            try:
+                float(v)
+                return True
+            except (TypeError, ValueError):
+                return False
 
     @staticmethod
     def is_basic_type(obj):
         if (
             isinstance(obj, str)
             or isinstance(obj, int)
             or isinstance(obj, float)
@@ -131,15 +139,15 @@
         returns the first item in the list 'current_list'
     next_item : (current_list : list) : variable
         returns the next item in the list 'current_list'
     array_comp : (first_array : list, second_array : list) : boolean
         compares two lists, returns true if they are identical (with max_error)
     spilt_data_line : (line : string) : list
         splits a string apart (using split) and then cleans up the results
-        dealing with various MODFLOW input file releated delimiters.  returns
+        dealing with various MODFLOW input file related delimiters.  returns
         the delimiter type used.
     clean_numeric : (text : string) : string
         returns a cleaned up version of 'text' with only numeric characters
     save_array_diff : (first_array : list, second_array : list,
                        first_array_name : string, second_array_name : string)
         saves lists 'first_array' and 'second_array' to files first_array_name
         and second_array_name and then saves the difference of the two
@@ -356,19 +364,29 @@
                         or PyListUtil.delimiter_list[delimiter]
                         < PyListUtil.delimiter_list[max_split_type]
                     ):
                         max_split_size = len(alt_split)
                         max_split_type = delimiter
                         max_split_list = alt_split
 
+            if max_split_type is None and max_split_size > 0:
+                split_first = max_split_list[0].strip().split(",")
+                if len(split_first) > 1:
+                    max_split_list = split_first + max_split_list[1:]
+                    max_split_size = len(max_split_list)
+                    max_split_type = "combo"
+
             if max_split_type is not None and max_split_size > 1:
                 clean_line = max_split_list
                 if PyListUtil.line_num == 0:
                     PyListUtil.delimiter_used = max_split_type
-                elif PyListUtil.delimiter_used != max_split_type:
+                elif (
+                    PyListUtil.delimiter_used != max_split_type
+                    or max_split_type == "combo"
+                ):
                     PyListUtil.consistent_delim = False
             if max_split_size > 1:
                 PyListUtil.line_num += 1
 
         arr_fixed_line = []
         index = 0
         # loop through line to fix quotes and delimiters
```

### Comparing `flopy-3.6.0/flopy/utils/flopy_io.py` & `flopy-3.7.0/flopy/utils/flopy_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,15 @@
     ncol : int
         number of columns to parse from line. (default is 1)
     length : int
         length of each column for fixed column widths. (default is 10)
     ipos : list, int, or numpy array
         user-provided column widths. (default is None)
     free : bool
-        boolean indicating if sting is free format. ncol, length, and
+        boolean indicating if string is free format. ncol, length, and
         ipos are not used if free is True. (default is False)
 
     Returns
     -------
     out : list
         padded list containing data parsed from the passed text string
 
@@ -287,29 +287,29 @@
     from . import CellBudgetFile as CBF
     from .util_list import MfList
 
     cbf = CBF(cbc_file, precision=precision, verbose=verbose)
 
     # create a empty numpy array of shape (time,layer,row,col)
     m4d = np.zeros((cbf.nper, cbf.nlay, cbf.nrow, cbf.ncol), dtype=np.float32)
-    m4d[:] = np.NaN
+    m4d[:] = np.nan
 
     # process the records in the cell budget file
     iper = -1
     for kstpkper in cbf.kstpkper:
         kstpkper = (kstpkper[0] - 1, kstpkper[1] - 1)
         kper = kstpkper[1]
         # if we haven't visited this kper yet
         if kper != iper:
             arr = cbf.get_data(kstpkper=kstpkper, text=text, full3D=True)
             if len(arr) > 0:
                 arr = arr[0]
                 print(arr.max(), arr.min(), arr.sum())
                 # masked where zero
-                arr[np.where(arr == 0.0)] = np.NaN
+                arr[np.where(arr == 0.0)] = np.nan
                 m4d[iper + 1] = arr
             iper += 1
 
     # model wasn't passed, then create a generic model
     if model is None:
         model = Modflow("test")
     # if model doesn't have a wel package, then make a generic one...
@@ -348,19 +348,18 @@
         Keyword arguments passed to numpy.loadtxt or pandas.read_csv.
 
     Returns
     -------
     ra : np.recarray
         Numpy record array of file contents.
     """
-    from ..utils import import_optional_dependency
 
     if use_pandas:
         if delimiter.isspace():
-            kwargs["delim_whitespace"] = True
+            kwargs["sep"] = "\\s+"
         if isinstance(dtype, np.dtype) and "names" not in kwargs:
             kwargs["names"] = dtype.names
 
     if use_pandas:
         df = pd.read_csv(file, dtype=dtype, skiprows=skiprows, **kwargs)
         return df.to_records(index=False)
     # default use of numpy
@@ -588,15 +587,15 @@
 
     return scrub_login(p) if scrub else p
 
 
 def scrub_login(s: str) -> str:
     """
     Remove the current login name from the given string,
-    replacing any occurences with "***".
+    replacing any occurrences with "***".
 
     Parameters
     ----------
     s : str
         the input string
 
     Returns
```

### Comparing `flopy-3.6.0/flopy/utils/formattedfile.py` & `flopy-3.7.0/flopy/utils/formattedfile.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/utils/geometry.py` & `flopy-3.7.0/flopy/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/utils/geospatial_utils.py` & `flopy-3.7.0/flopy/utils/geospatial_utils.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/utils/get_modflow.py` & `flopy-3.7.0/flopy/utils/get_modflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 
 This script originates from FloPy: https://github.com/modflowpy/flopy
 This file can be downloaded and run independently outside FloPy.
 It requires Python 3.6 or later, and has no dependencies.
 
 See https://developer.github.com/v3/repos/releases/ for GitHub Releases API.
 """
+
 import json
 import os
 import shutil
 import sys
 import tempfile
 import urllib
 import urllib.request
 import warnings
 import zipfile
 from importlib.util import find_spec
 from pathlib import Path
+from platform import processor
 
 __all__ = ["run_main"]
 __license__ = "CC0"
 
 from typing import Dict, List, Tuple
 
 default_owner = "MODFLOW-USGS"
@@ -29,15 +31,15 @@
 # key is the repo name, value is the renamed file prefix for the download
 renamed_prefix = {
     "modflow6": "modflow6",
     "executables": "modflow_executables",
     "modflow6-nightly-build": "modflow6_nightly",
 }
 available_repos = list(renamed_prefix.keys())
-available_ostags = ["linux", "mac", "win32", "win64"]
+available_ostags = ["linux", "mac", "macarm", "win32", "win64", "win64par"]
 max_http_tries = 3
 
 # Check if this is running from flopy
 within_flopy = False
 spec = find_spec("flopy")
 if spec is not None:
     within_flopy = (
@@ -61,19 +63,19 @@
         return "win" + ("64" if sys.maxsize > 2**32 else "32")
     elif sys.platform.startswith("darwin"):
         return "mac"
     raise ValueError(f"platform {sys.platform!r} not supported")
 
 
 def get_suffixes(ostag) -> Tuple[str, str]:
-    if ostag in ["win32", "win64"]:
+    if ostag in ["win32", "win64", "win64par"]:
         return ".exe", ".dll"
     elif ostag == "linux":
         return "", ".so"
-    elif ostag == "mac":
+    elif "mac" in ostag:
         return "", ".dylib"
     else:
         raise KeyError(
             f"unrecognized ostag {ostag!r}; choose one of {available_ostags}"
         )
 
 
@@ -401,28 +403,36 @@
         raise KeyError(
             f"repo {repo!r} not supported; choose one of {available_repos}"
         )
 
     # get the selected release
     release = get_release(owner, repo, release_id, quiet)
     assets = release.get("assets", [])
-
+    asset_names = [a["name"] for a in assets]
     for asset in assets:
-        if ostag in asset["name"]:
+        asset_name = asset["name"]
+        if ostag in asset_name:
+            # temporary hack for nightly gfortran build for ARM macs
+            # todo: clean up if/when all repos have an ARM mac build
+            if (
+                repo == "modflow6-nightly-build"
+                and "macarm.zip" in asset_names
+                and processor() == "arm"
+                and ostag == "mac.zip"
+            ):
+                continue
             break
     else:
         raise ValueError(
             f"could not find ostag {ostag!r} from release {release['tag_name']!r}; "
             f"see available assets here:\n{release['html_url']}"
         )
-    asset_name = asset["name"]
     download_url = asset["browser_download_url"]
     if repo == "modflow6":
         asset_pth = Path(asset_name)
-        asset_stem = asset_pth.stem
         asset_suffix = asset_pth.suffix
         dst_fname = "-".join([repo, release["tag_name"], ostag]) + asset_suffix
     else:
         # change local download name so it is more unique
         dst_fname = "-".join(
             [renamed_prefix[repo], release["tag_name"], asset_name]
         )
@@ -594,15 +604,15 @@
             bindir_path.rmdir()
             for subdir in rmdir.parents:
                 bindir_path = bindir / subdir
                 if bindir_path == bindir:
                     break
                 shutil.rmtree(str(bindir_path))
 
-    if ostag in ["linux", "mac"]:
+    if ostag in ["linux", "mac", "macarm"]:
         # similar to "chmod +x fname" for each executable
         for fname in chmod:
             pth = bindir / fname
             pth.chmod(pth.stat().st_mode | 0o111)
 
     # Show listing
     if not quiet:
```

### Comparing `flopy-3.6.0/flopy/utils/gridgen.py` & `flopy-3.7.0/flopy/utils/gridgen.py`

 * *Files 0% similar despite different names*

```diff
@@ -1888,15 +1888,14 @@
         fields = sf.fields
         attributes = [l[0] for l in fields[1:]]
         records = sf.records()
         idx = attributes.index("nodenumber")
         for i in range(len(shapes)):
             nodenumber = int(records[i][idx]) - 1
             self._vertdict[nodenumber] = shapes[i].points
-        return
 
     @staticmethod
     def read_qtg_nod(
         model_ws: Union[str, os.PathLike], nodes_only: bool = False
     ):
         """Read qtg.nod file
```

### Comparing `flopy-3.6.0/flopy/utils/gridintersect.py` & `flopy-3.7.0/flopy/utils/gridintersect.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,32 +138,37 @@
      - The optimized routines for structured grids can outperform the shapely
        routines for point and linestring intersections because of the reduced
        overhead of building and parsing the STR-tree. However, for polygons
        the STR-tree implementation is often faster than the optimized
        structured routines, especially for larger grids.
     """
 
-    def __init__(self, mfgrid, method=None, rtree=True):
+    def __init__(self, mfgrid, method=None, rtree=True, local=False):
         """Intersect shapes (Point, Linestring, Polygon) with a modflow grid.
 
         Parameters
         ----------
         mfgrid : flopy modflowgrid
             MODFLOW grid as implemented in flopy
         method : str, optional
-            default is None, which determines intersection method based on
-            the grid type. Options are either 'vertex' which uses shapely
-            interesection operations or 'structured' which uses optimized
-            methods that only work for structured grids
+            Options are either 'vertex' which uses shapely intersection operations
+            or 'structured' which uses optimized methods that only work for structured
+            grids. The default is None, which determines intersection method based on
+            the grid type.
         rtree : bool, optional
             whether to build an STR-Tree, default is True. If False no STR-tree
             is built, but intersects will loop through all model gridcells
             (which is generally slower). Only read when `method='vertex'`.
+        local : bool, optional
+            use local model coordinates from model grid to build grid geometries,
+            default is False and uses real-world coordinates (with offset and rotation),
+             if specified.
         """
         self.mfgrid = mfgrid
+        self.local = local
         if method is None:
             # determine method from grid_type
             self.method = self.mfgrid.grid_type
         else:
             # set method
             self.method = method
         self.rtree = rtree
@@ -352,16 +357,19 @@
         """
         shapely = import_optional_dependency("shapely")
 
         nrow = self.mfgrid.nrow
         ncol = self.mfgrid.ncol
         ncells = nrow * ncol
         cellids = np.arange(ncells)
-        xvertices = self.mfgrid.xvertices
-        yvertices = self.mfgrid.yvertices
+        if self.local:
+            xvertices, yvertices = np.meshgrid(*self.mfgrid.xyedges)
+        else:
+            xvertices = self.mfgrid.xvertices
+            yvertices = self.mfgrid.yvertices
 
         # arrays of coordinates for rectangle cells
         I, J = np.ogrid[0:nrow, 0:ncol]
         xverts = np.stack(
             [
                 xvertices[I, J],
                 xvertices[I, J + 1],
@@ -417,55 +425,36 @@
         Returns
         -------
         geoms : array_like
             array of shapely Polygons
         cellids : array_like
             array of cellids
         """
-        shapely_geo = import_optional_dependency("shapely.geometry")
-
-        # for cell2d rec-arrays
-        geoms = []
-        cellids = []
-        if isinstance(self.mfgrid._cell2d, np.recarray):
-            for icell in self.mfgrid._cell2d.icell2d:
-                points = []
-                icverts = [
-                    f"icvert_{i}"
-                    for i in range(self.mfgrid._cell2d["ncvert"][icell])
-                ]
-                for iv in self.mfgrid._cell2d[icverts][icell]:
-                    points.append(
-                        (
-                            self.mfgrid._vertices.xv[iv],
-                            self.mfgrid._vertices.yv[iv],
-                        )
-                    )
-                # close the polygon, if necessary
-                if points[0] != points[-1]:
-                    points.append(points[0])
-                geoms.append(shapely_geo.Polygon(points))
-                cellids.append(icell)
-        # for cell2d lists
-        elif isinstance(self.mfgrid._cell2d, list):
-            for icell in range(len(self.mfgrid._cell2d)):
-                points = []
-                for iv in self.mfgrid._cell2d[icell][4:]:
-                    points.append(
-                        (
-                            self.mfgrid._vertices[iv][1],
-                            self.mfgrid._vertices[iv][2],
+        shapely = import_optional_dependency("shapely")
+        if self.local:
+            geoms = [
+                shapely.polygons(
+                    list(
+                        zip(
+                            *self.mfgrid.get_local_coords(
+                                *np.array(
+                                    self.mfgrid.get_cell_vertices(node)
+                                ).T
+                            )
                         )
                     )
-                # close the polygon, if necessary
-                if points[0] != points[-1]:
-                    points.append(points[0])
-                geoms.append(shapely_geo.Polygon(points))
-                cellids.append(icell)
-        return np.array(geoms), np.array(cellids)
+                )
+                for node in range(self.mfgrid.ncpl)
+            ]
+        else:
+            geoms = [
+                shapely.polygons(self.mfgrid.get_cell_vertices(node))
+                for node in range(self.mfgrid.ncpl)
+            ]
+        return np.array(geoms), np.arange(self.mfgrid.ncpl)
 
     def _rect_grid_to_shape_list(self):
         """internal method, list of shapely polygons for structured grid cells.
 
         .. deprecated:: 3.3.6
             use _rect_grid_to_geoms_cellids() instead.
 
@@ -1203,15 +1192,15 @@
         ixshapes = []
         for p in shp:
             # if grid is rotated or offset transform point to local coords
             if (
                 self.mfgrid.angrot != 0.0
                 or self.mfgrid.xoffset != 0.0
                 or self.mfgrid.yoffset != 0.0
-            ):
+            ) and not self.local:
                 rx, ry = transform(
                     p.x,
                     p.y,
                     self.mfgrid.xoffset,
                     self.mfgrid.yoffset,
                     self.mfgrid.angrot_radians,
                     inverse=True,
@@ -1343,19 +1332,21 @@
             ymin = np.min(self.mfgrid.xyedges[1])
             ymax = np.max(self.mfgrid.xyedges[1])
         else:
             xmin, xmax, ymin, ymax = self.mfgrid.extent
         pl = shapely_geo.box(xmin, ymin, xmax, ymax)
 
         # rotate and translate linestring to local coords
-        if self.mfgrid.xoffset != 0.0 or self.mfgrid.yoffset != 0.0:
+        if (
+            self.mfgrid.xoffset != 0.0 or self.mfgrid.yoffset != 0.0
+        ) and not self.local:
             shp = affinity_loc.translate(
                 shp, xoff=-self.mfgrid.xoffset, yoff=-self.mfgrid.yoffset
             )
-        if self.mfgrid.angrot != 0.0:
+        if self.mfgrid.angrot != 0.0 and not self.local:
             shp = affinity_loc.rotate(
                 shp, -self.mfgrid.angrot, origin=(0.0, 0.0)
             )
 
         # clip line to mfgrid bbox
         lineclip = shp.intersection(pl)
 
@@ -1376,15 +1367,15 @@
                 lengths += l
                 # if necessary, transform coordinates back to real
                 # world coordinates
                 if (
                     self.mfgrid.angrot != 0.0
                     or self.mfgrid.xoffset != 0.0
                     or self.mfgrid.yoffset != 0.0
-                ):
+                ) and not self.local:
                     v_realworld = []
                     for pt in v:
                         pt = np.array(pt)
                         rx, ry = transform(
                             pt[:, 0],
                             pt[:, 1],
                             self.mfgrid.xoffset,
@@ -1420,15 +1411,15 @@
             )
             # if necessary, transform coordinates back to real
             # world coordinates
             if (
                 self.mfgrid.angrot != 0.0
                 or self.mfgrid.xoffset != 0.0
                 or self.mfgrid.yoffset != 0.0
-            ):
+            ) and not self.local:
                 v_realworld = []
                 for pt in vertices:
                     pt = np.array(pt)
                     rx, ry = transform(
                         pt[:, 0],
                         pt[:, 1],
                         self.mfgrid.xoffset,
@@ -1542,15 +1533,15 @@
         # linestring already in local coords but
         # because intersect_point does transform again
         # we transform back to real world here if necessary
         if (
             self.mfgrid.angrot != 0.0
             or self.mfgrid.xoffset != 0.0
             or self.mfgrid.yoffset != 0.0
-        ):
+        ) and not self.local:
             x0, y0 = transform(
                 [x[0]],
                 [y[0]],
                 self.mfgrid.xoffset,
                 self.mfgrid.yoffset,
                 self.mfgrid.angrot_radians,
                 inverse=False,
@@ -1909,19 +1900,21 @@
         # initialize the result lists
         nodelist = []
         areas = []
         vertices = []
         ixshapes = []
 
         # transform polygon to local grid coordinates
-        if self.mfgrid.xoffset != 0.0 or self.mfgrid.yoffset != 0.0:
+        if (
+            self.mfgrid.xoffset != 0.0 or self.mfgrid.yoffset != 0.0
+        ) and not self.local:
             shp = affinity_loc.translate(
                 shp, xoff=-self.mfgrid.xoffset, yoff=-self.mfgrid.yoffset
             )
-        if self.mfgrid.angrot != 0.0:
+        if self.mfgrid.angrot != 0.0 and not self.local:
             shp = affinity_loc.rotate(
                 shp, -self.mfgrid.angrot, origin=(0.0, 0.0)
             )
 
         # use the bounds of the polygon to restrict the cell search
         minx, miny, maxx, maxy = shp.bounds
         rectangle = ((minx, miny), (maxx, maxy))
@@ -1978,15 +1971,15 @@
 
                 # if necessary, transform coordinates back to real
                 # world coordinates
                 if (
                     self.mfgrid.angrot != 0.0
                     or self.mfgrid.xoffset != 0.0
                     or self.mfgrid.yoffset != 0.0
-                ):
+                ) and not self.local:
                     v_realworld = []
                     if intersect.geom_type.startswith("Multi"):
                         for ipoly in intersect.geoms:
                             v_realworld += (
                                 self._transform_geo_interface_polygon(ipoly)
                             )
                     else:
@@ -2249,21 +2242,25 @@
             coordinates for the left cell edge.
 
         x : float
             The x position to find in arr.
         """
         jpos = []
 
-        if x == arr[-1]:
+        if np.isclose(x, arr[-1]):
             return len(arr) - 2
 
-        if x < min(arr[0], arr[-1]):
-            return None
+        xmin = min(arr[0], arr[-1])
+        xmax = max(arr[0], arr[-1])
 
-        if x > max(arr[0], arr[-1]):
+        if np.isclose(x, xmin):
+            x = xmin
+        if np.isclose(x, xmax):
+            x = xmax
+        if not (xmin <= x <= xmax):
             return None
 
         # go through each position
         for j in range(len(arr) - 1):
             xl = arr[j]
             xr = arr[j + 1]
             frac = (x - xl) / (xr - xl)
```

### Comparing `flopy-3.6.0/flopy/utils/gridutil.py` & `flopy-3.7.0/flopy/utils/gridutil.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 
     Returns
     -------
         A list of tuples (layer index, node index)
     """
 
     if not isinstance(ncpl, (int, list, tuple, np.ndarray)):
-        raise ValueError(f"ncpl must be int or array-like")
+        raise ValueError("ncpl must be int or array-like")
     if not isinstance(nodes, (list, tuple, np.ndarray)):
-        raise ValueError(f"nodes must be array-like")
+        raise ValueError("nodes must be array-like")
 
     if len(nodes) == 0:
         return []
 
     if isinstance(ncpl, int):
         # infer min number of layers to hold given node numbers
         layers = range(floor(np.max(nodes) / ncpl) if len(nodes) > 0 else 1)
```

### Comparing `flopy-3.6.0/flopy/utils/lgrutil.py` & `flopy-3.7.0/flopy/utils/lgrutil.py`

 * *Files 4% similar despite different names*

```diff
@@ -177,33 +177,31 @@
                 self.ibcl[k] = self.ibcl[k - 1] + self.ncppl[k]
 
         # parent lower left
         self.xllp = xllp
         self.yllp = yllp
 
         # child grid properties
-        self.nplbeg = idxl.min()
-        self.nplend = idxl.max()
-        self.npcbeg = idxc.min()
-        self.npcend = idxc.max()
-        self.nprbeg = idxr.min()
-        self.nprend = idxr.max()
+        self.nplbeg = int(idxl.min())
+        self.nplend = int(idxl.max())
+        self.npcbeg = int(idxc.min())
+        self.npcend = int(idxc.max())
+        self.nprbeg = int(idxr.min())
+        self.nprend = int(idxr.max())
 
         # child grid dimensions
-        self.nlay = self.ncppl.sum()
+        self.nlay = int(self.ncppl.sum())
         self.nrow = (self.nprend - self.nprbeg + 1) * ncpp
         self.ncol = (self.npcend - self.npcbeg + 1) * ncpp
 
         # assign child properties
         self.delr, self.delc = self.get_delr_delc()
         self.top, self.botm = self.get_top_botm()
-        self.xll = xllp + self.delrp[0 : self.npcbeg].sum()
-        self.yll = yllp + self.delcp[self.nprend + 1 :].sum()
-
-        return
+        self.xll = xllp + float(self.delrp[0 : self.npcbeg].sum())
+        self.yll = yllp + float(self.delcp[self.nprend + 1 :].sum())
 
     def get_shape(self):
         """
         Return the shape of the child grid
 
         Returns
         -------
@@ -228,44 +226,44 @@
     def get_delr_delc(self):
         # create the delr and delc arrays for this child grid
         delr = np.zeros((self.ncol), dtype=float)
         delc = np.zeros((self.nrow), dtype=float)
         jstart = 0
         jend = self.ncpp
         for j in range(self.npcbeg, self.npcend + 1):
-            delr[jstart:jend] = self.delrp[j] / self.ncpp
+            delr[jstart:jend] = float(self.delrp[j]) / self.ncpp
             jstart = jend
             jend = jstart + self.ncpp
         istart = 0
         iend = self.ncpp
         for i in range(self.nprbeg, self.nprend + 1):
-            delc[istart:iend] = self.delcp[i] / self.ncpp
+            delc[istart:iend] = float(self.delcp[i]) / self.ncpp
             istart = iend
             iend = istart + self.ncpp
         return delr, delc
 
     def get_top_botm(self):
         bt = self.botmp
         tp = self.topp
         shp = tp.shape
         tp = tp.reshape(1, shp[0], shp[1])
         pbotm = np.vstack((tp, bt))
         botm = np.zeros((self.nlay + 1, self.nrow, self.ncol), dtype=float)
         for ip in range(self.nprbeg, self.nprend + 1):
             for jp in range(self.npcbeg, self.npcend + 1):
-                top = pbotm[0, ip, jp]
+                top = float(pbotm[0, ip, jp])
                 icrowstart = (ip - self.nprbeg) * self.ncpp
                 icrowend = icrowstart + self.ncpp
                 iccolstart = (jp - self.npcbeg) * self.ncpp
                 iccolend = iccolstart + self.ncpp
                 botm[0, icrowstart:icrowend, iccolstart:iccolend] = top
                 kc = 1
                 for kp in range(self.nplbeg, self.nplend + 1):
-                    top = pbotm[kp, ip, jp]
-                    bot = pbotm[kp + 1, ip, jp]
+                    top = float(pbotm[kp, ip, jp])
+                    bot = float(pbotm[kp + 1, ip, jp])
                     dz = (top - bot) / self.ncppl[kp]
                     for _ in range(self.ncppl[kp]):
                         botm[kc, icrowstart:icrowend, iccolstart:iccolend] = (
                             botm[
                                 kc - 1,
                                 icrowstart:icrowend,
                                 iccolstart:iccolend,
@@ -299,15 +297,15 @@
         )
         for ip in range(self.nprbeg, self.nprend + 1):
             for jp in range(self.npcbeg, self.npcend + 1):
                 icrowstart = (ip - self.nprbeg) * self.ncpp
                 icrowend = icrowstart + self.ncpp
                 iccolstart = (jp - self.npcbeg) * self.ncpp
                 iccolend = iccolstart + self.ncpp
-                value = parent_array[ip, jp]
+                value = int(parent_array[ip, jp])
                 child_array[icrowstart:icrowend, iccolstart:iccolend] = value
         return child_array
 
     def get_idomain(self):
         """
         Return the idomain array for the child model.  This will normally
         be all ones unless the idomain array for the parent model is
@@ -473,55 +471,62 @@
                                 angle = 90.0  # +y, north
 
                         # vertical connection
                         cl1 = None
                         cl2 = None
                         hwva = None
 
-                        tpp = topp[ip, jp]
-                        btp = botp[kp, ip, jp]
+                        tpp = float(topp[ip, jp])
+                        btp = float(botp[kp, ip, jp])
                         if kp > 0:
-                            tpp = botp[kp - 1, ip, jp]
+                            tpp = float(botp[kp - 1, ip, jp])
 
-                        tpc = topc[ic, jc]
-                        btc = botc[kc, ic, jc]
+                        tpc = float(topc[ic, jc])
+                        btc = float(botc[kc, ic, jc])
                         if kc > 0:
-                            tpc = botc[kc - 1, ic, jc]
+                            tpc = float(botc[kc - 1, ic, jc])
 
                         if ihc == 0:
                             cl1 = 0.5 * (tpp - btp)
                             cl2 = 0.5 * (tpc - btc)
-                            hwva = delrc[jc] * delcc[ic]
+                            hwva = float(delrc[jc]) * float(delcc[ic])
                         else:
                             if abs(idir) == 1:
-                                cl1 = 0.5 * delrp[jp]
-                                cl2 = 0.5 * delrc[jc]
-                                hwva = delcc[ic]
+                                cl1 = 0.5 * float(delrp[jp])
+                                cl2 = 0.5 * float(delrc[jc])
+                                hwva = float(delcc[ic])
                             elif abs(idir) == 2:
-                                cl1 = 0.5 * delcp[ip]
-                                cl2 = 0.5 * delcc[ic]
+                                cl1 = 0.5 * float(delcp[ip])
+                                cl2 = 0.5 * float(delcc[ic])
                                 hwva = delrc[jc]
 
                         # connection distance
                         cd = None
                         if cdist:
                             if abs(idir) == 3:
                                 cd = cl1 + cl2
                             else:
-                                x1 = xc[ic, jc]
-                                y1 = yc[ic, jc]
-                                x2 = xp[ip, jp]
-                                y2 = yp[ip, jp]
+                                x1 = float(xc[ic, jc])
+                                y1 = float(yc[ic, jc])
+                                x2 = float(xp[ip, jp])
+                                y2 = float(yp[ip, jp])
                                 cd = np.sqrt((x1 - x2) ** 2 + (y1 - y2) ** 2)
 
-                        exg = [(kp, ip, jp), (kc, ic, jc), ihc, cl1, cl2, hwva]
+                        exg = [
+                            (kp, ip, jp),
+                            (kc, ic, jc),
+                            ihc,
+                            cl1,
+                            cl2,
+                            hwva,
+                        ]
                         if angldegx:
-                            exg.append(angle)
+                            exg.append(float(angle))
                         if cdist:
-                            exg.append(cd)
+                            exg.append(float(cd))
                         exglist.append(exg)
         return exglist
 
     @property
     def parent(self):
         """
         Return a SimpleRegularGrid object for the parent model
```

### Comparing `flopy-3.6.0/flopy/utils/mflistfile.py` & `flopy-3.7.0/flopy/utils/mflistfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -702,15 +702,15 @@
         self.entries = incdict.keys()
         null_entries = {}
         incdict = {}
         cumdict = {}
         for entry in self.entries:
             incdict[entry] = []
             cumdict[entry] = []
-            null_entries[entry] = np.NaN
+            null_entries[entry] = np.nan
         self.null_entries = [null_entries, null_entries]
         return incdict, cumdict
 
     def _load(self, maxentries=None):
         self._build_index(maxentries)
         incdict, cumdict = self._set_entries()
         if incdict is None and cumdict is None:
@@ -859,35 +859,35 @@
         fx_str = line2[idx:].split()[0].strip()
 
         flux, cumu = None, None
         try:
             cumu = float(cu_str)
         except:
             if "NAN" in cu_str.strip().upper():
-                cumu = np.NaN
+                cumu = np.nan
         try:
             flux = float(fx_str)
         except:
             if "NAN" in fx_str.strip().upper():
-                flux = np.NaN
+                flux = np.nan
         return entry, flux, cumu
 
     def _get_totim(self, ts, sp, seekpoint):
         self.f.seek(seekpoint)
         # --read header lines
         ihead = 0
         while True:
             line = self.f.readline()
             ihead += 1
             if line == "":
                 print(
                     "end of file found while seeking budget "
                     "information for ts,sp: {} {}".format(ts, sp)
                 )
-                return np.NaN, np.NaN, np.NaN
+                return np.nan, np.nan, np.nan
             elif (
                 ihead == 2
                 and "SECONDS     MINUTES      HOURS       DAYS        YEARS"
                 not in line
             ):
                 break
             elif (
@@ -898,30 +898,30 @@
                 break
 
         if isinstance(self, SwtListBudget):
             translen = self._parse_time_line(line)
             line = self.f.readline()
             if translen is None:
                 print("error parsing translen for ts,sp", ts, sp)
-                return np.NaN, np.NaN, np.NaN
+                return np.nan, np.nan, np.nan
 
         tslen = self._parse_time_line(line)
         if tslen is None:
             print("error parsing tslen for ts,sp", ts, sp)
-            return np.NaN, np.NaN, np.NaN
+            return np.nan, np.nan, np.nan
 
         sptim = self._parse_time_line(self.f.readline())
         if sptim is None:
             print("error parsing sptim for ts,sp", ts, sp)
-            return np.NaN, np.NaN, np.NaN
+            return np.nan, np.nan, np.nan
 
         totim = self._parse_time_line(self.f.readline())
         if totim is None:
             print("error parsing totim for ts,sp", ts, sp)
-            return np.NaN, np.NaN, np.NaN
+            return np.nan, np.nan, np.nan
         return tslen, sptim, totim
 
     def _parse_time_line(self, line):
         if line == "":
             print("end of file found while parsing time information")
             return None
         try:
```

### Comparing `flopy-3.6.0/flopy/utils/mfreadnam.py` & `flopy-3.7.0/flopy/utils/mfreadnam.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/utils/mtlistfile.py` & `flopy-3.7.0/flopy/utils/mtlistfile.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/utils/observationfile.py` & `flopy-3.7.0/flopy/utils/observationfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     def get_nobs(self):
         """
         Get the number of observations in the file
 
         Returns
         ----------
         out : tuple of int
-            A tupe with the number of records and number of flow items
+            A tuple with the number of records and number of flow items
             in the file. The number of flow items is non-zero only if
             swrtype='flow'.
 
         """
         return self.nobs
 
     def get_obsnames(self):
```

### Comparing `flopy-3.6.0/flopy/utils/optionblock.py` & `flopy-3.7.0/flopy/utils/optionblock.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import warnings
+
 import numpy as np
 
 from ..utils import flopy_io
 
 
 class OptionBlock:
     """
@@ -45,21 +47,30 @@
     )
 
     def __init__(self, options_line, package, block=True):
         self._context = package._options
         self._attr_types = {}
         self.options_line = options_line
         self.package = package
-        self.auxillary = []
+        self.auxiliary = []
         self.noprint = False
         self.block = block
 
         self.__build_attr_types()
         self._set_attributes()
 
+    def __getattr__(self, key):
+        if key == "auxillary":  # catch typo from older version
+            key = "auxiliary"
+            warnings.warn(
+                "the atttribute 'auxillary' is deprecated, use 'auxiliary' instead",
+                category=DeprecationWarning,
+            )
+        return super().__getattribute__(key)
+
     @property
     def single_line_options(self):
         """
         Method to get the single line representation of the
         Options Block
 
         Returns
@@ -140,20 +151,27 @@
         """
         Syntactic sugar to allow for dynamic recarray/attribute
         interactions and data type enforcement on dynamic attributes
 
         Parameters
         ----------
             key : str
-                string refering to an attribute
+                string referring to an attribute
             value : object
                 a python object (int, str, float, bool) that
-                is consistant with the attribute data type
+                is consistent with the attribute data type
 
         """
+        if key == "auxillary":  # catch typo from older version
+            key = "auxiliary"
+            warnings.warn(
+                "the atttribute 'auxillary' is deprecated, use 'auxiliary' instead",
+                category=DeprecationWarning,
+            )
+
         err_msg = "Data type must be compatible with {}"
         if key in ("_context", "_attr_types", "options_line"):
             self.__dict__[key] = value
 
         elif value is None:
             super().__setattr__(key, value)
 
@@ -219,15 +237,15 @@
 
         return value
 
     def __build_attr_types(self):
         """
         Method to build a type dictionary for type
         enforcements in __setattr__. This uses the package's
-        contex tree to build and enforce attribute
+        context tree to build and enforce attribute
         types for the class
 
         """
         for key, value in self._context.items():
             self._attr_types[key] = value[OptionBlock.dtype]
             if OptionBlock.vars in value:
                 for k, d in value[OptionBlock.vars].items():
```

### Comparing `flopy-3.6.0/flopy/utils/parse_version.py` & `flopy-3.7.0/flopy/utils/parse_version.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/utils/postprocessing.py` & `flopy-3.7.0/flopy/utils/postprocessing.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/utils/rasters.py` & `flopy-3.7.0/flopy/utils/rasters.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     --------
     >>> from flopy.utils import Raster
     >>>
     >>> rio = Raster.load("myraster.tif")
 
     """
 
-    FLOAT32 = (float, np.float32, np.float_)
+    FLOAT32 = (float, np.float32, np.float64)
     FLOAT64 = (np.float64,)
     INT8 = (np.int8, np.uint8)
     INT16 = (np.int16, np.uint16)
     INT32 = (int, np.int32, np.uint32, np.uint, np.uintc, np.uint32)
     INT64 = (np.int64, np.uint64)
 
     def __init__(
@@ -684,15 +684,15 @@
 
         return mask
 
     def get_array(self, band, masked=True):
         """
         Method to get a numpy array corresponding to the
         provided raster band. Nodata vals are set to
-        np.NaN
+        np.nan
 
         Parameters
         ----------
         band : int
             band number from the raster
         masked : bool
             determines if nodatavals will be returned as np.nan to
```

### Comparing `flopy-3.6.0/flopy/utils/recarray_utils.py` & `flopy-3.7.0/flopy/utils/recarray_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
               dtype=[('x', '<f4'), ('y', '<f4')])
     """
     r = np.zeros(length, dtype=dtype)
     msg = "dtype argument must be an instance of np.dtype, not list."
     assert isinstance(dtype, np.dtype), msg
     for name in dtype.names:
         dt = dtype.fields[name][0]
-        if np.issubdtype(dt, np.float_):
+        if np.issubdtype(dt, np.float64):
             r[name] = default_value
     return r.view(np.recarray)
 
 
 def ra_slice(ra, cols):
     """
     Create a slice of a recarray
```

### Comparing `flopy-3.6.0/flopy/utils/reference.py` & `flopy-3.7.0/flopy/utils/reference.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/utils/sfroutputfile.py` & `flopy-3.7.0/flopy/utils/sfroutputfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
         -------
         df : pandas dataframe
             SFR output as a pandas dataframe
 
         """
         kwargs = {
             "filepath_or_buffer": self.filename,
-            "delim_whitespace": True,
+            "sep": "\\s+",
             "header": None,
             "names": self.names,
             "skiprows": self.sr,
             "low_memory": False,
         }
         df = pd.read_csv(**kwargs, on_bad_lines="skip")
```

### Comparing `flopy-3.6.0/flopy/utils/swroutputfile.py` & `flopy-3.7.0/flopy/utils/swroutputfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
     def get_nrecords(self):
         """
         Get the number of records in the file
 
         Returns
         ----------
         out : tuple of int
-            A tupe with the number of records and number of flow items
+            A tuple with the number of records and number of flow items
             in the file. The number of flow items is non-zero only if
             swrtype='flow'.
 
         """
         return self.nrecord, self.flowitems
 
     def get_kswrkstpkper(self):
```

### Comparing `flopy-3.6.0/flopy/utils/triangle.py` & `flopy-3.7.0/flopy/utils/triangle.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/utils/util_array.py` & `flopy-3.7.0/flopy/utils/util_array.py`

 * *Files 0% similar despite different names*

```diff
@@ -484,15 +484,15 @@
     ext_filename : string
         the external filename to write the array representation to
         (optional) (the default is None) .
         If type(value) is a string and is an accessible filename, the
         ext_filename is reset to value.
     bin : bool
         flag to control writing external arrays as binary (optional)
-        (the defaut is False)
+        (the default is False)
 
     Attributes
     ----------
     array : np.ndarray
         the array representation of the 3-D object
 
 
@@ -1401,15 +1401,15 @@
         dict(name: (masked) 4d numpy.ndarray
         Parameters
         ----------
             model : flopy.mbase derived type
             pak_name : str package name (e.g. RCH)
             m4ds : dict(name,(masked) 4d numpy.ndarray)
                 each ndarray must have shape (nper,1,nrow,ncol).
-                if an entire (nrow,ncol) slice is np.NaN, then
+                if an entire (nrow,ncol) slice is np.nan, then
                 that kper is skipped.
         Returns
         -------
             Transient2d instance
         """
 
         assert isinstance(m4ds, dict)
@@ -2387,15 +2387,15 @@
         get the string representation of value attribute
 
         Note:
             the string representation DOES NOT include the effects of the control
             record multiplier - this method is used primarily for writing model input files
 
         """
-        # convert array to sting with specified format
+        # convert array to string with specified format
         a_string = self.array2string(
             self.shape, self._array, python_format=self.format.py
         )
         return a_string
 
     @property
     def array(self):
```

### Comparing `flopy-3.6.0/flopy/utils/util_list.py` & `flopy-3.7.0/flopy/utils/util_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,14 +292,24 @@
                 )
         if use_free:
             fmt_string = " " + " ".join(fmts)
         else:
             fmt_string = "".join(fmts)
         return fmt_string
 
+    def __cast_tabular(self, data):
+        data = pd.DataFrame(data)
+        if "kper" in data.dtypes:
+            groups = data.groupby("kper")
+            data = {kper: group.drop("kper", axis=1) for kper, group in groups}
+            for kper, d in data.items():
+                self.__cast_dataframe(kper, d)
+        else:
+            self.__cast_dataframe(0, data)
+
     # Private method to cast the data argument
     # Should only be called by the constructor
     def __cast_data(self, data):
         # If data is a list, then all we can do is try to cast it to
         # an ndarray, then cast again to a recarray
         if isinstance(data, list):
             # warnings.warn("MfList casting list to array")
@@ -346,23 +356,26 @@
                     self.__vtype[kper] = None
                 else:
                     raise ValueError(
                         "MfList error: unsupported data type: "
                         f"{type(d)} at kper {kper}"
                     )
 
-        # A single recarray - same MfList for all stress periods
+        # A single dataframe
+        elif isinstance(data, pd.DataFrame):
+            self.__cast_tabular(data)
+
+        # A single recarray
         elif isinstance(data, np.recarray):
-            self.__cast_recarray(0, data)
+            self.__cast_tabular(data)
+
         # A single ndarray
         elif isinstance(data, np.ndarray):
             self.__cast_ndarray(0, data)
-        # A single dataframe
-        elif isinstance(data, pd.DataFrame):
-            self.__cast_dataframe(0, data)
+
         # A single filename
         elif isinstance(data, str):
             self.__cast_str(0, data)
         else:
             raise ValueError(
                 f"MfList error: unsupported data type: {type(data)}"
             )
@@ -413,15 +426,17 @@
         except Exception as e:
             raise ValueError(
                 f"MfList error: casting ndarray to recarray: {e!s}"
             )
         self.__vtype[kper] = np.recarray
 
     def __cast_dataframe(self, kper, d):
-        self.__cast_recarray(kper, d.to_records(index=False))
+        self.__cast_recarray(
+            kper, d.to_records(index=False).astype(self.dtype)
+        )
 
     def get_dataframe(self, squeeze=False):
         """
         Cast recarrays for stress periods into single
         dataframe containing all stress periods.
 
         Parameters
@@ -1024,15 +1039,15 @@
         specified stress period to a 3-D numpy array
 
         Parameters
         ----------
         kper : int
             MODFLOW zero-based stress period number to return. (default is zero)
         mask : boolean
-            return array with np.NaN instead of zero
+            return array with np.nan instead of zero
         Returns
         ----------
         out : dict of numpy.ndarrays
             Dictionary of 3-D numpy arrays containing the stress period data for
             a selected stress period. The dictionary keys are the MfList dtype
             names for the stress period data ('cond', 'flux', 'bhead', etc.).
 
@@ -1075,30 +1090,30 @@
             kpers = list(self.data.keys())
             kpers.sort()
             # if this kper is before the first entry,
             # (maybe) mask and return
             if kper < kpers[0]:
                 if mask:
                     for name, arr in arrays.items():
-                        arrays[name][:] = np.NaN
+                        arrays[name][:] = np.nan
                 return arrays
             # find the last kper
             else:
                 kper = self.__find_last_kper(kper)
 
         sarr = self.data[kper]
         if isinstance(sarr, str):
             sarr = self.__fromfile(sarr)
 
         if np.isscalar(sarr):
             # if there are no entries for this kper
             if sarr == 0:
                 if mask:
                     for name, arr in arrays.items():
-                        arrays[name][:] = np.NaN
+                        arrays[name][:] = np.nan
                 return arrays
             raise ValueError(
                 f"MfList: expected no entries for period {kper} but found {sarr}"
             )
 
         for name, arr in arrays.items():
             if unstructured:
@@ -1120,20 +1135,20 @@
                     cnt[rec["k"], rec["i"], rec["j"]] += 1.0
             # average keys that should not be added
             if name not in ("cond", "flux"):
                 idx = cnt > 0.0
                 arr[idx] /= cnt[idx]
             if mask:
                 arr = np.ma.masked_where(cnt == 0.0, arr)
-                arr[cnt == 0.0] = np.NaN
+                arr[cnt == 0.0] = np.nan
 
             arrays[name] = arr.copy()
         # elif mask:
         #     for name, arr in arrays.items():
-        #         arrays[name][:] = np.NaN
+        #         arrays[name][:] = np.nan
         return arrays
 
     @property
     def masked_4D_arrays(self):
         # get the first kper
         arrays = self.to_array(kper=0, mask=True)
```

### Comparing `flopy-3.6.0/flopy/utils/utils_def.py` & `flopy-3.7.0/flopy/utils/utils_def.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/utils/utl_import.py` & `flopy-3.7.0/flopy/utils/utl_import.py`

 * *Files identical despite different names*

### Comparing `flopy-3.6.0/flopy/utils/voronoi.py` & `flopy-3.7.0/flopy/utils/voronoi.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,15 +254,15 @@
     an array of input points that define cell centers.  The class handles
     boundary cells by closing polygons along the edge, something that cannot
     be done directly with the scipy.spatial.Voronoi class.
 
     Parameters
     ----------
     input : flopy.utils.Triangle
-        Constructred and built flopy Triangle object.
+        Constructed and built flopy Triangle object.
     kwargs : dict
         List of additional keyword arguments that will be passed through to
         scipy.spatial.Voronoi.  For circular shaped model grids, the
         qhull_options='Qz' option has been found to work well.
 
     Notes
     -----
@@ -364,15 +364,15 @@
         Get a matplotlib patch collection representation of the voronoi grid
 
         Parameters
         ----------
         ax : matplotlib.pyplot.Axes
             axes to plot the patch collection
         kwargs : dict
-            Additional keyward arguments to pass to the flopy.plot.plot_cvfd
+            Additional keyword arguments to pass to the flopy.plot.plot_cvfd
             function that returns a patch collection from verts and iverts
 
         Returns
         -------
         pc : matplotlib.collections.PatchCollection
             patch collection of model
```

### Comparing `flopy-3.6.0/flopy/utils/zonbud.py` & `flopy-3.7.0/flopy/utils/zonbud.py`

 * *Files 1% similar despite different names*

```diff
@@ -607,27 +607,27 @@
                 # Define the zone from which flow is coming
                 jl = j - 1
                 nzl = self.izone[k, i, jl]
 
                 # Get the face flow
                 q = data[k, i, jl]
 
-                # Get indices where flow face values are positive (flow out of higher zone)
+                # Get indices with positive flow face values (out of higher zone)
                 # Don't include CH to CH flow (can occur if CHTOCH option is used)
                 # Create an iterable tuple of (from zone, to zone, flux)
                 # Then group tuple by (from_zone, to_zone) and sum the flux values
                 idx = np.where(
                     (q > 0) & ((ich[k, i, j] != 1) | (ich[k, i, jl] != 1))
                 )
                 fzi, tzi, fi = sum_flux_tuples(nzl[idx], nz[idx], q[idx])
                 self._update_budget_fromfaceflow(
                     fzi, tzi, np.abs(fi), kstpkper, totim
                 )
 
-                # Get indices where flow face values are negative (flow into higher zone)
+                # Get indices with negative flow face values (into higher zone)
                 # Don't include CH to CH flow (can occur if CHTOCH option is used)
                 # Create an iterable tuple of (from zone, to zone, flux)
                 # Then group tuple by (from_zone, to_zone) and sum the flux values
                 idx = np.where(
                     (q < 0) & ((ich[k, i, j] != 1) | (ich[k, i, jl] != 1))
                 )
                 fzi, tzi, fi = sum_flux_tuples(nz[idx], nzl[idx], q[idx])
@@ -646,27 +646,27 @@
                 # Define the zone to which flow is going
                 jr = j + 1
                 nzr = self.izone[k, i, jr]
 
                 # Get the face flow
                 q = data[k, i, j]
 
-                # Get indices where flow face values are positive (flow out of higher zone)
+                # Get indices with positive flow face values (out of higher zone)
                 # Don't include CH to CH flow (can occur if CHTOCH option is used)
                 # Create an iterable tuple of (from zone, to zone, flux)
                 # Then group tuple by (from_zone, to_zone) and sum the flux values
                 idx = np.where(
                     (q > 0) & ((ich[k, i, j] != 1) | (ich[k, i, jr] != 1))
                 )
                 fzi, tzi, fi = sum_flux_tuples(nz[idx], nzr[idx], q[idx])
                 self._update_budget_fromfaceflow(
                     fzi, tzi, np.abs(fi), kstpkper, totim
                 )
 
-                # Get indices where flow face values are negative (flow into higher zone)
+                # Get indices with negative flow face values (into higher zone)
                 # Don't include CH to CH flow (can occur if CHTOCH option is used)
                 # Create an iterable tuple of (from zone, to zone, flux)
                 # Then group tuple by (from_zone, to_zone) and sum the flux values
                 idx = np.where(
                     (q < 0) & ((ich[k, i, j] != 1) | (ich[k, i, jr] != 1))
                 )
                 fzi, tzi, fi = sum_flux_tuples(nzr[idx], nz[idx], q[idx])
@@ -1376,15 +1376,15 @@
             if "zonebudget version" in line.lower():
                 otype = 0
             elif "time step" in line.lower():
                 otype = 1
             elif "totim" in line.lower():
                 otype = 2
             else:
-                raise AssertionError("Cant distinguish output type")
+                raise AssertionError("Can't distinguish output type")
         return otype
 
     @classmethod
     def read_output(cls, fname, net=False, dataframe=False, **kwargs):
         """
         Method to read a zonebudget output file into a recarray or pandas
         dataframe
@@ -1770,15 +1770,15 @@
     Parameters
     ----------
     name : str
         model name for zonebudget
     model_ws : str
         path to model
     exe_name : str
-        excutable name
+        executable name
     extension : str
         name file extension
     """
 
     def __init__(
         self,
         name="zonebud",
```

### Comparing `flopy-3.6.0/flopy.egg-info/PKG-INFO` & `flopy-3.7.0/flopy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flopy
-Version: 3.6.0
+Version: 3.7.0
 Summary: FloPy is a Python package to create, run, and post-process MODFLOW-based models
 Author-email: FloPy Team <modflow@usgs.gov>
 Maintainer-email: "Joseph D. Hughes" <jdhughes@usgs.gov>
 License: CC0
 Project-URL: Documentation, https://flopy.readthedocs.io
 Project-URL: Release Notes, https://github.com/modflowpy/flopy/blob/develop/docs/version_changes.md
 Project-URL: Bug Tracker, https://github.com/modflowpy/flopy/issues
@@ -25,32 +25,31 @@
 License-File: LICENSE.md
 Requires-Dist: numpy<2.0.0,>=1.15.0
 Requires-Dist: matplotlib>=1.4.0
 Requires-Dist: pandas>=2.0.0
 Provides-Extra: dev
 Requires-Dist: flopy[doc,lint,optional,test]; extra == "dev"
 Provides-Extra: lint
-Requires-Dist: black; extra == "lint"
 Requires-Dist: cffconvert; extra == "lint"
-Requires-Dist: flake8; extra == "lint"
-Requires-Dist: isort; extra == "lint"
-Requires-Dist: pylint; extra == "lint"
+Requires-Dist: ruff; extra == "lint"
 Provides-Extra: test
 Requires-Dist: flopy[lint]; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: flaky; extra == "test"
 Requires-Dist: filelock; extra == "test"
 Requires-Dist: jupyter; extra == "test"
 Requires-Dist: jupytext; extra == "test"
 Requires-Dist: modflow-devtools; extra == "test"
-Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest!=8.1.0; extra == "test"
 Requires-Dist: pytest-benchmark; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-dotenv; extra == "test"
 Requires-Dist: pytest-xdist; extra == "test"
+Requires-Dist: pyzmq>=25.1.2; extra == "test"
+Requires-Dist: syrupy; extra == "test"
 Requires-Dist: virtualenv; extra == "test"
 Provides-Extra: optional
 Requires-Dist: affine; extra == "optional"
 Requires-Dist: descartes; extra == "optional"
 Requires-Dist: fiona; extra == "optional"
 Requires-Dist: geojson; extra == "optional"
 Requires-Dist: geopandas; extra == "optional"
@@ -106,15 +105,15 @@
 
 *Citation for FloPy:*
 
 [Bakker, Mark, Post, Vincent, Langevin, C. D., Hughes, J. D., White, J. T., Starn, J. J. and Fienen, M. N., 2016, Scripting MODFLOW Model Development Using Python and FloPy: Groundwater, v. 54, p. 733–739, doi:10.1111/gwat.12413.](https://doi.org/10.1111/gwat.12413)
 
 *Software/Code citation for FloPy:*
 
-[Bakker, Mark, Post, Vincent, Hughes, J. D., Langevin, C. D., White, J. T., Leaf, A. T., Paulinski, S. R., Bellino, J. C., Morway, E. D., Toews, M. W., Larsen, J. D., Fienen, M. N., Starn, J. J., Brakenhoff, D. A., and Bonelli, W. P., 2024, FloPy v3.6.0: U.S. Geological Survey Software Release, 08 February 2024, https://doi.org/10.5066/F7BK19FH](https://doi.org/10.5066/F7BK19FH)
+[Bakker, Mark, Post, Vincent, Hughes, J. D., Langevin, C. D., White, J. T., Leaf, A. T., Paulinski, S. R., Bellino, J. C., Morway, E. D., Toews, M. W., Larsen, J. D., Fienen, M. N., Starn, J. J., Brakenhoff, D. A., and Bonelli, W. P., 2024, FloPy v3.7.0: U.S. Geological Survey Software Release, 23 May 2024, https://doi.org/10.5066/F7BK19FH](https://doi.org/10.5066/F7BK19FH)
 
 
 Disclaimer
 ----------
 
 This software is provided "as is" and "as-available", and makes no 
 representations or warranties of any kind concerning the software, whether
```

### Comparing `flopy-3.6.0/flopy.egg-info/SOURCES.txt` & `flopy-3.7.0/flopy.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -51,18 +51,39 @@
 flopy/mf6/data/mfdataplist.py
 flopy/mf6/data/mfdatascalar.py
 flopy/mf6/data/mfdatastorage.py
 flopy/mf6/data/mfdatautil.py
 flopy/mf6/data/mffileaccess.py
 flopy/mf6/data/mfstructure.py
 flopy/mf6/data/dfn/common.dfn
+flopy/mf6/data/dfn/exg-gwegwe.dfn
+flopy/mf6/data/dfn/exg-gwfgwe.dfn
 flopy/mf6/data/dfn/exg-gwfgwf.dfn
 flopy/mf6/data/dfn/exg-gwfgwt.dfn
+flopy/mf6/data/dfn/exg-gwfprt.dfn
 flopy/mf6/data/dfn/exg-gwtgwt.dfn
 flopy/mf6/data/dfn/flopy.dfn
+flopy/mf6/data/dfn/gwe-adv.dfn
+flopy/mf6/data/dfn/gwe-cnd.dfn
+flopy/mf6/data/dfn/gwe-ctp.dfn
+flopy/mf6/data/dfn/gwe-dis.dfn
+flopy/mf6/data/dfn/gwe-disu.dfn
+flopy/mf6/data/dfn/gwe-disv.dfn
+flopy/mf6/data/dfn/gwe-esl.dfn
+flopy/mf6/data/dfn/gwe-est.dfn
+flopy/mf6/data/dfn/gwe-fmi.dfn
+flopy/mf6/data/dfn/gwe-ic.dfn
+flopy/mf6/data/dfn/gwe-lke.dfn
+flopy/mf6/data/dfn/gwe-mve.dfn
+flopy/mf6/data/dfn/gwe-mwe.dfn
+flopy/mf6/data/dfn/gwe-nam.dfn
+flopy/mf6/data/dfn/gwe-oc.dfn
+flopy/mf6/data/dfn/gwe-sfe.dfn
+flopy/mf6/data/dfn/gwe-ssm.dfn
+flopy/mf6/data/dfn/gwe-uze.dfn
 flopy/mf6/data/dfn/gwf-api.dfn
 flopy/mf6/data/dfn/gwf-buy.dfn
 flopy/mf6/data/dfn/gwf-chd.dfn
 flopy/mf6/data/dfn/gwf-csub.dfn
 flopy/mf6/data/dfn/gwf-dis.dfn
 flopy/mf6/data/dfn/gwf-disu.dfn
 flopy/mf6/data/dfn/gwf-disv.dfn
@@ -103,54 +124,87 @@
 flopy/mf6/data/dfn/gwt-mwt.dfn
 flopy/mf6/data/dfn/gwt-nam.dfn
 flopy/mf6/data/dfn/gwt-oc.dfn
 flopy/mf6/data/dfn/gwt-sft.dfn
 flopy/mf6/data/dfn/gwt-src.dfn
 flopy/mf6/data/dfn/gwt-ssm.dfn
 flopy/mf6/data/dfn/gwt-uzt.dfn
+flopy/mf6/data/dfn/prt-dis.dfn
+flopy/mf6/data/dfn/prt-disv.dfn
+flopy/mf6/data/dfn/prt-fmi.dfn
+flopy/mf6/data/dfn/prt-mip.dfn
+flopy/mf6/data/dfn/prt-nam.dfn
+flopy/mf6/data/dfn/prt-oc.dfn
+flopy/mf6/data/dfn/prt-prp.dfn
 flopy/mf6/data/dfn/sim-nam.dfn
 flopy/mf6/data/dfn/sim-tdis.dfn
 flopy/mf6/data/dfn/sln-ems.dfn
 flopy/mf6/data/dfn/sln-ims.dfn
+flopy/mf6/data/dfn/sln-pts.dfn
 flopy/mf6/data/dfn/utl-ats.dfn
+flopy/mf6/data/dfn/utl-hpc.dfn
 flopy/mf6/data/dfn/utl-laktab.dfn
 flopy/mf6/data/dfn/utl-obs.dfn
 flopy/mf6/data/dfn/utl-sfrtab.dfn
 flopy/mf6/data/dfn/utl-spc.dfn
 flopy/mf6/data/dfn/utl-spca.dfn
+flopy/mf6/data/dfn/utl-spt.dfn
+flopy/mf6/data/dfn/utl-spta.dfn
 flopy/mf6/data/dfn/utl-tas.dfn
 flopy/mf6/data/dfn/utl-ts.dfn
 flopy/mf6/data/dfn/utl-tvk.dfn
 flopy/mf6/data/dfn/utl-tvs.dfn
 flopy/mf6/modflow/__init__.py
 flopy/mf6/modflow/mfems.py
 flopy/mf6/modflow/mfgnc.py
+flopy/mf6/modflow/mfgwe.py
+flopy/mf6/modflow/mfgweadv.py
+flopy/mf6/modflow/mfgwecnd.py
+flopy/mf6/modflow/mfgwectp.py
+flopy/mf6/modflow/mfgwedis.py
+flopy/mf6/modflow/mfgwedisu.py
+flopy/mf6/modflow/mfgwedisv.py
+flopy/mf6/modflow/mfgweesl.py
+flopy/mf6/modflow/mfgweest.py
+flopy/mf6/modflow/mfgwefmi.py
+flopy/mf6/modflow/mfgwegwe.py
+flopy/mf6/modflow/mfgweic.py
+flopy/mf6/modflow/mfgwelke.py
+flopy/mf6/modflow/mfgwemve.py
+flopy/mf6/modflow/mfgwemwe.py
+flopy/mf6/modflow/mfgwenam.py
+flopy/mf6/modflow/mfgweoc.py
+flopy/mf6/modflow/mfgwesfe.py
+flopy/mf6/modflow/mfgwessm.py
+flopy/mf6/modflow/mfgweuze.py
 flopy/mf6/modflow/mfgwf.py
 flopy/mf6/modflow/mfgwfapi.py
 flopy/mf6/modflow/mfgwfbuy.py
 flopy/mf6/modflow/mfgwfchd.py
 flopy/mf6/modflow/mfgwfcsub.py
 flopy/mf6/modflow/mfgwfdis.py
 flopy/mf6/modflow/mfgwfdisu.py
 flopy/mf6/modflow/mfgwfdisv.py
 flopy/mf6/modflow/mfgwfdrn.py
 flopy/mf6/modflow/mfgwfevt.py
 flopy/mf6/modflow/mfgwfevta.py
 flopy/mf6/modflow/mfgwfghb.py
 flopy/mf6/modflow/mfgwfgnc.py
+flopy/mf6/modflow/mfgwfgwe.py
 flopy/mf6/modflow/mfgwfgwf.py
 flopy/mf6/modflow/mfgwfgwt.py
 flopy/mf6/modflow/mfgwfhfb.py
 flopy/mf6/modflow/mfgwfic.py
 flopy/mf6/modflow/mfgwflak.py
 flopy/mf6/modflow/mfgwfmaw.py
 flopy/mf6/modflow/mfgwfmvr.py
 flopy/mf6/modflow/mfgwfnam.py
 flopy/mf6/modflow/mfgwfnpf.py
 flopy/mf6/modflow/mfgwfoc.py
+flopy/mf6/modflow/mfgwfprt.py
 flopy/mf6/modflow/mfgwfrch.py
 flopy/mf6/modflow/mfgwfrcha.py
 flopy/mf6/modflow/mfgwfriv.py
 flopy/mf6/modflow/mfgwfsfr.py
 flopy/mf6/modflow/mfgwfsto.py
 flopy/mf6/modflow/mfgwfuzf.py
 flopy/mf6/modflow/mfgwfvsc.py
@@ -177,22 +231,34 @@
 flopy/mf6/modflow/mfgwtsrc.py
 flopy/mf6/modflow/mfgwtssm.py
 flopy/mf6/modflow/mfgwtuzt.py
 flopy/mf6/modflow/mfims.py
 flopy/mf6/modflow/mfmvr.py
 flopy/mf6/modflow/mfmvt.py
 flopy/mf6/modflow/mfnam.py
+flopy/mf6/modflow/mfprt.py
+flopy/mf6/modflow/mfprtdis.py
+flopy/mf6/modflow/mfprtdisv.py
+flopy/mf6/modflow/mfprtfmi.py
+flopy/mf6/modflow/mfprtmip.py
+flopy/mf6/modflow/mfprtnam.py
+flopy/mf6/modflow/mfprtoc.py
+flopy/mf6/modflow/mfprtprp.py
+flopy/mf6/modflow/mfpts.py
 flopy/mf6/modflow/mfsimulation.py
 flopy/mf6/modflow/mftdis.py
 flopy/mf6/modflow/mfutlats.py
+flopy/mf6/modflow/mfutlhpc.py
 flopy/mf6/modflow/mfutllaktab.py
 flopy/mf6/modflow/mfutlobs.py
 flopy/mf6/modflow/mfutlsfrtab.py
 flopy/mf6/modflow/mfutlspc.py
 flopy/mf6/modflow/mfutlspca.py
+flopy/mf6/modflow/mfutlspt.py
+flopy/mf6/modflow/mfutlspta.py
 flopy/mf6/modflow/mfutltas.py
 flopy/mf6/modflow/mfutlts.py
 flopy/mf6/modflow/mfutltvk.py
 flopy/mf6/modflow/mfutltvs.py
 flopy/mf6/utils/__init__.py
 flopy/mf6/utils/binaryfile_utils.py
 flopy/mf6/utils/binarygrid_util.py
@@ -299,17 +365,15 @@
 flopy/pest/tplarray.py
 flopy/plot/__init__.py
 flopy/plot/crosssection.py
 flopy/plot/map.py
 flopy/plot/plotutil.py
 flopy/plot/styles.py
 flopy/plot/mplstyle/usgsmap.mplstyle
-flopy/plot/mplstyle/usgsmap_linux.mplstyle
 flopy/plot/mplstyle/usgsplot.mplstyle
-flopy/plot/mplstyle/usgsplot_linux.mplstyle
 flopy/seawat/__init__.py
 flopy/seawat/swt.py
 flopy/seawat/swtvdf.py
 flopy/seawat/swtvsc.py
 flopy/utils/__init__.py
 flopy/utils/binaryfile.py
 flopy/utils/check.py
@@ -330,14 +394,15 @@
 flopy/utils/mflistfile.py
 flopy/utils/mfreadnam.py
 flopy/utils/modpathfile.py
 flopy/utils/mtlistfile.py
 flopy/utils/observationfile.py
 flopy/utils/optionblock.py
 flopy/utils/parse_version.py
+flopy/utils/particletrackfile.py
 flopy/utils/postprocessing.py
 flopy/utils/rasters.py
 flopy/utils/recarray_utils.py
 flopy/utils/reference.py
 flopy/utils/sfroutputfile.py
 flopy/utils/swroutputfile.py
 flopy/utils/triangle.py
```

### Comparing `flopy-3.6.0/flopy.egg-info/requires.txt` & `flopy-3.7.0/flopy.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -14,19 +14,16 @@
 nbsphinx
 PyYAML
 rtds-action
 sphinx==7.1.2
 sphinx-rtd-theme>=1
 
 [lint]
-black
 cffconvert
-flake8
-isort
-pylint
+ruff
 
 [optional]
 affine
 descartes
 fiona
 geojson
 geopandas
@@ -49,13 +46,15 @@
 flopy[lint]
 coverage
 flaky
 filelock
 jupyter
 jupytext
 modflow-devtools
-pytest
+pytest!=8.1.0
 pytest-benchmark
 pytest-cov
 pytest-dotenv
 pytest-xdist
+pyzmq>=25.1.2
+syrupy
 virtualenv
```

### Comparing `flopy-3.6.0/pyproject.toml` & `flopy-3.7.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -34,33 +34,32 @@
     "pandas >=2.0.0"
 ]
 dynamic = ["version", "readme"]
 
 [project.optional-dependencies]
 dev = ["flopy[lint,test,optional,doc]"]
 lint = [
-    "black",
     "cffconvert",
-    "flake8",
-    "isort",
-    "pylint",
+    "ruff"
 ]
 test = [
     "flopy[lint]",
     "coverage",
     "flaky",
     "filelock",
     "jupyter",
     "jupytext",
     "modflow-devtools",
-    "pytest",
+    "pytest !=8.1.0",
     "pytest-benchmark",
     "pytest-cov",
     "pytest-dotenv",
     "pytest-xdist",
+    "pyzmq >=25.1.2",
+    "syrupy",
     "virtualenv"
 ]
 optional = [
     "affine",
     "descartes",
     "fiona",
     "geojson",
@@ -111,15 +110,37 @@
 [tool.setuptools.packages.find]
 include = ["flopy", "flopy.*"]
 
 [tool.setuptools.package-data]
 "flopy.mf6.data" = ["dfn/*.dfn"]
 "flopy.plot" = ["mplstyle/*.mplstyle"]
 
-[tool.black]
+[tool.ruff]
 line-length = 79
-target_version = ["py38"]
+target-version = "py38"
+include = [
+    "pyproject.toml",
+    "flopy/**/*.py",
+    "autotest/**/*.py",
+    "examples/**/*.py",
+    "scripts/**/*.py",
+    ".docs/**/*.py",
+]
+extend-include = [
+    "examples/**/*.ipynb"
+]
 
-[tool.isort]
-profile = "black"
-src_paths = ["flopy"]
-line_length = 79
+[tool.ruff.lint]
+select = ["F", "E", "I001"]
+ignore = [
+    "E402", # module level import not at top of file
+    "E501", # line too long TODO FIXME
+    "E712", # Avoid equality comparisons to `True`
+    "E722", # do not use bare `except`
+    "E741", # ambiguous variable name
+    "F401", # unused import
+    "F403", # unable to detect undefined names (star imports)
+    "F524", # `.format` missing argument(s) for placeholder(s)
+    "F811", # Redefinition of unused variable
+    "F821", # undefined name TODO FIXME
+    "F841", # local variable assigned but never used
+]
```

