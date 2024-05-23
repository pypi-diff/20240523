# Comparing `tmp/woningwaardering-0.2.16a0.tar.gz` & `tmp/woningwaardering-0.3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "woningwaardering-0.2.16a0.tar", last modified: Sun May 19 20:06:53 2024, max compression
+gzip compressed data, was "woningwaardering-0.3.0a0.tar", last modified: Thu May 23 11:39:56 2024, max compression
```

## Comparing `woningwaardering-0.2.16a0.tar` & `woningwaardering-0.3.0a0.tar`

### file list

```diff
@@ -1,451 +1,482 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.124357 woningwaardering-0.2.16a0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.044357 woningwaardering-0.2.16a0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.052357 woningwaardering-0.2.16a0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/.github/workflows/cicd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/.python-version
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    26722 2024-05-19 20:06:53.124357 woningwaardering-0.2.16a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24890 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.044357 woningwaardering-0.2.16a0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.052357 woningwaardering-0.2.16a0/docs/afbeeldingen/
--rw-r--r--   0 runner    (1001) docker     (127)    34043 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/docs/afbeeldingen/excel_viewer.png
--rw-r--r--   0 runner    (1001) docker     (127)    10340 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/docs/afbeeldingen/oppervlakte_van_vertrekken.excalidraw
--rw-r--r--   0 runner    (1001) docker     (127)   132221 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/docs/afbeeldingen/oppervlakte_van_vertrekken.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.044357 woningwaardering-0.2.16a0/docs/implementatietoelichting-beleidsboeken/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.056357 woningwaardering-0.2.16a0/docs/implementatietoelichting-beleidsboeken/2024/
--rw-r--r--   0 runner    (1001) docker     (127)    33544 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/docs/implementatietoelichting-beleidsboeken/2024/zelfstandige_woonruimten.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.056357 woningwaardering-0.2.16a0/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/scripts/genereer_opzet_woningwaarderinggroep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/scripts/genereer_test_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     8600 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/scripts/genereer_vera_referentiedata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/scripts/uitbreiden_vera_modellen.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 20:06:53.124357 woningwaardering-0.2.16a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/taskfile.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.056357 woningwaardering-0.2.16a0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.044357 woningwaardering-0.2.16a0/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.044357 woningwaardering-0.2.16a0/tests/data/input/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.056357 woningwaardering-0.2.16a0/tests/data/input/generiek/
--rw-r--r--   0 runner    (1001) docker     (127)    16677 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/input/generiek/37101000032.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.060357 woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/
--rw-r--r--   0 runner    (1001) docker     (127)    13487 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/12006000004.json
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/12006000004.md
--rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/23003000050.json
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/23003000050.md
--rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/25048000007.json
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/25048000007.md
--rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/28018000044.json
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/28018000044.md
--rw-r--r--   0 runner    (1001) docker     (127)    16677 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/37101000032.json
--rw-r--r--   0 runner    (1001) docker     (127)    14864 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/41027000003.json
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/41027000003.md
--rw-r--r--   0 runner    (1001) docker     (127)    16792 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/41123000005.json
--rw-r--r--   0 runner    (1001) docker     (127)    17301 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/41162000015.json
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/41162000015.md
--rw-r--r--   0 runner    (1001) docker     (127)    12899 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/41164000002.json
--rw-r--r--   0 runner    (1001) docker     (127)    13711 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/51011000042.json
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/51011000042.md
--rw-r--r--   0 runner    (1001) docker     (127)    13013 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/71211000027.json
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/71211000027.md
--rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/77795000000.json
--rw-r--r--   0 runner    (1001) docker     (127)    13280 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/81020000003.json
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/81020000003.md
--rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/81065000089.json
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/81065000089.md
--rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/85651000021.json
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/85651000021.md
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/87402000003.json
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/87402000003.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.044357 woningwaardering-0.2.16a0/tests/data/output/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.044357 woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.044357 woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/peildatum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.064357 woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/12006000004.json
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/23003000050.json
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/25048000007.json
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/28018000044.json
--rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/37101000032.json
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41027000003.json
--rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41123000005.json
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41162000015.json
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41164000002.json
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/51011000042.json
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/71211000027.json
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/77795000000.json
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/81020000003.json
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/81065000089.json
--rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/85651000021.json
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/87402000003.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.064357 woningwaardering-0.2.16a0/tests/stelsels/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.064357 woningwaardering-0.2.16a0/tests/stelsels/config/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/config/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.064357 woningwaardering-0.2.16a0/tests/stelsels/stelsel/
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/stelsel/test_select_geldige_stelselgroepversies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.064357 woningwaardering-0.2.16a0/tests/stelsels/stelselgroep/
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/stelselgroep/test_select_geldige_stelselgroepversie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/test_ZelfstandigeWoonruimten.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.064357 woningwaardering-0.2.16a0/tests/stelsels/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/utils/test_import_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/utils/test_is_geldig.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/utils/test_vind_yaml_bestanden.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.048357 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.064357 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.044357 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.068357 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_A++++_egw.json
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_A++++_egw.md
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_egw.json
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_egw.md
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_mgw.json
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_mgw.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.048357 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.048357 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.068357 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/2024-01-01/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/2024-01-01/eenheid_A++++_egw.json
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/2024-01-01/eenheid_epv_egw.json
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/2024-01-01/eenheid_epv_mgw.json
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/test_Energieprestatie.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.068357 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.048357 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.068357 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.json
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.048357 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.048357 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.068357 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/2024-01-01/
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/2024-01-01/zolder_overige_ruimten.json
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/test_OppervlakteVanOverigeRuimten.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.068357 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.048357 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.068357 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/badkamer_en_of_toilet_boven_en_onder_0.64.json
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/gedeelde_berging.json
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/ruimte_meer_of_minder_dan_4m2.json
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/zolder_vertrek.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.048357 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.048357 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.072357 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/badkamer_en_of_toilet_boven_en_onder_0.64.json
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/badkamer_en_of_toilet_boven_en_onder_0.64.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/gedeelde_berging.md
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/ruimte_meer_of_minder_dan_4m2.json
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/ruimte_meer_of_minder_dan_4m2.md
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/zolder_vertrek.json
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/zolder_vertrek.md
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/test_OppervlakteVanVertrekken.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.072357 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/verwarming/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.048357 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.072357 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_max_4_punten_overige_ruimten.json
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_max_4_punten_overige_ruimten_individueel.md
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_open_keuken.json
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_open_keuken.md
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_max_4_punten_overige_ruimten.json
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_max_4_punten_overige_ruimten_individueel.md
--rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_open_keuken.json
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_open_keuken.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.048357 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.048357 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.072357 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_max_4_punten_overige_ruimten.json
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_open_keuken.json
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_max_4_punten_overige_ruimten.json
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_open_keuken.json
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/verwarming/test_Verwarming.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.072357 woningwaardering-0.2.16a0/wettelijke-documenten/
--rw-r--r--   0 runner    (1001) docker     (127)   116885 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/wettelijke-documenten/BWBR0003237-geldend_van_01-01-2024_tm_heden_zichtdatum_06-03-2024.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.072357 woningwaardering-0.2.16a0/woningwaardering/
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-19 20:06:52.000000 woningwaardering-0.2.16a0/woningwaardering/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.076357 woningwaardering-0.2.16a0/woningwaardering/stelsels/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/stelsels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.076357 woningwaardering-0.2.16a0/woningwaardering/stelsels/config/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/stelsels/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/stelsels/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/stelsels/config/zelfstandige_woonruimten.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/stelsels/stelsel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/stelsels/stelselgroep.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/stelsels/stelselgroepversie.py
--rw-r--r--   0 runner    (1001) docker     (127)     8737 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/stelsels/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.076357 woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.076357 woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/energieprestatie.py
--rw-r--r--   0 runner    (1001) docker     (127)    11817 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/energieprestatie_2024.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.076357 woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/bouwjaar_punten.csv
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oppervlakte_0-25m2_energielabel_punten.csv
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oppervlakte_25-40m2_energielabel_punten.csv
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oppervlakte_40m2+_energielabel_punten.csv
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oud_energielabel_punten.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.080357 woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten.py
--rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten_2024.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.080357 woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken.py
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken_2024.py
--rw-r--r--   0 runner    (1001) docker     (127)     7042 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.080357 woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming.py
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming_2024.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/zelfstandige_woonruimten.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.048357 woningwaardering-0.2.16a0/woningwaardering/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.048357 woningwaardering-0.2.16a0/woningwaardering/templates/stelsels/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.080357 woningwaardering-0.2.16a0/woningwaardering/templates/stelsels/stelsel/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/templates/stelsels/stelsel/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/templates/stelsels/stelsel/stelsel.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.080357 woningwaardering-0.2.16a0/woningwaardering/templates/stelsels/stelsel/stelselgroep/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/templates/stelsels/stelsel/stelselgroep/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroep.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroepversie.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.080357 woningwaardering-0.2.16a0/woningwaardering/vera/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.080357 woningwaardering-0.2.16a0/woningwaardering/vera/bvg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/bvg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   137423 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/bvg/generated.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.084357 woningwaardering-0.2.16a0/woningwaardering/vera/bvg/model_uitbreidingen/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_eenheid.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_energieprestatie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_ruimte.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/bvg/model_uitbreidingen/referentiedata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.120357 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/
--rw-r--r--   0 runner    (1001) docker     (127)    15108 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/aanbiedingdetailstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/aanbiedingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/aanvullendedoelgroep.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/accountstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/adressoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/afletterstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/afrekenwijzesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/afspraakstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/afspraakverzoeksoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/afwezigheidsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/aktesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/authentiekgegevenbron.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/authentiekgegevensoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/authentiekgegevenstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/bedrijfsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/begrotingversie.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/bestemming.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/betaalgegevensoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/betaalwijzedeelsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/betaalwijzesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/betalingsregelingeindereden.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/betalingsregelingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/boekingdetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/boekingsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/boekingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/boekjaarperiodesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/boekjaarperiodestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/boekjaarstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)    27844 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/bouwkundigelementdetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/bouwkundigelementplaatsing.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/bouwkundigelementsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/brandwerendheidscore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/btw.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/btwaangiftestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/burgerlijkestaat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/clustersoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/collectiefobjectsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/communicatiekanaal.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/communicatierichting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/conditiescore.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/contactgegevendetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/contactgegevensoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/contactgegevenstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/contactgegevenvoorkeur.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/crediteursoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/crediteurstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/dagdeel.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/debiteursoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/debiteurstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/defectlocatie.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/defectoorzaak.py
--rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/defectsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/defectstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/doelgroep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.120357 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/dossier/
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/dossier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eenheidcriteriasoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     6190 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eenheidcriteriumdetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eenheidcriteriumsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eenheidcriteriumtoepassing.py
--rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eenheiddetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eenheiddetailstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eenheidenergievoorziening.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eenheidinterieur.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eenheidisolatie.py
--rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eenheidklimaatbeheersing.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eenheidklimaatbeheersingsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eenheidligging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eenheidmonument.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eenheidprijsconditie.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eenheidsanitair.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eenheidsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eenheidstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eindedetailreden.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eindereden.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.120357 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/energie/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/energie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/energielabel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/energieprestatiesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/energieprestatiestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/energieprestatievergoedingsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/externeincassosoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/externeincassostatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/factuurbetaalwijze.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/factuursoort.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.120357 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/financien/
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/financien/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/gebeurtenissoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/geometriesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/geslacht.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/grootboekmutatieherkomst.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/grootboekrekeningsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/grootboekrekeningstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/huurgeschilsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/huurgeschilstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/huurklasse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/huuropzeggingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/incassomoment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/inexploitatiereden.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/informatieobjectdetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/informatieobjectsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/inkomensbron.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/inkomenssoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/inkomensverklaringsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/inkoopfactuurstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/inkoopopdrachtregelsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/inschrijvingherkomst.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/inspectierapportsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/inspectierapportstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/kandidaatdetailstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/kandidaatstatus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.120357 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/kwaliteit/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/kwaliteit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/kwaliteitsniveau.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/leningaflosvorm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/leningdetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/leningsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/maatschappelijklabel.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/machtigingsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)    35393 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/materiaaldetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/materiaalsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/medewerkerrol.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/medewerkersoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/meeteenheid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.120357 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/onderhoud/
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/onderhoud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/onderhoudsbestedingsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/onderhoudslabel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/onderhoudsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/onderhoudsorderstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     8627 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/onderhoudspecialisme.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/onderhoudstaakdetailstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/onderhoudstaakstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/onderhoudsverzoekstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/opleidingsniveau.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/oppervlaktesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/opzegtermijn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.120357 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/organisatie/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/organisatie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/organisatievorm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/overeenkomstdetailsoort.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.120357 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/overeenkomsten/
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/overeenkomsten/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/overeenkomstkoppelingdetailstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/overeenkomstkoppelingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/overeenkomstsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/overeenkomststatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/passendheiddetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/passendheidssoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/prestatieafspraak.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/prijsaanpassingsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)    14827 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/prijscomponentdetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/prijscomponentsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/prijscomponentsubsidiesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/prijscomponentwijzigingsreden.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/projectbudgetregelregelsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/projectbudgetregelsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/projectbudgetregelstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/projectfasebesluitstatus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.120357 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/projectontwikkeling/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/projectontwikkeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/projectsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/projectstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/provincie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/publicatiedetailmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/publicatiedetailstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/publicatieintakevorm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/publicatiemodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/publicatiestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/puntenberekeningsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/puntenmutatiesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/reclamatiesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/reclamatiestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/redenontbinding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/redenopzegging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/redenvernietiging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/regiesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/relatieadressoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/relatiedetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)    13143 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/relatierolsoort.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.120357 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/relaties/
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/relaties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/relatiesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/relatiestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/rentesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)    13384 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/ruimtedetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/ruimteligging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/ruimtesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/sanctiesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/sanctiestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/signaleringdetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/signaleringsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/signaleringstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/taal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/toegankelijkheidslabel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/uitexploitatiereden.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/uitvoerendesoort.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.120357 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/vastgoed/
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/vastgoed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/verantwoordingconsolidatie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/verantwoordingregime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/verbijzonderingsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/verbijzonderingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/verrekeningsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/vertrouwelijkheid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/voorrangdetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/voorrangsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/vragenlijstregelherkomst.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/woningtype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/woningwaarderingstelsel.py
--rw-r--r--   0 runner    (1001) docker     (127)    14624 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/woningwaarderingstelselgroep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.120357 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/woonruimteverdeling/
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/woonruimteverdeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/woonsituatiesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/woonvorm.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/zaakobjectsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/zaakrol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/zaakstatussoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/zaaktypedetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/zaaktypesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/zekerheidverpandingsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata_uitbreiding.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-19 20:06:38.000000 woningwaardering-0.2.16a0/woningwaardering/vera/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:06:53.120357 woningwaardering-0.2.16a0/woningwaardering.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    26722 2024-05-19 20:06:52.000000 woningwaardering-0.2.16a0/woningwaardering.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23957 2024-05-19 20:06:53.000000 woningwaardering-0.2.16a0/woningwaardering.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 20:06:52.000000 woningwaardering-0.2.16a0/woningwaardering.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-19 20:06:52.000000 woningwaardering-0.2.16a0/woningwaardering.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-19 20:06:52.000000 woningwaardering-0.2.16a0/woningwaardering.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.853829 woningwaardering-0.3.0a0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.781828 woningwaardering-0.3.0a0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/.github/labeler.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.781828 woningwaardering-0.3.0a0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/.github/workflows/cicd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/.python-version
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    26709 2024-05-23 11:39:56.853829 woningwaardering-0.3.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24886 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.773828 woningwaardering-0.3.0a0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.781828 woningwaardering-0.3.0a0/docs/afbeeldingen/
+-rw-r--r--   0 runner    (1001) docker     (127)    34043 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/docs/afbeeldingen/excel_viewer.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10340 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/docs/afbeeldingen/oppervlakte_van_vertrekken.excalidraw
+-rw-r--r--   0 runner    (1001) docker     (127)   132221 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/docs/afbeeldingen/oppervlakte_van_vertrekken.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.773828 woningwaardering-0.3.0a0/docs/implementatietoelichting-beleidsboeken/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.785828 woningwaardering-0.3.0a0/docs/implementatietoelichting-beleidsboeken/2024/
+-rw-r--r--   0 runner    (1001) docker     (127)    39279 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/docs/implementatietoelichting-beleidsboeken/2024/zelfstandige_woonruimten.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.785828 woningwaardering-0.3.0a0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/scripts/genereer_opzet_woningwaarderinggroep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/scripts/genereer_test_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8600 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/scripts/genereer_vera_referentiedata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/scripts/uitbreiden_vera_modellen.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 11:39:56.853829 woningwaardering-0.3.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/taskfile.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.785828 woningwaardering-0.3.0a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.773828 woningwaardering-0.3.0a0/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.773828 woningwaardering-0.3.0a0/tests/data/input/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.785828 woningwaardering-0.3.0a0/tests/data/input/generiek/
+-rw-r--r--   0 runner    (1001) docker     (127)    16677 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/input/generiek/37101000032.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.789828 woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/
+-rw-r--r--   0 runner    (1001) docker     (127)    13487 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/12006000004.json
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/12006000004.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/23003000050.json
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/23003000050.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/25048000007.json
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/25048000007.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/28018000044.json
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/28018000044.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16677 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/37101000032.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14864 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/41027000003.json
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/41027000003.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16792 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/41123000005.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17301 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/41162000015.json
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/41162000015.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12899 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/41164000002.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13711 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/51011000042.json
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/51011000042.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13013 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/71211000027.json
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/71211000027.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/77795000000.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13280 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/81020000003.json
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/81020000003.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/81065000089.json
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/81065000089.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/85651000021.json
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/85651000021.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/87402000003.json
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/87402000003.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.773828 woningwaardering-0.3.0a0/tests/data/output/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.773828 woningwaardering-0.3.0a0/tests/data/output/zelfstandige_woonruimten/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.773828 woningwaardering-0.3.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.793828 woningwaardering-0.3.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/12006000004.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/23003000050.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/25048000007.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/28018000044.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/37101000032.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41027000003.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41123000005.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41162000015.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41164000002.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/51011000042.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/71211000027.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/77795000000.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/81020000003.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/81065000089.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/85651000021.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/87402000003.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.793828 woningwaardering-0.3.0a0/tests/stelsels/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.793828 woningwaardering-0.3.0a0/tests/stelsels/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/config/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.793828 woningwaardering-0.3.0a0/tests/stelsels/stelsel/
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/stelsel/test_select_geldige_stelselgroepversies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.793828 woningwaardering-0.3.0a0/tests/stelsels/stelselgroep/
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/stelselgroep/test_select_geldige_stelselgroepversie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/test_ZelfstandigeWoonruimten.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.793828 woningwaardering-0.3.0a0/tests/stelsels/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/utils/test_import_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/utils/test_is_geldig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/utils/test_vind_yaml_bestanden.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.777828 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.793828 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.773828 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.797828 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_A++++_egw.json
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_A++++_egw.md
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_egw.json
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_egw.md
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_mgw.json
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_mgw.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.773828 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.773828 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.797828 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/2024-01-01/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/2024-01-01/eenheid_A++++_egw.json
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/2024-01-01/eenheid_epv_egw.json
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/2024-01-01/eenheid_epv_mgw.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/test_Energieprestatie.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.797828 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.773828 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.797828 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.json
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.773828 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.773828 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.797828 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/2024-01-01/
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/2024-01-01/zolder_overige_ruimten.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/test_OppervlakteVanOverigeRuimten.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.797828 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.777828 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.797828 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/badkamer_en_of_toilet_boven_en_onder_0.64.json
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/gedeelde_berging.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/ruimte_meer_of_minder_dan_4m2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/zolder_vertrek.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.777828 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.777828 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.801828 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/badkamer_en_of_toilet_boven_en_onder_0.64.json
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/badkamer_en_of_toilet_boven_en_onder_0.64.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/gedeelde_berging.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/ruimte_meer_of_minder_dan_4m2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/ruimte_meer_of_minder_dan_4m2.md
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/zolder_vertrek.json
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/zolder_vertrek.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/test_OppervlakteVanVertrekken.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.801828 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.777828 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.801828 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/bad.json
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/bad_en_douche.json
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/bidet.json
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/douche.json
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/geen_sanitair.json
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/lavet.json
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/toilet.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/twee_bad_en_douche.json
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/wastafel.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.777828 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.777828 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.801828 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/bad.json
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/bad_en_douche.json
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/bidet.json
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/douche.json
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/geen_sanitair.json
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/lavet.json
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/toilet.json
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/twee_bad_en_douche.json
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/wastafel.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/test_Sanitair.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.801828 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.777828 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.805828 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_max_4_punten_overige_ruimten.json
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_max_4_punten_overige_ruimten_individueel.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_open_keuken.json
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_open_keuken.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_max_4_punten_overige_ruimten.json
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_max_4_punten_overige_ruimten_individueel.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_open_keuken.json
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_open_keuken.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.777828 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.777828 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.805828 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_max_4_punten_overige_ruimten.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_open_keuken.json
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_max_4_punten_overige_ruimten.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_open_keuken.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/test_Verwarming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.805828 woningwaardering-0.3.0a0/wettelijke-documenten/
+-rw-r--r--   0 runner    (1001) docker     (127)   116885 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/wettelijke-documenten/BWBR0003237-geldend_van_01-01-2024_tm_heden_zichtdatum_06-03-2024.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.805828 woningwaardering-0.3.0a0/woningwaardering/
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-23 11:39:56.000000 woningwaardering-0.3.0a0/woningwaardering/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.809829 woningwaardering-0.3.0a0/woningwaardering/stelsels/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/stelsels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.809829 woningwaardering-0.3.0a0/woningwaardering/stelsels/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/stelsels/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/stelsels/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/stelsels/config/zelfstandige_woonruimten.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/stelsels/stelsel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/stelsels/stelselgroep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/stelsels/stelselgroepversie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8737 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/stelsels/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.809829 woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.809829 woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/energieprestatie.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11817 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/energieprestatie_2024.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.809829 woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/bouwjaar_punten.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oppervlakte_0-25m2_energielabel_punten.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oppervlakte_25-40m2_energielabel_punten.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oppervlakte_40m2+_energielabel_punten.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oud_energielabel_punten.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.809829 woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten_2024.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.813829 woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken_2024.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.813829 woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/sanitair/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/sanitair/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/sanitair/sanitair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/sanitair/sanitair_2024.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.813829 woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming_2024.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/zelfstandige_woonruimten.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.777828 woningwaardering-0.3.0a0/woningwaardering/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.777828 woningwaardering-0.3.0a0/woningwaardering/templates/stelsels/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.813829 woningwaardering-0.3.0a0/woningwaardering/templates/stelsels/stelsel/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/templates/stelsels/stelsel/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/templates/stelsels/stelsel/stelsel.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.813829 woningwaardering-0.3.0a0/woningwaardering/templates/stelsels/stelsel/stelselgroep/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/templates/stelsels/stelsel/stelselgroep/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroep.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroepversie.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.813829 woningwaardering-0.3.0a0/woningwaardering/vera/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.813829 woningwaardering-0.3.0a0/woningwaardering/vera/bvg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/bvg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137423 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/bvg/generated.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.813829 woningwaardering-0.3.0a0/woningwaardering/vera/bvg/model_uitbreidingen/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_eenheid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_energieprestatie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_ruimte.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/bvg/model_uitbreidingen/referentiedata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.849829 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/
+-rw-r--r--   0 runner    (1001) docker     (127)    15108 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/aanbiedingdetailstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/aanbiedingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/aanvullendedoelgroep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/accountstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/adressoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/afletterstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/afrekenwijzesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/afspraakstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/afspraakverzoeksoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/afwezigheidsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/aktesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/authentiekgegevenbron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/authentiekgegevensoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/authentiekgegevenstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/bedrijfsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/begrotingversie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/bestemming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/betaalgegevensoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/betaalwijzedeelsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/betaalwijzesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/betalingsregelingeindereden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/betalingsregelingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/boekingdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/boekingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/boekingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/boekjaarperiodesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/boekjaarperiodestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/boekjaarstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28284 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/bouwkundigelementdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/bouwkundigelementplaatsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/bouwkundigelementsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/brandwerendheidscore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/btw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/btwaangiftestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/burgerlijkestaat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/clustersoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/collectiefobjectsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/communicatiekanaal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/communicatierichting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/conditiescore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/contactgegevendetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/contactgegevensoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/contactgegevenstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/contactgegevenvoorkeur.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/crediteursoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/crediteurstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/dagdeel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/debiteursoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/debiteurstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/defectlocatie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/defectoorzaak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/defectsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/defectstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/doelgroep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.849829 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/dossier/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/dossier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eenheidcriteriasoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6190 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eenheidcriteriumdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eenheidcriteriumsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eenheidcriteriumtoepassing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eenheiddetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eenheiddetailstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eenheidenergievoorziening.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eenheidinterieur.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eenheidisolatie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eenheidklimaatbeheersing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eenheidklimaatbeheersingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eenheidligging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eenheidmonument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eenheidprijsconditie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eenheidsanitair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eenheidsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eenheidstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eindedetailreden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eindereden.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.849829 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/energie/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/energie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/energielabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/energieprestatiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/energieprestatiestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/energieprestatievergoedingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/externeincassosoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/externeincassostatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/factuurbetaalwijze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/factuursoort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.849829 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/financien/
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/financien/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/gebeurtenissoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/geometriesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/geslacht.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/grootboekmutatieherkomst.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/grootboekrekeningsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/grootboekrekeningstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/huurgeschilsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/huurgeschilstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/huurklasse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/huuropzeggingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/incassomoment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/inexploitatiereden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/informatieobjectdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/informatieobjectsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/inkomensbron.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/inkomenssoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/inkomensverklaringsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/inkoopfactuurstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/inkoopopdrachtregelsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/inschrijvingherkomst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/inspectierapportsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/inspectierapportstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/kandidaatdetailstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/kandidaatstatus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.849829 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/kwaliteit/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/kwaliteit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/kwaliteitsniveau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/leningaflosvorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/leningdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/leningsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/maatschappelijklabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/machtigingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35393 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/materiaaldetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/materiaalsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/medewerkerrol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/medewerkersoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/meeteenheid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.849829 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/onderhoud/
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/onderhoud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/onderhoudsbestedingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/onderhoudslabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/onderhoudsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/onderhoudsorderstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8627 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/onderhoudspecialisme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/onderhoudstaakdetailstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/onderhoudstaakstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/onderhoudsverzoekstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/opleidingsniveau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/oppervlaktesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/opzegtermijn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.849829 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/organisatie/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/organisatie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/organisatievorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/overeenkomstdetailsoort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.849829 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/overeenkomsten/
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/overeenkomsten/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/overeenkomstkoppelingdetailstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/overeenkomstkoppelingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/overeenkomstsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/overeenkomststatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/passendheiddetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/passendheidssoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/prestatieafspraak.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/prijsaanpassingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14827 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/prijscomponentdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/prijscomponentsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/prijscomponentsubsidiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/prijscomponentwijzigingsreden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/projectbudgetregelregelsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/projectbudgetregelsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/projectbudgetregelstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/projectfasebesluitstatus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.849829 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/projectontwikkeling/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/projectontwikkeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/projectsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/projectstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/provincie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/publicatiedetailmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/publicatiedetailstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/publicatieintakevorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/publicatiemodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/publicatiestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/puntenberekeningsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/puntenmutatiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/reclamatiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/reclamatiestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/redenontbinding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/redenopzegging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/redenvernietiging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/regiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/relatieadressoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/relatiedetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13143 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/relatierolsoort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.849829 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/relaties/
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/relaties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/relatiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/relatiestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/rentesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13384 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/ruimtedetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/ruimteligging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/ruimtesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/sanctiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/sanctiestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/signaleringdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/signaleringsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/signaleringstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/taal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/toegankelijkheidslabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/uitexploitatiereden.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/uitvoerendesoort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.853829 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/vastgoed/
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/vastgoed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/verantwoordingconsolidatie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/verantwoordingregime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/verbijzonderingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/verbijzonderingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/verrekeningsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/vertrouwelijkheid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/voorrangdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/voorrangsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/vragenlijstregelherkomst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/woningtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/woningwaarderingstelsel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14624 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/woningwaarderingstelselgroep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.853829 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/woonruimteverdeling/
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/woonruimteverdeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/woonsituatiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/woonvorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/zaakobjectsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/zaakrol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/zaakstatussoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/zaaktypedetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/zaaktypesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/zekerheidverpandingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata_uitbreiding.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-23 11:39:52.000000 woningwaardering-0.3.0a0/woningwaardering/vera/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:39:56.853829 woningwaardering-0.3.0a0/woningwaardering.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    26709 2024-05-23 11:39:56.000000 woningwaardering-0.3.0a0/woningwaardering.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    25834 2024-05-23 11:39:56.000000 woningwaardering-0.3.0a0/woningwaardering.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 11:39:56.000000 woningwaardering-0.3.0a0/woningwaardering.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-23 11:39:56.000000 woningwaardering-0.3.0a0/woningwaardering.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-23 11:39:56.000000 woningwaardering-0.3.0a0/woningwaardering.egg-info/top_level.txt
```

### Comparing `woningwaardering-0.2.16a0/.github/workflows/cicd.yml` & `woningwaardering-0.3.0a0/.github/workflows/cicd.yml`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/.github/workflows/publish-to-pypi.yml` & `woningwaardering-0.3.0a0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/.gitignore` & `woningwaardering-0.3.0a0/.gitignore`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/.pre-commit-config.yaml` & `woningwaardering-0.3.0a0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/LICENSE` & `woningwaardering-0.3.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/PKG-INFO` & `woningwaardering-0.3.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: woningwaardering
-Version: 0.2.16a0
+Version: 0.3.0a0
 Summary: Berekent de punten van een woning op basis van het woningwaarderingsstelsel.
 Author-email: Woonstad Rotterdam <info@woonstadrotterdam.nl>, Ben Verhees <ben.verhees@woonstadrotterdam.nl>, Tiddo Loos <tiddo.loos@woonstadrotterdam.nl>, Tomer Gabay <tomer.gabay@woonstadrotterdam.nl>
-Project-URL: Homepage, https://github.com/WoonstadRotterdamTemp/woningwaardering
-Project-URL: Issues, https://github.com/WoonstadRotterdamTemp/woningwaardering/issues
+Project-URL: Homepage, https://github.com/woonstadrotterdam/woningwaardering
+Project-URL: Issues, https://github.com/woonstadrotterdam/woningwaardering/issues
 Keywords: woning,waardering,stelsel,woningwaarderingsstelsel,wws
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -134,15 +134,15 @@
 ## 2. Contributing
 
 ### Setup
 
 Om de woningwaardering-package en de daarbij behorende developer dependencies te installeren, run onderstaand command:
 
 ```
-git clone https://github.com/WoonstadRotterdamTemp/woningwaardering.git
+git clone https://github.com/woonstadrotterdam/woningwaardering.git
 cd woningwaardering
 pip install -e ".[dev]"
 ```
 
 ### Naamgeving van classes
 
 Voor de naamgeving van de classes in de woningwaardering module volgen we de VERA referentiedata. Deze referentiedata is gedefinieerd in de referentiedata enums, te vinden onder [woningwaardering/vera/referentiedata](woningwaardering/vera/referentiedata).
```

### Comparing `woningwaardering-0.2.16a0/README.md` & `woningwaardering-0.3.0a0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 ## 2. Contributing
 
 ### Setup
 
 Om de woningwaardering-package en de daarbij behorende developer dependencies te installeren, run onderstaand command:
 
 ```
-git clone https://github.com/WoonstadRotterdamTemp/woningwaardering.git
+git clone https://github.com/woonstadrotterdam/woningwaardering.git
 cd woningwaardering
 pip install -e ".[dev]"
 ```
 
 ### Naamgeving van classes
 
 Voor de naamgeving van de classes in de woningwaardering module volgen we de VERA referentiedata. Deze referentiedata is gedefinieerd in de referentiedata enums, te vinden onder [woningwaardering/vera/referentiedata](woningwaardering/vera/referentiedata).
```

### Comparing `woningwaardering-0.2.16a0/docs/afbeeldingen/excel_viewer.png` & `woningwaardering-0.3.0a0/docs/afbeeldingen/excel_viewer.png`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/docs/afbeeldingen/oppervlakte_van_vertrekken.excalidraw` & `woningwaardering-0.3.0a0/docs/afbeeldingen/oppervlakte_van_vertrekken.excalidraw`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/docs/afbeeldingen/oppervlakte_van_vertrekken.png` & `woningwaardering-0.3.0a0/docs/afbeeldingen/oppervlakte_van_vertrekken.png`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/docs/implementatietoelichting-beleidsboeken/2024/zelfstandige_woonruimten.md` & `woningwaardering-0.3.0a0/docs/implementatietoelichting-beleidsboeken/2024/zelfstandige_woonruimten.md`

 * *Files 12% similar despite different names*

```diff
@@ -440,8 +440,94 @@
 ~~Het eigen oordeel is uitsluitend in de voorliggende zaak van kracht, wordt niet geregistreerd in het register van de Rijksdienst voor Ondernemend Nederland en komt te vervallen na ontbinding van de huurovereenkomst.~~
 
 > Wanneer een eigen oordeel van kracht is, en de waardering daarop gebaseerd moet worden, dient de gewijzigde energieprestatie opgegeven te worden in plaats van de geregistreerde energieprestatie.
 
 ### 4.5.6 Energieprestatievergoeding
 Voor woningen die zelf (gedeeltelijk) in hun energieverbruik voorzien, door bijvoorbeeld zonnepanelen, kan bij het verhuren een energieprestatievergoeding (EPV) worden afgesproken. De woning zal dan moeten voldoen aan de eisen voor een EPV. Als dit het geval is dan is het aantal punten op basis van het puntenstelsel voor energieprestatie lager. Om te voorkomen dat in de gevallen waarin een energieprestatievergoeding is overeengekomen, de opwekking van energie voor de huurder tevens wordt verdisconteerd in de huurprijs, wordt voor deze woningen een correctiefactor toegepast op het aantal punten voor de energieprestatie. In die gevallen wordt de energieprestatie gewaardeerd met een aantal punten gelijk aan de waardering voor een Energie-Index 1,2 < EI ≤ 1,4 (of Energielabel B), met 32 punten voor een ééngezinswoning en 28 punten voor meergezins- en duplexwoningen.
 
-> Hiervoor is het `EenhedenEnergieprestatie` model uitgebreid met het attribuut `energieprestatievergoeding`. Dit attribuut dient gevuld te zijn met een boolean die aangeeft of er bij het verhuren een energieprestatievergoeding (EPV) is overeengekomen.
+> Hiervoor is het `EenhedenEnergieprestatie` model uitgebreid met het attribuut `energieprestatievergoeding`. Dit attribuut dient gevuld te zijn met een boolean die aangeeft of er bij het verhuren een energieprestatievergoeding (EPV) is overeengekomen.
+
+## 4.7 Sanitair
+Het woningwaarderingsstelsel kent aan een zelfstandige woonruimte punten toe voor het
+onderdeel sanitair. De waardering van het sanitair wordt bepaald op grond van de aanwezigheid
+van bepaalde voorzieningen binnen de woning. Hieronder wordt uiteengezet aan welke sanitaire
+voorzieningen punten worden toegekend en hoeveel punten die voorzieningen krijgen. Ook wordt
+besproken wanneer er extra kwaliteitspunten worden toegekend aan deze sanitaire
+voorzieningen.
+### 4.7.1 Sanitaire voorzieningen
+Het woningwaarderingsstelsel geeft punten aan de sanitaire voorzieningen toilet, wastafel, bad
+en douche. De puntentoekenning is als volgt:
+| Voorziening | Punten |
+| -------- | -------- |
+| toilet   | 3   |
+| wastafel  | 1  |
+| bidet    | 1  |
+| lavet*   | 1  |
+| douche   | 4  |
+| bad      | 6  |
+| bad en douche | 7  |
+
+> De punten hierboven in de tabel zijn het aantal punten dat wordt toegekend aan de sanitaire voorziening. De gedetailleerde voorwaarden die hieronder volgen in het beleidsboek worden niet getoetst in de implementatie. Het is aan de gebruiker om alleen voorzieningen op te geven die voldoen aan de voorwaarden.
+
+~~_*Een lavet wordt met vier punten gewaardeerd, als deze is voorzien van aansluitpunten voor warm en koud
+water én van douchegarnituur._~~
+
+**Toilet**  
+Drie punten worden toegekend aan een toilet ~~met waterspoeling als het toilet is geplaatst in een
+daartoe bestemde ruimte en als het toilet binnen het woongebouw is gelegen. Wanneer sprake is
+van een toilet dat buiten de woning maar binnen het woongebouw is gelegen, dan geldt dat het
+toilet in de waardering wordt meegenomen als het gebruik van het toilet door derden is uit te
+sluiten.~~  
+
+**Wastafel**  
+Wastafels worden met één punt gewaardeerd. ~~Als wastafels worden alle bakken geteld voor
+wassen en spoelen die op de waterleiding én op het huisriool zijn aangesloten. Een dergelijke bak
+wordt niet als wastafel gewaardeerd indien boven de bak een douche is aangebracht. Een bad en
+spoelbakken in een keukenaanrecht worden niet als wastafels gewaardeerd.
+Als wastafel waardeert de Huurcommissie een fonteintje en een aanrecht dat niet voor punten in
+aanmerking komt, waarvan de aanrechtlengte korter is dan één meter.~~
+
+**Bad en douche**  
+Douches worden gewaardeerd met vier punten. ~~Als douche wordt meegeteld iedere door de
+verhuurder aangebrachte installatie voor het nemen van een stortbad. Hieronder valt eveneens
+een zogenaamde douchecabine, die voldoet aan bovengenoemde voorwaarden, als de douchecabine
+in een vertrek (anders dan bad- of doucheruimte) of overige ruimte is geplaatst. De oppervlakte van dat vertrek of van die overige ruimte wordt in dat geval niet verminderd met de door de
+douchecabine ingenomen oppervlakte.~~
+Aan baden worden zes punten toegekend, ~~ongeacht de lengte van het bad. Indien een bad is
+voorzien van een (hand)douche, dan wordt het douchegarnituur niet afzonderlijk geteld.~~
+Indien in de badruimte behalve het bad tevens een afzonderlijke douche is aangebracht, geldt een
+waardering van zeven punten.  
+
+> Het is ambigu hoeveel punten er zouden moeten worden toegekend indien een badruimte meer dan één douche bevat en één bad of vice versa. I.v.m. de onwaarschijnlijkheid van het voortkomen van deze situatie is er gekozen om deze situatie niet te ondersteunen in de implementatie. Indien er een bad en een douche in dezelfde ruimte aanwezig zijn worden er 7 punten toegekend per combinatie van bad en douche.  
+>
+> Oftewel:
+>
+> - één bad en één douche in dezelfde ruimte: 7 punten  
+> - één bad en twee douches in dezelfde ruimte: 7 punten
+> - twee baden en één douche in dezelfde ruimte: 7 punten
+> - twee baden en twee douches in dezelfde ruimte: 14 punten
+
+~~**Voorzieningen in een bad- en doucheruimte**~~  
+~~Indien sprake is van sanitaire voorzieningen in een bad- of doucheruimte*, dan worden alleen
+punten toegekend aan die voorzieningen indien de bad -of doucheruimte voldoet aan drie
+voorwaarden.
+Ten eerste moet de wand- en vloerafwerking van de bad- of douchruimte voldoende waterdicht
+zijn. Een bad in een vertrek met een niet-waterdichte vloer wordt door de Huurcommissie wel
+gewaardeerd, omdat het bad zelf als een waterdichte afwerking wordt gezien. Ten tweede moet
+de bad- en doucheruimte zijn voorzien van aansluitingspunten voor warm en koud water. Met
+aansluitingspunten voor warm en koud water wordt niet een warmwater apparaat bedoeld. Als
+sprake is van een geiser of boiler dan hoeven deze niet door de verhuurder te zijn verstrekt. Ten
+derde moet het bad of de douche zijn voorzien van douchegarnituur. Met douchegarnituur bedoelt
+de Huurcommissie een warm- en koudwaterkraan of een mengkraan.
+Indien het aansluitpunt voor warm en koud water bedoeld is voor gecombineerd gebruik van
+zowel een wastafel als de naastgelegen douche of bad (bijvoorbeeld door middel van een
+zogenaamde zwenkarm), dan wordt uitsluitend de douche of het bad gewaardeerd. Dus niet én 1
+punt voor wastafel én 4 of 6 punten voor douche of lavet, respectievelijk bad.
+Indien in de bad- of doucheruimte een toilet is geplaatst wordt dit toilet volledig gewaardeerd met
+drie punten.~~
+
+~~_*De Huurcommissie verstaat onder een bad-/doucheruimte een (afzonderlijke) ruimte met een vrije hoogte van ten
+minste 2 meter, gemeten vanaf de vloer tot aan het zichtbare plafond. Daarin dient tenminste aanwezig te zijn een
+wastafel of een douche of een bad. Voor een gecombineerde bad-/douche- en toiletruimte geldt, vanwege de
+oppervlakte-eis voor toilet- ruimten, een minimale oppervlakte van 0,64 m2 . Indien een douche- of badruimte,
+eventueel gecombineerd met een toilet, niet een vrije hoogte heeft van 2,00 m, dan wordt de ruimte gewaardeerd
+als overige ruimte._~~
```

### Comparing `woningwaardering-0.2.16a0/pyproject.toml` & `woningwaardering-0.3.0a0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -28,16 +28,16 @@
     "types-pyyaml==6.*",
     "PyYAML==6.*",
     "prettytable==3.*",
     "pandas==2.*"
 ]
 
 [project.urls]
-Homepage = "https://github.com/WoonstadRotterdamTemp/woningwaardering"
-Issues = "https://github.com/WoonstadRotterdamTemp/woningwaardering/issues"
+Homepage = "https://github.com/woonstadrotterdam/woningwaardering"
+Issues = "https://github.com/woonstadrotterdam/woningwaardering/issues"
 
 [tool.setuptools.packages.find]
 include = ["woningwaardering*"]
 
 [tool.setuptools_scm]
 version_file = "woningwaardering/_version.py"
```

### Comparing `woningwaardering-0.2.16a0/scripts/genereer_opzet_woningwaarderinggroep.py` & `woningwaardering-0.3.0a0/scripts/genereer_opzet_woningwaarderinggroep.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/scripts/genereer_test_output.py` & `woningwaardering-0.3.0a0/scripts/genereer_test_output.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/scripts/genereer_vera_referentiedata.py` & `woningwaardering-0.3.0a0/scripts/genereer_vera_referentiedata.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/scripts/uitbreiden_vera_modellen.py` & `woningwaardering-0.3.0a0/scripts/uitbreiden_vera_modellen.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/taskfile.yml` & `woningwaardering-0.3.0a0/taskfile.yml`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/conftest.py` & `woningwaardering-0.3.0a0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/data/input/generiek/37101000032.json` & `woningwaardering-0.3.0a0/tests/data/input/generiek/37101000032.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/12006000004.json` & `woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/12006000004.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/23003000050.json` & `woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/23003000050.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/25048000007.json` & `woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/25048000007.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/28018000044.json` & `woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/28018000044.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/37101000032.json` & `woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/37101000032.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/41027000003.json` & `woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/41027000003.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/41123000005.json` & `woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/41123000005.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/41162000015.json` & `woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/41162000015.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/41164000002.json` & `woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/41164000002.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/51011000042.json` & `woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/51011000042.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/71211000027.json` & `woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/71211000027.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/77795000000.json` & `woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/77795000000.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/81020000003.json` & `woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/81020000003.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/81065000089.json` & `woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/81065000089.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/85651000021.json` & `woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/85651000021.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/data/input/zelfstandige_woonruimten/87402000003.json` & `woningwaardering-0.3.0a0/tests/data/input/zelfstandige_woonruimten/87402000003.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/12006000004.json` & `woningwaardering-0.3.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/25048000007.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7734722222222222%*

 * *Differences: {"'groepen'": "{0: {'punten': 61.0, 'woningwaarderingen': {0: {'aantal': 30.12, 'criterium': "*

 * *              "{'naam': 'Woonkamer'}}, 1: {'aantal': 11.72, 'criterium': {'naam': 'Slaapkamer'}}, "*

 * *              "2: {'aantal': 4.64, 'criterium': {'naam': 'Badruimte'}}, 3: {'aantal': 9.21}, 4: "*

 * *              "{'aantal': 5.76, 'criterium': {'naam': 'Keuken'}}}}, 1: {'punten': 3.75, "*

 * *              "'woningwaarderingen': [OrderedDict([('aantal', 5.1), ('criterium', "*

 * *              "OrderedDict([('naam', 'Berging […]*

```diff
@@ -7,64 +7,64 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OVZ",
                     "naam": "Oppervlakte van vertrekken"
                 }
             },
-            "punten": 60.0,
+            "punten": 61.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 3.58,
+                    "aantal": 30.12,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Badruimte"
+                        "naam": "Woonkamer"
                     }
                 },
                 {
-                    "aantal": 10.18,
+                    "aantal": 11.72,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Keuken + 2 kasten"
+                        "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 26.82,
+                    "aantal": 4.64,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Woonkamer + 1 kast"
+                        "naam": "Badruimte"
                     }
                 },
                 {
-                    "aantal": 6.49,
+                    "aantal": 9.21,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 12.98,
+                    "aantal": 5.76,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer"
+                        "naam": "Keuken"
                     }
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
@@ -72,16 +72,27 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OOZ",
                     "naam": "Oppervlakte van overige ruimten"
                 }
             },
-            "punten": 0.0,
-            "woningwaarderingen": []
+            "punten": 3.75,
+            "woningwaarderingen": [
+                {
+                    "aantal": 5.1,
+                    "criterium": {
+                        "meeteenheid": {
+                            "code": "M2",
+                            "naam": "Vierkante meter, m2"
+                        },
+                        "naam": "Berging"
+                    }
+                }
+            ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
                     "code": "ZEL",
                     "naam": "Zelfstandige woonruimten"
                 },
@@ -90,39 +101,39 @@
                     "naam": "Verwarming"
                 }
             },
             "punten": 10.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "Badruimte"
+                        "naam": "Woonkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Keuken"
+                        "naam": "Slaapkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Woonkamer"
+                        "naam": "Badruimte"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Slaapkamer"
+                        "naam": "Keuken"
                     },
                     "punten": 2.0
                 }
             ]
         },
         {
             "criteriumGroep": {
@@ -131,24 +142,38 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "ENE",
                     "naam": "Energieprestatie"
                 }
             },
-            "punten": 5.0,
+            "punten": 28.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "Bouwjaar 1981"
+                        "naam": "B (oud)"
                     },
-                    "punten": 5.0
+                    "punten": 28.0
                 }
             ]
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
+                },
+                "stelselgroep": {
+                    "code": "SAN",
+                    "naam": "Sanitair"
+                }
+            },
+            "punten": 0.0,
+            "woningwaarderingen": []
         }
     ],
-    "punten": 75.0,
+    "punten": 103.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/23003000050.json` & `woningwaardering-0.3.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/87402000003.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7776388888888889%*

 * *Differences: {"'groepen'": "{0: {'punten': 53.0, 'woningwaarderingen': {0: {'aantal': 11.65}, 1: {'aantal': "*

 * *              "3.12, 'criterium': {'naam': 'Badruimte'}}, 2: {'aantal': 6.37, 'criterium': "*

 * *              "{'naam': 'Keuken'}}, 3: {'aantal': 23.1, 'criterium': {'naam': 'Woonkamer'}}, 4: "*

 * *              "{'aantal': 8.35, 'criterium': {'naam': 'Slaapkamer'}}}}, 1: {'punten': 3.75, "*

 * *              "'woningwaarderingen': {0: {'aantal': 5.25}}}, 2: {'woningwaarderingen': {1: "*

 * *              "{'criterium': {'naam': […]*

```diff
@@ -7,64 +7,64 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OVZ",
                     "naam": "Oppervlakte van vertrekken"
                 }
             },
-            "punten": 61.0,
+            "punten": 53.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 11.88,
+                    "aantal": 11.65,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 9.73,
+                    "aantal": 3.12,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer"
+                        "naam": "Badruimte"
                     }
                 },
                 {
-                    "aantal": 22.85,
+                    "aantal": 6.37,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Woonkamer"
+                        "naam": "Keuken"
                     }
                 },
                 {
-                    "aantal": 3.94,
+                    "aantal": 23.1,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Badruimte"
+                        "naam": "Woonkamer"
                     }
                 },
                 {
-                    "aantal": 12.22,
+                    "aantal": 8.35,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Keuken"
+                        "naam": "Slaapkamer"
                     }
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
@@ -72,18 +72,18 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OOZ",
                     "naam": "Oppervlakte van overige ruimten"
                 }
             },
-            "punten": 3.0,
+            "punten": 3.75,
             "woningwaarderingen": [
                 {
-                    "aantal": 4.41,
+                    "aantal": 5.25,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Berging"
                     }
@@ -107,33 +107,33 @@
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Slaapkamer"
+                        "naam": "Badruimte"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Woonkamer"
+                        "naam": "Keuken"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Badruimte"
+                        "naam": "Woonkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Keuken"
+                        "naam": "Slaapkamer"
                     },
                     "punten": 2.0
                 }
             ]
         },
         {
             "criteriumGroep": {
@@ -142,24 +142,38 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "ENE",
                     "naam": "Energieprestatie"
                 }
             },
-            "punten": 15.0,
+            "punten": 0.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "C (oud)"
+                        "naam": "Bouwjaar 1898"
                     },
-                    "punten": 15.0
+                    "punten": 0.0
                 }
             ]
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
+                },
+                "stelselgroep": {
+                    "code": "SAN",
+                    "naam": "Sanitair"
+                }
+            },
+            "punten": 0.0,
+            "woningwaarderingen": []
         }
     ],
-    "punten": 89.0,
+    "punten": 67.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/25048000007.json` & `woningwaardering-0.3.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/81065000089.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7689930555555556%*

 * *Differences: {"'groepen'": "{0: {'punten': 58.0, 'woningwaarderingen': {0: {'aantal': 11.63, 'criterium': "*

 * *              "{'naam': 'Slaapkamer'}}, 1: {'aantal': 7.62}, 2: {'aantal': 17.77, 'criterium': "*

 * *              "{'naam': 'Woonkamer'}}, 3: {'aantal': 12.72, 'criterium': {'naam': 'Keuken'}}, 4: "*

 * *              "{'aantal': 8.34, 'criterium': {'naam': 'Slaapkamer'}}}}, 1: {'punten': 4.5, "*

 * *              "'woningwaarderingen': {1: {'aantal': 2.86, 'criterium': {'naam': 'Wasruimte'}}, "*

 * *              "insert: [(0, Ord […]*

```diff
@@ -7,64 +7,64 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OVZ",
                     "naam": "Oppervlakte van vertrekken"
                 }
             },
-            "punten": 61.0,
+            "punten": 58.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 30.12,
+                    "aantal": 11.63,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Woonkamer"
+                        "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 11.72,
+                    "aantal": 7.62,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 4.64,
+                    "aantal": 17.77,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Badruimte"
+                        "naam": "Woonkamer"
                     }
                 },
                 {
-                    "aantal": 9.21,
+                    "aantal": 12.72,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer"
+                        "naam": "Keuken"
                     }
                 },
                 {
-                    "aantal": 5.76,
+                    "aantal": 8.34,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Keuken"
+                        "naam": "Slaapkamer"
                     }
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
@@ -72,24 +72,34 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OOZ",
                     "naam": "Oppervlakte van overige ruimten"
                 }
             },
-            "punten": 3.75,
+            "punten": 4.5,
             "woningwaarderingen": [
                 {
-                    "aantal": 5.1,
+                    "aantal": 3.56,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Berging"
+                        "naam": "Zolder"
+                    }
+                },
+                {
+                    "aantal": 2.86,
+                    "criterium": {
+                        "meeteenheid": {
+                            "code": "M2",
+                            "naam": "Vierkante meter, m2"
+                        },
+                        "naam": "Wasruimte"
                     }
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
@@ -97,69 +107,97 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "VZE",
                     "naam": "Verwarming"
                 }
             },
-            "punten": 10.0,
+            "punten": 11.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "Woonkamer"
+                        "naam": "Slaapkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Badruimte"
+                        "naam": "Woonkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Slaapkamer"
+                        "naam": "Wasruimte"
                     },
-                    "punten": 2.0
+                    "punten": 1.0
                 },
                 {
                     "criterium": {
                         "naam": "Keuken"
                     },
                     "punten": 2.0
+                },
+                {
+                    "criterium": {
+                        "naam": "Slaapkamer"
+                    },
+                    "punten": 2.0
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
                     "code": "ZEL",
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "ENE",
                     "naam": "Energieprestatie"
                 }
             },
-            "punten": 28.0,
+            "punten": 32.0,
+            "woningwaarderingen": [
+                {
+                    "criterium": {
+                        "naam": "B + 78.84m2"
+                    },
+                    "punten": 32.0
+                }
+            ]
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
+                },
+                "stelselgroep": {
+                    "code": "SAN",
+                    "naam": "Sanitair"
+                }
+            },
+            "punten": 4.0,
             "woningwaarderingen": [
                 {
+                    "aantal": 1.0,
                     "criterium": {
-                        "naam": "B (oud)"
+                        "naam": "Douche"
                     },
-                    "punten": 28.0
+                    "punten": 4.0
                 }
             ]
         }
     ],
-    "punten": 103.0,
+    "punten": 110.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/28018000044.json` & `woningwaardering-0.3.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/23003000050.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7766782407407408%*

 * *Differences: {"'groepen'": "{0: {'punten': 61.0, 'woningwaarderingen': {0: {'aantal': 11.88}, 1: {'aantal': "*

 * *              "9.73}, 2: {'aantal': 22.85}, 3: {'aantal': 3.94}, 4: {'aantal': 12.22, 'criterium': "*

 * *              "{'naam': 'Keuken'}}, delete: [2]}}, 1: {'woningwaarderingen': {0: {'aantal': "*

 * *              "4.41}}}, 2: {'punten': 10.0, 'woningwaarderingen': {4: {'criterium': {'naam': "*

 * *              "'Keuken'}}, delete: [2]}}, 3: {'punten': 15.0, 'woningwaarderingen': {0: "*

 * *              "{'criterium': {'naam […]*

```diff
@@ -7,74 +7,64 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OVZ",
                     "naam": "Oppervlakte van vertrekken"
                 }
             },
-            "punten": 67.0,
+            "punten": 61.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 10.0,
+                    "aantal": 11.88,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 7.02,
+                    "aantal": 9.73,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 7.64,
-                    "criterium": {
-                        "meeteenheid": {
-                            "code": "M2",
-                            "naam": "Vierkante meter, m2"
-                        },
-                        "naam": "Keuken"
-                    }
-                },
-                {
-                    "aantal": 23.62,
+                    "aantal": 22.85,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Woonkamer"
                     }
                 },
                 {
-                    "aantal": 5.18,
+                    "aantal": 3.94,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Badruimte"
                     }
                 },
                 {
-                    "aantal": 13.35,
+                    "aantal": 12.22,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer"
+                        "naam": "Keuken"
                     }
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
@@ -85,15 +75,15 @@
                     "code": "OOZ",
                     "naam": "Oppervlakte van overige ruimten"
                 }
             },
             "punten": 3.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 4.1,
+                    "aantal": 4.41,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Berging"
                     }
@@ -107,15 +97,15 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "VZE",
                     "naam": "Verwarming"
                 }
             },
-            "punten": 12.0,
+            "punten": 10.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
                     "punten": 2.0
                 },
@@ -123,33 +113,27 @@
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Keuken"
-                    },
-                    "punten": 2.0
-                },
-                {
-                    "criterium": {
                         "naam": "Woonkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
                         "naam": "Badruimte"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Slaapkamer"
+                        "naam": "Keuken"
                     },
                     "punten": 2.0
                 }
             ]
         },
         {
             "criteriumGroep": {
@@ -158,24 +142,60 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "ENE",
                     "naam": "Energieprestatie"
                 }
             },
-            "punten": 22.0,
+            "punten": 15.0,
+            "woningwaarderingen": [
+                {
+                    "criterium": {
+                        "naam": "C (oud)"
+                    },
+                    "punten": 15.0
+                }
+            ]
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
+                },
+                "stelselgroep": {
+                    "code": "SAN",
+                    "naam": "Sanitair"
+                }
+            },
+            "punten": 9.0,
             "woningwaarderingen": [
                 {
+                    "aantal": 1.0,
+                    "criterium": {
+                        "naam": "Closetcombinatie"
+                    },
+                    "punten": 3.0
+                },
+                {
+                    "aantal": 2.0,
+                    "criterium": {
+                        "naam": "Wastafel"
+                    },
+                    "punten": 2.0
+                },
+                {
+                    "aantal": 1.0,
                     "criterium": {
-                        "naam": "Bouwjaar 1992"
+                        "naam": "Douche"
                     },
-                    "punten": 22.0
+                    "punten": 4.0
                 }
             ]
         }
     ],
-    "punten": 104.0,
+    "punten": 98.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/37101000032.json` & `woningwaardering-0.3.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/81020000003.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7698908730158731%*

 * *Differences: {"'groepen'": "{0: {'punten': 79.0, 'woningwaarderingen': {0: {'aantal': 3.8, 'criterium': "*

 * *              "{'naam': 'Badruimte'}}, 1: {'aantal': 15.74, 'criterium': {'naam': 'Slaapkamer'}}, "*

 * *              "2: {'aantal': 5.92}, 3: {'aantal': 15.15}, 4: {'aantal': 26.54, 'criterium': "*

 * *              "{'naam': 'Woonkamer + 1 kast'}}, 5: {'aantal': 12.23}, delete: [3]}}, 1: {'punten': "*

 * *              "3.75, 'woningwaarderingen': {0: {'aantal': 5.19}}}, 2: {'punten': 9.0, "*

 * *              "'woningwaarderingen': […]*

```diff
@@ -7,78 +7,68 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OVZ",
                     "naam": "Oppervlakte van vertrekken"
                 }
             },
-            "punten": 140.0,
+            "punten": 79.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 21.05,
+                    "aantal": 3.8,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer"
+                        "naam": "Badruimte"
                     }
                 },
                 {
-                    "aantal": 41.0,
+                    "aantal": 15.74,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Woonkamer"
+                        "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 20.37,
+                    "aantal": 5.92,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Keuken"
                     }
                 },
                 {
-                    "aantal": 6.5,
-                    "criterium": {
-                        "meeteenheid": {
-                            "code": "M2",
-                            "naam": "Vierkante meter, m2"
-                        },
-                        "naam": "Badruimte"
-                    }
-                },
-                {
-                    "aantal": 15.98,
+                    "aantal": 15.15,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 19.15,
+                    "aantal": 26.54,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer"
+                        "naam": "Woonkamer + 1 kast"
                     }
                 },
                 {
-                    "aantal": 15.82,
+                    "aantal": 12.23,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
@@ -92,18 +82,18 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OOZ",
                     "naam": "Oppervlakte van overige ruimten"
                 }
             },
-            "punten": 5.25,
+            "punten": 3.75,
             "woningwaarderingen": [
                 {
-                    "aantal": 6.65,
+                    "aantal": 5.19,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Berging"
                     }
@@ -117,81 +107,111 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "VZE",
                     "naam": "Verwarming"
                 }
             },
-            "punten": 14.0,
+            "punten": 9.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "Slaapkamer"
+                        "naam": "Badruimte"
                     },
-                    "punten": 2.0
+                    "punten": 1.5
                 },
                 {
                     "criterium": {
-                        "naam": "Woonkamer"
+                        "naam": "Slaapkamer"
                     },
-                    "punten": 2.0
+                    "punten": 1.5
                 },
                 {
                     "criterium": {
                         "naam": "Keuken"
                     },
-                    "punten": 2.0
+                    "punten": 1.5
                 },
                 {
                     "criterium": {
-                        "naam": "Badruimte"
+                        "naam": "Slaapkamer"
                     },
-                    "punten": 2.0
+                    "punten": 1.5
                 },
                 {
                     "criterium": {
-                        "naam": "Slaapkamer"
+                        "naam": "Woonkamer"
                     },
-                    "punten": 2.0
+                    "punten": 1.5
                 },
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
-                    "punten": 2.0
+                    "punten": 1.5
+                }
+            ]
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
                 },
+                "stelselgroep": {
+                    "code": "ENE",
+                    "naam": "Energieprestatie"
+                }
+            },
+            "punten": 36.0,
+            "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "Slaapkamer"
+                        "naam": "A (oud)"
                     },
-                    "punten": 2.0
+                    "punten": 36.0
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
                     "code": "ZEL",
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
-                    "code": "ENE",
-                    "naam": "Energieprestatie"
+                    "code": "SAN",
+                    "naam": "Sanitair"
                 }
             },
-            "punten": 22.0,
+            "punten": 12.0,
             "woningwaarderingen": [
                 {
+                    "aantal": 2.0,
+                    "criterium": {
+                        "naam": "Closetcombinatie"
+                    },
+                    "punten": 6.0
+                },
+                {
+                    "aantal": 2.0,
+                    "criterium": {
+                        "naam": "Wastafel"
+                    },
+                    "punten": 2.0
+                },
+                {
+                    "aantal": 1.0,
                     "criterium": {
-                        "naam": "C (oud)"
+                        "naam": "Douche"
                     },
-                    "punten": 22.0
+                    "punten": 4.0
                 }
             ]
         }
     ],
-    "punten": 181.0,
+    "punten": 140.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41027000003.json` & `woningwaardering-0.3.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/12006000004.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.791875%*

 * *Differences: {"'groepen'": "{0: {'punten': 60.0, 'woningwaarderingen': {0: {'aantal': 3.58}, 1: {'aantal': "*

 * *              "10.18, 'criterium': {'naam': 'Keuken + 2 kasten'}}, 2: {'aantal': 26.82}, 3: "*

 * *              "{'aantal': 6.49, 'criterium': {'naam': 'Slaapkamer'}}, 4: {'aantal': 12.98, "*

 * *              "'criterium': {'naam': 'Slaapkamer'}}}}, 2: {'woningwaarderingen': {1: {'criterium': "*

 * *              "{'naam': 'Keuken'}}, 3: {'criterium': {'naam': 'Slaapkamer'}}}}, 3: "*

 * *              "{'woningwaarderingen': {0: { […]*

```diff
@@ -7,64 +7,64 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OVZ",
                     "naam": "Oppervlakte van vertrekken"
                 }
             },
-            "punten": 43.0,
+            "punten": 60.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 2.18,
+                    "aantal": 3.58,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Badruimte"
                     }
                 },
                 {
-                    "aantal": 12.1,
+                    "aantal": 10.18,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer + 1 kast"
+                        "naam": "Keuken + 2 kasten"
                     }
                 },
                 {
-                    "aantal": 16.65,
+                    "aantal": 26.82,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Woonkamer + 1 kast"
                     }
                 },
                 {
-                    "aantal": 4.84,
+                    "aantal": 6.49,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Keuken + 1 kast"
+                        "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 6.84,
+                    "aantal": 12.98,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer + 2 kasten"
+                        "naam": "Slaapkamer"
                     }
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
@@ -96,27 +96,27 @@
                     "criterium": {
                         "naam": "Badruimte"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Slaapkamer"
+                        "naam": "Keuken"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
                         "naam": "Woonkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Keuken"
+                        "naam": "Slaapkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
@@ -135,20 +135,56 @@
                     "naam": "Energieprestatie"
                 }
             },
             "punten": 5.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "E (oud)"
+                        "naam": "Bouwjaar 1981"
                     },
                     "punten": 5.0
                 }
             ]
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
+                },
+                "stelselgroep": {
+                    "code": "SAN",
+                    "naam": "Sanitair"
+                }
+            },
+            "punten": 9.0,
+            "woningwaarderingen": [
+                {
+                    "aantal": 2.0,
+                    "criterium": {
+                        "naam": "Wastafel"
+                    },
+                    "punten": 2.0
+                },
+                {
+                    "aantal": 1.0,
+                    "criterium": {
+                        "naam": "Douche"
+                    },
+                    "punten": 4.0
+                },
+                {
+                    "aantal": 1.0,
+                    "criterium": {
+                        "naam": "Closetcombinatie"
+                    },
+                    "punten": 3.0
+                }
+            ]
         }
     ],
-    "punten": 58.0,
+    "punten": 84.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41123000005.json` & `woningwaardering-0.3.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41123000005.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7999999999999999%*

 * *Differences: {"'groepen'": "{insert: [(4, OrderedDict([('criteriumGroep', OrderedDict([('stelsel', "*

 * *              "OrderedDict([('code', 'ZEL'), ('naam', 'Zelfstandige woonruimten')])), "*

 * *              "('stelselgroep', OrderedDict([('code', 'SAN'), ('naam', 'Sanitair')]))])), "*

 * *              "('punten', 20.0), ('woningwaarderingen', [OrderedDict([('aantal', 2.0), "*

 * *              "('criterium', OrderedDict([('naam', 'Wastafel')])), ('punten', 2.0)]), "*

 * *              "OrderedDict([('aantal', 3.0), ('criterium', OrderedD […]*

```diff
@@ -257,15 +257,51 @@
                 {
                     "criterium": {
                         "naam": "B (oud)"
                     },
                     "punten": 32.0
                 }
             ]
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
+                },
+                "stelselgroep": {
+                    "code": "SAN",
+                    "naam": "Sanitair"
+                }
+            },
+            "punten": 20.0,
+            "woningwaarderingen": [
+                {
+                    "aantal": 2.0,
+                    "criterium": {
+                        "naam": "Wastafel"
+                    },
+                    "punten": 2.0
+                },
+                {
+                    "aantal": 3.0,
+                    "criterium": {
+                        "naam": "Douche"
+                    },
+                    "punten": 12.0
+                },
+                {
+                    "aantal": 2.0,
+                    "criterium": {
+                        "naam": "Closetcombinatie"
+                    },
+                    "punten": 6.0
+                }
+            ]
         }
     ],
-    "punten": 173.0,
+    "punten": 193.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41162000015.json` & `woningwaardering-0.3.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41162000015.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7999999999999999%*

 * *Differences: {"'groepen'": "{insert: [(4, OrderedDict([('criteriumGroep', OrderedDict([('stelsel', "*

 * *              "OrderedDict([('code', 'ZEL'), ('naam', 'Zelfstandige woonruimten')])), "*

 * *              "('stelselgroep', OrderedDict([('code', 'SAN'), ('naam', 'Sanitair')]))])), "*

 * *              "('punten', 9.0), ('woningwaarderingen', [OrderedDict([('aantal', 2.0), "*

 * *              "('criterium', OrderedDict([('naam', 'Wastafel')])), ('punten', 2.0)]), "*

 * *              "OrderedDict([('aantal', 1.0), ('criterium', OrderedDi […]*

```diff
@@ -177,15 +177,51 @@
                 {
                     "criterium": {
                         "naam": "C (oud)"
                     },
                     "punten": 15.0
                 }
             ]
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
+                },
+                "stelselgroep": {
+                    "code": "SAN",
+                    "naam": "Sanitair"
+                }
+            },
+            "punten": 9.0,
+            "woningwaarderingen": [
+                {
+                    "aantal": 2.0,
+                    "criterium": {
+                        "naam": "Wastafel"
+                    },
+                    "punten": 2.0
+                },
+                {
+                    "aantal": 1.0,
+                    "criterium": {
+                        "naam": "Douche"
+                    },
+                    "punten": 4.0
+                },
+                {
+                    "aantal": 1.0,
+                    "criterium": {
+                        "naam": "Closetcombinatie"
+                    },
+                    "punten": 3.0
+                }
+            ]
         }
     ],
-    "punten": 89.0,
+    "punten": 98.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41164000002.json` & `woningwaardering-0.3.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/71211000027.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7686755952380953%*

 * *Differences: {"'groepen'": "{0: {'punten': 54.0, 'woningwaarderingen': {0: {'aantal': 15.89, 'criterium': "*

 * *              "{'naam': 'Woonkamer + 1 kast'}}, 1: {'aantal': 10.63, 'criterium': {'naam': "*

 * *              "'Keuken'}}, 2: {'aantal': 9.08}, 3: {'aantal': 4.73}, 4: {'aantal': 8.72, "*

 * *              "'criterium': {'naam': 'Slaapkamer'}}, 5: {'aantal': 4.94, 'criterium': {'naam': "*

 * *              "'Badruimte'}}, delete: [3]}}, 1: {'punten': 6.75, 'woningwaarderingen': {1: "*

 * *              "{'aantal': 5.05, 'criterium' […]*

```diff
@@ -7,84 +7,74 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OVZ",
                     "naam": "Oppervlakte van vertrekken"
                 }
             },
-            "punten": 138.0,
+            "punten": 54.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 6.33,
+                    "aantal": 15.89,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Badruimte"
+                        "naam": "Woonkamer + 1 kast"
                     }
                 },
                 {
-                    "aantal": 23.42,
+                    "aantal": 10.63,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer + 1 kast"
+                        "naam": "Keuken"
                     }
                 },
                 {
-                    "aantal": 22.66,
+                    "aantal": 9.08,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 14.71,
-                    "criterium": {
-                        "meeteenheid": {
-                            "code": "M2",
-                            "naam": "Vierkante meter, m2"
-                        },
-                        "naam": "Keuken"
-                    }
-                },
-                {
-                    "aantal": 17.63,
+                    "aantal": 4.73,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 32.95,
+                    "aantal": 8.72,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Woonkamer"
+                        "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 20.45,
+                    "aantal": 4.94,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer + 1 kast"
+                        "naam": "Badruimte"
                     }
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
@@ -92,24 +82,34 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OOZ",
                     "naam": "Oppervlakte van overige ruimten"
                 }
             },
-            "punten": 3.0,
+            "punten": 6.75,
             "woningwaarderingen": [
                 {
-                    "aantal": 4.31,
+                    "aantal": 4.4,
+                    "criterium": {
+                        "meeteenheid": {
+                            "code": "M2",
+                            "naam": "Vierkante meter, m2"
+                        },
+                        "naam": "Zolder"
+                    }
+                },
+                {
+                    "aantal": 5.05,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Wasruimte"
+                        "naam": "Berging"
                     }
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
@@ -117,81 +117,111 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "VZE",
                     "naam": "Verwarming"
                 }
             },
-            "punten": 14.0,
+            "punten": 12.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "Badruimte"
+                        "naam": "Woonkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Slaapkamer"
+                        "naam": "Keuken"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Keuken"
+                        "naam": "Slaapkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Woonkamer"
+                        "naam": "Badruimte"
                     },
                     "punten": 2.0
+                }
+            ]
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
                 },
+                "stelselgroep": {
+                    "code": "ENE",
+                    "naam": "Energieprestatie"
+                }
+            },
+            "punten": 14.0,
+            "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "Slaapkamer"
+                        "naam": "D (oud)"
                     },
-                    "punten": 2.0
+                    "punten": 14.0
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
                     "code": "ZEL",
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
-                    "code": "ENE",
-                    "naam": "Energieprestatie"
+                    "code": "SAN",
+                    "naam": "Sanitair"
                 }
             },
-            "punten": 32.0,
+            "punten": 9.0,
             "woningwaarderingen": [
                 {
+                    "aantal": 1.0,
+                    "criterium": {
+                        "naam": "Closetcombinatie"
+                    },
+                    "punten": 3.0
+                },
+                {
+                    "aantal": 2.0,
+                    "criterium": {
+                        "naam": "Wastafel"
+                    },
+                    "punten": 2.0
+                },
+                {
+                    "aantal": 1.0,
                     "criterium": {
-                        "naam": "B (oud)"
+                        "naam": "Douche"
                     },
-                    "punten": 32.0
+                    "punten": 4.0
                 }
             ]
         }
     ],
-    "punten": 187.0,
+    "punten": 96.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/51011000042.json` & `woningwaardering-0.3.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41027000003.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7766865079365081%*

 * *Differences: {"'groepen'": "{0: {'punten': 43.0, 'woningwaarderingen': {0: {'aantal': 2.18, 'criterium': "*

 * *              "{'naam': 'Badruimte'}}, 1: {'aantal': 12.1}, 2: {'aantal': 16.65, 'criterium': "*

 * *              "{'naam': 'Woonkamer + 1 kast'}}, 3: {'aantal': 4.84, 'criterium': {'naam': 'Keuken "*

 * *              "+ 1 kast'}}, 4: {'aantal': 6.84, 'criterium': {'naam': 'Slaapkamer + 2 kasten'}}, "*

 * *              "delete: [3, 2]}}, 2: {'punten': 10.0, 'woningwaarderingen': {0: {'criterium': "*

 * *              "{'naam': 'Bad […]*

```diff
@@ -7,84 +7,64 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OVZ",
                     "naam": "Oppervlakte van vertrekken"
                 }
             },
-            "punten": 60.0,
+            "punten": 43.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 17.56,
+                    "aantal": 2.18,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Woonkamer + 1 kast"
+                        "naam": "Badruimte"
                     }
                 },
                 {
-                    "aantal": 11.8,
+                    "aantal": 12.1,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer + 1 kast"
                     }
                 },
                 {
-                    "aantal": 6.99,
+                    "aantal": 16.65,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer + 2 kasten"
-                    }
-                },
-                {
-                    "aantal": 8.15,
-                    "criterium": {
-                        "meeteenheid": {
-                            "code": "M2",
-                            "naam": "Vierkante meter, m2"
-                        },
-                        "naam": "Slaapkamer"
-                    }
-                },
-                {
-                    "aantal": 1.92,
-                    "criterium": {
-                        "meeteenheid": {
-                            "code": "M2",
-                            "naam": "Vierkante meter, m2"
-                        },
-                        "naam": "Badruimte"
+                        "naam": "Woonkamer + 1 kast"
                     }
                 },
                 {
-                    "aantal": 7.06,
+                    "aantal": 4.84,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Keuken"
+                        "naam": "Keuken + 1 kast"
                     }
                 },
                 {
-                    "aantal": 6.92,
+                    "aantal": 6.84,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer"
+                        "naam": "Slaapkamer + 2 kasten"
                     }
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
@@ -106,43 +86,31 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "VZE",
                     "naam": "Verwarming"
                 }
             },
-            "punten": 14.0,
+            "punten": 10.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "Woonkamer"
-                    },
-                    "punten": 2.0
-                },
-                {
-                    "criterium": {
-                        "naam": "Slaapkamer"
-                    },
-                    "punten": 2.0
-                },
-                {
-                    "criterium": {
-                        "naam": "Slaapkamer"
+                        "naam": "Badruimte"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Badruimte"
+                        "naam": "Woonkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
                         "naam": "Keuken"
                     },
@@ -163,24 +131,60 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "ENE",
                     "naam": "Energieprestatie"
                 }
             },
-            "punten": 32.0,
+            "punten": 5.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "A (oud)"
+                        "naam": "E (oud)"
+                    },
+                    "punten": 5.0
+                }
+            ]
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
+                },
+                "stelselgroep": {
+                    "code": "SAN",
+                    "naam": "Sanitair"
+                }
+            },
+            "punten": 9.0,
+            "woningwaarderingen": [
+                {
+                    "aantal": 2.0,
+                    "criterium": {
+                        "naam": "Wastafel"
+                    },
+                    "punten": 2.0
+                },
+                {
+                    "aantal": 1.0,
+                    "criterium": {
+                        "naam": "Douche"
+                    },
+                    "punten": 4.0
+                },
+                {
+                    "aantal": 1.0,
+                    "criterium": {
+                        "naam": "Closetcombinatie"
                     },
-                    "punten": 32.0
+                    "punten": 3.0
                 }
             ]
         }
     ],
-    "punten": 106.0,
+    "punten": 67.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/71211000027.json` & `woningwaardering-0.3.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/37101000032.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7690972222222222%*

 * *Differences: {"'groepen'": "{0: {'punten': 140.0, 'woningwaarderingen': {1: {'aantal': 41.0, 'criterium': "*

 * *              "{'naam': 'Woonkamer'}}, 2: {'aantal': 20.37}, 3: {'aantal': 6.5, 'criterium': "*

 * *              "{'naam': 'Badruimte'}}, 4: {'aantal': 15.98}, 5: {'aantal': 19.15}, 6: {'aantal': "*

 * *              "15.82, 'criterium': {'naam': 'Slaapkamer'}}, insert: [(0, OrderedDict([('aantal', "*

 * *              "21.05), ('criterium', OrderedDict([('naam', 'Slaapkamer'), ('meeteenheid', "*

 * *              "OrderedDict([('co […]*

```diff
@@ -7,74 +7,84 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OVZ",
                     "naam": "Oppervlakte van vertrekken"
                 }
             },
-            "punten": 54.0,
+            "punten": 140.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 15.89,
+                    "aantal": 21.05,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Woonkamer + 1 kast"
+                        "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 10.63,
+                    "aantal": 41.0,
+                    "criterium": {
+                        "meeteenheid": {
+                            "code": "M2",
+                            "naam": "Vierkante meter, m2"
+                        },
+                        "naam": "Woonkamer"
+                    }
+                },
+                {
+                    "aantal": 20.37,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Keuken"
                     }
                 },
                 {
-                    "aantal": 9.08,
+                    "aantal": 6.5,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer"
+                        "naam": "Badruimte"
                     }
                 },
                 {
-                    "aantal": 4.73,
+                    "aantal": 15.98,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 8.72,
+                    "aantal": 19.15,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 4.94,
+                    "aantal": 15.82,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Badruimte"
+                        "naam": "Slaapkamer"
                     }
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
@@ -82,28 +92,18 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OOZ",
                     "naam": "Oppervlakte van overige ruimten"
                 }
             },
-            "punten": 6.75,
+            "punten": 5.25,
             "woningwaarderingen": [
                 {
-                    "aantal": 4.4,
-                    "criterium": {
-                        "meeteenheid": {
-                            "code": "M2",
-                            "naam": "Vierkante meter, m2"
-                        },
-                        "naam": "Zolder"
-                    }
-                },
-                {
-                    "aantal": 5.05,
+                    "aantal": 6.65,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Berging"
                     }
@@ -117,31 +117,37 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "VZE",
                     "naam": "Verwarming"
                 }
             },
-            "punten": 12.0,
+            "punten": 14.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
+                        "naam": "Slaapkamer"
+                    },
+                    "punten": 2.0
+                },
+                {
+                    "criterium": {
                         "naam": "Woonkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
                         "naam": "Keuken"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Slaapkamer"
+                        "naam": "Badruimte"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
@@ -151,15 +157,15 @@
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Badruimte"
+                        "naam": "Slaapkamer"
                     },
                     "punten": 2.0
                 }
             ]
         },
         {
             "criteriumGroep": {
@@ -168,24 +174,60 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "ENE",
                     "naam": "Energieprestatie"
                 }
             },
-            "punten": 14.0,
+            "punten": 22.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "D (oud)"
+                        "naam": "C (oud)"
+                    },
+                    "punten": 22.0
+                }
+            ]
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
+                },
+                "stelselgroep": {
+                    "code": "SAN",
+                    "naam": "Sanitair"
+                }
+            },
+            "punten": 16.0,
+            "woningwaarderingen": [
+                {
+                    "aantal": 2.0,
+                    "criterium": {
+                        "naam": "Closetcombinatie"
+                    },
+                    "punten": 6.0
+                },
+                {
+                    "aantal": 3.0,
+                    "criterium": {
+                        "naam": "Wastafel"
+                    },
+                    "punten": 3.0
+                },
+                {
+                    "aantal": 1.0,
+                    "criterium": {
+                        "naam": "Bad en Douche in zelfde ruimte"
                     },
-                    "punten": 14.0
+                    "punten": 7.0
                 }
             ]
         }
     ],
-    "punten": 87.0,
+    "punten": 197.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/77795000000.json` & `woningwaardering-0.3.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/77795000000.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7999999999999999%*

 * *Differences: {"'groepen'": "{insert: [(4, OrderedDict([('criteriumGroep', OrderedDict([('stelsel', "*

 * *              "OrderedDict([('code', 'ZEL'), ('naam', 'Zelfstandige woonruimten')])), "*

 * *              "('stelselgroep', OrderedDict([('code', 'SAN'), ('naam', 'Sanitair')]))])), "*

 * *              "('punten', 12.0), ('woningwaarderingen', [OrderedDict([('aantal', 2.0), "*

 * *              "('criterium', OrderedDict([('naam', 'Closetcombinatie')])), ('punten', 6.0)]), "*

 * *              "OrderedDict([('aantal', 2.0), ('criterium',  […]*

```diff
@@ -173,15 +173,51 @@
                 {
                     "criterium": {
                         "naam": "A (oud)"
                     },
                     "punten": 36.0
                 }
             ]
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
+                },
+                "stelselgroep": {
+                    "code": "SAN",
+                    "naam": "Sanitair"
+                }
+            },
+            "punten": 12.0,
+            "woningwaarderingen": [
+                {
+                    "aantal": 2.0,
+                    "criterium": {
+                        "naam": "Closetcombinatie"
+                    },
+                    "punten": 6.0
+                },
+                {
+                    "aantal": 2.0,
+                    "criterium": {
+                        "naam": "Wastafel"
+                    },
+                    "punten": 2.0
+                },
+                {
+                    "aantal": 1.0,
+                    "criterium": {
+                        "naam": "Douche"
+                    },
+                    "punten": 4.0
+                }
+            ]
         }
     ],
-    "punten": 131.0,
+    "punten": 143.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/81020000003.json` & `woningwaardering-0.3.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41164000002.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7698908730158731%*

 * *Differences: {"'groepen'": "{0: {'punten': 138.0, 'woningwaarderingen': {0: {'aantal': 6.33}, 2: {'aantal': "*

 * *              "22.66}, 3: {'aantal': 14.71}, 4: {'aantal': 17.63}, 5: {'aantal': 32.95, "*

 * *              "'criterium': {'naam': 'Woonkamer'}}, 6: {'aantal': 20.45, 'criterium': {'naam': "*

 * *              "'Slaapkamer + 1 kast'}}, insert: [(1, OrderedDict([('aantal', 23.42), ('criterium', "*

 * *              "OrderedDict([('naam', 'Slaapkamer + 1 kast'), ('meeteenheid', OrderedDict([('code', "*

 * *              "'M2'), ('na […]*

```diff
@@ -7,74 +7,84 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OVZ",
                     "naam": "Oppervlakte van vertrekken"
                 }
             },
-            "punten": 79.0,
+            "punten": 138.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 3.8,
+                    "aantal": 6.33,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Badruimte"
                     }
                 },
                 {
-                    "aantal": 15.74,
+                    "aantal": 23.42,
+                    "criterium": {
+                        "meeteenheid": {
+                            "code": "M2",
+                            "naam": "Vierkante meter, m2"
+                        },
+                        "naam": "Slaapkamer + 1 kast"
+                    }
+                },
+                {
+                    "aantal": 22.66,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 5.92,
+                    "aantal": 14.71,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Keuken"
                     }
                 },
                 {
-                    "aantal": 15.15,
+                    "aantal": 17.63,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 26.54,
+                    "aantal": 32.95,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Woonkamer + 1 kast"
+                        "naam": "Woonkamer"
                     }
                 },
                 {
-                    "aantal": 12.23,
+                    "aantal": 20.45,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer"
+                        "naam": "Slaapkamer + 1 kast"
                     }
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
@@ -82,24 +92,24 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OOZ",
                     "naam": "Oppervlakte van overige ruimten"
                 }
             },
-            "punten": 3.75,
+            "punten": 3.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 5.19,
+                    "aantal": 4.31,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Berging"
+                        "naam": "Wasruimte"
                     }
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
@@ -107,75 +117,110 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "VZE",
                     "naam": "Verwarming"
                 }
             },
-            "punten": 9.0,
+            "punten": 14.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
                         "naam": "Badruimte"
                     },
-                    "punten": 1.5
+                    "punten": 2.0
                 },
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
-                    "punten": 1.5
+                    "punten": 2.0
+                },
+                {
+                    "criterium": {
+                        "naam": "Slaapkamer"
+                    },
+                    "punten": 2.0
                 },
                 {
                     "criterium": {
                         "naam": "Keuken"
                     },
-                    "punten": 1.5
+                    "punten": 2.0
                 },
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
-                    "punten": 1.5
+                    "punten": 2.0
                 },
                 {
                     "criterium": {
                         "naam": "Woonkamer"
                     },
-                    "punten": 1.5
+                    "punten": 2.0
                 },
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
-                    "punten": 1.5
+                    "punten": 2.0
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
                     "code": "ZEL",
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "ENE",
                     "naam": "Energieprestatie"
                 }
             },
-            "punten": 36.0,
+            "punten": 32.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "A (oud)"
+                        "naam": "B (oud)"
+                    },
+                    "punten": 32.0
+                }
+            ]
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
+                },
+                "stelselgroep": {
+                    "code": "SAN",
+                    "naam": "Sanitair"
+                }
+            },
+            "punten": 7.0,
+            "woningwaarderingen": [
+                {
+                    "aantal": 4.0,
+                    "criterium": {
+                        "naam": "Wastafel"
+                    },
+                    "punten": 4.0
+                },
+                {
+                    "aantal": 1.0,
+                    "criterium": {
+                        "naam": "Closetcombinatie"
                     },
-                    "punten": 36.0
+                    "punten": 3.0
                 }
             ]
         }
     ],
-    "punten": 128.0,
+    "punten": 194.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/81065000089.json` & `woningwaardering-0.3.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/85651000021.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7672685185185185%*

 * *Differences: {"'groepen'": "{0: {'punten': 60.0, 'woningwaarderingen': {0: {'aantal': 8.05, 'criterium': "*

 * *              "{'naam': 'Keuken'}}, 1: {'aantal': 5.78, 'criterium': {'naam': 'Badruimte'}}, 2: "*

 * *              "{'aantal': 25.54}, 3: {'aantal': 12.06, 'criterium': {'naam': 'Slaapkamer'}}, 4: "*

 * *              "{'aantal': 8.11}}}, 1: {'punten': 0.0, 'woningwaarderingen': []}, 2: {'punten': "*

 * *              "10.0, 'woningwaarderingen': {0: {'criterium': {'naam': 'Keuken'}}, 1: {'criterium': "*

 * *              "{'naam':  […]*

```diff
@@ -7,58 +7,58 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OVZ",
                     "naam": "Oppervlakte van vertrekken"
                 }
             },
-            "punten": 58.0,
+            "punten": 60.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 11.63,
+                    "aantal": 8.05,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer"
+                        "naam": "Keuken"
                     }
                 },
                 {
-                    "aantal": 7.62,
+                    "aantal": 5.78,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer"
+                        "naam": "Badruimte"
                     }
                 },
                 {
-                    "aantal": 17.77,
+                    "aantal": 25.54,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Woonkamer"
                     }
                 },
                 {
-                    "aantal": 12.72,
+                    "aantal": 12.06,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Keuken"
+                        "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 8.34,
+                    "aantal": 8.11,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
@@ -72,78 +72,51 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OOZ",
                     "naam": "Oppervlakte van overige ruimten"
                 }
             },
-            "punten": 4.5,
-            "woningwaarderingen": [
-                {
-                    "aantal": 3.56,
-                    "criterium": {
-                        "meeteenheid": {
-                            "code": "M2",
-                            "naam": "Vierkante meter, m2"
-                        },
-                        "naam": "Zolder"
-                    }
-                },
-                {
-                    "aantal": 2.86,
-                    "criterium": {
-                        "meeteenheid": {
-                            "code": "M2",
-                            "naam": "Vierkante meter, m2"
-                        },
-                        "naam": "Wasruimte"
-                    }
-                }
-            ]
+            "punten": 0.0,
+            "woningwaarderingen": []
         },
         {
             "criteriumGroep": {
                 "stelsel": {
                     "code": "ZEL",
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "VZE",
                     "naam": "Verwarming"
                 }
             },
-            "punten": 11.0,
+            "punten": 10.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "Slaapkamer"
+                        "naam": "Keuken"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Slaapkamer"
+                        "naam": "Badruimte"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
                         "naam": "Woonkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Wasruimte"
-                    },
-                    "punten": 1.0
-                },
-                {
-                    "criterium": {
-                        "naam": "Keuken"
+                        "naam": "Slaapkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
@@ -158,24 +131,60 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "ENE",
                     "naam": "Energieprestatie"
                 }
             },
-            "punten": 32.0,
+            "punten": 0.0,
+            "woningwaarderingen": [
+                {
+                    "criterium": {
+                        "naam": "Bouwjaar 1897"
+                    },
+                    "punten": 0.0
+                }
+            ]
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
+                },
+                "stelselgroep": {
+                    "code": "SAN",
+                    "naam": "Sanitair"
+                }
+            },
+            "punten": 9.0,
             "woningwaarderingen": [
                 {
+                    "aantal": 2.0,
+                    "criterium": {
+                        "naam": "Wastafel"
+                    },
+                    "punten": 2.0
+                },
+                {
+                    "aantal": 1.0,
+                    "criterium": {
+                        "naam": "Douche"
+                    },
+                    "punten": 4.0
+                },
+                {
+                    "aantal": 1.0,
                     "criterium": {
-                        "naam": "B + 78.84m2"
+                        "naam": "Closetcombinatie"
                     },
-                    "punten": 32.0
+                    "punten": 3.0
                 }
             ]
         }
     ],
-    "punten": 106.0,
+    "punten": 79.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/85651000021.json` & `woningwaardering-0.3.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/28018000044.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7666087962962963%*

 * *Differences: {"'groepen'": "{0: {'punten': 67.0, 'woningwaarderingen': {1: {'aantal': 7.02, 'criterium': "*

 * *              "{'naam': 'Slaapkamer'}}, 2: {'aantal': 7.64, 'criterium': {'naam': 'Keuken'}}, 3: "*

 * *              "{'aantal': 23.62}, 4: {'aantal': 5.18, 'criterium': {'naam': 'Badruimte'}}, 5: "*

 * *              "{'aantal': 13.35}, insert: [(0, OrderedDict([('aantal', 10.0), ('criterium', "*

 * *              "OrderedDict([('naam', 'Slaapkamer'), ('meeteenheid', OrderedDict([('code', 'M2'), "*

 * *              "('naam', 'Vierk […]*

```diff
@@ -7,58 +7,68 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OVZ",
                     "naam": "Oppervlakte van vertrekken"
                 }
             },
-            "punten": 60.0,
+            "punten": 67.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 8.05,
+                    "aantal": 10.0,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Keuken"
+                        "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 5.78,
+                    "aantal": 7.02,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Badruimte"
+                        "naam": "Slaapkamer"
+                    }
+                },
+                {
+                    "aantal": 7.64,
+                    "criterium": {
+                        "meeteenheid": {
+                            "code": "M2",
+                            "naam": "Vierkante meter, m2"
+                        },
+                        "naam": "Keuken"
                     }
                 },
                 {
-                    "aantal": 25.54,
+                    "aantal": 23.62,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Woonkamer"
                     }
                 },
                 {
-                    "aantal": 12.06,
+                    "aantal": 5.18,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer"
+                        "naam": "Badruimte"
                     }
                 },
                 {
-                    "aantal": 8.11,
+                    "aantal": 13.35,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
@@ -72,51 +82,68 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OOZ",
                     "naam": "Oppervlakte van overige ruimten"
                 }
             },
-            "punten": 0.0,
-            "woningwaarderingen": []
+            "punten": 3.0,
+            "woningwaarderingen": [
+                {
+                    "aantal": 4.1,
+                    "criterium": {
+                        "meeteenheid": {
+                            "code": "M2",
+                            "naam": "Vierkante meter, m2"
+                        },
+                        "naam": "Berging"
+                    }
+                }
+            ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
                     "code": "ZEL",
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "VZE",
                     "naam": "Verwarming"
                 }
             },
-            "punten": 10.0,
+            "punten": 12.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "Keuken"
+                        "naam": "Slaapkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Badruimte"
+                        "naam": "Slaapkamer"
+                    },
+                    "punten": 2.0
+                },
+                {
+                    "criterium": {
+                        "naam": "Keuken"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
                         "naam": "Woonkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Slaapkamer"
+                        "naam": "Badruimte"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
@@ -131,24 +158,60 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "ENE",
                     "naam": "Energieprestatie"
                 }
             },
-            "punten": 0.0,
+            "punten": 22.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "Bouwjaar 1897"
+                        "naam": "Bouwjaar 1992"
+                    },
+                    "punten": 22.0
+                }
+            ]
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
+                },
+                "stelselgroep": {
+                    "code": "SAN",
+                    "naam": "Sanitair"
+                }
+            },
+            "punten": 9.0,
+            "woningwaarderingen": [
+                {
+                    "aantal": 1.0,
+                    "criterium": {
+                        "naam": "Closetcombinatie"
+                    },
+                    "punten": 3.0
+                },
+                {
+                    "aantal": 2.0,
+                    "criterium": {
+                        "naam": "Wastafel"
+                    },
+                    "punten": 2.0
+                },
+                {
+                    "aantal": 1.0,
+                    "criterium": {
+                        "naam": "Douche"
                     },
-                    "punten": 0.0
+                    "punten": 4.0
                 }
             ]
         }
     ],
-    "punten": 70.0,
+    "punten": 113.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.2.16a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/87402000003.json` & `woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/ruimte_meer_of_minder_dan_4m2.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3979166666666667%*

 * *Differences: {"'groepen'": "{0: {'punten': 7.0, 'woningwaarderingen': {0: {'aantal': 2.0}, 1: {'aantal': 4.0, "*

 * *              "'criterium': {'naam': 'Slaapkamer'}}, 2: {'aantal': 1.0, 'criterium': {'naam': "*

 * *              "'Badkamer/toilet'}}, delete: [1, 0]}}, 1: {'criteriumGroep': {'stelselgroep': "*

 * *              "{'code': 'OOZ', 'naam': 'Oppervlakte van overige ruimten'}}, 'woningwaarderingen': "*

 * *              '[]}, delete: [2, 1]}',*

 * * "'punten'": '7.0',*

 * * 'delete': "['stelsel']"}*

```diff
@@ -7,64 +7,44 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OVZ",
                     "naam": "Oppervlakte van vertrekken"
                 }
             },
-            "punten": 53.0,
+            "punten": 7.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 11.65,
-                    "criterium": {
-                        "meeteenheid": {
-                            "code": "M2",
-                            "naam": "Vierkante meter, m2"
-                        },
-                        "naam": "Slaapkamer"
-                    }
-                },
-                {
-                    "aantal": 3.12,
-                    "criterium": {
-                        "meeteenheid": {
-                            "code": "M2",
-                            "naam": "Vierkante meter, m2"
-                        },
-                        "naam": "Badruimte"
-                    }
-                },
-                {
-                    "aantal": 6.37,
+                    "aantal": 2.0,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Keuken"
                     }
                 },
                 {
-                    "aantal": 23.1,
+                    "aantal": 4.0,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Woonkamer"
+                        "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 8.35,
+                    "aantal": 1.0,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer"
+                        "naam": "Badkamer/toilet"
                     }
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
@@ -72,94 +52,13 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OOZ",
                     "naam": "Oppervlakte van overige ruimten"
                 }
             },
-            "punten": 3.75,
-            "woningwaarderingen": [
-                {
-                    "aantal": 5.25,
-                    "criterium": {
-                        "meeteenheid": {
-                            "code": "M2",
-                            "naam": "Vierkante meter, m2"
-                        },
-                        "naam": "Berging"
-                    }
-                }
-            ]
-        },
-        {
-            "criteriumGroep": {
-                "stelsel": {
-                    "code": "ZEL",
-                    "naam": "Zelfstandige woonruimten"
-                },
-                "stelselgroep": {
-                    "code": "VZE",
-                    "naam": "Verwarming"
-                }
-            },
-            "punten": 10.0,
-            "woningwaarderingen": [
-                {
-                    "criterium": {
-                        "naam": "Slaapkamer"
-                    },
-                    "punten": 2.0
-                },
-                {
-                    "criterium": {
-                        "naam": "Badruimte"
-                    },
-                    "punten": 2.0
-                },
-                {
-                    "criterium": {
-                        "naam": "Keuken"
-                    },
-                    "punten": 2.0
-                },
-                {
-                    "criterium": {
-                        "naam": "Woonkamer"
-                    },
-                    "punten": 2.0
-                },
-                {
-                    "criterium": {
-                        "naam": "Slaapkamer"
-                    },
-                    "punten": 2.0
-                }
-            ]
-        },
-        {
-            "criteriumGroep": {
-                "stelsel": {
-                    "code": "ZEL",
-                    "naam": "Zelfstandige woonruimten"
-                },
-                "stelselgroep": {
-                    "code": "ENE",
-                    "naam": "Energieprestatie"
-                }
-            },
             "punten": 0.0,
-            "woningwaarderingen": [
-                {
-                    "criterium": {
-                        "naam": "Bouwjaar 1898"
-                    },
-                    "punten": 0.0
-                }
-            ]
+            "woningwaarderingen": []
         }
     ],
-    "punten": 67.0,
-    "stelsel": {
-        "code": "ZEL",
-        "naam": "Zelfstandige woonruimten"
-    }
+    "punten": 7.0
 }
```

### Comparing `woningwaardering-0.2.16a0/tests/stelsels/config/test_config.py` & `woningwaardering-0.3.0a0/tests/stelsels/config/test_config.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/stelsels/stelsel/test_select_geldige_stelselgroepversies.py` & `woningwaardering-0.3.0a0/tests/stelsels/stelsel/test_select_geldige_stelselgroepversies.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from datetime import date
+
 import pytest
 
 from woningwaardering.stelsels.stelsel import Stelsel
 from woningwaardering.stelsels.stelselgroep import Stelselgroep
 from woningwaardering.vera.referentiedata import (
     Woningwaarderingstelsel,
 )
@@ -10,15 +11,15 @@
 
 @pytest.mark.parametrize(
     "peildatum, stelsel, aantal_geldige_stelselgroepen",
     [
         (
             date(2025, 1, 1),
             Woningwaarderingstelsel.zelfstandige_woonruimten,
-            4,
+            5,
         )
     ],
 )
 def test_select_geldige_stelselgroepen(
     peildatum, stelsel, aantal_geldige_stelselgroepen
 ):
     geldigige_stelselgroepen = Stelsel.select_geldige_stelselgroepen(
```

### Comparing `woningwaardering-0.2.16a0/tests/stelsels/stelselgroep/test_select_geldige_stelselgroepversie.py` & `woningwaardering-0.3.0a0/tests/stelsels/stelselgroep/test_select_geldige_stelselgroepversie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/stelsels/test_ZelfstandigeWoonruimten.py` & `woningwaardering-0.3.0a0/tests/stelsels/test_ZelfstandigeWoonruimten.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/stelsels/utils/test_import_class.py` & `woningwaardering-0.3.0a0/tests/stelsels/utils/test_import_class.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/stelsels/utils/test_is_geldig.py` & `woningwaardering-0.3.0a0/tests/stelsels/utils/test_is_geldig.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_A++++_egw.json` & `woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_A++++_egw.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_egw.json` & `woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_egw.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_mgw.json` & `woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_mgw.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/test_Energieprestatie.py` & `woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/test_Energieprestatie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.json` & `woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.md` & `woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.md`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/2024-01-01/zolder_overige_ruimten.json` & `woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/2024-01-01/zolder_overige_ruimten.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/test_OppervlakteVanOverigeRuimten.py` & `woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/test_OppervlakteVanOverigeRuimten.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/badkamer_en_of_toilet_boven_en_onder_0.64.json` & `woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/badkamer_en_of_toilet_boven_en_onder_0.64.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/gedeelde_berging.json` & `woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/gedeelde_berging.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/ruimte_meer_of_minder_dan_4m2.json` & `woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/ruimte_meer_of_minder_dan_4m2.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/zolder_vertrek.json` & `woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/zolder_vertrek.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/badkamer_en_of_toilet_boven_en_onder_0.64.json` & `woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/badkamer_en_of_toilet_boven_en_onder_0.64.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/ruimte_meer_of_minder_dan_4m2.json` & `woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_max_4_punten_overige_ruimten.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3328993055555556%*

 * *Differences: {"'groepen'": "{0: {'criteriumGroep': {'stelselgroep': {'code': 'VZE', 'naam': 'Verwarming'}}, "*

 * *              "'punten': 4.0, 'woningwaarderingen': {3: {'criterium': {'naam': 'Woonkamer4', "*

 * *              "delete: ['meeteenheid']}, 'punten': 0.75, delete: ['aantal']}, 4: {'criterium': "*

 * *              "{'naam': 'Woonkamer5', delete: ['meeteenheid']}, 'punten': 0.75, delete: "*

 * *              "['aantal']}, 5: {'criterium': {'naam': 'Woonkamer6', delete: ['meeteenheid']}, "*

 * *              "'punten': 0.25, delete […]*

```diff
@@ -3,62 +3,53 @@
         {
             "criteriumGroep": {
                 "stelsel": {
                     "code": "ZEL",
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
-                    "code": "OVZ",
-                    "naam": "Oppervlakte van vertrekken"
+                    "code": "VZE",
+                    "naam": "Verwarming"
                 }
             },
-            "punten": 7.0,
+            "punten": 4.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 2.0,
                     "criterium": {
-                        "meeteenheid": {
-                            "code": "M2",
-                            "naam": "Vierkante meter, m2"
-                        },
-                        "naam": "Keuken"
-                    }
-                },
-                {
-                    "aantal": 4.0,
-                    "criterium": {
-                        "meeteenheid": {
-                            "code": "M2",
-                            "naam": "Vierkante meter, m2"
-                        },
-                        "naam": "Slaapkamer"
-                    }
-                },
-                {
-                    "aantal": 1.0,
-                    "criterium": {
-                        "meeteenheid": {
-                            "code": "M2",
-                            "naam": "Vierkante meter, m2"
-                        },
-                        "naam": "Badkamer/toilet"
-                    }
-                }
-            ]
-        },
-        {
-            "criteriumGroep": {
-                "stelsel": {
-                    "code": "ZEL",
-                    "naam": "Zelfstandige woonruimten"
+                        "naam": "Woonkamer1"
+                    },
+                    "punten": 0.75
                 },
-                "stelselgroep": {
-                    "code": "OOZ",
-                    "naam": "Oppervlakte van overige ruimten"
+                {
+                    "criterium": {
+                        "naam": "Woonkamer2"
+                    },
+                    "punten": 0.75
+                },
+                {
+                    "criterium": {
+                        "naam": "Woonkamer3"
+                    },
+                    "punten": 0.75
+                },
+                {
+                    "criterium": {
+                        "naam": "Woonkamer4"
+                    },
+                    "punten": 0.75
+                },
+                {
+                    "criterium": {
+                        "naam": "Woonkamer5"
+                    },
+                    "punten": 0.75
+                },
+                {
+                    "criterium": {
+                        "naam": "Woonkamer6"
+                    },
+                    "punten": 0.25
                 }
-            },
-            "punten": 0.0,
-            "woningwaarderingen": []
+            ]
         }
-    ],
-    "punten": 7.0
+    ]
 }
```

### Comparing `woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/zolder_vertrek.json` & `woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/zolder_vertrek.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/test_OppervlakteVanVertrekken.py` & `woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/test_OppervlakteVanVertrekken.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_max_4_punten_overige_ruimten.json` & `woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_max_4_punten_overige_ruimten.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_open_keuken.json` & `woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_open_keuken.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_max_4_punten_overige_ruimten.json` & `woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_max_4_punten_overige_ruimten.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_open_keuken.json` & `woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_open_keuken.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_max_4_punten_overige_ruimten.json` & `woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/twee_bad_en_douche.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('ruimten', [OrderedDict([('bouwkundigeElementen', "*

 * *            "[OrderedDict([('naam', 'Bad'), ('soort', OrderedDict([('code', 'SAN'), ('naam', "*

 * *            "'Sanitaire voorziening')])), ('detailSoort', OrderedDict([('code', 'BAD'), ('naam', "*

 * *            "'Bad')]))]), OrderedDict([('naam', 'Bad'), ('soort', OrderedDict([('code', 'SAN'), "*

 * *            "('naam', 'Sanitaire voorziening')])), ('detailSoort', OrderedDict([('code', 'BAD'), "*

 * *            "('naam', 'Bad')]))]), Ordered […]*

```diff
@@ -1,55 +1,52 @@
 {
-    "groepen": [
+    "ruimten": [
         {
-            "criteriumGroep": {
-                "stelsel": {
-                    "code": "ZEL",
-                    "naam": "Zelfstandige woonruimten"
-                },
-                "stelselgroep": {
-                    "code": "VZE",
-                    "naam": "Verwarming"
-                }
-            },
-            "punten": 4.0,
-            "woningwaarderingen": [
-                {
-                    "criterium": {
-                        "naam": "Woonkamer1"
-                    },
-                    "punten": 0.75
-                },
-                {
-                    "criterium": {
-                        "naam": "Woonkamer2"
-                    },
-                    "punten": 0.75
-                },
-                {
-                    "criterium": {
-                        "naam": "Woonkamer3"
-                    },
-                    "punten": 0.75
-                },
-                {
-                    "criterium": {
-                        "naam": "Woonkamer4"
-                    },
-                    "punten": 0.75
-                },
+            "bouwkundigeElementen": [
                 {
-                    "criterium": {
-                        "naam": "Woonkamer5"
-                    },
-                    "punten": 0.75
-                },
-                {
-                    "criterium": {
-                        "naam": "Woonkamer6"
-                    },
-                    "punten": 0.25
+                    "detailSoort": {
+                        "code": "BAD",
+                        "naam": "Bad"
+                    },
+                    "naam": "Bad",
+                    "soort": {
+                        "code": "SAN",
+                        "naam": "Sanitaire voorziening"
+                    }
+                },
+                {
+                    "detailSoort": {
+                        "code": "BAD",
+                        "naam": "Bad"
+                    },
+                    "naam": "Bad",
+                    "soort": {
+                        "code": "SAN",
+                        "naam": "Sanitaire voorziening"
+                    }
+                },
+                {
+                    "detailSoort": {
+                        "code": "DOU",
+                        "naam": "Douche"
+                    },
+                    "naam": "Douche",
+                    "soort": {
+                        "code": "SAN",
+                        "naam": "Sanitaire voorziening"
+                    }
+                },
+                {
+                    "detailSoort": {
+                        "code": "DOU",
+                        "naam": "Douche"
+                    },
+                    "naam": "Douche",
+                    "soort": {
+                        "code": "SAN",
+                        "naam": "Sanitaire voorziening"
+                    }
                 }
             ]
         }
     ]
 }
```

### Comparing `woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_open_keuken.json` & `woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_open_keuken.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_max_4_punten_overige_ruimten.json` & `woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_max_4_punten_overige_ruimten.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_open_keuken.json` & `woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_open_keuken.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/stelsels/zelfstandige_woonruimten/verwarming/test_Verwarming.py` & `woningwaardering-0.3.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/test_Verwarming.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/tests/test_utils.py` & `woningwaardering-0.3.0a0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/wettelijke-documenten/BWBR0003237-geldend_van_01-01-2024_tm_heden_zichtdatum_06-03-2024.txt` & `woningwaardering-0.3.0a0/wettelijke-documenten/BWBR0003237-geldend_van_01-01-2024_tm_heden_zichtdatum_06-03-2024.txt`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/__init__.py` & `woningwaardering-0.3.0a0/woningwaardering/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/stelsels/config/config.py` & `woningwaardering-0.3.0a0/woningwaardering/stelsels/config/config.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/stelsels/config/zelfstandige_woonruimten.yml` & `woningwaardering-0.3.0a0/woningwaardering/stelsels/config/zelfstandige_woonruimten.yml`

 * *Files 6% similar despite different names*

```diff
@@ -29,7 +29,15 @@
     module: energieprestatie
     class_naam: Energieprestatie
     begindatum: 2024-01-01
     versies:
       - module: energieprestatie_2024
         class_naam: Energieprestatie2024
         begindatum: 2024-01-01
+  sanitair:
+    module: sanitair
+    class_naam: Sanitair
+    begindatum: 2024-01-01
+    versies:
+      - module: sanitair_2024
+        class_naam: Sanitair2024
+        begindatum: 2024-01-01
```

### Comparing `woningwaardering-0.2.16a0/woningwaardering/stelsels/stelsel.py` & `woningwaardering-0.3.0a0/woningwaardering/stelsels/stelsel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from datetime import date
 from decimal import ROUND_HALF_UP, Decimal
 
-
 from woningwaardering.stelsels.config import Stelselconfig
 from woningwaardering.stelsels.stelselgroep import (
     Stelselgroep,
 )
 from woningwaardering.stelsels.utils import import_class, is_geldig
 from woningwaardering.vera.bvg.generated import (
     EenhedenEenheid,
```

### Comparing `woningwaardering-0.2.16a0/woningwaardering/stelsels/stelselgroep.py` & `woningwaardering-0.3.0a0/woningwaardering/stelsels/stelselgroep.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/stelsels/stelselgroepversie.py` & `woningwaardering-0.3.0a0/woningwaardering/stelsels/stelselgroepversie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/stelsels/utils.py` & `woningwaardering-0.3.0a0/woningwaardering/stelsels/utils.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/energieprestatie.py` & `woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/energieprestatie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/energieprestatie_2024.py` & `woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/energieprestatie_2024.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten.py` & `woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten_2024.py` & `woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten_2024.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,30 +136,28 @@
         Args:
             ruimte (EenhedenRuimte): Het EenhedenRuimte object dat een zolder type is.
 
         Returns:
             float: De berekende oppervlakte voor de zolder.
         """
         if ruimte.detail_soort is not None and ruimte.oppervlakte is not None:
-            trap = heeft_bouwkundig_element(
-                ruimte, Bouwkundigelementdetailsoort.trap.code
-            )
+            trap = heeft_bouwkundig_element(ruimte, Bouwkundigelementdetailsoort.trap)
 
             if trap:
                 logger.debug(
                     f"Trap gevonden in {ruimte.naam} ({ruimte.id}): telt mee voor {Woningwaarderingstelselgroep.oppervlakte_van_overige_ruimten.naam}"
                 )
                 return float(
                     Decimal(str(ruimte.oppervlakte)).quantize(
                         Decimal("0.01"), ROUND_HALF_UP
                     )
                 )
 
             vlizotrap = heeft_bouwkundig_element(
-                ruimte, Bouwkundigelementdetailsoort.vlizotrap.code
+                ruimte, Bouwkundigelementdetailsoort.vlizotrap
             )
 
             if vlizotrap:
                 logger.debug(
                     f"Vlizotrap gevonden in {ruimte.naam} ({ruimte.id}): telt mee voor oppervlakte van overige ruimten"
                 )
                 return max(
```

### Comparing `woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken.py` & `woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken_2024.py` & `woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken_2024.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/utils.py` & `woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,30 +71,28 @@
     ]:
         if ruimte.oppervlakte >= 2:
             return Ruimtesoort.overige_ruimtes
         else:
             return None
 
     if ruimte.detail_soort.code == Ruimtedetailsoort.zolder.code:
-        if heeft_bouwkundig_element(ruimte, Bouwkundigelementdetailsoort.trap.code):
+        if heeft_bouwkundig_element(ruimte, Bouwkundigelementdetailsoort.trap):
             logger.debug(
                 f"Vaste trap gevonden in {ruimte.naam} ({ruimte.id}): wordt gewaardeerd als {ruimte.soort.naam}"
             )
             if (
                 ruimte.soort.code == Ruimtesoort.vertrek.code
                 and ruimte.oppervlakte >= 4
             ):
                 return Ruimtesoort.vertrek
             elif ruimte.oppervlakte >= 2:
                 return Ruimtesoort.overige_ruimtes
             else:
                 return None
-        elif heeft_bouwkundig_element(
-            ruimte, Bouwkundigelementdetailsoort.vlizotrap.code
-        ):
+        elif heeft_bouwkundig_element(ruimte, Bouwkundigelementdetailsoort.vlizotrap):
             logger.debug(
                 f"Vlizo trap gevonden in {ruimte.naam} ({ruimte.id}): wordt gewaardeerd als {Ruimtesoort.overige_ruimtes}"
             )
             if ruimte.oppervlakte >= 2:
                 return Ruimtesoort.overige_ruimtes
             else:
                 return None
```

### Comparing `woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming.py` & `woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming_2024.py` & `woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming_2024.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
                 or ruimte.detail_soort.code
                 in [
                     Ruimtedetailsoort.woonkamer.code,
                     Ruimtedetailsoort.woon_en_of_slaapkamer.code,
                     Ruimtedetailsoort.slaapkamer.code,
                 ]
                 and heeft_bouwkundig_element(
-                    ruimte, Bouwkundigelementdetailsoort.aanrecht.code
+                    ruimte, Bouwkundigelementdetailsoort.aanrecht
                 )
             ):
                 woningwaardering_groep.woningwaarderingen.append(
                     WoningwaarderingResultatenWoningwaardering(
                         criterium=WoningwaarderingResultatenWoningwaarderingCriterium(
                             naam=f"Open keuken in {ruimte.naam}",
                         ),
```

### Comparing `woningwaardering-0.2.16a0/woningwaardering/stelsels/zelfstandige_woonruimten/zelfstandige_woonruimten.py` & `woningwaardering-0.3.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/zelfstandige_woonruimten.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/templates/stelsels/stelsel/stelsel.py.j2` & `woningwaardering-0.3.0a0/woningwaardering/templates/stelsels/stelsel/stelsel.py.j2`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroep.py.j2` & `woningwaardering-0.3.0a0/woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroep.py.j2`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroepversie.py.j2` & `woningwaardering-0.3.0a0/woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroepversie.py.j2`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/bvg/generated.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/bvg/generated.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_eenheid.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_eenheid.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_energieprestatie.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_energieprestatie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_ruimte.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_ruimte.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/__init__.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/aanbiedingdetailstatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/aanbiedingdetailstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/aanbiedingstatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/aanbiedingstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/aanvullendedoelgroep.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/aanvullendedoelgroep.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/accountstatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/accountstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/adressoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/adressoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/afletterstatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/afletterstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/afrekenwijzesoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/afrekenwijzesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/afspraakstatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/afspraakstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/afspraakverzoeksoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/afspraakverzoeksoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/afwezigheidsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/afwezigheidsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/aktesoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/aktesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/authentiekgegevenbron.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/authentiekgegevenbron.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/authentiekgegevensoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/authentiekgegevensoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/authentiekgegevenstatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/authentiekgegevenstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/bedrijfsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/bedrijfsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/begrotingversie.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/begrotingversie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/bestemming.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/bestemming.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/betaalgegevensoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/betaalgegevensoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/betaalwijzedeelsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/betaalwijzedeelsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/betaalwijzesoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/betaalwijzesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/betalingsregelingeindereden.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/betalingsregelingeindereden.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/betalingsregelingstatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/betalingsregelingstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/boekingdetailsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/boekingdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/boekingsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/boekingsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/boekingstatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/boekingstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/boekjaarperiodesoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/boekjaarperiodesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/boekjaarperiodestatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/boekjaarperiodestatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/boekjaarstatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/boekjaarstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/bouwkundigelementdetailsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/bouwkundigelementdetailsoort.py`

 * *Files 0% similar despite different names*

```diff
@@ -1172,14 +1172,38 @@
         naam="Waterleiding/hoofdkraan",
         parent=Referentiedata(
             code="VOO",
             naam="Voorziening",
         ),
     )
 
+    bidet = Referentiedata(
+        code="BID",
+        naam="Bidet",
+        parent=Referentiedata(
+            code="VOO",
+            naam="Voorziening",
+        ),
+    )
+    """
+    Een bidet (UITBREIDING).
+    """
+
+    lavet = Referentiedata(
+        code="LAV",
+        naam="Lavet",
+        parent=Referentiedata(
+            code="VOO",
+            naam="Voorziening",
+        ),
+    )
+    """
+    Een Lavet (UITBREIDING).
+    """
+
     @property
     def code(self) -> str:
         if self.value.code is None:
             raise TypeError("de code van een Referentiedata object mag niet None zijn")
         return self.value.code
 
     @property
```

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/bouwkundigelementplaatsing.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/bouwkundigelementplaatsing.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/bouwkundigelementsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/bouwkundigelementsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/brandwerendheidscore.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/brandwerendheidscore.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/btw.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/btw.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/btwaangiftestatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/btwaangiftestatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/burgerlijkestaat.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/burgerlijkestaat.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/clustersoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/clustersoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/collectiefobjectsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/collectiefobjectsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/communicatiekanaal.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/communicatiekanaal.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/communicatierichting.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/communicatierichting.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/conditiescore.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/conditiescore.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/contactgegevendetailsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/contactgegevendetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/contactgegevensoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/contactgegevensoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/contactgegevenstatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/contactgegevenstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/contactgegevenvoorkeur.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/contactgegevenvoorkeur.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/crediteursoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/crediteursoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/crediteurstatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/crediteurstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/dagdeel.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/dagdeel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/debiteursoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/debiteursoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/debiteurstatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/debiteurstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/defectlocatie.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/defectlocatie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/defectoorzaak.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/defectoorzaak.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/defectsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/defectsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/defectstatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/defectstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/doelgroep.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/doelgroep.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/dossier/__init__.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/dossier/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eenheidcriteriasoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eenheidcriteriasoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eenheidcriteriumdetailsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eenheidcriteriumdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eenheidcriteriumsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eenheidcriteriumsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eenheidcriteriumtoepassing.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eenheidcriteriumtoepassing.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eenheiddetailsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eenheiddetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eenheiddetailstatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eenheiddetailstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eenheidenergievoorziening.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eenheidenergievoorziening.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eenheidinterieur.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eenheidinterieur.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eenheidisolatie.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eenheidisolatie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eenheidklimaatbeheersing.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eenheidklimaatbeheersing.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eenheidklimaatbeheersingsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eenheidklimaatbeheersingsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eenheidligging.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eenheidligging.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eenheidmonument.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eenheidmonument.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eenheidprijsconditie.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eenheidprijsconditie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eenheidsanitair.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eenheidsanitair.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eenheidsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eenheidsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eenheidstatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eenheidstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eindedetailreden.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eindedetailreden.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/eindereden.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/eindereden.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/energielabel.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/energielabel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/energieprestatiesoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/energieprestatiesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/energieprestatiestatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/energieprestatiestatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/energieprestatievergoedingsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/energieprestatievergoedingsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/externeincassosoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/externeincassosoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/externeincassostatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/externeincassostatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/factuurbetaalwijze.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/factuurbetaalwijze.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/factuursoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/factuursoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/financien/__init__.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/financien/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/gebeurtenissoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/gebeurtenissoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/geometriesoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/geometriesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/geslacht.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/geslacht.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/grootboekmutatieherkomst.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/grootboekmutatieherkomst.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/grootboekrekeningsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/grootboekrekeningsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/grootboekrekeningstatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/grootboekrekeningstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/huurgeschilsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/huurgeschilsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/huurgeschilstatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/huurgeschilstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/huurklasse.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/huurklasse.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/huuropzeggingstatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/huuropzeggingstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/incassomoment.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/incassomoment.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/inexploitatiereden.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/inexploitatiereden.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/informatieobjectdetailsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/informatieobjectdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/informatieobjectsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/informatieobjectsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/inkomensbron.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/inkomensbron.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/inkomenssoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/inkomenssoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/inkomensverklaringsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/inkomensverklaringsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/inkoopfactuurstatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/inkoopfactuurstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/inkoopopdrachtregelsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/inkoopopdrachtregelsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/inschrijvingherkomst.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/inschrijvingherkomst.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/inspectierapportsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/inspectierapportsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/inspectierapportstatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/inspectierapportstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/kandidaatdetailstatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/kandidaatdetailstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/kandidaatstatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/kandidaatstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/kwaliteitsniveau.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/kwaliteitsniveau.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/leningaflosvorm.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/leningaflosvorm.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/leningdetailsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/leningdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/leningsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/leningsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/maatschappelijklabel.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/maatschappelijklabel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/machtigingsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/machtigingsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/materiaaldetailsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/materiaaldetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/materiaalsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/materiaalsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/medewerkerrol.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/medewerkerrol.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/medewerkersoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/medewerkersoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/meeteenheid.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/meeteenheid.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/onderhoud/__init__.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/onderhoud/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/onderhoudsbestedingsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/onderhoudsbestedingsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/onderhoudslabel.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/onderhoudslabel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/onderhoudsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/onderhoudsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/onderhoudsorderstatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/onderhoudsorderstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/onderhoudspecialisme.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/onderhoudspecialisme.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/onderhoudstaakdetailstatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/onderhoudstaakdetailstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/onderhoudstaakstatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/onderhoudstaakstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/onderhoudsverzoekstatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/onderhoudsverzoekstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/opleidingsniveau.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/opleidingsniveau.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/oppervlaktesoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/oppervlaktesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/opzegtermijn.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/opzegtermijn.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/organisatievorm.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/organisatievorm.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/overeenkomstdetailsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/overeenkomstdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/overeenkomsten/__init__.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/overeenkomsten/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/overeenkomstkoppelingdetailstatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/overeenkomstkoppelingdetailstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/overeenkomstkoppelingstatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/overeenkomstkoppelingstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/overeenkomstsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/overeenkomstsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/overeenkomststatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/overeenkomststatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/passendheiddetailsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/passendheiddetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/passendheidssoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/passendheidssoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/prestatieafspraak.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/prestatieafspraak.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/prijsaanpassingsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/prijsaanpassingsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/prijscomponentdetailsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/prijscomponentdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/prijscomponentsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/prijscomponentsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/prijscomponentsubsidiesoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/prijscomponentsubsidiesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/prijscomponentwijzigingsreden.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/prijscomponentwijzigingsreden.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/projectbudgetregelregelsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/projectbudgetregelregelsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/projectbudgetregelsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/projectbudgetregelsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/projectbudgetregelstatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/projectbudgetregelstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/projectfasebesluitstatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/projectfasebesluitstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/projectsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/projectsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/projectstatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/projectstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/provincie.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/provincie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/publicatiedetailmodel.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/publicatiedetailmodel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/publicatiedetailstatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/publicatiedetailstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/publicatieintakevorm.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/publicatieintakevorm.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/publicatiemodel.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/publicatiemodel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/publicatiestatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/publicatiestatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/puntenberekeningsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/puntenberekeningsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/puntenmutatiesoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/puntenmutatiesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/reclamatiesoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/reclamatiesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/reclamatiestatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/reclamatiestatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/redenontbinding.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/redenontbinding.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/redenopzegging.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/redenopzegging.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/redenvernietiging.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/redenvernietiging.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/regiesoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/regiesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/relatieadressoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/relatieadressoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/relatiedetailsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/relatiedetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/relatierolsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/relatierolsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/relaties/__init__.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/relaties/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/relatiesoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/relatiesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/relatiestatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/relatiestatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/rentesoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/rentesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/ruimtedetailsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/ruimtedetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/ruimteligging.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/ruimteligging.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/ruimtesoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/ruimtesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/sanctiesoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/sanctiesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/sanctiestatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/sanctiestatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/signaleringdetailsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/signaleringdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/signaleringsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/signaleringsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/signaleringstatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/signaleringstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/taal.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/taal.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/toegankelijkheidslabel.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/toegankelijkheidslabel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/uitexploitatiereden.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/uitexploitatiereden.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/uitvoerendesoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/uitvoerendesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/vastgoed/__init__.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/vastgoed/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/verantwoordingconsolidatie.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/verantwoordingconsolidatie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/verantwoordingregime.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/verantwoordingregime.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/verbijzonderingsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/verbijzonderingsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/verbijzonderingstatus.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/verbijzonderingstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/verrekeningsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/verrekeningsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/vertrouwelijkheid.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/vertrouwelijkheid.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/voorrangdetailsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/voorrangdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/voorrangsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/voorrangsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/vragenlijstregelherkomst.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/vragenlijstregelherkomst.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/woningtype.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/woningtype.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/woningwaarderingstelsel.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/woningwaarderingstelsel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/woningwaarderingstelselgroep.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/woningwaarderingstelselgroep.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/woonruimteverdeling/__init__.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/woonruimteverdeling/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/woonsituatiesoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/woonsituatiesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/woonvorm.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/woonvorm.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/zaakobjectsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/zaakobjectsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/zaakrol.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/zaakrol.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/zaakstatussoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/zaakstatussoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/zaaktypedetailsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/zaaktypedetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/zaaktypesoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/zaaktypesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata/zekerheidverpandingsoort.py` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata/zekerheidverpandingsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.16a0/woningwaardering/vera/referentiedata_uitbreiding.csv` & `woningwaardering-0.3.0a0/woningwaardering/vera/referentiedata_uitbreiding.csv`

 * *Files 24% similar despite different names*

```diff
@@ -1,6 +1,8 @@
 Soort;Code;Naam;Omschrijving;Begindatum;Einddatum;Parent;Informatiedomein
 RUIMTEDETAILSOORT;OVL;Overloop;Verkeersruimte: (UITBREIDING) Gang op een bovenverdieping.;3-4-2024;;RUIMTESOORT.OVR;Vastgoed
 RUIMTEDETAILSOORT;ENT;Entree;Verkeersruimte: (UITBREIDING) Ingang van een gebouw.;3-4-2024;;RUIMTESOORT.OVR;Vastgoed
 RUIMTEDETAILSOORT;KAS;Kast;Overige ruimte: (UITBREIDING);8-4-2024;;RUIMTESOORT.OVR;Vastgoed
 WONINGTYPE;EGW;Eengezinswoning;Een woning die tevens een geheel pand vormt.;6-5-2024;;EENHEIDSOORT.WOO;Vastgoed
 WONINGTYPE;MGW;Meergezinswoning;Een woning die samen met andere woonruimten c.q. bedrijfsruimten een geheel pand vormt.;6-5-2024;;EENHEIDSOORT.WOO;Vastgoed
+BOUWKUNDIGELEMENTDETAILSOORT;BID;Bidet;Een bidet (UITBREIDING).;17-5-2024;;BOUWKUNDIGELEMENTSOORT.VOO;Vastgoed
+BOUWKUNDIGELEMENTDETAILSOORT;LAV;Lavet;Een Lavet (UITBREIDING).;17-5-2024;;BOUWKUNDIGELEMENTSOORT.VOO;Vastgoed
```

### Comparing `woningwaardering-0.2.16a0/woningwaardering.egg-info/PKG-INFO` & `woningwaardering-0.3.0a0/woningwaardering.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: woningwaardering
-Version: 0.2.16a0
+Version: 0.3.0a0
 Summary: Berekent de punten van een woning op basis van het woningwaarderingsstelsel.
 Author-email: Woonstad Rotterdam <info@woonstadrotterdam.nl>, Ben Verhees <ben.verhees@woonstadrotterdam.nl>, Tiddo Loos <tiddo.loos@woonstadrotterdam.nl>, Tomer Gabay <tomer.gabay@woonstadrotterdam.nl>
-Project-URL: Homepage, https://github.com/WoonstadRotterdamTemp/woningwaardering
-Project-URL: Issues, https://github.com/WoonstadRotterdamTemp/woningwaardering/issues
+Project-URL: Homepage, https://github.com/woonstadrotterdam/woningwaardering
+Project-URL: Issues, https://github.com/woonstadrotterdam/woningwaardering/issues
 Keywords: woning,waardering,stelsel,woningwaarderingsstelsel,wws
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -134,15 +134,15 @@
 ## 2. Contributing
 
 ### Setup
 
 Om de woningwaardering-package en de daarbij behorende developer dependencies te installeren, run onderstaand command:
 
 ```
-git clone https://github.com/WoonstadRotterdamTemp/woningwaardering.git
+git clone https://github.com/woonstadrotterdam/woningwaardering.git
 cd woningwaardering
 pip install -e ".[dev]"
 ```
 
 ### Naamgeving van classes
 
 Voor de naamgeving van de classes in de woningwaardering module volgen we de VERA referentiedata. Deze referentiedata is gedefinieerd in de referentiedata enums, te vinden onder [woningwaardering/vera/referentiedata](woningwaardering/vera/referentiedata).
```

### Comparing `woningwaardering-0.2.16a0/woningwaardering.egg-info/SOURCES.txt` & `woningwaardering-0.3.0a0/woningwaardering.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 .pre-commit-config.yaml
 .python-version
 LICENSE
 README.md
 mypy.ini
 pyproject.toml
 taskfile.yml
+.github/labeler.yml
 .github/workflows/cicd.yml
+.github/workflows/labeler.yml
 .github/workflows/publish-to-pypi.yml
 docs/afbeeldingen/excel_viewer.png
 docs/afbeeldingen/oppervlakte_van_vertrekken.excalidraw
 docs/afbeeldingen/oppervlakte_van_vertrekken.png
 docs/implementatietoelichting-beleidsboeken/2024/zelfstandige_woonruimten.md
 scripts/genereer_opzet_woningwaarderinggroep.py
 scripts/genereer_test_output.py
@@ -92,14 +94,33 @@
 tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/badkamer_en_of_toilet_boven_en_onder_0.64.json
 tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/badkamer_en_of_toilet_boven_en_onder_0.64.md
 tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/gedeelde_berging.md
 tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/ruimte_meer_of_minder_dan_4m2.json
 tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/ruimte_meer_of_minder_dan_4m2.md
 tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/zolder_vertrek.json
 tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/zolder_vertrek.md
+tests/stelsels/zelfstandige_woonruimten/sanitair/test_Sanitair.py
+tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/bad.json
+tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/bad_en_douche.json
+tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/bidet.json
+tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/douche.json
+tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/geen_sanitair.json
+tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/lavet.json
+tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/toilet.json
+tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/twee_bad_en_douche.json
+tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/wastafel.json
+tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/bad.json
+tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/bad_en_douche.json
+tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/bidet.json
+tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/douche.json
+tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/geen_sanitair.json
+tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/lavet.json
+tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/toilet.json
+tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/twee_bad_en_douche.json
+tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/wastafel.json
 tests/stelsels/zelfstandige_woonruimten/verwarming/test_Verwarming.py
 tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_max_4_punten_overige_ruimten.json
 tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_max_4_punten_overige_ruimten_individueel.md
 tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_open_keuken.json
 tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_open_keuken.md
 tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_max_4_punten_overige_ruimten.json
 tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_max_4_punten_overige_ruimten_individueel.md
@@ -138,14 +159,17 @@
 woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oud_energielabel_punten.csv
 woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/__init__.py
 woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten.py
 woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten_2024.py
 woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/__init__.py
 woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken.py
 woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken_2024.py
+woningwaardering/stelsels/zelfstandige_woonruimten/sanitair/__init__.py
+woningwaardering/stelsels/zelfstandige_woonruimten/sanitair/sanitair.py
+woningwaardering/stelsels/zelfstandige_woonruimten/sanitair/sanitair_2024.py
 woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/__init__.py
 woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming.py
 woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming_2024.py
 woningwaardering/templates/stelsels/stelsel/__init__.py.j2
 woningwaardering/templates/stelsels/stelsel/stelsel.py.j2
 woningwaardering/templates/stelsels/stelsel/stelselgroep/__init__.py.j2
 woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroep.py.j2
```

