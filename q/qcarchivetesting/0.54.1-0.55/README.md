# Comparing `tmp/qcarchivetesting-0.54.1.tar.gz` & `tmp/qcarchivetesting-0.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcarchivetesting-0.54.1.tar", last modified: Fri Apr 12 13:20:57 2024, max compression
+gzip compressed data, was "qcarchivetesting-0.55.tar", last modified: Thu May 23 18:50:51 2024, max compression
```

## Comparing `qcarchivetesting-0.54.1.tar` & `qcarchivetesting-0.55.tar`

### file list

```diff
@@ -1,169 +1,166 @@
-drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-04-12 13:20:57.100509 qcarchivetesting-0.54.1/
--rw-r--r--   0 ben       (1000) users      (984)      681 2024-04-12 13:20:57.100509 qcarchivetesting-0.54.1/PKG-INFO
--rw-r--r--   0 ben       (1000) users      (984)     1178 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/pyproject.toml
-drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-04-12 13:20:57.097175 qcarchivetesting-0.54.1/qcarchivetesting/
--rw-r--r--   0 ben       (1000) users      (984)      416 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/__init__.py
-drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-04-12 13:20:57.097175 qcarchivetesting-0.54.1/qcarchivetesting/config_files/
--rw-r--r--   0 ben       (1000) users      (984)      342 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/config_files/gha_fractal_compute.yaml
--rw-r--r--   0 ben       (1000) users      (984)      517 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/config_files/gha_fractal_oldcompute_dask.yaml
--rw-r--r--   0 ben       (1000) users      (984)      518 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/config_files/gha_fractal_oldcompute_parsl.yaml
--rw-r--r--   0 ben       (1000) users      (984)      465 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/config_files/gha_fractal_oldcompute_pool.yaml
--rw-r--r--   0 ben       (1000) users      (984)      429 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/config_files/gha_fractal_server.yaml
--rw-r--r--   0 ben       (1000) users      (984)      288 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/config_files/qcf_basic.yaml
--rw-r--r--   0 ben       (1000) users      (984)     3752 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/data_generator.py
-drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-04-12 13:20:57.097175 qcarchivetesting-0.54.1/qcarchivetesting/hash_data/
--rw-r--r--   0 ben       (1000) users      (984)    16240 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/hash_data/dict_hash_test_data.json.xz
--rw-r--r--   0 ben       (1000) users      (984)     1682 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/hash_data/generate_random.py
--rw-r--r--   0 ben       (1000) users      (984)     5617 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/helpers.py
-drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-04-12 13:20:57.097175 qcarchivetesting-0.54.1/qcarchivetesting/migration_data/
--rw-r--r--   0 ben       (1000) users      (984)    77051 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/migration_data/empty_v0.15.8.sql_dump
--rw-r--r--   0 ben       (1000) users      (984)      541 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/migration_data/qcfractal_config_v0.15.8.yaml
-drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-04-12 13:20:57.097175 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/
--rw-r--r--   0 ben       (1000) users      (984)     3468 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/benzene_dimer.json
--rw-r--r--   0 ben       (1000) users      (984)     1684 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/go_C4H4N2OS.json
--rw-r--r--   0 ben       (1000) users      (984)     1851 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/go_C6H5N3.json
--rw-r--r--   0 ben       (1000) users      (984)     1056 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/go_H3NS.json
--rw-r--r--   0 ben       (1000) users      (984)      383 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/hooh.json
-drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-04-12 13:20:57.100509 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/
--rw-r--r--   0 ben       (1000) users      (984)     1055 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_0.json
--rw-r--r--   0 ben       (1000) users      (984)     1055 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_1.json
--rw-r--r--   0 ben       (1000) users      (984)     1056 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_10.json
--rw-r--r--   0 ben       (1000) users      (984)     1055 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_11.json
--rw-r--r--   0 ben       (1000) users      (984)     1053 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_12.json
--rw-r--r--   0 ben       (1000) users      (984)     1056 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_13.json
--rw-r--r--   0 ben       (1000) users      (984)     1055 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_14.json
--rw-r--r--   0 ben       (1000) users      (984)     1052 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_15.json
--rw-r--r--   0 ben       (1000) users      (984)     1056 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_16.json
--rw-r--r--   0 ben       (1000) users      (984)     1056 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_17.json
--rw-r--r--   0 ben       (1000) users      (984)     1055 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_18.json
--rw-r--r--   0 ben       (1000) users      (984)     1056 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_19.json
--rw-r--r--   0 ben       (1000) users      (984)     1056 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_2.json
--rw-r--r--   0 ben       (1000) users      (984)     1055 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_20.json
--rw-r--r--   0 ben       (1000) users      (984)     1055 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_3.json
--rw-r--r--   0 ben       (1000) users      (984)     1057 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_4.json
--rw-r--r--   0 ben       (1000) users      (984)     1055 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_5.json
--rw-r--r--   0 ben       (1000) users      (984)     1050 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_6.json
--rw-r--r--   0 ben       (1000) users      (984)     1055 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_7.json
--rw-r--r--   0 ben       (1000) users      (984)     1057 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_8.json
--rw-r--r--   0 ben       (1000) users      (984)     1052 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_9.json
--rw-r--r--   0 ben       (1000) users      (984)     1373 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_0.json
--rw-r--r--   0 ben       (1000) users      (984)     1376 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_1.json
--rw-r--r--   0 ben       (1000) users      (984)     1374 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_10.json
--rw-r--r--   0 ben       (1000) users      (984)     1373 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_11.json
--rw-r--r--   0 ben       (1000) users      (984)     1375 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_12.json
--rw-r--r--   0 ben       (1000) users      (984)     1371 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_13.json
--rw-r--r--   0 ben       (1000) users      (984)     1372 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_14.json
--rw-r--r--   0 ben       (1000) users      (984)     1369 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_15.json
--rw-r--r--   0 ben       (1000) users      (984)     1374 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_16.json
--rw-r--r--   0 ben       (1000) users      (984)     1370 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_17.json
--rw-r--r--   0 ben       (1000) users      (984)     1374 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_18.json
--rw-r--r--   0 ben       (1000) users      (984)     1370 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_19.json
--rw-r--r--   0 ben       (1000) users      (984)     1370 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_2.json
--rw-r--r--   0 ben       (1000) users      (984)     1372 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_20.json
--rw-r--r--   0 ben       (1000) users      (984)     1372 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_3.json
--rw-r--r--   0 ben       (1000) users      (984)     1372 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_4.json
--rw-r--r--   0 ben       (1000) users      (984)     1374 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_5.json
--rw-r--r--   0 ben       (1000) users      (984)     1371 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_6.json
--rw-r--r--   0 ben       (1000) users      (984)     1372 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_7.json
--rw-r--r--   0 ben       (1000) users      (984)     1375 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_8.json
--rw-r--r--   0 ben       (1000) users      (984)     1375 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_9.json
--rw-r--r--   0 ben       (1000) users      (984)      708 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_HCN_0.json
--rw-r--r--   0 ben       (1000) users      (984)      711 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_HCN_1.json
--rw-r--r--   0 ben       (1000) users      (984)      710 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_HCN_10.json
--rw-r--r--   0 ben       (1000) users      (984)      712 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_HCN_2.json
--rw-r--r--   0 ben       (1000) users      (984)      710 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_HCN_3.json
--rw-r--r--   0 ben       (1000) users      (984)      711 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_HCN_4.json
--rw-r--r--   0 ben       (1000) users      (984)      710 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_HCN_5.json
--rw-r--r--   0 ben       (1000) users      (984)      711 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_HCN_6.json
--rw-r--r--   0 ben       (1000) users      (984)      710 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_HCN_7.json
--rw-r--r--   0 ben       (1000) users      (984)      709 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_HCN_8.json
--rw-r--r--   0 ben       (1000) users      (984)      710 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_HCN_9.json
--rw-r--r--   0 ben       (1000) users      (984)      529 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neon_tetramer.json
--rw-r--r--   0 ben       (1000) users      (984)      685 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/peroxide2.json
--rw-r--r--   0 ben       (1000) users      (984)      456 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/rxn_H.json
--rw-r--r--   0 ben       (1000) users      (984)      480 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/rxn_H2.json
--rw-r--r--   0 ben       (1000) users      (984)      555 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/rxn_H2O.json
--rw-r--r--   0 ben       (1000) users      (984)      481 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/rxn_O2.json
--rw-r--r--   0 ben       (1000) users      (984)     5235 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/td_C7H8N2OS_1.json
--rw-r--r--   0 ben       (1000) users      (984)     5236 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/td_C7H8N2OS_2.json
--rw-r--r--   0 ben       (1000) users      (984)     4125 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/td_C9H11NO2_0.json
--rw-r--r--   0 ben       (1000) users      (984)     4124 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/td_C9H11NO2_1.json
--rw-r--r--   0 ben       (1000) users      (984)     4129 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/td_C9H11NO2_2.json
--rw-r--r--   0 ben       (1000) users      (984)     4128 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/td_C9H11NO2_3.json
--rw-r--r--   0 ben       (1000) users      (984)     4128 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/td_C9H11NO2_4.json
--rw-r--r--   0 ben       (1000) users      (984)     4127 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/td_C9H11NO2_5.json
--rw-r--r--   0 ben       (1000) users      (984)     4127 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/td_C9H11NO2_6.json
--rw-r--r--   0 ben       (1000) users      (984)     4128 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/td_C9H11NO2_7.json
--rw-r--r--   0 ben       (1000) users      (984)     4132 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/td_C9H11NO2_8.json
--rw-r--r--   0 ben       (1000) users      (984)     4132 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/td_C9H11NO2_9.json
--rw-r--r--   0 ben       (1000) users      (984)      905 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/water_dimer_minima.json
--rw-r--r--   0 ben       (1000) users      (984)      221 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/water_dimer_minima.psimol
--rw-r--r--   0 ben       (1000) users      (984)      939 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/water_dimer_stretch.json
--rw-r--r--   0 ben       (1000) users      (984)      213 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/water_dimer_stretch.psimol
--rw-r--r--   0 ben       (1000) users      (984)      896 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/water_dimer_stretch2.json
--rw-r--r--   0 ben       (1000) users      (984)      216 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/water_dimer_stretch2.psimol
--rw-r--r--   0 ben       (1000) users      (984)     1281 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/water_stacked.json
-drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-04-12 13:20:57.100509 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/
--rw-r--r--   0 ben       (1000) users      (984)      185 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/clean.py
--rw-r--r--   0 ben       (1000) users      (984)      489 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/gen_all.sh
--rw-r--r--   0 ben       (1000) users      (984)     2217 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/generate_gridoptimization.py
--rw-r--r--   0 ben       (1000) users      (984)     2175 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/generate_manybody.py
--rw-r--r--   0 ben       (1000) users      (984)     2291 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/generate_neb.py
--rw-r--r--   0 ben       (1000) users      (984)     2060 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/generate_optimization.py
--rw-r--r--   0 ben       (1000) users      (984)     2300 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/generate_reaction.py
--rw-r--r--   0 ben       (1000) users      (984)     2127 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/generate_singlepoint.py
--rw-r--r--   0 ben       (1000) users      (984)     2225 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/generate_torsiondrive.py
--rw-r--r--   0 ben       (1000) users      (984)   485944 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/go_C4H4N2OS_mopac_pm6.json.xz
--rw-r--r--   0 ben       (1000) users      (984)     5812 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/go_H2O2_psi4_b3lyp.json.xz
--rw-r--r--   0 ben       (1000) users      (984)     5844 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/go_H2O2_psi4_pbe.json.xz
--rw-r--r--   0 ben       (1000) users      (984)    35992 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/go_H3NS_psi4_pbe.json.xz
--rw-r--r--   0 ben       (1000) users      (984)    57048 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/mb_cp_he4_psi4_mp2.json.xz
--rw-r--r--   0 ben       (1000) users      (984)    31472 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/mb_none_he4_psi4_mp2.json.xz
--rw-r--r--   0 ben       (1000) users      (984)   323700 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/neb_HCN_psi4_b3lyp_opt3.json.xz
--rw-r--r--   0 ben       (1000) users      (984)   307128 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/neb_HCN_psi4_pbe.json.xz
--rw-r--r--   0 ben       (1000) users      (984)   358332 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/neb_HCN_psi4_pbe0_opt1.json.xz
--rw-r--r--   0 ben       (1000) users      (984)   322480 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/neb_HCN_psi4_pbe_opt2.json.xz
--rw-r--r--   0 ben       (1000) users      (984)   385408 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/neb_HCN_psi4_pbe_opt_diff.json.xz
--rw-r--r--   0 ben       (1000) users      (984)    27700 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/opt_psi4_benzene.json.xz
--rw-r--r--   0 ben       (1000) users      (984)     2268 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/opt_psi4_fluoroethane_notraj.json.xz
--rw-r--r--   0 ben       (1000) users      (984)    12508 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/opt_psi4_methane_sometraj.json.xz
--rw-r--r--   0 ben       (1000) users      (984)    15628 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/rxn_H2O_psi4_b3lyp_sp.json.xz
--rw-r--r--   0 ben       (1000) users      (984)    95380 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/rxn_H2O_psi4_mp2_opt.json.xz
--rw-r--r--   0 ben       (1000) users      (984)   110060 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/rxn_H2O_psi4_mp2_optsp.json.xz
--rw-r--r--   0 ben       (1000) users      (984)    10220 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/rxn_H2_psi4_b3lyp_sp.json.xz
--rw-r--r--   0 ben       (1000) users      (984)     6800 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/sp_psi4_benzene_energy_1.json.xz
--rw-r--r--   0 ben       (1000) users      (984)     6816 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/sp_psi4_benzene_energy_2.json.xz
--rw-r--r--   0 ben       (1000) users      (984)     6824 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/sp_psi4_benzene_energy_3.json.xz
--rw-r--r--   0 ben       (1000) users      (984)     9612 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/sp_psi4_fluoroethane_wfn.json.xz
--rw-r--r--   0 ben       (1000) users      (984)     6820 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/sp_psi4_h2_b3lyp_nativefiles.json.xz
--rw-r--r--   0 ben       (1000) users      (984)     8632 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/sp_psi4_peroxide_energy_wfn.json.xz
--rw-r--r--   0 ben       (1000) users      (984)     5936 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/sp_psi4_water_energy.json.xz
--rw-r--r--   0 ben       (1000) users      (984)     6380 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/sp_psi4_water_gradient.json.xz
--rw-r--r--   0 ben       (1000) users      (984)    10964 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/sp_psi4_water_hessian.json.xz
--rw-r--r--   0 ben       (1000) users      (984)     1136 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/sp_rdkit_benzene_energy.json.xz
--rw-r--r--   0 ben       (1000) users      (984)      948 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/sp_rdkit_water_energy.json.xz
--rw-r--r--   0 ben       (1000) users      (984)  2388372 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/td_C9H11NO2_mopac_pm6.json.xz
--rw-r--r--   0 ben       (1000) users      (984)    11064 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/td_H2O2_mopac_pm6.json.xz
--rw-r--r--   0 ben       (1000) users      (984)    10720 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/td_H2O2_psi4_pbe.json.xz
--rw-r--r--   0 ben       (1000) users      (984)    10740 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/td_H2O2_psi4_pbe0.json.xz
--rw-r--r--   0 ben       (1000) users      (984)     1238 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/pytest_config.py
--rw-r--r--   0 ben       (1000) users      (984)     3600 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/test_full_gridoptimization.py
--rw-r--r--   0 ben       (1000) users      (984)     2318 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/test_full_manybody.py
--rw-r--r--   0 ben       (1000) users      (984)     6542 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/test_full_neb.py
--rw-r--r--   0 ben       (1000) users      (984)     1845 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/test_full_optimization.py
--rw-r--r--   0 ben       (1000) users      (984)     3367 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/test_full_reaction.py
--rw-r--r--   0 ben       (1000) users      (984)     3006 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/test_full_singlepoint.py
--rw-r--r--   0 ben       (1000) users      (984)     1672 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/test_full_torsiondrive.py
--rw-r--r--   0 ben       (1000) users      (984)     8940 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/testing_classes.py
--rw-r--r--   0 ben       (1000) users      (984)     7064 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/testing_fixtures.py
-drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-04-12 13:20:57.100509 qcarchivetesting-0.54.1/qcarchivetesting/wavefunction_data/
--rw-r--r--   0 ben       (1000) users      (984)    12508 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/wavefunction_data/psi4_fluoroethane.json
--rw-r--r--   0 ben       (1000) users      (984)    13894 2024-04-12 13:20:33.000000 qcarchivetesting-0.54.1/qcarchivetesting/wavefunction_data/psi4_peroxide.json
-drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-04-12 13:20:57.100509 qcarchivetesting-0.54.1/qcarchivetesting.egg-info/
--rw-r--r--   0 ben       (1000) users      (984)      681 2024-04-12 13:20:57.000000 qcarchivetesting-0.54.1/qcarchivetesting.egg-info/PKG-INFO
--rw-r--r--   0 ben       (1000) users      (984)     8202 2024-04-12 13:20:57.000000 qcarchivetesting-0.54.1/qcarchivetesting.egg-info/SOURCES.txt
--rw-r--r--   0 ben       (1000) users      (984)        1 2024-04-12 13:20:57.000000 qcarchivetesting-0.54.1/qcarchivetesting.egg-info/dependency_links.txt
--rw-r--r--   0 ben       (1000) users      (984)      118 2024-04-12 13:20:57.000000 qcarchivetesting-0.54.1/qcarchivetesting.egg-info/entry_points.txt
--rw-r--r--   0 ben       (1000) users      (984)       26 2024-04-12 13:20:57.000000 qcarchivetesting-0.54.1/qcarchivetesting.egg-info/requires.txt
--rw-r--r--   0 ben       (1000) users      (984)       17 2024-04-12 13:20:57.000000 qcarchivetesting-0.54.1/qcarchivetesting.egg-info/top_level.txt
--rw-r--r--   0 ben       (1000) users      (984)       38 2024-04-12 13:20:57.100509 qcarchivetesting-0.54.1/setup.cfg
+drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-05-23 18:50:51.570359 qcarchivetesting-0.55/
+-rw-r--r--   0 ben       (1000) users      (984)      686 2024-05-23 18:50:51.570359 qcarchivetesting-0.55/PKG-INFO
+-rw-r--r--   0 ben       (1000) users      (984)     1185 2024-05-23 18:47:51.000000 qcarchivetesting-0.55/pyproject.toml
+drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-05-23 18:50:51.550359 qcarchivetesting-0.55/qcarchivetesting/
+-rw-r--r--   0 ben       (1000) users      (984)      416 2024-05-07 13:50:39.000000 qcarchivetesting-0.55/qcarchivetesting/__init__.py
+drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-05-23 18:50:51.550359 qcarchivetesting-0.55/qcarchivetesting/config_files/
+-rw-r--r--   0 ben       (1000) users      (984)      342 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/config_files/gha_fractal_compute.yaml
+-rw-r--r--   0 ben       (1000) users      (984)      477 2024-05-22 00:19:35.000000 qcarchivetesting-0.55/qcarchivetesting/config_files/gha_fractal_server.yaml
+-rw-r--r--   0 ben       (1000) users      (984)      336 2024-05-22 00:19:35.000000 qcarchivetesting-0.55/qcarchivetesting/config_files/qcf_basic.yaml
+-rw-r--r--   0 ben       (1000) users      (984)     3752 2024-05-07 13:50:39.000000 qcarchivetesting-0.55/qcarchivetesting/data_generator.py
+drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-05-23 18:50:51.550359 qcarchivetesting-0.55/qcarchivetesting/hash_data/
+-rw-r--r--   0 ben       (1000) users      (984)    16240 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/hash_data/dict_hash_test_data.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)     1682 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/hash_data/generate_random.py
+-rw-r--r--   0 ben       (1000) users      (984)     5618 2024-05-19 15:35:34.000000 qcarchivetesting-0.55/qcarchivetesting/helpers.py
+drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-05-23 18:50:51.550359 qcarchivetesting-0.55/qcarchivetesting/migration_data/
+-rw-r--r--   0 ben       (1000) users      (984)    77051 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/migration_data/empty_v0.15.8.sql_dump
+-rw-r--r--   0 ben       (1000) users      (984)      555 2024-05-22 00:19:35.000000 qcarchivetesting-0.55/qcarchivetesting/migration_data/qcfractal_config_v0.15.8.yaml
+drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-05-23 18:50:51.553692 qcarchivetesting-0.55/qcarchivetesting/molecule_data/
+-rw-r--r--   0 ben       (1000) users      (984)     3468 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/benzene_dimer.json
+-rw-r--r--   0 ben       (1000) users      (984)     1684 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/go_C4H4N2OS.json
+-rw-r--r--   0 ben       (1000) users      (984)     1851 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/go_C6H5N3.json
+-rw-r--r--   0 ben       (1000) users      (984)     1056 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/go_H3NS.json
+-rw-r--r--   0 ben       (1000) users      (984)      383 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/hooh.json
+drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-05-23 18:50:51.557026 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/
+-rw-r--r--   0 ben       (1000) users      (984)     1055 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_0.json
+-rw-r--r--   0 ben       (1000) users      (984)     1055 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_1.json
+-rw-r--r--   0 ben       (1000) users      (984)     1056 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_10.json
+-rw-r--r--   0 ben       (1000) users      (984)     1055 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_11.json
+-rw-r--r--   0 ben       (1000) users      (984)     1053 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_12.json
+-rw-r--r--   0 ben       (1000) users      (984)     1056 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_13.json
+-rw-r--r--   0 ben       (1000) users      (984)     1055 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_14.json
+-rw-r--r--   0 ben       (1000) users      (984)     1052 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_15.json
+-rw-r--r--   0 ben       (1000) users      (984)     1056 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_16.json
+-rw-r--r--   0 ben       (1000) users      (984)     1056 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_17.json
+-rw-r--r--   0 ben       (1000) users      (984)     1055 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_18.json
+-rw-r--r--   0 ben       (1000) users      (984)     1056 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_19.json
+-rw-r--r--   0 ben       (1000) users      (984)     1056 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_2.json
+-rw-r--r--   0 ben       (1000) users      (984)     1055 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_20.json
+-rw-r--r--   0 ben       (1000) users      (984)     1055 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_3.json
+-rw-r--r--   0 ben       (1000) users      (984)     1057 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_4.json
+-rw-r--r--   0 ben       (1000) users      (984)     1055 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_5.json
+-rw-r--r--   0 ben       (1000) users      (984)     1050 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_6.json
+-rw-r--r--   0 ben       (1000) users      (984)     1055 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_7.json
+-rw-r--r--   0 ben       (1000) users      (984)     1057 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_8.json
+-rw-r--r--   0 ben       (1000) users      (984)     1052 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_9.json
+-rw-r--r--   0 ben       (1000) users      (984)     1373 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_0.json
+-rw-r--r--   0 ben       (1000) users      (984)     1376 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_1.json
+-rw-r--r--   0 ben       (1000) users      (984)     1374 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_10.json
+-rw-r--r--   0 ben       (1000) users      (984)     1373 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_11.json
+-rw-r--r--   0 ben       (1000) users      (984)     1375 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_12.json
+-rw-r--r--   0 ben       (1000) users      (984)     1371 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_13.json
+-rw-r--r--   0 ben       (1000) users      (984)     1372 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_14.json
+-rw-r--r--   0 ben       (1000) users      (984)     1369 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_15.json
+-rw-r--r--   0 ben       (1000) users      (984)     1374 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_16.json
+-rw-r--r--   0 ben       (1000) users      (984)     1370 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_17.json
+-rw-r--r--   0 ben       (1000) users      (984)     1374 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_18.json
+-rw-r--r--   0 ben       (1000) users      (984)     1370 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_19.json
+-rw-r--r--   0 ben       (1000) users      (984)     1370 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_2.json
+-rw-r--r--   0 ben       (1000) users      (984)     1372 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_20.json
+-rw-r--r--   0 ben       (1000) users      (984)     1372 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_3.json
+-rw-r--r--   0 ben       (1000) users      (984)     1372 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_4.json
+-rw-r--r--   0 ben       (1000) users      (984)     1374 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_5.json
+-rw-r--r--   0 ben       (1000) users      (984)     1371 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_6.json
+-rw-r--r--   0 ben       (1000) users      (984)     1372 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_7.json
+-rw-r--r--   0 ben       (1000) users      (984)     1375 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_8.json
+-rw-r--r--   0 ben       (1000) users      (984)     1375 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_9.json
+-rw-r--r--   0 ben       (1000) users      (984)      708 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_HCN_0.json
+-rw-r--r--   0 ben       (1000) users      (984)      711 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_HCN_1.json
+-rw-r--r--   0 ben       (1000) users      (984)      710 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_HCN_10.json
+-rw-r--r--   0 ben       (1000) users      (984)      712 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_HCN_2.json
+-rw-r--r--   0 ben       (1000) users      (984)      710 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_HCN_3.json
+-rw-r--r--   0 ben       (1000) users      (984)      711 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_HCN_4.json
+-rw-r--r--   0 ben       (1000) users      (984)      710 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_HCN_5.json
+-rw-r--r--   0 ben       (1000) users      (984)      711 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_HCN_6.json
+-rw-r--r--   0 ben       (1000) users      (984)      710 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_HCN_7.json
+-rw-r--r--   0 ben       (1000) users      (984)      709 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_HCN_8.json
+-rw-r--r--   0 ben       (1000) users      (984)      710 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_HCN_9.json
+-rw-r--r--   0 ben       (1000) users      (984)      529 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/neon_tetramer.json
+-rw-r--r--   0 ben       (1000) users      (984)      685 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/peroxide2.json
+-rw-r--r--   0 ben       (1000) users      (984)      456 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/rxn_H.json
+-rw-r--r--   0 ben       (1000) users      (984)      480 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/rxn_H2.json
+-rw-r--r--   0 ben       (1000) users      (984)      555 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/rxn_H2O.json
+-rw-r--r--   0 ben       (1000) users      (984)      481 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/rxn_O2.json
+-rw-r--r--   0 ben       (1000) users      (984)     5235 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/td_C7H8N2OS_1.json
+-rw-r--r--   0 ben       (1000) users      (984)     5236 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/td_C7H8N2OS_2.json
+-rw-r--r--   0 ben       (1000) users      (984)     4125 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/td_C9H11NO2_0.json
+-rw-r--r--   0 ben       (1000) users      (984)     4124 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/td_C9H11NO2_1.json
+-rw-r--r--   0 ben       (1000) users      (984)     4129 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/td_C9H11NO2_2.json
+-rw-r--r--   0 ben       (1000) users      (984)     4128 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/td_C9H11NO2_3.json
+-rw-r--r--   0 ben       (1000) users      (984)     4128 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/td_C9H11NO2_4.json
+-rw-r--r--   0 ben       (1000) users      (984)     4127 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/td_C9H11NO2_5.json
+-rw-r--r--   0 ben       (1000) users      (984)     4127 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/td_C9H11NO2_6.json
+-rw-r--r--   0 ben       (1000) users      (984)     4128 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/td_C9H11NO2_7.json
+-rw-r--r--   0 ben       (1000) users      (984)     4132 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/td_C9H11NO2_8.json
+-rw-r--r--   0 ben       (1000) users      (984)     4132 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/td_C9H11NO2_9.json
+-rw-r--r--   0 ben       (1000) users      (984)      905 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/water_dimer_minima.json
+-rw-r--r--   0 ben       (1000) users      (984)      221 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/water_dimer_minima.psimol
+-rw-r--r--   0 ben       (1000) users      (984)      939 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/water_dimer_stretch.json
+-rw-r--r--   0 ben       (1000) users      (984)      213 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/water_dimer_stretch.psimol
+-rw-r--r--   0 ben       (1000) users      (984)      896 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/water_dimer_stretch2.json
+-rw-r--r--   0 ben       (1000) users      (984)      216 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/water_dimer_stretch2.psimol
+-rw-r--r--   0 ben       (1000) users      (984)     1281 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/molecule_data/water_stacked.json
+drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-05-23 18:50:51.570359 qcarchivetesting-0.55/qcarchivetesting/procedure_data/
+-rw-r--r--   0 ben       (1000) users      (984)      185 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/clean.py
+-rw-r--r--   0 ben       (1000) users      (984)      489 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/gen_all.sh
+-rw-r--r--   0 ben       (1000) users      (984)     2217 2024-03-11 20:25:46.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/generate_gridoptimization.py
+-rw-r--r--   0 ben       (1000) users      (984)     2175 2024-05-21 15:52:03.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/generate_manybody.py
+-rw-r--r--   0 ben       (1000) users      (984)     2291 2024-05-07 13:50:39.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/generate_neb.py
+-rw-r--r--   0 ben       (1000) users      (984)     2060 2024-03-11 20:25:46.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/generate_optimization.py
+-rw-r--r--   0 ben       (1000) users      (984)     2300 2024-03-11 20:25:46.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/generate_reaction.py
+-rw-r--r--   0 ben       (1000) users      (984)     2127 2024-03-11 20:25:46.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/generate_singlepoint.py
+-rw-r--r--   0 ben       (1000) users      (984)     2225 2024-03-11 20:25:46.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/generate_torsiondrive.py
+-rw-r--r--   0 ben       (1000) users      (984)   485944 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/go_C4H4N2OS_mopac_pm6.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)     5812 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/go_H2O2_psi4_b3lyp.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)     5844 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/go_H2O2_psi4_pbe.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)    35992 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/go_H3NS_psi4_pbe.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)    57048 2024-05-21 15:52:03.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/mb_cp_he4_psi4_mp2.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)    31472 2024-05-21 15:52:03.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/mb_none_he4_psi4_mp2.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)   323700 2024-05-07 13:50:39.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/neb_HCN_psi4_b3lyp_opt3.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)   307128 2024-05-07 13:50:39.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/neb_HCN_psi4_pbe.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)   358332 2024-05-07 13:50:39.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/neb_HCN_psi4_pbe0_opt1.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)   322480 2024-05-07 13:50:39.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/neb_HCN_psi4_pbe_opt2.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)   385408 2024-05-07 13:50:39.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/neb_HCN_psi4_pbe_opt_diff.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)    27700 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/opt_psi4_benzene.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)     2268 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/opt_psi4_fluoroethane_notraj.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)    12508 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/opt_psi4_methane_sometraj.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)    15628 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/rxn_H2O_psi4_b3lyp_sp.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)    95380 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/rxn_H2O_psi4_mp2_opt.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)   110060 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/rxn_H2O_psi4_mp2_optsp.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)    10220 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/rxn_H2_psi4_b3lyp_sp.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)     6800 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/sp_psi4_benzene_energy_1.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)     6816 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/sp_psi4_benzene_energy_2.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)     6824 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/sp_psi4_benzene_energy_3.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)     9612 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/sp_psi4_fluoroethane_wfn.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)     6820 2024-04-12 19:49:42.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/sp_psi4_h2_b3lyp_nativefiles.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)     8632 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/sp_psi4_peroxide_energy_wfn.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)     5936 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/sp_psi4_water_energy.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)     6380 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/sp_psi4_water_gradient.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)    10964 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/sp_psi4_water_hessian.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)     1136 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/sp_rdkit_benzene_energy.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)      948 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/sp_rdkit_water_energy.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)  2388372 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/td_C9H11NO2_mopac_pm6.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)    11064 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/td_H2O2_mopac_pm6.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)    10720 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/td_H2O2_psi4_pbe.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)    10740 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/procedure_data/td_H2O2_psi4_pbe0.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)     1238 2024-03-11 20:25:46.000000 qcarchivetesting-0.55/qcarchivetesting/pytest_config.py
+-rw-r--r--   0 ben       (1000) users      (984)     3600 2024-03-11 20:25:46.000000 qcarchivetesting-0.55/qcarchivetesting/test_full_gridoptimization.py
+-rw-r--r--   0 ben       (1000) users      (984)     2318 2024-05-21 15:52:03.000000 qcarchivetesting-0.55/qcarchivetesting/test_full_manybody.py
+-rw-r--r--   0 ben       (1000) users      (984)     6542 2024-05-19 15:35:34.000000 qcarchivetesting-0.55/qcarchivetesting/test_full_neb.py
+-rw-r--r--   0 ben       (1000) users      (984)     1845 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/test_full_optimization.py
+-rw-r--r--   0 ben       (1000) users      (984)     3367 2024-05-07 13:50:39.000000 qcarchivetesting-0.55/qcarchivetesting/test_full_reaction.py
+-rw-r--r--   0 ben       (1000) users      (984)     3006 2024-03-11 20:25:46.000000 qcarchivetesting-0.55/qcarchivetesting/test_full_singlepoint.py
+-rw-r--r--   0 ben       (1000) users      (984)     1672 2024-03-11 20:25:46.000000 qcarchivetesting-0.55/qcarchivetesting/test_full_torsiondrive.py
+-rw-r--r--   0 ben       (1000) users      (984)     8899 2024-05-19 15:35:34.000000 qcarchivetesting-0.55/qcarchivetesting/testing_classes.py
+-rw-r--r--   0 ben       (1000) users      (984)     7065 2024-05-19 15:35:34.000000 qcarchivetesting-0.55/qcarchivetesting/testing_fixtures.py
+drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-05-23 18:50:51.570359 qcarchivetesting-0.55/qcarchivetesting/wavefunction_data/
+-rw-r--r--   0 ben       (1000) users      (984)    12508 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/wavefunction_data/psi4_fluoroethane.json
+-rw-r--r--   0 ben       (1000) users      (984)    13894 2023-09-11 13:38:01.000000 qcarchivetesting-0.55/qcarchivetesting/wavefunction_data/psi4_peroxide.json
+drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-05-23 18:50:51.570359 qcarchivetesting-0.55/qcarchivetesting.egg-info/
+-rw-r--r--   0 ben       (1000) users      (984)      686 2024-05-23 18:50:51.000000 qcarchivetesting-0.55/qcarchivetesting.egg-info/PKG-INFO
+-rw-r--r--   0 ben       (1000) users      (984)     8012 2024-05-23 18:50:51.000000 qcarchivetesting-0.55/qcarchivetesting.egg-info/SOURCES.txt
+-rw-r--r--   0 ben       (1000) users      (984)        1 2024-05-23 18:50:51.000000 qcarchivetesting-0.55/qcarchivetesting.egg-info/dependency_links.txt
+-rw-r--r--   0 ben       (1000) users      (984)      118 2024-05-23 18:50:51.000000 qcarchivetesting-0.55/qcarchivetesting.egg-info/entry_points.txt
+-rw-r--r--   0 ben       (1000) users      (984)       33 2024-05-23 18:50:51.000000 qcarchivetesting-0.55/qcarchivetesting.egg-info/requires.txt
+-rw-r--r--   0 ben       (1000) users      (984)       17 2024-05-23 18:50:51.000000 qcarchivetesting-0.55/qcarchivetesting.egg-info/top_level.txt
+-rw-r--r--   0 ben       (1000) users      (984)       38 2024-05-23 18:50:51.570359 qcarchivetesting-0.55/setup.cfg
```

### Comparing `qcarchivetesting-0.54.1/PKG-INFO` & `qcarchivetesting-0.55/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: qcarchivetesting
-Version: 0.54.1
+Version: 0.55
 Summary: A distributed compute and database platform for quantum chemistry.
 Author-email: Benjamin Pritchard <qcarchive@molssi.org>
 Project-URL: Homepage, https://github.com/MolSSI/QCFractal
 Project-URL: Bug Tracker, https://github.com/MolSSI/QCFractal/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: qcfractal
-Requires-Dist: qcengine
+Requires-Dist: qcengine<0.70a0
 Requires-Dist: pytest
```

### Comparing `qcarchivetesting-0.54.1/pyproject.toml` & `qcarchivetesting-0.55/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS",
 ]
 dependencies = [
     "qcfractal",
-    "qcengine",
+    "qcengine<0.70a0",
     "pytest",
 ]
 
 
 [project.urls]
 "Homepage" = "https://github.com/MolSSI/QCFractal"
 "Bug Tracker" = "https://github.com/MolSSI/QCFractal/issues"
```

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/data_generator.py` & `qcarchivetesting-0.55/qcarchivetesting/data_generator.py`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/hash_data/dict_hash_test_data.json.xz` & `qcarchivetesting-0.55/qcarchivetesting/hash_data/dict_hash_test_data.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/hash_data/generate_random.py` & `qcarchivetesting-0.55/qcarchivetesting/hash_data/generate_random.py`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/helpers.py` & `qcarchivetesting-0.55/qcarchivetesting/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Contains testing infrastructure for QCFractal.
 """
+
 from __future__ import annotations
 
 import json
 import lzma
 import os
 import signal
 import sys
```

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/migration_data/empty_v0.15.8.sql_dump` & `qcarchivetesting-0.55/qcarchivetesting/migration_data/empty_v0.15.8.sql_dump`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/migration_data/qcfractal_config_v0.15.8.yaml` & `qcarchivetesting-0.55/qcarchivetesting/migration_data/qcfractal_config_v0.15.8.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 base_folder: .
 database:
   database_name: qcfractal_default
   directory: null
   host: localhost
   logfile: qcfractal_postgres.log
   own: true
-  password: null
+  password: qcfractal1234
   port: 5444
-  username: null
+  username: qcfractal
 fractal:
   allow_read: true
   compress_response: true
   cprofile: null
   geo_file_path: null
   heartbeat_frequency: 1800
   log_apis: false
```

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/benzene_dimer.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/benzene_dimer.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/go_C4H4N2OS.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/go_C4H4N2OS.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/go_C6H5N3.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/go_C6H5N3.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/go_H3NS.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/go_H3NS.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_0.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_0.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_1.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_1.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_10.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_10.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_11.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_11.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_12.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_12.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_13.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_13.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_14.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_14.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_15.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_15.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_16.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_16.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_17.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_17.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_18.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_18.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_19.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_19.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_2.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_2.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_20.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_20.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_3.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_3.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_4.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_4.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_5.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_5.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_6.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_6.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_7.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_7.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_8.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_8.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C3H2N_9.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C3H2N_9.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_0.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_0.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_1.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_1.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_10.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_10.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_11.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_11.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_12.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_12.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_13.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_13.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_14.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_14.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_15.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_15.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_16.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_16.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_17.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_17.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_18.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_18.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_19.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_19.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_2.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_2.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_20.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_20.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_3.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_3.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_4.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_4.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_5.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_5.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_6.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_6.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_7.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_7.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_8.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_8.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_C4H3N2_9.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_C4H3N2_9.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_HCN_0.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_HCN_0.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_HCN_1.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_HCN_1.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_HCN_10.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_HCN_10.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_HCN_2.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_HCN_2.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_HCN_3.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_HCN_3.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_HCN_4.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_HCN_4.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_HCN_5.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_HCN_5.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_HCN_6.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_HCN_6.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_HCN_7.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_HCN_7.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_HCN_8.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_HCN_8.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neb/neb_HCN_9.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neb/neb_HCN_9.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/neon_tetramer.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/neon_tetramer.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/peroxide2.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/peroxide2.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/rxn_H2O.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/rxn_H2O.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/td_C7H8N2OS_1.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/td_C7H8N2OS_1.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/td_C7H8N2OS_2.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/td_C7H8N2OS_2.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/td_C9H11NO2_0.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/td_C9H11NO2_0.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/td_C9H11NO2_1.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/td_C9H11NO2_1.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/td_C9H11NO2_2.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/td_C9H11NO2_2.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/td_C9H11NO2_3.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/td_C9H11NO2_3.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/td_C9H11NO2_4.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/td_C9H11NO2_4.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/td_C9H11NO2_5.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/td_C9H11NO2_5.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/td_C9H11NO2_6.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/td_C9H11NO2_6.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/td_C9H11NO2_7.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/td_C9H11NO2_7.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/td_C9H11NO2_8.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/td_C9H11NO2_8.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/td_C9H11NO2_9.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/td_C9H11NO2_9.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/water_dimer_minima.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/water_dimer_minima.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/water_dimer_stretch.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/water_dimer_stretch.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/water_dimer_stretch2.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/water_dimer_stretch2.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/molecule_data/water_stacked.json` & `qcarchivetesting-0.55/qcarchivetesting/molecule_data/water_stacked.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/generate_gridoptimization.py` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/generate_gridoptimization.py`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/generate_manybody.py` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/generate_manybody.py`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/generate_neb.py` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/generate_neb.py`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/generate_optimization.py` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/generate_optimization.py`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/generate_reaction.py` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/generate_reaction.py`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/generate_singlepoint.py` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/generate_singlepoint.py`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/generate_torsiondrive.py` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/generate_torsiondrive.py`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/go_C4H4N2OS_mopac_pm6.json.xz` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/go_C4H4N2OS_mopac_pm6.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/go_H2O2_psi4_b3lyp.json.xz` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/go_H2O2_psi4_b3lyp.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/go_H2O2_psi4_pbe.json.xz` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/go_H2O2_psi4_pbe.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/go_H3NS_psi4_pbe.json.xz` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/go_H3NS_psi4_pbe.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/mb_cp_he4_psi4_mp2.json.xz` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/mb_cp_he4_psi4_mp2.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/mb_none_he4_psi4_mp2.json.xz` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/mb_none_he4_psi4_mp2.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/neb_HCN_psi4_b3lyp_opt3.json.xz` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/neb_HCN_psi4_b3lyp_opt3.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/neb_HCN_psi4_pbe.json.xz` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/neb_HCN_psi4_pbe.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/neb_HCN_psi4_pbe0_opt1.json.xz` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/neb_HCN_psi4_pbe0_opt1.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/neb_HCN_psi4_pbe_opt2.json.xz` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/neb_HCN_psi4_pbe_opt2.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/neb_HCN_psi4_pbe_opt_diff.json.xz` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/neb_HCN_psi4_pbe_opt_diff.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/opt_psi4_benzene.json.xz` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/opt_psi4_benzene.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/opt_psi4_fluoroethane_notraj.json.xz` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/opt_psi4_fluoroethane_notraj.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/opt_psi4_methane_sometraj.json.xz` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/opt_psi4_methane_sometraj.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/rxn_H2O_psi4_b3lyp_sp.json.xz` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/rxn_H2O_psi4_b3lyp_sp.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/rxn_H2O_psi4_mp2_opt.json.xz` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/rxn_H2O_psi4_mp2_opt.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/rxn_H2O_psi4_mp2_optsp.json.xz` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/rxn_H2O_psi4_mp2_optsp.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/rxn_H2_psi4_b3lyp_sp.json.xz` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/rxn_H2_psi4_b3lyp_sp.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/sp_psi4_benzene_energy_1.json.xz` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/sp_psi4_benzene_energy_1.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/sp_psi4_benzene_energy_2.json.xz` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/sp_psi4_benzene_energy_2.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/sp_psi4_benzene_energy_3.json.xz` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/sp_psi4_benzene_energy_3.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/sp_psi4_fluoroethane_wfn.json.xz` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/sp_psi4_fluoroethane_wfn.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/sp_psi4_h2_b3lyp_nativefiles.json.xz` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/sp_psi4_h2_b3lyp_nativefiles.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/sp_psi4_peroxide_energy_wfn.json.xz` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/sp_psi4_peroxide_energy_wfn.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/sp_psi4_water_energy.json.xz` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/sp_psi4_water_energy.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/sp_psi4_water_gradient.json.xz` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/sp_psi4_water_gradient.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/sp_psi4_water_hessian.json.xz` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/sp_psi4_water_hessian.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/sp_rdkit_benzene_energy.json.xz` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/sp_rdkit_benzene_energy.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/sp_rdkit_water_energy.json.xz` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/sp_rdkit_water_energy.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/td_C9H11NO2_mopac_pm6.json.xz` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/td_C9H11NO2_mopac_pm6.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/td_H2O2_mopac_pm6.json.xz` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/td_H2O2_mopac_pm6.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/td_H2O2_psi4_pbe.json.xz` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/td_H2O2_psi4_pbe.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/procedure_data/td_H2O2_psi4_pbe0.json.xz` & `qcarchivetesting-0.55/qcarchivetesting/procedure_data/td_H2O2_psi4_pbe0.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/pytest_config.py` & `qcarchivetesting-0.55/qcarchivetesting/pytest_config.py`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/test_full_gridoptimization.py` & `qcarchivetesting-0.55/qcarchivetesting/test_full_gridoptimization.py`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/test_full_manybody.py` & `qcarchivetesting-0.55/qcarchivetesting/test_full_manybody.py`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/test_full_neb.py` & `qcarchivetesting-0.55/qcarchivetesting/test_full_neb.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 import time
 from typing import TYPE_CHECKING
 
+from qcarchivetesting import load_molecule_data
 from qcportal.neb import NEBKeywords
 from qcportal.optimization import OptimizationSpecification
 from qcportal.record_models import RecordStatusEnum
-from qcarchivetesting import load_molecule_data
 from qcportal.singlepoint import QCSpecification
 
 if TYPE_CHECKING:
     from qcportal import PortalClient
 
 
 def test_neb_full_1(fulltest_client: PortalClient):
```

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/test_full_optimization.py` & `qcarchivetesting-0.55/qcarchivetesting/test_full_optimization.py`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/test_full_reaction.py` & `qcarchivetesting-0.55/qcarchivetesting/test_full_reaction.py`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/test_full_singlepoint.py` & `qcarchivetesting-0.55/qcarchivetesting/test_full_singlepoint.py`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/test_full_torsiondrive.py` & `qcarchivetesting-0.55/qcarchivetesting/test_full_torsiondrive.py`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/testing_classes.py` & `qcarchivetesting-0.55/qcarchivetesting/testing_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,32 +126,31 @@
         api_limits = {
             "manager_tasks_claim": 5,
             "manager_tasks_return": 2,
             "get_records": 10,
             "get_dataset_entries": 5,
             "get_molecules": 11,
             "get_managers": 10,
-            "get_server_stats": 10,
             "get_error_logs": 10,
             "get_access_logs": 10,
         }
 
         qcf_config["api"] = api_config
         qcf_config["api_limits"] = api_limits
 
         qcf_config["enable_security"] = enable_security
         qcf_config["allow_unauthenticated_read"] = allow_unauthenticated_read
         qcf_config["service_frequency"] = 5
         qcf_config["loglevel"] = "DEBUG"
         qcf_config["heartbeat_frequency"] = 3
         qcf_config["heartbeat_max_missed"] = 2
-        qcf_config["statistics_frequency"] = 3
 
         qcf_config["database"] = {"pool_size": 0}
         qcf_config["log_access"] = log_access
+        qcf_config["access_log_keep"] = 1
 
         if ip_tests_enabled:
             qcf_config["geoip2_dir"] = geoip_path
             qcf_config["geoip2_filename"] = geoip_filename
 
         qcf_config["auto_reset"] = {"enabled": False}
```

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/testing_fixtures.py` & `qcarchivetesting-0.55/qcarchivetesting/testing_fixtures.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Pytest fixtures for QCArchive
 """
+
 from __future__ import annotations
 
 import secrets
 from typing import Tuple
 
 import pytest
```

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/wavefunction_data/psi4_fluoroethane.json` & `qcarchivetesting-0.55/qcarchivetesting/wavefunction_data/psi4_fluoroethane.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting/wavefunction_data/psi4_peroxide.json` & `qcarchivetesting-0.55/qcarchivetesting/wavefunction_data/psi4_peroxide.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting.egg-info/PKG-INFO` & `qcarchivetesting-0.55/qcarchivetesting.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: qcarchivetesting
-Version: 0.54.1
+Version: 0.55
 Summary: A distributed compute and database platform for quantum chemistry.
 Author-email: Benjamin Pritchard <qcarchive@molssi.org>
 Project-URL: Homepage, https://github.com/MolSSI/QCFractal
 Project-URL: Bug Tracker, https://github.com/MolSSI/QCFractal/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: qcfractal
-Requires-Dist: qcengine
+Requires-Dist: qcengine<0.70a0
 Requires-Dist: pytest
```

### Comparing `qcarchivetesting-0.54.1/qcarchivetesting.egg-info/SOURCES.txt` & `qcarchivetesting-0.55/qcarchivetesting.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,14 @@
 qcarchivetesting.egg-info/PKG-INFO
 qcarchivetesting.egg-info/SOURCES.txt
 qcarchivetesting.egg-info/dependency_links.txt
 qcarchivetesting.egg-info/entry_points.txt
 qcarchivetesting.egg-info/requires.txt
 qcarchivetesting.egg-info/top_level.txt
 qcarchivetesting/config_files/gha_fractal_compute.yaml
-qcarchivetesting/config_files/gha_fractal_oldcompute_dask.yaml
-qcarchivetesting/config_files/gha_fractal_oldcompute_parsl.yaml
-qcarchivetesting/config_files/gha_fractal_oldcompute_pool.yaml
 qcarchivetesting/config_files/gha_fractal_server.yaml
 qcarchivetesting/config_files/qcf_basic.yaml
 qcarchivetesting/hash_data/dict_hash_test_data.json.xz
 qcarchivetesting/hash_data/generate_random.py
 qcarchivetesting/migration_data/empty_v0.15.8.sql_dump
 qcarchivetesting/migration_data/qcfractal_config_v0.15.8.yaml
 qcarchivetesting/molecule_data/benzene_dimer.json
```

