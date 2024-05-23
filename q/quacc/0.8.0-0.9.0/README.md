# Comparing `tmp/quacc-0.8.0.tar.gz` & `tmp/quacc-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quacc-0.8.0.tar", last modified: Sun May 12 22:33:18 2024, max compression
+gzip compressed data, was "quacc-0.9.0.tar", last modified: Thu May 23 21:18:29 2024, max compression
```

## Comparing `quacc-0.8.0.tar` & `quacc-0.9.0.tar`

### file list

```diff
@@ -1,177 +1,177 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.435920 quacc-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-12 22:31:57.000000 quacc-0.8.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-12 22:31:57.000000 quacc-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-05-12 22:33:18.435920 quacc-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-12 22:31:57.000000 quacc-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-12 22:31:57.000000 quacc-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 22:33:18.435920 quacc-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.403920 quacc-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.407920 quacc-0.8.0/src/quacc/
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.407920 quacc-0.8.0/src/quacc/_cli/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/_cli/quacc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.411920 quacc-0.8.0/src/quacc/atoms/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/atoms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/atoms/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/atoms/defects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/atoms/deformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/atoms/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/atoms/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.411920 quacc-0.8.0/src/quacc/calculators/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.411920 quacc-0.8.0/src/quacc/calculators/espresso/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/espresso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17294 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/espresso/espresso.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.411920 quacc-0.8.0/src/quacc/calculators/espresso/presets/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/espresso/presets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/espresso/presets/esm_metal_slab_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/espresso/presets/esm_metal_slab_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/espresso/presets/metal_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/espresso/presets/metal_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/espresso/presets/molecule_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/espresso/presets/semiconductors_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/espresso/presets/semiconductors_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/espresso/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.415920 quacc-0.8.0/src/quacc/calculators/qchem/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/qchem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/qchem/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/qchem/params.py
--rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/qchem/qchem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/qchem/qchem_custodian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.415920 quacc-0.8.0/src/quacc/calculators/vasp/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/vasp/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    14869 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/vasp/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.415920 quacc-0.8.0/src/quacc/calculators/vasp/presets/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/vasp/presets/BulkSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/vasp/presets/QMOFSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/vasp/presets/SlabSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/vasp/presets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/vasp/presets/magmoms_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/vasp/presets/setups_pbe54.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/vasp/presets/setups_qmof.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/vasp/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/vasp/vasp_custodian.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.415920 quacc-0.8.0/src/quacc/recipes/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.415920 quacc-0.8.0/src/quacc/recipes/common/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/common/defects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/common/elastic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/common/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/common/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.419920 quacc-0.8.0/src/quacc/recipes/dftb/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/dftb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/dftb/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/dftb/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.419920 quacc-0.8.0/src/quacc/recipes/emt/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/emt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/emt/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/emt/defects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/emt/elastic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/emt/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/emt/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.419920 quacc-0.8.0/src/quacc/recipes/espresso/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/espresso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/espresso/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13160 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/espresso/bands.py
--rw-r--r--   0 runner    (1001) docker     (127)    15333 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/espresso/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/espresso/dos.py
--rw-r--r--   0 runner    (1001) docker     (127)    24396 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/espresso/phonons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.419920 quacc-0.8.0/src/quacc/recipes/gaussian/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/gaussian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/gaussian/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/gaussian/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.419920 quacc-0.8.0/src/quacc/recipes/gulp/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/gulp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/gulp/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/gulp/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.419920 quacc-0.8.0/src/quacc/recipes/lj/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/lj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/lj/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.423920 quacc-0.8.0/src/quacc/recipes/mlp/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/mlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/mlp/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/mlp/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/mlp/phonons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.423920 quacc-0.8.0/src/quacc/recipes/newtonnet/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/newtonnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7243 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/newtonnet/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9109 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/newtonnet/ts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.423920 quacc-0.8.0/src/quacc/recipes/onetep/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/onetep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/onetep/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/onetep/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.423920 quacc-0.8.0/src/quacc/recipes/orca/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/orca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/orca/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12465 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/orca/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.423920 quacc-0.8.0/src/quacc/recipes/psi4/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/psi4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/psi4/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/psi4/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.423920 quacc-0.8.0/src/quacc/recipes/qchem/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/qchem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/qchem/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/qchem/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/qchem/ts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.427920 quacc-0.8.0/src/quacc/recipes/tblite/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/tblite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/tblite/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/tblite/phonons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.427920 quacc-0.8.0/src/quacc/recipes/vasp/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/vasp/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/vasp/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    12467 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/vasp/mp.py
--rw-r--r--   0 runner    (1001) docker     (127)    10161 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/vasp/qmof.py
--rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/vasp/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.427920 quacc-0.8.0/src/quacc/runners/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12138 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/runners/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/runners/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/runners/prep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/runners/thermo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.427920 quacc-0.8.0/src/quacc/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.431920 quacc-0.8.0/src/quacc/schemas/_aliases/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/schemas/_aliases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/schemas/_aliases/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/schemas/_aliases/atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/schemas/_aliases/cclib.py
--rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/schemas/_aliases/emmet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/schemas/_aliases/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/schemas/_aliases/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)    13456 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/schemas/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/schemas/atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)    17451 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/schemas/cclib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/schemas/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/schemas/prep.py
--rw-r--r--   0 runner    (1001) docker     (127)    12266 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/schemas/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)    17135 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.431920 quacc-0.8.0/src/quacc/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/utils/dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9240 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/utils/kpts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/utils/lists.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.431920 quacc-0.8.0/src/quacc/wflow_tools/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/wflow_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/wflow_tools/customizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/wflow_tools/db.py
--rw-r--r--   0 runner    (1001) docker     (127)    13248 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/wflow_tools/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.431920 quacc-0.8.0/src/quacc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-05-12 22:33:18.000000 quacc-0.8.0/src/quacc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-05-12 22:33:18.000000 quacc-0.8.0/src/quacc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 22:33:18.000000 quacc-0.8.0/src/quacc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-12 22:33:18.000000 quacc-0.8.0/src/quacc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-12 22:33:18.000000 quacc-0.8.0/src/quacc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-12 22:33:18.000000 quacc-0.8.0/src/quacc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.440842 quacc-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-23 21:17:10.000000 quacc-0.9.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-23 21:17:10.000000 quacc-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-05-23 21:18:29.440842 quacc-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-23 21:17:10.000000 quacc-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-05-23 21:17:10.000000 quacc-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 21:18:29.440842 quacc-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.404842 quacc-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.408842 quacc-0.9.0/src/quacc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.412842 quacc-0.9.0/src/quacc/_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/_cli/quacc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.412842 quacc-0.9.0/src/quacc/atoms/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/atoms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/atoms/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/atoms/defects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/atoms/deformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/atoms/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/atoms/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.412842 quacc-0.9.0/src/quacc/calculators/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.412842 quacc-0.9.0/src/quacc/calculators/espresso/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/espresso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17294 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/espresso/espresso.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.416842 quacc-0.9.0/src/quacc/calculators/espresso/presets/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/espresso/presets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/espresso/presets/esm_metal_slab_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/espresso/presets/esm_metal_slab_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/espresso/presets/metal_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/espresso/presets/metal_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/espresso/presets/molecule_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/espresso/presets/semiconductors_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/espresso/presets/semiconductors_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/espresso/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.416842 quacc-0.9.0/src/quacc/calculators/qchem/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/qchem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/qchem/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/qchem/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/qchem/qchem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/qchem/qchem_custodian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.416842 quacc-0.9.0/src/quacc/calculators/vasp/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/vasp/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14869 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/vasp/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.420842 quacc-0.9.0/src/quacc/calculators/vasp/presets/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/vasp/presets/BulkSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/vasp/presets/QMOFSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/vasp/presets/SlabSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/vasp/presets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/vasp/presets/magmoms_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/vasp/presets/setups_pbe54.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/vasp/presets/setups_qmof.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/vasp/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/calculators/vasp/vasp_custodian.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.420842 quacc-0.9.0/src/quacc/recipes/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.420842 quacc-0.9.0/src/quacc/recipes/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/common/defects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/common/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/common/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/common/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.420842 quacc-0.9.0/src/quacc/recipes/dftb/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/dftb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/dftb/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/dftb/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.420842 quacc-0.9.0/src/quacc/recipes/emt/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/emt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/emt/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/emt/defects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/emt/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/emt/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/emt/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.424842 quacc-0.9.0/src/quacc/recipes/espresso/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/espresso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/espresso/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13161 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/espresso/bands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15333 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/espresso/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10208 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/espresso/dos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24148 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/espresso/phonons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.424842 quacc-0.9.0/src/quacc/recipes/gaussian/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/gaussian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/gaussian/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/gaussian/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.424842 quacc-0.9.0/src/quacc/recipes/gulp/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/gulp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/gulp/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/gulp/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.424842 quacc-0.9.0/src/quacc/recipes/lj/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/lj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/lj/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.424842 quacc-0.9.0/src/quacc/recipes/mlp/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/mlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/mlp/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/mlp/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/mlp/phonons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.424842 quacc-0.9.0/src/quacc/recipes/newtonnet/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/newtonnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7243 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/newtonnet/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9109 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/newtonnet/ts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.428842 quacc-0.9.0/src/quacc/recipes/onetep/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/onetep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/onetep/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/onetep/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.428842 quacc-0.9.0/src/quacc/recipes/orca/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/orca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/orca/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12465 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/orca/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.428842 quacc-0.9.0/src/quacc/recipes/psi4/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/psi4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/psi4/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/psi4/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.428842 quacc-0.9.0/src/quacc/recipes/qchem/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/qchem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/qchem/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/qchem/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/qchem/ts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.428842 quacc-0.9.0/src/quacc/recipes/tblite/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/tblite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/tblite/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/tblite/phonons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.428842 quacc-0.9.0/src/quacc/recipes/vasp/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/vasp/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/vasp/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12469 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/vasp/mp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10130 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/vasp/qmof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/recipes/vasp/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.432842 quacc-0.9.0/src/quacc/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12522 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/runners/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/runners/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/runners/prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/runners/thermo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.432842 quacc-0.9.0/src/quacc/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.432842 quacc-0.9.0/src/quacc/schemas/_aliases/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/schemas/_aliases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/schemas/_aliases/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/schemas/_aliases/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/schemas/_aliases/cclib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/schemas/_aliases/emmet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/schemas/_aliases/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/schemas/_aliases/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13451 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/schemas/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/schemas/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17451 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/schemas/cclib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/schemas/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/schemas/prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12266 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/schemas/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16906 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.432842 quacc-0.9.0/src/quacc/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6494 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/utils/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9240 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/utils/kpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/utils/lists.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.436842 quacc-0.9.0/src/quacc/wflow_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/wflow_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/wflow_tools/customizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/wflow_tools/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13248 2024-05-23 21:17:10.000000 quacc-0.9.0/src/quacc/wflow_tools/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:18:29.436842 quacc-0.9.0/src/quacc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-05-23 21:18:29.000000 quacc-0.9.0/src/quacc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-05-23 21:18:29.000000 quacc-0.9.0/src/quacc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 21:18:29.000000 quacc-0.9.0/src/quacc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-23 21:18:29.000000 quacc-0.9.0/src/quacc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-23 21:18:29.000000 quacc-0.9.0/src/quacc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 21:18:29.000000 quacc-0.9.0/src/quacc.egg-info/top_level.txt
```

### Comparing `quacc-0.8.0/LICENSE.md` & `quacc-0.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/PKG-INFO` & `quacc-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quacc
-Version: 0.8.0
+Version: 0.9.0
 Summary: A platform to enable high-throughput, database-driven quantum chemistry and computational materials science
 Author-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 Maintainer-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 License: BSD-3
 Project-URL: repository, https://github.com/Quantum-Accelerators/quacc
 Project-URL: documentation, https://quantum-accelerators.github.io/quacc/
 Project-URL: changelog, https://github.com/Quantum-Accelerators/quacc/blob/main/CHANGELOG.md
@@ -25,15 +25,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: ase>=3.23.0b1
 Requires-Dist: cclib>=1.8
 Requires-Dist: custodian>=2024.3.12
 Requires-Dist: emmet-core>=0.80.0
 Requires-Dist: maggma>=0.64.0
-Requires-Dist: monty>=2024.2.26
+Requires-Dist: monty>=2024.5.15
 Requires-Dist: numpy>=1.25.0
 Requires-Dist: psutil
 Requires-Dist: pydantic>=2.0.1
 Requires-Dist: pydantic-settings>=2.2.0
 Requires-Dist: pymatgen>=2024.4.13
 Requires-Dist: ruamel.yaml>=0.17.40
 Requires-Dist: typer>=0.12.1
@@ -60,21 +60,20 @@
 Requires-Dist: newtonnet>=1.1; extra == "newtonnet"
 Provides-Extra: parsl
 Requires-Dist: parsl[monitoring]>=2023.10.23; platform_system != "Windows" and extra == "parsl"
 Provides-Extra: phonons
 Requires-Dist: phonopy>=2.20.0; extra == "phonons"
 Requires-Dist: seekpath>=2.1.0; extra == "phonons"
 Provides-Extra: prefect
-Requires-Dist: prefect>=2.14.14; extra == "prefect"
-Requires-Dist: prefect-dask>=0.2.6; extra == "prefect"
+Requires-Dist: prefect[dask]>=2.19.0; extra == "prefect"
 Requires-Dist: dask-jobqueue>=0.8.2; extra == "prefect"
 Provides-Extra: redun
 Requires-Dist: redun>=0.16.2; extra == "redun"
 Provides-Extra: sella
-Requires-Dist: sella>=2.3.3; extra == "sella"
+Requires-Dist: sella>=2.3.4; extra == "sella"
 Provides-Extra: tblite
 Requires-Dist: tblite>=0.3.0; platform_system == "Linux" and extra == "tblite"
 Provides-Extra: dev
 Requires-Dist: pytest>=7.4.0; extra == "dev"
 Requires-Dist: pytest-cov>=3.0.0; extra == "dev"
 Requires-Dist: ruff>=0.0.285; extra == "dev"
 Provides-Extra: docs
```

### Comparing `quacc-0.8.0/README.md` & `quacc-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/pyproject.toml` & `quacc-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quacc"
 description="A platform to enable high-throughput, database-driven quantum chemistry and computational materials science"
-version = "0.8.0"
+version = "0.9.0"
 readme = "README.md"
 license = { text = "BSD-3" }
 authors = [{ name = "Andrew S. Rosen", email = "asrosen@princeton.edu" }]
 maintainers = [{ name = "Andrew S. Rosen", email = "asrosen@princeton.edu" }]
 keywords = ["high-throughput", "automated", "workflow", "dft"]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -28,15 +28,15 @@
 requires-python = ">=3.9"
 dependencies = [
     "ase>=3.23.0b1", # for Atoms object and calculators
     "cclib>=1.8", # for I/O parsing of molecular DFT codes
     "custodian>=2024.3.12", # for automated error corrections
     "emmet-core>=0.80.0", # for pre-made schemas
     "maggma>=0.64.0", # for database handling
-    "monty>=2024.2.26", # miscellaneous Python utilities
+    "monty>=2024.5.15", # miscellaneous Python utilities
     "numpy>=1.25.0", # for array handling
     "psutil", # for getting compute architecture details
     "pydantic>=2.0.1", # for settings management
     "pydantic-settings>=2.2.0", # for settings management
     "pymatgen>=2024.4.13", # for structure manipulation
     "ruamel.yaml>=0.17.40", # for YAML
     "typer>=0.12.1", # for the CLI
@@ -48,17 +48,17 @@
 defects = ["pymatgen-analysis-defects>=2023.8.22", "shakenbreak>=3.2.0"]
 jobflow = ["jobflow[fireworks]>=0.1.14", "jobflow-remote>=0.1.0"]
 mlp = ["matgl>=1.0.0", "chgnet>=0.3.3", "mace-torch>=0.3.3", "torch-dftd>=0.4.0"]
 mp = ["atomate2>=0.0.14"]
 newtonnet = ["newtonnet>=1.1"]
 parsl = ["parsl[monitoring]>=2023.10.23; platform_system!='Windows'"]
 phonons = ["phonopy>=2.20.0", "seekpath>=2.1.0"]
-prefect = ["prefect>=2.14.14", "prefect-dask>=0.2.6", "dask-jobqueue>=0.8.2"]
+prefect = ["prefect[dask]>=2.19.0", "dask-jobqueue>=0.8.2"]
 redun = ["redun>=0.16.2"]
-sella = ["sella>=2.3.3"]
+sella = ["sella>=2.3.4"]
 tblite = ["tblite>=0.3.0; platform_system=='Linux'"]
 dev = ["pytest>=7.4.0", "pytest-cov>=3.0.0", "ruff>=0.0.285"]
 docs = [
     "blacken-docs>=1.16.0",
     "mkdocs-material>=9.5.16",
     "mkdocstrings[python]>=0.22.0",
     "mkdocs-gen-files>=0.5.0",
```

### Comparing `quacc-0.8.0/src/quacc/__init__.py` & `quacc-0.9.0/src/quacc/__init__.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/_cli/quacc.py` & `quacc-0.9.0/src/quacc/_cli/quacc.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/atoms/core.py` & `quacc-0.9.0/src/quacc/atoms/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/atoms/defects.py` & `quacc-0.9.0/src/quacc/atoms/defects.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 """Utility functions for dealing with defects."""
 
 from __future__ import annotations
 
+from importlib.util import find_spec
 from typing import TYPE_CHECKING
 
 from monty.dev import requires
 from pymatgen.core.periodic_table import DummySpecies
 from pymatgen.entries.computed_entries import ComputedStructureEntry
 from pymatgen.io.ase import AseAtomsAdaptor
 
-try:
+has_deps = (
+    find_spec("pymatgen.analysis.defects") is not None
+    and find_spec("shakenbreak") is not None
+)
+
+if has_deps:
     from pymatgen.analysis.defects.generators import VacancyGenerator
     from shakenbreak.input import Distortions
 
-    has_deps = True
-except ImportError:
-    has_deps = False
 
 if TYPE_CHECKING:
     from ase.atoms import Atoms
     from numpy.typing import NDArray
     from pymatgen.core.structure import Structure
 
     if has_deps:
```

### Comparing `quacc-0.8.0/src/quacc/atoms/deformation.py` & `quacc-0.9.0/src/quacc/atoms/deformation.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/atoms/phonons.py` & `quacc-0.9.0/src/quacc/atoms/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/atoms/slabs.py` & `quacc-0.9.0/src/quacc/atoms/slabs.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/calculators/espresso/espresso.py` & `quacc-0.9.0/src/quacc/calculators/espresso/espresso.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml` & `quacc-0.9.0/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml` & `quacc-0.9.0/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml` & `quacc-0.9.0/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/calculators/espresso/utils.py` & `quacc-0.9.0/src/quacc/calculators/espresso/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     Returns
     -------
     float
         The max(ecutwfc) value
     float
         The max(ecutrho) value
     dict[str, str]
-        The pseudopotentials dictinoary, e.g. {"O": "O.pbe-n-kjpaw_psl.0.1.UPF"}
+        The pseudopotentials dictionary, e.g. {"O": "O.pbe-n-kjpaw_psl.0.1.UPF"}
     """
     unique_elements = list(set(atoms.get_chemical_symbols()))
     ecutwfc, ecutrho = 0, 0
     pseudopotentials = {}
     for element in unique_elements:
         if pp_dict[element]["cutoff_wfc"] > ecutwfc:
             ecutwfc = pp_dict[element]["cutoff_wfc"]
```

### Comparing `quacc-0.8.0/src/quacc/calculators/qchem/io.py` & `quacc-0.9.0/src/quacc/calculators/qchem/io.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/calculators/qchem/params.py` & `quacc-0.9.0/src/quacc/calculators/qchem/params.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/calculators/qchem/qchem.py` & `quacc-0.9.0/src/quacc/calculators/qchem/qchem.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/calculators/qchem/qchem_custodian.py` & `quacc-0.9.0/src/quacc/calculators/qchem/qchem_custodian.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """Custodian handlers for QChem."""
 
 from __future__ import annotations
 
+from importlib.util import find_spec
 from typing import TYPE_CHECKING
 
 from monty.dev import requires
 
 from quacc import SETTINGS
 
 if TYPE_CHECKING:
     from pathlib import Path
 
-try:
-    import openbabel as ob
-except ImportError:
-    ob = None
+has_ob = find_spec("openbabel")
 
 _DEFAULT_SETTING = ()
 
 
-@requires(ob, "Openbabel must be installed. Try conda install -c conda-forge openbabel")
+@requires(
+    has_ob, "Openbabel must be installed. Try conda install -c conda-forge openbabel"
+)
 def run_custodian(
     qchem_cmd: str = _DEFAULT_SETTING,
     qchem_cores: int = _DEFAULT_SETTING,
     qchem_local_scratch: str | Path = _DEFAULT_SETTING,
     qchem_use_error_handlers: bool = _DEFAULT_SETTING,
     qchem_custodian_max_errors: int = _DEFAULT_SETTING,
     qchem_nbo_exe: str | Path = _DEFAULT_SETTING,
```

### Comparing `quacc-0.8.0/src/quacc/calculators/vasp/io.py` & `quacc-0.9.0/src/quacc/calculators/vasp/io.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/calculators/vasp/params.py` & `quacc-0.9.0/src/quacc/calculators/vasp/params.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml` & `quacc-0.9.0/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/calculators/vasp/presets/setups_pbe54.yaml` & `quacc-0.9.0/src/quacc/calculators/vasp/presets/setups_pbe54.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/calculators/vasp/presets/setups_qmof.yaml` & `quacc-0.9.0/src/quacc/calculators/vasp/presets/setups_qmof.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/calculators/vasp/vasp.py` & `quacc-0.9.0/src/quacc/calculators/vasp/vasp.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/calculators/vasp/vasp_custodian.py` & `quacc-0.9.0/src/quacc/calculators/vasp/vasp_custodian.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/recipes/common/defects.py` & `quacc-0.9.0/src/quacc/recipes/common/defects.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/recipes/common/elastic.py` & `quacc-0.9.0/src/quacc/recipes/common/elastic.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/recipes/common/phonons.py` & `quacc-0.9.0/src/quacc/recipes/common/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/recipes/common/slabs.py` & `quacc-0.9.0/src/quacc/recipes/common/slabs.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/recipes/dftb/_base.py` & `quacc-0.9.0/src/quacc/recipes/dftb/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/recipes/dftb/core.py` & `quacc-0.9.0/src/quacc/recipes/dftb/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/recipes/emt/core.py` & `quacc-0.9.0/src/quacc/recipes/emt/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/recipes/emt/defects.py` & `quacc-0.9.0/src/quacc/recipes/emt/defects.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,23 +94,23 @@
     Returns
     -------
     list[RunSchema | OptSchema]
         List of dictionary of results from [quacc.schemas.ase.summarize_run][]
         or [quacc.schemas.ase.summarize_opt_run][].
         See the return type-hint for the data structure.
     """
-    make_defects_kwargs = recursive_dict_merge(
-        make_defects_kwargs, {"defect_gen": defect_gen, "defect_charge": defect_charge}
-    )
     relax_job_, static_job_ = customize_funcs(
         ["relax_job", "static_job"],
         [relax_job, static_job],
-        parameters=job_params,
+        param_swaps=job_params,
         decorators=job_decorators,
     )
+    make_defects_kwargs = recursive_dict_merge(
+        make_defects_kwargs, {"defect_gen": defect_gen, "defect_charge": defect_charge}
+    )
 
     return bulk_to_defects_subflow(
         atoms,
         relax_job_,
         static_job=static_job_ if run_static else None,
         make_defects_kwargs=make_defects_kwargs,
     )
```

### Comparing `quacc-0.8.0/src/quacc/recipes/emt/elastic.py` & `quacc-0.9.0/src/quacc/recipes/emt/elastic.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         [RunSchema][quacc.schemas.ase.summarize_run] or
         [OptSchema][quacc.schemas.ase.summarize_opt_run] for each deformation.
         See the return type-hint for the data structure.
     """
     relax_job_, static_job_ = customize_funcs(
         ["relax_job", "static_job"],
         [relax_job, static_job],
-        parameters=job_params,
+        param_swaps=job_params,
         decorators=job_decorators,
     )
 
     return bulk_to_deformations_subflow(
         atoms,
         relax_job_,
         static_job=static_job_ if run_static else None,
```

### Comparing `quacc-0.8.0/src/quacc/recipes/emt/phonons.py` & `quacc-0.9.0/src/quacc/recipes/emt/phonons.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from quacc import flow
 from quacc.recipes.common.phonons import phonon_subflow
 from quacc.recipes.emt.core import relax_job, static_job
-from quacc.utils.dicts import recursive_dict_merge
 from quacc.wflow_tools.customizers import customize_funcs
 
 if TYPE_CHECKING:
     from typing import Any, Callable
 
     from ase.atoms import Atoms
 
@@ -67,33 +66,32 @@
     t_min
         Min temperature (K).
     t_max
         Max temperature (K).
     run_relax
         Whether to run a relaxation beforehand.
     job_params
-        Custom parameters to pass to each Job in the Flow. This is a dictinoary where
+        Custom parameters to pass to each Job in the Flow. This is a dictionary where
         the keys are the names of the jobs and the values are dictionaries of parameters.
     job_decorators
         Custom decorators to apply to each Job in the Flow. This is a dictionary where
         the keys are the names of the jobs and the values are decorators.
 
     Returns
     -------
     PhononSchema
         Dictionary of results from [quacc.schemas.phonons.summarize_phonopy][].
         See the return type-hint for the data structure.
     """
-    calc_defaults = {"relax_job": {"opt_params": {"fmax": 1e-3}}}
-    job_params = recursive_dict_merge(calc_defaults, job_params)
-
+    job_param_defaults = {"relax_job": {"opt_params": {"fmax": 1e-3}}}
     relax_job_, static_job_ = customize_funcs(
         ["relax_job", "static_job"],
         [relax_job, static_job],
-        parameters=job_params,
+        param_defaults=job_param_defaults,
+        param_swaps=job_params,
         decorators=job_decorators,
     )
     if run_relax:
         atoms = relax_job_(atoms)["atoms"]
 
     return phonon_subflow(
         atoms,
```

### Comparing `quacc-0.8.0/src/quacc/recipes/emt/slabs.py` & `quacc-0.9.0/src/quacc/recipes/emt/slabs.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     atoms
         Atoms object
     run_static
         Whether to run static calculations.
     make_slabs_kwargs
         Additional keyword arguments to pass to [quacc.atoms.slabs.make_slabs_from_bulk][]
     job_params
-        Custom parameters to pass to each Job in the Flow. This is a dictinoary where
+        Custom parameters to pass to each Job in the Flow. This is a dictionary where
         the keys are the names of the jobs and the values are dictionaries of parameters.
     job_decorators
         Custom decorators to apply to each Job in the Flow. This is a dictionary where
         the keys are the names of the jobs and the values are decorators.
 
     Returns
     -------
@@ -59,15 +59,15 @@
         [RunSchema][quacc.schemas.ase.summarize_run] or
         [OptSchema][quacc.schemas.ase.summarize_opt_run] for each slab.
         See the return type-hint for the data structure.
     """
     relax_job_, static_job_ = customize_funcs(
         ["relax_job", "static_job"],
         [relax_job, static_job],
-        parameters=job_params,
+        param_swaps=job_params,
         decorators=job_decorators,
     )
 
     return bulk_to_slabs_subflow(
         atoms,
         relax_job_,
         static_job=static_job_ if run_static else None,
```

### Comparing `quacc-0.8.0/src/quacc/recipes/espresso/_base.py` & `quacc-0.9.0/src/quacc/recipes/espresso/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/recipes/espresso/bands.py` & `quacc-0.9.0/src/quacc/recipes/espresso/bands.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,30 +291,30 @@
     force_gamma
         Forces gamma-centered k-points when using make_bandpath
         For more information [quacc.utils.kpts.convert_pmg_kpts][]
     parallel_info
         Dictionary containing information about the parallelization of the
         calculation. See the ASE documentation for more information.
     job_params
-        Custom parameters to pass to each Job in the Flow. This is a dictinoary where
+        Custom parameters to pass to each Job in the Flow. This is a dictionary where
         the keys are the names of the jobs and the values are dictionaries of parameters.
     job_decorators
         Custom decorators to apply to each Job in the Flow. This is a dictionary where
         the keys are the names of the jobs and the values are decorators.
 
     Returns
     -------
     BandsSchema
         Dictionary of results from [quacc.schemas.ase.summarize_run][].
         See the type-hint for the data structure.
     """
     (bands_pw_job_, bands_pp_job_, fermi_surface_job_) = customize_funcs(
         ["bands_pw_job", "bands_pp_job", "fermi_surface_job"],
         [bands_pw_job, bands_pp_job, fermi_surface_job],
-        parameters=job_params,
+        param_swaps=job_params,
         decorators=job_decorators,
     )
 
     bands_results = bands_pw_job_(
         atoms,
         copy_files,
         make_bandpath=make_bandpath,
```

### Comparing `quacc-0.8.0/src/quacc/recipes/espresso/core.py` & `quacc-0.9.0/src/quacc/recipes/espresso/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/recipes/espresso/dos.py` & `quacc-0.9.0/src/quacc/recipes/espresso/dos.py`

 * *Files 5% similar despite different names*

```diff
@@ -163,59 +163,53 @@
         - job: [quacc.recipes.espresso.dos.dos_job][]
 
     Parameters
     ----------
     atoms
         Atoms object
     job_params
-        Custom parameters to pass to each Job in the Flow. This is a dictinoary where
+        Custom parameters to pass to each Job in the Flow. This is a dictionary where
         the keys are the names of the jobs and the values are dictionaries of parameters.
     job_decorators
         Custom decorators to apply to each Job in the Flow. This is a dictionary where
         the keys are the names of the jobs and the values are decorators.
 
     Returns
     -------
     DosSchema
         Dictionary of results from [quacc.schemas.ase.summarize_run][].
         See the type-hint for the data structure.
     """
-    static_job_defaults = {
-        "kspacing": 0.2,
-        "input_data": {"system": {"occupations": "tetrahedra"}},
-    }
-    non_scf_job_defaults = recursive_dict_merge(
-        job_params.get("static_job"),
-        {
-            "kspacing": 0.01,
-            "input_data": {
-                "control": {"calculation": "nscf", "verbosity": "high"},
-                "system": {"occupations": "tetrahedra"},
-            },
+    default_job_params = {
+        "static_job": {
+            "kspacing": 0.2,
+            "input_data": {"system": {"occupations": "tetrahedra"}},
         },
-    )
-
-    calc_defaults = {
-        "static_job": static_job_defaults,
-        "non_scf_job": non_scf_job_defaults,
-        "dos_job": None,
+        "non_scf_job": recursive_dict_merge(
+            job_params.get("static_job"),
+            {
+                "kspacing": 0.01,
+                "input_data": {
+                    "control": {"calculation": "nscf", "verbosity": "high"},
+                    "system": {"occupations": "tetrahedra"},
+                },
+            },
+        ),
     }
-    job_params = recursive_dict_merge(calc_defaults, job_params)
 
     static_job_, non_scf_job_, dos_job_ = customize_funcs(
         ["static_job", "non_scf_job", "dos_job"],
         [static_job, non_scf_job, dos_job],
-        parameters=job_params,
+        param_defaults=default_job_params,
+        param_swaps=job_params,
         decorators=job_decorators,
     )
 
     static_results = static_job_(atoms)
-
     non_scf_results = non_scf_job_(atoms, prev_outdir=static_results["dir_name"])
-
     dos_results = dos_job_(prev_outdir=static_results["dir_name"])
 
     return {
         "static_job": static_results,
         "non_scf_job": non_scf_results,
         "dos_job": dos_results,
     }
@@ -245,59 +239,52 @@
         - job: [quacc.recipes.espresso.dos.projwfc_job][]
 
     Parameters
     ----------
     atoms
         Atoms object
     job_params
-        Custom parameters to pass to each Job in the Flow. This is a dictinoary where
+        Custom parameters to pass to each Job in the Flow. This is a dictionary where
         the keys are the names of the jobs and the values are dictionaries of parameters.
     job_decorators
         Custom decorators to apply to each Job in the Flow. This is a dictionary where
         the keys are the names of the jobs and the values are decorators.
 
     Returns
     -------
     ProjwfcSchema
         Dictionary of results from [quacc.schemas.ase.summarize_run][].
         See the type-hint for the data structure.
     """
-    static_job_defaults = {
-        "kspacing": 0.2,
-        "input_data": {"system": {"occupations": "tetrahedra"}},
-    }
-    non_scf_job_defaults = recursive_dict_merge(
-        job_params.get("static_job"),
-        {
-            "kspacing": 0.01,
-            "input_data": {
-                "control": {"calculation": "nscf", "verbosity": "high"},
-                "system": {"occupations": "tetrahedra"},
-            },
+    default_job_params = {
+        "static_job": {
+            "kspacing": 0.2,
+            "input_data": {"system": {"occupations": "tetrahedra"}},
         },
-    )
-
-    calc_defaults = {
-        "static_job": static_job_defaults,
-        "non_scf_job": non_scf_job_defaults,
-        "projwfc_job": None,
+        "non_scf_job": recursive_dict_merge(
+            job_params.get("static_job"),
+            {
+                "kspacing": 0.01,
+                "input_data": {
+                    "control": {"calculation": "nscf", "verbosity": "high"},
+                    "system": {"occupations": "tetrahedra"},
+                },
+            },
+        ),
     }
-    job_params = recursive_dict_merge(calc_defaults, job_params)
-
     static_job_, non_scf_job_, projwfc_job_ = customize_funcs(
         ["static_job", "non_scf_job", "projwfc_job"],
         [static_job, non_scf_job, projwfc_job],
-        parameters=job_params,
+        param_defaults=default_job_params,
+        param_swaps=job_params,
         decorators=job_decorators,
     )
 
     static_results = static_job_(atoms)
-
     non_scf_results = non_scf_job_(atoms, prev_outdir=static_results["dir_name"])
-
     projwfc_results = projwfc_job_(prev_outdir=static_results["dir_name"])
 
     return {
         "static_job": static_results,
         "non_scf_job": non_scf_results,
         "projwfc_job": projwfc_results,
     }
```

### Comparing `quacc-0.8.0/src/quacc/recipes/espresso/phonons.py` & `quacc-0.9.0/src/quacc/recipes/espresso/phonons.py`

 * *Files 6% similar despite different names*

```diff
@@ -251,49 +251,43 @@
 
     Returns
     -------
     RunSchema
         Dictionary of results from [quacc.schemas.ase.summarize_run][].
         See the type-hint for the data structure.
     """
-    relax_job_defaults = {
-        "input_data": {
-            "control": {"forc_conv_thr": 5.0e-5},
-            "electrons": {"conv_thr": 1e-12},
-        }
-    }
-    ph_job_defaults = {
-        "input_data": {
-            "inputph": {
-                "tr2_ph": 1e-12,
-                "alpha_mix(1)": 0.1,
-                "verbosity": "high",
-                "ldisp": True,
-                "nq1": 4,
-                "nq2": 4,
-                "nq3": 4,
+    default_job_params = {
+        "relax_job": {
+            "input_data": {
+                "control": {"forc_conv_thr": 5.0e-5},
+                "electrons": {"conv_thr": 1e-12},
             }
-        }
-    }
-    matdyn_job_defaults = {
-        "input_data": {"input": {"dos": True, "nk1": 32, "nk2": 32, "nk3": 32}}
-    }
-
-    calc_defaults = {
-        "relax_job": relax_job_defaults,
-        "phonon_job": ph_job_defaults,
-        "matdyn_job": matdyn_job_defaults,
+        },
+        "phonon_job": {
+            "input_data": {
+                "inputph": {
+                    "tr2_ph": 1e-12,
+                    "alpha_mix(1)": 0.1,
+                    "verbosity": "high",
+                    "ldisp": True,
+                    "nq1": 4,
+                    "nq2": 4,
+                    "nq3": 4,
+                }
+            }
+        },
+        "matdyn_job": {
+            "input_data": {"input": {"dos": True, "nk1": 32, "nk2": 32, "nk3": 32}}
+        },
     }
-
-    job_params = recursive_dict_merge(calc_defaults, job_params)
-
     pw_job, ph_job, fc_job, dos_job = customize_funcs(
         ["relax_job", "phonon_job", "q2r_job", "matdyn_job"],
         [relax_job, phonon_job, q2r_job, matdyn_job],
-        parameters=job_params,
+        param_defaults=default_job_params,
+        param_swaps=job_params,
         decorators=job_decorators,
     )
 
     pw_job_results = pw_job(atoms)
     ph_job_results = ph_job(prev_outdir=pw_job_results["dir_name"])
     fc_job_results = fc_job(copy_files=ph_job_results["dir_name"])
     dos_job_results = dos_job(copy_files=fc_job_results["dir_name"])
@@ -361,15 +355,15 @@
         Atoms object
     nblocks
         The number of representations to group together in a single job.
         This will reduce the amount of data produced by a factor of nblocks.
         If nblocks = 0, each job will contain all the representations for a
         single q-point.
     job_params
-        Custom parameters to pass to each Job in the Flow. This is a dictinoary where
+        Custom parameters to pass to each Job in the Flow. This is a dictionary where
         the keys are the names of the jobs and the values are dictionaries of parameters.
     job_decorators
         Custom decorators to apply to each Job in the Flow. This is a dictionary where
         the keys are the names of the jobs and the values are decorators.
 
     Returns
     -------
@@ -439,48 +433,40 @@
                 ph_job_results = ph_job(
                     deepcopy(files_to_copy), input_data=deepcopy(ph_input_data)
                 )
                 grid_results.append(ph_job_results)
 
         return grid_results
 
-    job_params = job_params or {}
-    relax_job_defaults = {
-        "input_data": {
-            "control": {"forc_conv_thr": 5.0e-5},
-            "electrons": {"conv_thr": 1e-12},
-        }
-    }
-    ph_init_job_defaults = recursive_dict_merge(
-        {"input_data": {"inputph": {"lqdir": True, "only_init": True}}},
-        job_params.get("ph_job"),
-    )
-    ph_job_defaults = {
-        "input_data": {
-            "inputph": {"lqdir": True, "low_directory_check": True, "recover": True}
-        }
-    }
-    ph_recover_job_defaults = recursive_dict_merge(
-        {"input_data": {"inputph": {"recover": True, "lqdir": True}}},
-        job_params.get("ph_job"),
-    )
-
-    calc_defaults = {
-        "relax_job": relax_job_defaults,
-        "ph_init_job": ph_init_job_defaults,
-        "ph_job": ph_job_defaults,
-        "ph_recover_job": ph_recover_job_defaults,
+    default_job_params = {
+        "relax_job": {
+            "input_data": {
+                "control": {"forc_conv_thr": 5.0e-5},
+                "electrons": {"conv_thr": 1e-12},
+            }
+        },
+        "ph_init_job": recursive_dict_merge(
+            {"input_data": {"inputph": {"lqdir": True, "only_init": True}}},
+            job_params.get("ph_job"),
+        ),
+        "ph_job": {
+            "input_data": {
+                "inputph": {"lqdir": True, "low_directory_check": True, "recover": True}
+            }
+        },
+        "ph_recover_job": recursive_dict_merge(
+            {"input_data": {"inputph": {"recover": True, "lqdir": True}}},
+            job_params.get("ph_job"),
+        ),
     }
-
-    job_params = recursive_dict_merge(calc_defaults, job_params)
-
     pw_job, ph_init_job, ph_job, ph_recover_job = customize_funcs(
         ["relax_job", "ph_init_job", "ph_job", "ph_recover_job"],
         [relax_job, phonon_job, phonon_job, phonon_job],
-        parameters=job_params,
+        param_defaults=default_job_params,
+        param_swaps=job_params,
         decorators=job_decorators,
     )
 
     pw_job_results = pw_job(atoms)
 
     ph_init_job_results = ph_init_job(prev_outdir=pw_job_results["dir_name"])
```

### Comparing `quacc-0.8.0/src/quacc/recipes/gaussian/_base.py` & `quacc-0.9.0/src/quacc/recipes/gaussian/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/recipes/gaussian/core.py` & `quacc-0.9.0/src/quacc/recipes/gaussian/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/recipes/gulp/_base.py` & `quacc-0.9.0/src/quacc/recipes/gulp/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/recipes/gulp/core.py` & `quacc-0.9.0/src/quacc/recipes/gulp/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/recipes/lj/core.py` & `quacc-0.9.0/src/quacc/recipes/lj/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/recipes/mlp/_base.py` & `quacc-0.9.0/src/quacc/recipes/mlp/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/recipes/mlp/core.py` & `quacc-0.9.0/src/quacc/recipes/mlp/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/recipes/mlp/phonons.py` & `quacc-0.9.0/src/quacc/recipes/mlp/phonons.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from typing import TYPE_CHECKING
 
 from monty.dev import requires
 
 from quacc import flow
 from quacc.recipes.common.phonons import phonon_subflow
 from quacc.recipes.mlp.core import relax_job, static_job
-from quacc.utils.dicts import recursive_dict_merge
 from quacc.wflow_tools.customizers import customize_funcs
 
 has_deps = find_spec("phonopy") is not None and find_spec("seekpath") is not None
 
 if TYPE_CHECKING:
     from typing import Any, Callable, Literal
 
@@ -77,36 +76,35 @@
     t_step
         Temperature step (K).
     t_min
         Min temperature (K).
     t_max
         Max temperature (K).
     job_params
-        Custom parameters to pass to each Job in the Flow. This is a dictinoary where
+        Custom parameters to pass to each Job in the Flow. This is a dictionary where
         the keys are the names of the jobs and the values are dictionaries of parameters.
     job_decorators
         Custom decorators to apply to each Job in the Flow. This is a dictionary where
         the keys are the names of the jobs and the values are decorators.
 
     Returns
     -------
     PhononSchema
         Dictionary of results from [quacc.schemas.phonons.summarize_phonopy][].
         See the type-hint for the data structure.
     """
-    calc_defaults = {
-        "relax_job": {"method": method, "opt_params": {"fmax": 1e-3}},
-        "static_job": {"method": method},
+    job_param_defaults = {
+        "all": {"method": method},
+        "relax_job": {"opt_params": {"fmax": 1e-3}},
     }
-    job_params = recursive_dict_merge(calc_defaults, job_params)
-
     relax_job_, static_job_ = customize_funcs(
         ["relax_job", "static_job"],
         [relax_job, static_job],
-        parameters=job_params,
+        param_defaults=job_param_defaults,
+        param_swaps=job_params,
         decorators=job_decorators,
     )
     if run_relax:
         atoms = relax_job_(atoms)["atoms"]
 
     return phonon_subflow(
         atoms,
```

### Comparing `quacc-0.8.0/src/quacc/recipes/newtonnet/core.py` & `quacc-0.9.0/src/quacc/recipes/newtonnet/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/recipes/newtonnet/ts.py` & `quacc-0.9.0/src/quacc/recipes/newtonnet/ts.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/recipes/onetep/_base.py` & `quacc-0.9.0/src/quacc/recipes/onetep/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/recipes/onetep/core.py` & `quacc-0.9.0/src/quacc/recipes/onetep/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/recipes/orca/_base.py` & `quacc-0.9.0/src/quacc/recipes/orca/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/recipes/orca/core.py` & `quacc-0.9.0/src/quacc/recipes/orca/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/recipes/psi4/_base.py` & `quacc-0.9.0/src/quacc/recipes/psi4/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/recipes/psi4/core.py` & `quacc-0.9.0/src/quacc/recipes/psi4/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 """Core recipes for Psi4."""
 
 from __future__ import annotations
 
+from importlib.util import find_spec
 from typing import TYPE_CHECKING
 
 from monty.dev import requires
 
 from quacc import job
 from quacc.recipes.psi4._base import run_and_summarize
 
-try:
-    import psi4
-except ImportError:
-    psi4 = None
+has_psi4 = find_spec("psi4") is not None
 
 if TYPE_CHECKING:
     from ase.atoms import Atoms
 
     from quacc.schemas._aliases.ase import RunSchema
     from quacc.utils.files import Filenames, SourceDirectory
 
 
 @job
-@requires(psi4, "Psi4 not installed. Try conda install -c psi4 psi4")
+@requires(has_psi4, "Psi4 not installed. Try conda install -c psi4 psi4")
 def static_job(
     atoms: Atoms,
     charge: int = 0,
     spin_multiplicity: int = 1,
     method: str = "wb97x-v",
     basis: str = "def2-tzvp",
     copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
```

### Comparing `quacc-0.8.0/src/quacc/recipes/qchem/_base.py` & `quacc-0.9.0/src/quacc/recipes/qchem/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/recipes/qchem/core.py` & `quacc-0.9.0/src/quacc/recipes/qchem/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/recipes/qchem/ts.py` & `quacc-0.9.0/src/quacc/recipes/qchem/ts.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/recipes/tblite/core.py` & `quacc-0.9.0/src/quacc/recipes/tblite/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/recipes/tblite/phonons.py` & `quacc-0.9.0/src/quacc/recipes/tblite/phonons.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from typing import TYPE_CHECKING
 
 from monty.dev import requires
 
 from quacc import flow
 from quacc.recipes.common.phonons import phonon_subflow
 from quacc.recipes.tblite.core import relax_job, static_job
-from quacc.utils.dicts import recursive_dict_merge
 from quacc.wflow_tools.customizers import customize_funcs
 
 has_deps_tblite = find_spec("tblite") is not None
 has_deps_phonons = (
     find_spec("phonopy") is not None and find_spec("seekpath") is not None
 )
 
@@ -80,33 +79,33 @@
     t_step
         Temperature step (K).
     t_min
         Min temperature (K).
     t_max
         Max temperature (K).
     job_params
-        Custom parameters to pass to each Job in the Flow. This is a dictinoary where
+        Custom parameters to pass to each Job in the Flow. This is a dictionary where
         the keys are the names of the jobs and the values are dictionaries of parameters.
     job_decorators
         Custom decorators to apply to each Job in the Flow. This is a dictionary where
         the keys are the names of the jobs and the values are decorators.
 
     Returns
     -------
     PhononSchema
         Dictionary of results from [quacc.schemas.phonons.summarize_phonopy][].
         See the type-hint for the data structure.
     """
-    calc_defaults = {"relax_job": {"opt_params": {"fmax": 1e-3}}}
-    job_params = recursive_dict_merge(calc_defaults, job_params)
+    job_param_defaults = {"relax_job": {"opt_params": {"fmax": 1e-3}}}
 
     relax_job_, static_job_ = customize_funcs(
         ["relax_job", "static_job"],
         [relax_job, static_job],
-        parameters=job_params,
+        param_defaults=job_param_defaults,
+        param_swaps=job_params,
         decorators=job_decorators,
     )
     if run_relax:
         atoms = relax_job_(atoms)["atoms"]
 
     return phonon_subflow(
         atoms,
```

### Comparing `quacc-0.8.0/src/quacc/recipes/vasp/_base.py` & `quacc-0.9.0/src/quacc/recipes/vasp/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/recipes/vasp/core.py` & `quacc-0.9.0/src/quacc/recipes/vasp/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/recipes/vasp/mp.py` & `quacc-0.9.0/src/quacc/recipes/vasp/mp.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,15 @@
     -------
     MPGGARelaxFlowSchema
         Dictionary of results. See the type-hint for the data structure.
     """
     (mp_gga_relax_job_, mp_gga_static_job_) = customize_funcs(
         ["mp_gga_relax_job", "mp_gga_static_job"],
         [mp_gga_relax_job, mp_gga_static_job],
-        parameters=job_params,
+        param_swaps=job_params,
         decorators=job_decorators,
     )
 
     # Run the relax
     relax_results = mp_gga_relax_job_(atoms)
 
     # Run the second relax
@@ -357,15 +357,15 @@
         customize_funcs(
             [
                 "mp_metagga_prerelax_job",
                 "mp_metagga_relax_job",
                 "mp_metagga_static_job",
             ],
             [mp_metagga_prerelax_job, mp_metagga_relax_job, mp_metagga_static_job],
-            parameters=job_params,
+            param_swaps=job_params,
             decorators=job_decorators,
         )
     )
 
     # Run the prerelax
     prerelax_results = mp_metagga_prerelax_job_(atoms)
```

### Comparing `quacc-0.8.0/src/quacc/recipes/vasp/qmof.py` & `quacc-0.9.0/src/quacc/recipes/vasp/qmof.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,52 +66,51 @@
         a pre-existing key entirely. Applies for all jobs.
 
     Returns
     -------
     QMOFRelaxSchema
         Dictionary of results. See the type-hint for the data structure.
     """
-    with change_settings({"VASP_USE_CUSTODIAN": True}):
-        copy_files = None
+    copy_files = None
 
-        # 1. Pre-relaxation
-        if run_prerelax:
-            summary1 = _prerelax(atoms, **calc_kwargs)
-            atoms = summary1["atoms"]
-            copy_files = {summary1["dir_name"]: ["WAVECAR*"]}
-
-        # 2. Position relaxation (loose)
-        summary2 = _loose_relax_positions(atoms, copy_files=copy_files, **calc_kwargs)
-        atoms = summary2["atoms"]
-        copy_files = {summary2["dir_name"]: ["WAVECAR*"]}
-
-        # 3. Optional: Volume relaxation (loose)
-        if relax_cell:
-            summary3 = _loose_relax_cell(atoms, copy_files=copy_files, **calc_kwargs)
-            atoms = summary3["atoms"]
-            copy_files = {summary3["dir_name"]: ["WAVECAR*"]}
-
-        # 4. Double Relaxation
-        # This is done for two reasons: a) because it can
-        # resolve repadding issues when dV is large; b) because we can use LREAL =
-        # Auto for the first relaxation and the default LREAL for the second.
-        summary4 = _double_relax(
-            atoms, relax_cell=relax_cell, copy_files=copy_files, **calc_kwargs
-        )
-        atoms = summary4[-1]["atoms"]
-        copy_files = {summary4[-1]["dir_name"]: ["WAVECAR*"]}
+    # 1. Pre-relaxation
+    if run_prerelax:
+        summary1 = _prerelax(atoms, **calc_kwargs)
+        atoms = summary1["atoms"]
+        copy_files = {summary1["dir_name"]: ["WAVECAR*"]}
+
+    # 2. Position relaxation (loose)
+    summary2 = _loose_relax_positions(atoms, copy_files=copy_files, **calc_kwargs)
+    atoms = summary2["atoms"]
+    copy_files = {summary2["dir_name"]: ["WAVECAR*"]}
+
+    # 3. Optional: Volume relaxation (loose)
+    if relax_cell:
+        summary3 = _loose_relax_cell(atoms, copy_files=copy_files, **calc_kwargs)
+        atoms = summary3["atoms"]
+        copy_files = {summary3["dir_name"]: ["WAVECAR*"]}
+
+    # 4. Double Relaxation
+    # This is done for two reasons: a) because it can
+    # resolve repadding issues when dV is large; b) because we can use LREAL =
+    # Auto for the first relaxation and the default LREAL for the second.
+    summary4 = _double_relax(
+        atoms, relax_cell=relax_cell, copy_files=copy_files, **calc_kwargs
+    )
+    atoms = summary4[-1]["atoms"]
+    copy_files = {summary4[-1]["dir_name"]: ["WAVECAR*"]}
 
-        # 5. Static Calculation
-        summary5 = _static(atoms, copy_files=copy_files, **calc_kwargs)
-        summary5["prerelax_lowacc"] = summary1 if run_prerelax else None
-        summary5["position_relax_lowacc"] = summary2
-        summary5["volume_relax_lowacc"] = summary3 if relax_cell else None
-        summary5["double_relax"] = summary4
+    # 5. Static Calculation
+    summary5 = _static(atoms, copy_files=copy_files, **calc_kwargs)
+    summary5["prerelax_lowacc"] = summary1 if run_prerelax else None
+    summary5["position_relax_lowacc"] = summary2
+    summary5["volume_relax_lowacc"] = summary3 if relax_cell else None
+    summary5["double_relax"] = summary4
 
-        return summary5
+    return summary5
 
 
 def _prerelax(
     atoms: Atoms,
     copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
     **calc_kwargs,
 ) -> OptSchema:
@@ -278,22 +277,25 @@
         "ibrion": 2,
         "isif": 3 if relax_cell else 2,
         "lcharg": False,
         "lreal": "auto",
         "lwave": True,
         "nsw": 500 if relax_cell else 250,
     }
-    summary1 = run_and_summarize(
-        atoms,
-        preset="QMOFSet",
-        calc_defaults=calc_defaults,
-        calc_swaps=calc_kwargs,
-        additional_fields={"name": "QMOF DoubleRelax 1"},
-        copy_files=copy_files,
-    )
+
+    # To ensure vasp_gam --> vasp_std issues are auto-fixed
+    with change_settings({"VASP_USE_CUSTODIAN": True}):
+        summary1 = run_and_summarize(
+            atoms,
+            preset="QMOFSet",
+            calc_defaults=calc_defaults,
+            calc_swaps=calc_kwargs,
+            additional_fields={"name": "QMOF DoubleRelax 1"},
+            copy_files=copy_files,
+        )
 
     # Update atoms for Relaxation 2
     atoms = summary1["atoms"]
 
     # Reset LREAL
     del calc_defaults["lreal"]
```

### Comparing `quacc-0.8.0/src/quacc/recipes/vasp/slabs.py` & `quacc-0.9.0/src/quacc/recipes/vasp/slabs.py`

 * *Files 6% similar despite different names*

```diff
@@ -144,30 +144,30 @@
     atoms
         Atoms object
     make_slabs_kwargs
         Additional keyword arguments to pass to [quacc.atoms.slabs.make_slabs_from_bulk][]
     run_static
         Whether to run static calculations.
     job_params
-        Custom parameters to pass to each Job in the Flow. This is a dictinoary where
+        Custom parameters to pass to each Job in the Flow. This is a dictionary where
         the keys are the names of the jobs and the values are dictionaries of parameters.
     job_decorators
         Custom decorators to apply to each Job in the Flow. This is a dictionary where
         the keys are the names of the jobs and the values are decorators.
 
     Returns
     -------
     list[VaspSchema]
         List of dictionary results from [quacc.schemas.vasp.vasp_summarize_run][].
         See the type-hint for the data structure.
     """
     relax_job_, static_job_ = customize_funcs(
         ["relax_job", "static_job"],
         [relax_job, static_job],
-        parameters=job_params,
+        param_swaps=job_params,
         decorators=job_decorators,
     )
 
     return bulk_to_slabs_subflow(
         atoms,
         relax_job_,
         static_job=static_job_ if run_static else None,
@@ -204,30 +204,30 @@
     adsorbate
         Atoms object for the adsorbate.
     run_static
         Whether to run static calculations.
     make_ads_kwargs
         Additional keyword arguments to pass to [quacc.atoms.slabs.make_adsorbate_structures][]
     job_params
-        Custom parameters to pass to each Job in the Flow. This is a dictinoary where
+        Custom parameters to pass to each Job in the Flow. This is a dictionary where
         the keys are the names of the jobs and the values are dictionaries of parameters.
     job_decorators
         Custom decorators to apply to each Job in the Flow. This is a dictionary where
         the keys are the names of the jobs and the values are decorators.
 
     Returns
     -------
     list[VaspSchema]
         List of dictionaries of results from [quacc.schemas.vasp.vasp_summarize_run][].
         See the type-hint for the data structure.
     """
     relax_job_, static_job_ = customize_funcs(
         ["relax_job", "static_job"],
         [relax_job, static_job],
-        parameters=job_params,
+        param_swaps=job_params,
         decorators=job_decorators,
     )
 
     return slab_to_ads_subflow(
         slab,
         adsorbate,
         relax_job_,
```

### Comparing `quacc-0.8.0/src/quacc/runners/ase.py` & `quacc-0.9.0/src/quacc/runners/ase.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from ase.optimize import BFGS
 from ase.vibrations import Vibrations
 from monty.dev import requires
 from monty.os.path import zpath
 
 from quacc import SETTINGS
 from quacc.atoms.core import copy_atoms, get_final_atoms_from_dynamics
-from quacc.runners.prep import calc_cleanup, calc_setup
+from quacc.runners.prep import calc_cleanup, calc_setup, terminate
 from quacc.utils.dicts import recursive_dict_merge
 
 try:
     from sella import Sella
 
 except ImportError:
     Sella = None
@@ -102,18 +102,21 @@
     # Copy atoms so we don't modify it in-place
     atoms = copy_atoms(atoms)
 
     # Perform staging operations
     tmpdir, job_results_dir = calc_setup(atoms, copy_files=copy_files)
 
     # Run calculation
-    if get_forces:
-        atoms.get_forces()
-    else:
-        atoms.get_potential_energy()
+    try:
+        if get_forces:
+            atoms.get_forces()
+        else:
+            atoms.get_potential_energy()
+    except Exception as exception:
+        terminate(tmpdir, exception)
 
     # Most ASE calculators do not update the atoms object in-place with a call
     # to .get_potential_energy(), which is important if an internal optimizer is
     # used. This section is done to ensure that the atoms object is updated to
     # the final geometry if `geom_file` is provided.
     # Note: We have to be careful to make sure we don't lose the calculator
     # object, as this contains important information such as the parameters
@@ -229,32 +232,37 @@
     optimizer_kwargs["trajectory"] = traj
 
     # Set volume relaxation constraints, if relevant
     if relax_cell and atoms.pbc.any():
         atoms = FrechetCellFilter(atoms)
 
     # Run optimization
-    with traj, optimizer(atoms, **optimizer_kwargs) as dyn:
-        if optimizer.__name__.startswith("SciPy"):
-            # https://gitlab.com/ase/ase/-/issues/1475
-            dyn.run(fmax=fmax, steps=max_steps, **run_kwargs)
-        else:
-            for i, _ in enumerate(dyn.irun(fmax=fmax, steps=max_steps, **run_kwargs)):
-                if store_intermediate_results:
-                    _copy_intermediate_files(
-                        tmpdir,
-                        i,
-                        files_to_ignore=[
-                            traj_file,
-                            optimizer_kwargs["restart"],
-                            optimizer_kwargs["logfile"],
-                        ],
-                    )
-                if fn_hook:
-                    fn_hook(dyn)
+    try:
+        with traj, optimizer(atoms, **optimizer_kwargs) as dyn:
+            if optimizer.__name__.startswith("SciPy"):
+                # https://gitlab.com/ase/ase/-/issues/1475
+                dyn.run(fmax=fmax, steps=max_steps, **run_kwargs)
+            else:
+                for i, _ in enumerate(
+                    dyn.irun(fmax=fmax, steps=max_steps, **run_kwargs)
+                ):
+                    if store_intermediate_results:
+                        _copy_intermediate_files(
+                            tmpdir,
+                            i,
+                            files_to_ignore=[
+                                traj_file,
+                                optimizer_kwargs["restart"],
+                                optimizer_kwargs["logfile"],
+                            ],
+                        )
+                    if fn_hook:
+                        fn_hook(dyn)
+    except Exception as exception:
+        terminate(tmpdir, exception)
 
     # Store the trajectory atoms
     dyn.traj_atoms = read(traj_file, index=":")
 
     # Perform cleanup operations
     calc_cleanup(get_final_atoms_from_dynamics(dyn), tmpdir, job_results_dir)
 
@@ -295,15 +303,18 @@
     vib_kwargs = vib_kwargs or {}
 
     # Perform staging operations
     tmpdir, job_results_dir = calc_setup(atoms, copy_files=copy_files)
 
     # Run calculation
     vib = Vibrations(atoms, name=str(tmpdir / "vib"), **vib_kwargs)
-    vib.run()
+    try:
+        vib.run()
+    except Exception as exception:
+        terminate(tmpdir, exception)
 
     # Summarize run
     vib.summary(log=sys.stdout if SETTINGS.DEBUG else str(tmpdir / "vib_summary.log"))
 
     # Perform cleanup operations
     calc_cleanup(vib.atoms, tmpdir, job_results_dir)
```

### Comparing `quacc-0.8.0/src/quacc/runners/phonons.py` & `quacc-0.9.0/src/quacc/runners/phonons.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,25 +4,21 @@
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 from monty.dev import requires
 
 from quacc.runners.prep import calc_cleanup, calc_setup
 
-try:
-    import phonopy
+has_deps = find_spec("phonopy") is not None and find_spec("seekpath") is not None
 
-    has_deps = phonopy is not None and find_spec("seekpath") is not None
-except ImportError:
-    has_deps = False
 
 if TYPE_CHECKING:
     from numpy.typing import NDArray
 
-    if phonopy:
+    if has_deps:
         from phonopy import Phonopy
 
 
 @requires(has_deps, "Phonopy or seekpath is not installed.")
 def run_phonopy(
     phonon: Phonopy,
     forces: NDArray,
```

### Comparing `quacc-0.8.0/src/quacc/runners/prep.py` & `quacc-0.9.0/src/quacc/runners/prep.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,17 +64,16 @@
     # Define the results directory
     job_results_dir = SETTINGS.RESULTS_DIR
     if SETTINGS.CREATE_UNIQUE_DIR:
         job_results_dir /= f"{tmpdir.name.split('tmp-')[-1]}"
 
     # Create a symlink to the tmpdir
     if os.name != "nt" and SETTINGS.SCRATCH_DIR:
-        symlink = SETTINGS.RESULTS_DIR / f"symlink-{tmpdir.name}"
-        symlink.unlink(missing_ok=True)
-        symlink.symlink_to(tmpdir, target_is_directory=True)
+        symlink_path = SETTINGS.RESULTS_DIR / f"symlink-{tmpdir.name}"
+        symlink_path.symlink_to(tmpdir, target_is_directory=True)
 
     # Copy files to tmpdir and decompress them if needed
     if copy_files:
         if isinstance(copy_files, (str, Path)):
             copy_files = {copy_files: "*"}
 
         for source_directory, filenames in copy_files.items():
@@ -97,44 +96,72 @@
         The Atoms object after the calculation. Must have a calculator
         attached.
     tmpdir
         The path to the tmpdir, where the calculation will be run. It will be
         deleted after the calculation is complete.
     job_results_dir
         The path to the job_results_dir, where the files will ultimately be
-        stored. A symlink to the tmpdir will be made here during the calculation
-        for convenience.
+        stored.
 
     Returns
     -------
     None
     """
     job_results_dir, tmpdir = Path(job_results_dir), Path(tmpdir)
-    logger.info(f"Calculation results stored at {job_results_dir}")
 
     # Safety check
     if "tmp-" not in str(tmpdir):
         msg = f"{tmpdir} does not appear to be a tmpdir... exiting for safety!"
         raise ValueError(msg)
 
     # Reset the calculator's directory
     if atoms is not None:
         atoms.calc.directory = job_results_dir
 
-    # Make the results directory
-    job_results_dir.mkdir(parents=True, exist_ok=True)
-
     # Gzip files in tmpdir
     if SETTINGS.GZIP_FILES:
         gzip_dir(tmpdir)
 
     # Move files from tmpdir to job_results_dir
-    for file_name in os.listdir(tmpdir):
-        move(tmpdir / file_name, job_results_dir / file_name)
+    if SETTINGS.CREATE_UNIQUE_DIR:
+        move(tmpdir, job_results_dir)
+    else:
+        for file_name in os.listdir(tmpdir):
+            move(tmpdir / file_name, job_results_dir / file_name)
+        rmtree(tmpdir)
+    logger.info(f"Calculation results stored at {job_results_dir}")
 
     # Remove symlink to tmpdir
     if os.name != "nt" and SETTINGS.SCRATCH_DIR:
         symlink_path = SETTINGS.RESULTS_DIR / f"symlink-{tmpdir.name}"
         symlink_path.unlink(missing_ok=True)
 
-    # Remove the tmpdir
-    rmtree(tmpdir, ignore_errors=True)
+
+def terminate(tmpdir: Path | str, exception: Exception) -> Exception:
+    """
+    Terminate a calculation and move files to a failed directory.
+
+    Parameters
+    ----------
+    tmpdir
+        The path to the tmpdir, where the calculation was run.
+    exception
+        The exception that caused the calculation to fail.
+
+    Raises
+    -------
+    Exception
+        The exception that caused the calculation to fail.
+    """
+    job_failed_dir = tmpdir.with_name(tmpdir.name.replace("tmp-", "failed-"))
+    tmpdir.rename(job_failed_dir)
+
+    msg = f"Calculation failed! Files stored at {job_failed_dir}"
+    logging.info(msg)
+
+    if os.name != "nt" and SETTINGS.SCRATCH_DIR:
+        old_symlink_path = SETTINGS.RESULTS_DIR / f"symlink-{tmpdir.name}"
+        symlink_path = SETTINGS.RESULTS_DIR / f"symlink-{job_failed_dir.name}"
+        old_symlink_path.unlink(missing_ok=True)
+        symlink_path.symlink_to(job_failed_dir, target_is_directory=True)
+
+    raise exception
```

### Comparing `quacc-0.8.0/src/quacc/runners/thermo.py` & `quacc-0.9.0/src/quacc/runners/thermo.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/schemas/_aliases/ase.py` & `quacc-0.9.0/src/quacc/schemas/_aliases/ase.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 
 
 class Parameters(TypedDict):
     """Dictionary of parameters from atoms.calc.parameters"""
 
 
 class ParametersOpt(TypedDict):
-    """Dictionary of parameters from Optimizer.todict()"""
+    """Dictionary of parameters from Optimizer.todict() and fmax"""
+
+    fmax: float | None
 
 
 class RunSchema(AtomsSchema):
     """Schema for [quacc.schemas.ase.summarize_run][]"""
 
     input_atoms: AtomsSchema | None
     nid: str
```

### Comparing `quacc-0.8.0/src/quacc/schemas/_aliases/atoms.py` & `quacc-0.9.0/src/quacc/schemas/_aliases/atoms.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/schemas/_aliases/cclib.py` & `quacc-0.9.0/src/quacc/schemas/_aliases/cclib.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/schemas/_aliases/emmet.py` & `quacc-0.9.0/src/quacc/schemas/_aliases/emmet.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/schemas/_aliases/phonons.py` & `quacc-0.9.0/src/quacc/schemas/_aliases/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/schemas/_aliases/vasp.py` & `quacc-0.9.0/src/quacc/schemas/_aliases/vasp.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/schemas/ase.py` & `quacc-0.9.0/src/quacc/schemas/ase.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,20 +189,19 @@
         initial_atoms,
         charge_and_multiplicity=charge_and_multiplicity,
         move_magmoms=move_magmoms,
         store=None,
     )
 
     # Clean up the opt parameters
-    parameters_opt = dyn.todict()
+    parameters_opt = dyn.todict() | {"fmax": getattr(dyn, "fmax", None)}
     parameters_opt.pop("logfile", None)
     parameters_opt.pop("restart", None)
 
     opt_fields = {
-        "fmax": getattr(dyn, "fmax", None),
         "parameters_opt": parameters_opt,
         "converged": is_converged,
         "nsteps": dyn.get_number_of_steps(),
         "trajectory": trajectory,
         "trajectory_results": [atoms.calc.results for atoms in trajectory],
     }
```

### Comparing `quacc-0.8.0/src/quacc/schemas/atoms.py` & `quacc-0.9.0/src/quacc/schemas/atoms.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/schemas/cclib.py` & `quacc-0.9.0/src/quacc/schemas/cclib.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/schemas/phonons.py` & `quacc-0.9.0/src/quacc/schemas/phonons.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 """Summarizer for phonopy."""
 
 from __future__ import annotations
 
+from importlib.util import find_spec
 from typing import TYPE_CHECKING
 
 from monty.dev import requires
 
 from quacc import SETTINGS, __version__
 from quacc.schemas.atoms import atoms_to_metadata
 from quacc.utils.dicts import finalize_dict
 from quacc.utils.files import get_uri
 
-try:
-    import phonopy
-except ImportError:
-    phonopy = None
+has_phonopy = find_spec("phonopy") is not None
 
 if TYPE_CHECKING:
     from pathlib import Path
     from typing import Any
 
     from ase.atoms import Atoms
     from maggma.core import Store
 
     from quacc.schemas._aliases.phonons import PhononSchema
 
-    if phonopy:
+    if has_phonopy:
         from phonopy import Phonopy
 
 _DEFAULT_SETTING = ()
 
 
-@requires(phonopy, "This schema relies on phonopy")
+@requires(has_phonopy, "This schema relies on phonopy")
 def summarize_phonopy(
     phonon: Phonopy,
     input_atoms: Atoms,
     directory: str | Path,
     parameters: dict[str, Any] | None = None,
     additional_fields: dict[str, Any] | None = None,
     store: Store | None = _DEFAULT_SETTING,
```

### Comparing `quacc-0.8.0/src/quacc/schemas/prep.py` & `quacc-0.9.0/src/quacc/schemas/prep.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/schemas/vasp.py` & `quacc-0.9.0/src/quacc/schemas/vasp.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/settings.py` & `quacc-0.9.0/src/quacc/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     ] = Field(None, description=("The workflow manager to use, if any."))
 
     # ---------------------------
     # General Settings
     # ---------------------------
 
     RESULTS_DIR: Path = Field(
-        Path.cwd(),
+        Path(),
         description=(
             """
             Directory to permanently store I/O-based calculation results in.
             Note that this behavior may be modified by the chosen workflow engine.
             """
         ),
     )
@@ -428,18 +428,15 @@
         return v
 
     @field_validator("RESULTS_DIR", "SCRATCH_DIR")
     @classmethod
     def make_directories(cls, v: Optional[Path]) -> Optional[Path]:
         """Make directories."""
         if v:
-            if not v.is_absolute():
-                raise ValueError(f"{v} must be an absolute path.")
-            if not v.exists():
-                v.mkdir(parents=True)
+            v.mkdir(exist_ok=True, parents=True)
         return v
 
     @field_validator("STORE")
     @classmethod
     def generate_store(cls, v: Union[dict[str, dict[str, Any]], Store]) -> Store:
         """Generate the Maggma store."""
         from maggma import stores
@@ -522,27 +519,22 @@
             elif value.lower() in {"true", "false"}:
                 settings[key] = value.lower() == "true"
 
     return settings
 
 
 @contextmanager
-def change_settings(changes: dict[str, Any]) -> QuaccSettings:  # type: ignore
+def change_settings(changes: dict[str, Any]):
     """
     Temporarily change an attribute of an object.
 
     Parameters
     ----------
     changes
         Dictionary of changes to make formatted as attribute: value.
-
-    Returns
-    -------
-    QuaccSettings
-        Updated settings.
     """
     from quacc import SETTINGS
 
     original_values = {attr: getattr(SETTINGS, attr) for attr in changes}
 
     for attr, new_value in changes.items():
         setattr(SETTINGS, attr, new_value)
```

### Comparing `quacc-0.8.0/src/quacc/utils/dicts.py` & `quacc-0.9.0/src/quacc/utils/dicts.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Utility functions for dealing with dictionaries."""
 
 from __future__ import annotations
 
-import gzip
 import logging
-import pickle
 from collections.abc import MutableMapping
 from copy import deepcopy
 from pathlib import Path
 from typing import TYPE_CHECKING
 
+from monty.json import jsanitize
+from monty.serialization import dumpfn
+
 from quacc.wflow_tools.db import results_to_db
 
 if TYPE_CHECKING:
     from typing import Any
 
     from maggma.stores import Store
 
@@ -226,22 +227,28 @@
     Returns
     -------
     dict
         Cleaned task document
     """
 
     cleaned_task_doc = clean_dict(task_doc)
-
     if directory:
         if "tmp-quacc" in str(directory):
             raise ValueError("The directory should not be a temporary directory.")
-        with (
-            gzip.open(Path(directory, "quacc_results.pkl.gz"), "wb")
-            if gzip_file
-            else Path(directory, "quacc_results.pkl").open("wb")
-        ) as f:
-            pickle.dump(task_doc, f)
+
+        sanitized_schema = jsanitize(
+            cleaned_task_doc, enum_values=True, recursive_msonable=True
+        )
+        dumpfn(
+            sanitized_schema,
+            Path(
+                directory,
+                "quacc_results.json.gz" if gzip_file else "quacc_results.json",
+            ),
+            fmt="json",
+            indent=4,
+        )
 
     if store:
         results_to_db(store, task_doc)
 
     return cleaned_task_doc
```

### Comparing `quacc-0.8.0/src/quacc/utils/files.py` & `quacc-0.9.0/src/quacc/utils/files.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/utils/kpts.py` & `quacc-0.9.0/src/quacc/utils/kpts.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/utils/lists.py` & `quacc-0.9.0/src/quacc/utils/lists.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/wflow_tools/customizers.py` & `quacc-0.9.0/src/quacc/wflow_tools/customizers.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 from __future__ import annotations
 
 from copy import deepcopy
 from functools import partial
 from typing import TYPE_CHECKING, Literal
 
+from quacc.utils.dicts import recursive_dict_merge
+
 if TYPE_CHECKING:
     from typing import Any, Callable
 
 
 def strip_decorator(func: Callable) -> Callable:
     """
     Strip the decorators from a function.
@@ -134,41 +136,46 @@
 
     return partial(func, **params)
 
 
 def customize_funcs(
     names: list[str] | str,
     funcs: list[Callable] | Callable,
-    parameters: dict[str, dict[str, Any]] | None = None,
+    param_defaults: dict[str, dict[str, Any]] | None = None,
+    param_swaps: dict[str, dict[str, Any]] | None = None,
     decorators: dict[str, Callable | None] | None = None,
 ) -> tuple[Callable, ...] | Callable:
     """
     Customize a set of functions with decorators and common parameters.
 
     Parameters
     ----------
     names
         The names of the functions to customize, in the order they should be returned.
     funcs
         The functions to customize, in the order they are described in `names`.
-    parameters
-        Custom parameters to apply to each function. The keys of this dictionary correspond
+    param_defaults
+        Default parameters to apply to each function. The keys of this dictionary correspond
+        to the strings in `names`. If the key `"all"` is present, it will be applied to all
+        functions. If the value is `None`, no custom parameters will be applied to that function.
+    param_swaps
+        User-overrides of parameters to apply to each function. The keys of this dictionary correspond
         to the strings in `names`. If the key `"all"` is present, it will be applied to all
         functions. If the value is `None`, no custom parameters will be applied to that function.
     decorators
         Custom decorators to apply to each function. The keys of this dictionary correspond
         to the strings in `names`. If the key `"all"` is present, it will be applied to all
         functions. If a value is `None`, no decorator will be applied that function.
 
     Returns
     -------
     tuple[Callable, ...] | Callable
         The customized functions, returned in the same order as provided in `funcs`.
     """
-    parameters = parameters or {}
+    parameters = recursive_dict_merge(param_defaults, param_swaps)
     decorators = decorators or {}
     updated_funcs = []
 
     if not isinstance(names, (list, tuple)):
         names = [names]
     if not isinstance(funcs, (list, tuple)):
         funcs = [funcs]
```

### Comparing `quacc-0.8.0/src/quacc/wflow_tools/db.py` & `quacc-0.9.0/src/quacc/wflow_tools/db.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc/wflow_tools/decorators.py` & `quacc-0.9.0/src/quacc/wflow_tools/decorators.py`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc.egg-info/PKG-INFO` & `quacc-0.9.0/src/quacc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quacc
-Version: 0.8.0
+Version: 0.9.0
 Summary: A platform to enable high-throughput, database-driven quantum chemistry and computational materials science
 Author-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 Maintainer-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 License: BSD-3
 Project-URL: repository, https://github.com/Quantum-Accelerators/quacc
 Project-URL: documentation, https://quantum-accelerators.github.io/quacc/
 Project-URL: changelog, https://github.com/Quantum-Accelerators/quacc/blob/main/CHANGELOG.md
@@ -25,15 +25,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: ase>=3.23.0b1
 Requires-Dist: cclib>=1.8
 Requires-Dist: custodian>=2024.3.12
 Requires-Dist: emmet-core>=0.80.0
 Requires-Dist: maggma>=0.64.0
-Requires-Dist: monty>=2024.2.26
+Requires-Dist: monty>=2024.5.15
 Requires-Dist: numpy>=1.25.0
 Requires-Dist: psutil
 Requires-Dist: pydantic>=2.0.1
 Requires-Dist: pydantic-settings>=2.2.0
 Requires-Dist: pymatgen>=2024.4.13
 Requires-Dist: ruamel.yaml>=0.17.40
 Requires-Dist: typer>=0.12.1
@@ -60,21 +60,20 @@
 Requires-Dist: newtonnet>=1.1; extra == "newtonnet"
 Provides-Extra: parsl
 Requires-Dist: parsl[monitoring]>=2023.10.23; platform_system != "Windows" and extra == "parsl"
 Provides-Extra: phonons
 Requires-Dist: phonopy>=2.20.0; extra == "phonons"
 Requires-Dist: seekpath>=2.1.0; extra == "phonons"
 Provides-Extra: prefect
-Requires-Dist: prefect>=2.14.14; extra == "prefect"
-Requires-Dist: prefect-dask>=0.2.6; extra == "prefect"
+Requires-Dist: prefect[dask]>=2.19.0; extra == "prefect"
 Requires-Dist: dask-jobqueue>=0.8.2; extra == "prefect"
 Provides-Extra: redun
 Requires-Dist: redun>=0.16.2; extra == "redun"
 Provides-Extra: sella
-Requires-Dist: sella>=2.3.3; extra == "sella"
+Requires-Dist: sella>=2.3.4; extra == "sella"
 Provides-Extra: tblite
 Requires-Dist: tblite>=0.3.0; platform_system == "Linux" and extra == "tblite"
 Provides-Extra: dev
 Requires-Dist: pytest>=7.4.0; extra == "dev"
 Requires-Dist: pytest-cov>=3.0.0; extra == "dev"
 Requires-Dist: ruff>=0.0.285; extra == "dev"
 Provides-Extra: docs
```

### Comparing `quacc-0.8.0/src/quacc.egg-info/SOURCES.txt` & `quacc-0.9.0/src/quacc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quacc-0.8.0/src/quacc.egg-info/requires.txt` & `quacc-0.9.0/src/quacc.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ase>=3.23.0b1
 cclib>=1.8
 custodian>=2024.3.12
 emmet-core>=0.80.0
 maggma>=0.64.0
-monty>=2024.2.26
+monty>=2024.5.15
 numpy>=1.25.0
 psutil
 pydantic>=2.0.1
 pydantic-settings>=2.2.0
 pymatgen>=2024.4.13
 ruamel.yaml>=0.17.40
 typer>=0.12.1
@@ -62,21 +62,20 @@
 parsl[monitoring]>=2023.10.23
 
 [phonons]
 phonopy>=2.20.0
 seekpath>=2.1.0
 
 [prefect]
-prefect>=2.14.14
-prefect-dask>=0.2.6
+prefect[dask]>=2.19.0
 dask-jobqueue>=0.8.2
 
 [redun]
 redun>=0.16.2
 
 [sella]
-sella>=2.3.3
+sella>=2.3.4
 
 [tblite]
 
 [tblite:platform_system == "Linux"]
 tblite>=0.3.0
```

