# Comparing `tmp/great_tables-0.6.0.tar.gz` & `tmp/great_tables-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "great_tables-0.6.0.tar", last modified: Thu May 16 20:30:47 2024, max compression
+gzip compressed data, was "great_tables-0.6.1.tar", last modified: Thu May 23 18:26:43 2024, max compression
```

## Comparing `great_tables-0.6.0.tar` & `great_tables-0.6.1.tar`

### file list

```diff
@@ -1,280 +1,278 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.106188 great_tables-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.046188 great_tables-0.6.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-16 20:30:42.000000 great_tables-0.6.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-16 20:30:42.000000 great_tables-0.6.0/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.046188 great_tables-0.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-16 20:30:42.000000 great_tables-0.6.0/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-16 20:30:42.000000 great_tables-0.6.0/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-16 20:30:42.000000 great_tables-0.6.0/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-16 20:30:42.000000 great_tables-0.6.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.050188 great_tables-0.6.0/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-16 20:30:42.000000 great_tables-0.6.0/.github/scripts/no_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-16 20:30:42.000000 great_tables-0.6.0/.github/scripts/save_browser_table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.050188 great_tables-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-16 20:30:42.000000 great_tables-0.6.0/.github/workflows/ci-docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-05-16 20:30:42.000000 great_tables-0.6.0/.github/workflows/ci-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-16 20:30:42.000000 great_tables-0.6.0/.github/workflows/code-checks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-16 20:30:42.000000 great_tables-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-16 20:30:42.000000 great_tables-0.6.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.050188 great_tables-0.6.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-16 20:30:42.000000 great_tables-0.6.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-16 20:30:42.000000 great_tables-0.6.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-16 20:30:42.000000 great_tables-0.6.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-16 20:30:42.000000 great_tables-0.6.0/CHANGELOG.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     5243 2024-05-16 20:30:42.000000 great_tables-0.6.0/CODE_OF_CONDUCT.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     2259 2024-05-16 20:30:42.000000 great_tables-0.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-16 20:30:42.000000 great_tables-0.6.0/HISTORY.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     1081 2024-05-16 20:30:42.000000 great_tables-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-16 20:30:42.000000 great_tables-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-16 20:30:42.000000 great_tables-0.6.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    10846 2024-05-16 20:30:47.106188 great_tables-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-05-16 20:30:42.000000 great_tables-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.050188 great_tables-0.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.042188 great_tables-0.6.0/docs/_extensions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.042188 great_tables-0.6.0/docs/_extensions/machow/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.050188 great_tables-0.6.0/docs/_extensions/machow/interlinks/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/_extensions/machow/interlinks/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/_extensions/machow/interlinks/_extension.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/_extensions/machow/interlinks/interlinks.lua
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/_quarto.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.050188 great_tables-0.6.0/docs/articles/
--rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/articles/intro.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.054188 great_tables-0.6.0/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/assets/GT_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)  2325288 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/assets/datasets.png
--rw-r--r--   0 runner    (1001) docker     (127)   136430 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/assets/gt_parts_of_a_table.svg
--rw-r--r--   0 runner    (1001) docker     (127)   342328 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/assets/gt_sp500_table.svg
--rw-r--r--   0 runner    (1001) docker     (127)    74998 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/assets/gt_workflow_diagram.svg
--rw-r--r--   0 runner    (1001) docker     (127)   209904 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/assets/tables_from_the_web.png
--rw-r--r--   0 runner    (1001) docker     (127)   139817 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/assets/the_components_of_a_table.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.054188 great_tables-0.6.0/docs/blog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.054188 great_tables-0.6.0/docs/blog/bring-your-own-df/
--rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/bring-your-own-df/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.062188 great_tables-0.6.0/docs/blog/design-philosophy/
--rw-r--r--   0 runner    (1001) docker     (127)   241842 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/design-philosophy/a_simple_table.png
--rw-r--r--   0 runner    (1001) docker     (127)   195558 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/design-philosophy/cave_grids.png
--rw-r--r--   0 runner    (1001) docker     (127)   656631 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/design-philosophy/composition_of_a_table_in_GT.png
--rw-r--r--   0 runner    (1001) docker     (127)   801735 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/design-philosophy/computer_tables.png
--rw-r--r--   0 runner    (1001) docker     (127)    22595 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/design-philosophy/index.qmd
--rw-r--r--   0 runner    (1001) docker     (127)  1486510 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/design-philosophy/nippur_cuneiform_tablet.png
--rw-r--r--   0 runner    (1001) docker     (127)  1629638 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/design-philosophy/snippets_from_manual_tablular_presentation.png
--rw-r--r--   0 runner    (1001) docker     (127)   458471 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/design-philosophy/uruk_tablet_with_annotations.png
--rw-r--r--   0 runner    (1001) docker     (127)   812542 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/design-philosophy/visicalc.png
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.066188 great_tables-0.6.0/docs/blog/introduction-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/introduction-0.2.0/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.066188 great_tables-0.6.0/docs/blog/introduction-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     8361 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/introduction-0.3.0/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.066188 great_tables-0.6.0/docs/blog/introduction-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/introduction-0.4.0/index.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/introduction_great_tables.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.066188 great_tables-0.6.0/docs/blog/polars-styling/
--rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/polars-styling/index.qmd
--rw-r--r--   0 runner    (1001) docker     (127)   132380 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/polars-styling/table-preview.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.070188 great_tables-0.6.0/docs/blog/superbowl-squares/
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/superbowl-squares/_code.py
--rw-r--r--   0 runner    (1001) docker     (127)  1949299 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/superbowl-squares/games.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/superbowl-squares/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.070188 great_tables-0.6.0/docs/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.070188 great_tables-0.6.0/docs/examples/_data/
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/_data/coffee-sales.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.070188 great_tables-0.6.0/docs/examples/_data/coffee-table-icons/
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/_data/coffee-table-icons/aeropress.png
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/_data/coffee-table-icons/cezve.png
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/_data/coffee-table-icons/chemex.png
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/_data/coffee-table-icons/cold-brew.png
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/_data/coffee-table-icons/drip-machine.png
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/_data/coffee-table-icons/espresso-machine.png
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/_data/coffee-table-icons/filter.png
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/_data/coffee-table-icons/french-press.png
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/_data/coffee-table-icons/grinder.png
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/_data/coffee-table-icons/kettle.png
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/_data/coffee-table-icons/moka-pot.png
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/_data/coffee-table-icons/noun-drip-machine-6065915.png
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/_data/coffee-table-icons/pour-over.png
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/_data/coffee-table-icons/scale.png
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/_data/coffee-table-icons/total.png
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/_data/power_cie_prepared_tbl.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10751 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.074188 great_tables-0.6.0/docs/examples/sports-earnings/
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/sports-earnings/basketball.png
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/sports-earnings/boxing.png
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/sports-earnings/golf.png
--rw-r--r--   0 runner    (1001) docker     (127)    76604 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/sports-earnings/index.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/sports-earnings/soccer.png
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/sports-earnings/sports_earnings.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/sports-earnings/tennis.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.074188 great_tables-0.6.0/docs/get-started/
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/get-started/basic-column-labels.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/get-started/basic-formatting.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/get-started/basic-header.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/get-started/basic-stub.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     7558 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/get-started/basic-styling.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/get-started/colorizing-with-data.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/get-started/column-selection.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/get-started/index.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    10497 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/get-started/nanoplots.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/get-started/overview.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/get-started/row-selection.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/get-started/table-theme-options.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/get-started/table-theme-premade.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.082188 great_tables-0.6.0/great_tables/
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_boxhead.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.082188 great_tables-0.6.0/great_tables/_data_color/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_data_color/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23399 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_data_color/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    27133 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_data_color/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_data_color/palettes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_databackend.py
--rw-r--r--   0 runner    (1001) docker     (127)    10685 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_export.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_footnotes.py
--rw-r--r--   0 runner    (1001) docker     (127)   151727 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)    40689 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_formats_vals.py
--rw-r--r--   0 runner    (1001) docker     (127)    43858 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_gt_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_heading.py
--rw-r--r--   0 runner    (1001) docker     (127)    32945 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_locale.py
--rw-r--r--   0 runner    (1001) docker     (127)    14848 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)    74939 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_render.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_row_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_scss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_source_notes.py
--rw-r--r--   0 runner    (1001) docker     (127)    25728 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_spanners.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_stub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_stubhead.py
--rw-r--r--   0 runner    (1001) docker     (127)    12616 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_styles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6289 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_substitution.py
--rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_tab_create_modify.py
--rw-r--r--   0 runner    (1001) docker     (127)    16646 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_tbl_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_text.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    55726 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_utils_nanoplots.py
--rw-r--r--   0 runner    (1001) docker     (127)    27424 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_utils_render_html.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.082188 great_tables-0.6.0/great_tables/css/
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/css/gt_colors.scss
--rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/css/gt_styles_default.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.090188 great_tables-0.6.0/great_tables/data/
--rw-r--r--   0 runner    (1001) docker     (127)   412361 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/01-countrypops.csv
--rw-r--r--   0 runner    (1001) docker     (127)    12898 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/02-sza.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/03-gtcars.csv
--rw-r--r--   0 runner    (1001) docker     (127)   906055 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/04-sp500.csv
--rw-r--r--   0 runner    (1001) docker     (127)  2848391 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/05-pizzaplace.csv
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/06-exibble.csv
--rw-r--r--   0 runner    (1001) docker     (127)    81025 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/07-towny.csv
--rw-r--r--   0 runner    (1001) docker     (127)    20916 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/08-metro.csv
--rw-r--r--   0 runner    (1001) docker     (127)    21007 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/09-constants.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/10-illness.csv
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/11-islands.csv
--rw-r--r--   0 runner    (1001) docker     (127)    28139 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.098188 great_tables-0.6.0/great_tables/data/metro_images/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/metro_1.svg
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/metro_10.svg
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/metro_11.svg
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/metro_12.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/metro_13.svg
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/metro_14.svg
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/metro_2.svg
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/metro_3.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/metro_3bis.svg
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/metro_4.svg
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/metro_5.svg
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/metro_6.svg
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/metro_7.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/metro_7bis.svg
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/metro_8.svg
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/metro_9.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/rer_A.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/rer_B.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/rer_C.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/rer_D.svg
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/rer_E.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/tram_T1.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/tram_T11.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/tram_T13.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/tram_T2.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/tram_T3a.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/tram_T3b.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/tram_T4.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/tram_T5.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/tram_T6.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/tram_T7.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/tram_T8.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/tram_T9.svg
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/transilien_H.svg
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/transilien_J.svg
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/transilien_K.svg
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/transilien_L.svg
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/transilien_N.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/transilien_P.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/transilien_R.svg
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/transilien_U.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/x-airquality.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/x_currencies.csv
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/x_currency_symbols.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/x_default_locales.csv
--rw-r--r--   0 runner    (1001) docker     (127)   255709 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/x_locales.csv
--rw-r--r--   0 runner    (1001) docker     (127)    15541 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/gt.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/loc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/shiny.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/style.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/utils_render_common.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/vals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.106188 great_tables-0.6.0/great_tables.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10846 2024-05-16 20:30:46.000000 great_tables-0.6.0/great_tables.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-05-16 20:30:47.000000 great_tables-0.6.0/great_tables.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:30:46.000000 great_tables-0.6.0/great_tables.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-16 20:30:46.000000 great_tables-0.6.0/great_tables.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 20:30:46.000000 great_tables-0.6.0/great_tables.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-16 20:30:42.000000 great_tables-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-16 20:30:42.000000 great_tables-0.6.0/pyrightconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 20:30:47.106188 great_tables-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.102188 great_tables-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.106188 great_tables-0.6.0/tests/__snapshots__/
--rw-r--r--   0 runner    (1001) docker     (127)    10002 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/__snapshots__/test_export.ambr
--rw-r--r--   0 runner    (1001) docker     (127)    14024 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/__snapshots__/test_formats.ambr
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/__snapshots__/test_locations.ambr
--rw-r--r--   0 runner    (1001) docker     (127)    14728 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/__snapshots__/test_options.ambr
--rw-r--r--   0 runner    (1001) docker     (127)    31704 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/__snapshots__/test_repr.ambr
--rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/__snapshots__/test_scss.ambr
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/__snapshots__/test_tbl_data.ambr
--rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/__snapshots__/test_utils_render_html.ambr
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.106188 great_tables-0.6.0/tests/data_color/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.106188 great_tables-0.6.0/tests/data_color/__snapshots__/
--rw-r--r--   0 runner    (1001) docker     (127)    22008 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/data_color/__snapshots__/test_data_color.ambr
--rw-r--r--   0 runner    (1001) docker     (127)     9178 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/data_color/test_data_color.py
--rw-r--r--   0 runner    (1001) docker     (127)    18147 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/data_color/test_data_color_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test__boxhead.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test__formats_vals.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test__stubhead.py
--rw-r--r--   0 runner    (1001) docker     (127)    54571 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test__utils_nanoplots.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_boxhead.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    56339 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_formats_nanoplots.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_gt.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_gt_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_heading.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)    18349 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_repr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_scss.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_shiny.py
--rw-r--r--   0 runner    (1001) docker     (127)    10528 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_spanners.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_styles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_tab_create_modify.py
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_tbl_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_utils_render_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_utils_render_html.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.469805 great_tables-0.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.413805 great_tables-0.6.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-23 18:26:38.000000 great_tables-0.6.1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-23 18:26:38.000000 great_tables-0.6.1/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.413805 great_tables-0.6.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-23 18:26:38.000000 great_tables-0.6.1/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-23 18:26:38.000000 great_tables-0.6.1/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-23 18:26:38.000000 great_tables-0.6.1/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-23 18:26:38.000000 great_tables-0.6.1/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.413805 great_tables-0.6.1/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-23 18:26:38.000000 great_tables-0.6.1/.github/scripts/no_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-23 18:26:38.000000 great_tables-0.6.1/.github/scripts/save_browser_table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.413805 great_tables-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-23 18:26:38.000000 great_tables-0.6.1/.github/workflows/ci-docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-05-23 18:26:38.000000 great_tables-0.6.1/.github/workflows/ci-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-23 18:26:38.000000 great_tables-0.6.1/.github/workflows/code-checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-23 18:26:38.000000 great_tables-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-23 18:26:38.000000 great_tables-0.6.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.413805 great_tables-0.6.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-23 18:26:38.000000 great_tables-0.6.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-23 18:26:38.000000 great_tables-0.6.1/.vscode/settings.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1081 2024-05-23 18:26:38.000000 great_tables-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-23 18:26:38.000000 great_tables-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-23 18:26:38.000000 great_tables-0.6.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-05-23 18:26:43.469805 great_tables-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-05-23 18:26:38.000000 great_tables-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.413805 great_tables-0.6.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.409805 great_tables-0.6.1/docs/_extensions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.409805 great_tables-0.6.1/docs/_extensions/machow/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.413805 great_tables-0.6.1/docs/_extensions/machow/interlinks/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/_extensions/machow/interlinks/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/_extensions/machow/interlinks/_extension.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/_extensions/machow/interlinks/interlinks.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/_quarto.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.413805 great_tables-0.6.1/docs/articles/
+-rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/articles/intro.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.421805 great_tables-0.6.1/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/assets/GT_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)  2325288 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/assets/datasets.png
+-rw-r--r--   0 runner    (1001) docker     (127)   136430 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/assets/gt_parts_of_a_table.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   342328 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/assets/gt_sp500_table.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    74998 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/assets/gt_workflow_diagram.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   209904 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/assets/tables_from_the_web.png
+-rw-r--r--   0 runner    (1001) docker     (127)   139817 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/assets/the_components_of_a_table.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.421805 great_tables-0.6.1/docs/blog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.421805 great_tables-0.6.1/docs/blog/bring-your-own-df/
+-rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/blog/bring-your-own-df/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.429805 great_tables-0.6.1/docs/blog/design-philosophy/
+-rw-r--r--   0 runner    (1001) docker     (127)   241842 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/blog/design-philosophy/a_simple_table.png
+-rw-r--r--   0 runner    (1001) docker     (127)   195558 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/blog/design-philosophy/cave_grids.png
+-rw-r--r--   0 runner    (1001) docker     (127)   656631 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/blog/design-philosophy/composition_of_a_table_in_GT.png
+-rw-r--r--   0 runner    (1001) docker     (127)   801735 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/blog/design-philosophy/computer_tables.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22595 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/blog/design-philosophy/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)  1486510 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/blog/design-philosophy/nippur_cuneiform_tablet.png
+-rw-r--r--   0 runner    (1001) docker     (127)  1629638 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/blog/design-philosophy/snippets_from_manual_tablular_presentation.png
+-rw-r--r--   0 runner    (1001) docker     (127)   458471 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/blog/design-philosophy/uruk_tablet_with_annotations.png
+-rw-r--r--   0 runner    (1001) docker     (127)   812542 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/blog/design-philosophy/visicalc.png
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/blog/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.429805 great_tables-0.6.1/docs/blog/introduction-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/blog/introduction-0.2.0/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.429805 great_tables-0.6.1/docs/blog/introduction-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8361 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/blog/introduction-0.3.0/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.429805 great_tables-0.6.1/docs/blog/introduction-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/blog/introduction-0.4.0/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/blog/introduction_great_tables.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.429805 great_tables-0.6.1/docs/blog/polars-styling/
+-rw-r--r--   0 runner    (1001) docker     (127)     8771 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/blog/polars-styling/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)   132380 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/blog/polars-styling/table-preview.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.429805 great_tables-0.6.1/docs/blog/pycon-2024-great-tables-are-possible/
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/blog/pycon-2024-great-tables-are-possible/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)   144854 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/blog/pycon-2024-great-tables-are-possible/table.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.433805 great_tables-0.6.1/docs/blog/superbowl-squares/
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/blog/superbowl-squares/_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1949299 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/blog/superbowl-squares/games.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/blog/superbowl-squares/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.433805 great_tables-0.6.1/docs/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.433805 great_tables-0.6.1/docs/examples/_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/examples/_data/coffee-sales.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.437805 great_tables-0.6.1/docs/examples/_data/coffee-table-icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/examples/_data/coffee-table-icons/aeropress.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/examples/_data/coffee-table-icons/cezve.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/examples/_data/coffee-table-icons/chemex.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/examples/_data/coffee-table-icons/cold-brew.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/examples/_data/coffee-table-icons/drip-machine.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/examples/_data/coffee-table-icons/espresso-machine.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/examples/_data/coffee-table-icons/filter.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/examples/_data/coffee-table-icons/french-press.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/examples/_data/coffee-table-icons/grinder.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/examples/_data/coffee-table-icons/kettle.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/examples/_data/coffee-table-icons/moka-pot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/examples/_data/coffee-table-icons/noun-drip-machine-6065915.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/examples/_data/coffee-table-icons/pour-over.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/examples/_data/coffee-table-icons/scale.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/examples/_data/coffee-table-icons/total.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/examples/_data/power_cie_prepared_tbl.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10751 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/examples/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.437805 great_tables-0.6.1/docs/examples/sports-earnings/
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/examples/sports-earnings/basketball.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/examples/sports-earnings/boxing.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/examples/sports-earnings/golf.png
+-rw-r--r--   0 runner    (1001) docker     (127)    76604 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/examples/sports-earnings/index.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/examples/sports-earnings/soccer.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/examples/sports-earnings/sports_earnings.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/examples/sports-earnings/tennis.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.441805 great_tables-0.6.1/docs/get-started/
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/get-started/basic-column-labels.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/get-started/basic-formatting.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/get-started/basic-header.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/get-started/basic-stub.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/get-started/basic-styling.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/get-started/colorizing-with-data.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/get-started/column-selection.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/get-started/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    10497 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/get-started/nanoplots.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/get-started/overview.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/get-started/row-selection.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/get-started/table-theme-options.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/get-started/table-theme-premade.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-23 18:26:38.000000 great_tables-0.6.1/docs/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.445805 great_tables-0.6.1/great_tables/
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/_boxhead.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.445805 great_tables-0.6.1/great_tables/_data_color/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/_data_color/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23399 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/_data_color/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27133 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/_data_color/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/_data_color/palettes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/_databackend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/_footnotes.py
+-rw-r--r--   0 runner    (1001) docker     (127)   151727 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40689 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/_formats_vals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43858 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/_gt_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/_heading.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32073 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/_locale.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14848 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74939 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/_row_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/_scss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/_source_notes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25728 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/_spanners.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/_stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/_stubhead.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12616 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/_styles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6289 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/_tab_create_modify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17251 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/_tbl_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55726 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/_utils_nanoplots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27424 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/_utils_render_html.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.449805 great_tables-0.6.1/great_tables/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/css/gt_colors.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/css/gt_styles_default.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.457805 great_tables-0.6.1/great_tables/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   412361 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/01-countrypops.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    12898 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/02-sza.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/03-gtcars.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   906055 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/04-sp500.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  2848391 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/05-pizzaplace.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/06-exibble.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    81025 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/07-towny.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    20916 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/08-metro.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    21007 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/09-constants.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/10-illness.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/11-islands.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    28139 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.461805 great_tables-0.6.1/great_tables/data/metro_images/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/metro_1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/metro_10.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/metro_11.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/metro_12.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/metro_13.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/metro_14.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/metro_2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/metro_3.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/metro_3bis.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/metro_4.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/metro_5.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/metro_6.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/metro_7.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/metro_7bis.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/metro_8.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/metro_9.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/rer_A.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/rer_B.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/rer_C.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/rer_D.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/rer_E.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/tram_T1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/tram_T11.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/tram_T13.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/tram_T2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/tram_T3a.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/tram_T3b.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/tram_T4.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/tram_T5.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/tram_T6.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/tram_T7.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/tram_T8.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/tram_T9.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/transilien_H.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/transilien_J.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/transilien_K.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/transilien_L.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/transilien_N.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/transilien_P.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/transilien_R.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/metro_images/transilien_U.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/x-airquality.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/x_currencies.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/x_currency_symbols.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/x_default_locales.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   255709 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/data/x_locales.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    15541 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/gt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/loc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/shiny.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/utils_render_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-23 18:26:38.000000 great_tables-0.6.1/great_tables/vals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.469805 great_tables-0.6.1/great_tables.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-05-23 18:26:43.000000 great_tables-0.6.1/great_tables.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8444 2024-05-23 18:26:43.000000 great_tables-0.6.1/great_tables.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 18:26:43.000000 great_tables-0.6.1/great_tables.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-23 18:26:43.000000 great_tables-0.6.1/great_tables.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-23 18:26:43.000000 great_tables-0.6.1/great_tables.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-23 18:26:38.000000 great_tables-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-23 18:26:38.000000 great_tables-0.6.1/pyrightconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 18:26:43.469805 great_tables-0.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.465805 great_tables-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.469805 great_tables-0.6.1/tests/__snapshots__/
+-rw-r--r--   0 runner    (1001) docker     (127)    10002 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/__snapshots__/test_export.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)    14024 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/__snapshots__/test_formats.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/__snapshots__/test_locations.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)    14728 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/__snapshots__/test_options.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)    31704 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/__snapshots__/test_repr.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/__snapshots__/test_scss.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/__snapshots__/test_tbl_data.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/__snapshots__/test_utils_render_html.ambr
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.469805 great_tables-0.6.1/tests/data_color/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:43.469805 great_tables-0.6.1/tests/data_color/__snapshots__/
+-rw-r--r--   0 runner    (1001) docker     (127)    22008 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/data_color/__snapshots__/test_data_color.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)     9178 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/data_color/test_data_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18147 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/data_color/test_data_color_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/test__boxhead.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/test__formats_vals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/test__stubhead.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54571 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/test__utils_nanoplots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/test_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/test_boxhead.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56333 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/test_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/test_formats_nanoplots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/test_gt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/test_gt_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/test_heading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/test_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18349 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/test_scss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/test_shiny.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10528 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/test_spanners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/test_styles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/test_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/test_tab_create_modify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/test_tbl_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/test_utils_render_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-05-23 18:26:38.000000 great_tables-0.6.1/tests/test_utils_render_html.py
```

### Comparing `great_tables-0.6.0/.github/CODE_OF_CONDUCT.md` & `great_tables-0.6.1/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/.github/CONTRIBUTING.md` & `great_tables-0.6.1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/.github/ISSUE_TEMPLATE/bug.md` & `great_tables-0.6.1/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/.github/ISSUE_TEMPLATE/feature.md` & `great_tables-0.6.1/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/.github/ISSUE_TEMPLATE/question.md` & `great_tables-0.6.1/.github/ISSUE_TEMPLATE/question.md`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/.github/PULL_REQUEST_TEMPLATE.md` & `great_tables-0.6.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/.github/scripts/no_pandas.py` & `great_tables-0.6.1/.github/scripts/no_pandas.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/.github/scripts/save_browser_table.py` & `great_tables-0.6.1/.github/scripts/save_browser_table.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/.github/workflows/ci-docs.yaml` & `great_tables-0.6.1/.github/workflows/ci-docs.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 on:
   push:
     branches:
       - main
+      - 'docs-preview-**'
   pull_request:
     branches:
       - main
 
 name: CI Docs
 
 jobs:
```

### Comparing `great_tables-0.6.0/.github/workflows/ci-tests.yaml` & `great_tables-0.6.1/.github/workflows/ci-tests.yaml`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/.github/workflows/code-checks.yaml` & `great_tables-0.6.1/.github/workflows/code-checks.yaml`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/.gitignore` & `great_tables-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/.pre-commit-config.yaml` & `great_tables-0.6.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/LICENSE` & `great_tables-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/Makefile` & `great_tables-0.6.1/Makefile`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/PKG-INFO` & `great_tables-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: great-tables
-Version: 0.6.0
+Version: 0.6.1
 Summary: Easily generate information-rich, publication-quality tables from Python.
 Author-email: Richard Iannone <rich@posit.co>, Michael Chow <michael.chow@posit.co>
 License: MIT License
         
         Copyright (c) 2022-2024 Posit Software, PBC
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,15 +43,14 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-License-File: AUTHORS.rst
 Requires-Dist: commonmark>=0.9.1
 Requires-Dist: htmltools>=0.4.1
 Requires-Dist: importlib-metadata
 Requires-Dist: typing_extensions>=3.10.0.0
 Requires-Dist: numpy>=1.22.4
 Requires-Dist: Babel>=2.13.1
 Requires-Dist: importlib-resources
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: great-tables Version: 0.6.0 Summary: Easily
+Metadata-Version: 2.1 Name: great-tables Version: 0.6.1 Summary: Easily
 generate information-rich, publication-quality tables from Python. Author-
 email: Richard Iannone
 posit.co>, Michael Chow
 posit.co> License: MIT License Copyright (c) 2022-2024 Posit Software, PBC
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
@@ -27,28 +27,28 @@
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Programming Language :: Python :: Implementation :: PyPy Classifier: Topic ::
 Internet :: WWW/HTTP :: Dynamic Content Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Topic :: Text Processing
 :: Markup :: HTML Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
-LICENSE License-File: AUTHORS.rst Requires-Dist: commonmark>=0.9.1 Requires-
-Dist: htmltools>=0.4.1 Requires-Dist: importlib-metadata Requires-Dist:
-typing_extensions>=3.10.0.0 Requires-Dist: numpy>=1.22.4 Requires-Dist:
-Babel>=2.13.1 Requires-Dist: importlib-resources Provides-Extra: all Requires-
-Dist: great_tables[extra]; extra == "all" Requires-Dist: great_tables[dev];
-extra == "all" Provides-Extra: extra Requires-Dist: selenium>=4.18.1; extra ==
-"extra" Requires-Dist: Pillow>=10.2.0; extra == "extra" Provides-Extra: dev
-Requires-Dist: great_tables[dev-no-pandas]; extra == "dev" Requires-Dist:
-pandas; extra == "dev" Provides-Extra: dev-no-pandas Requires-Dist: black;
-extra == "dev-no-pandas" Requires-Dist: jupyter; extra == "dev-no-pandas"
-Requires-Dist: quartodoc>=0.7.1; python_version >= "3.9" and extra == "dev-no-
-pandas" Requires-Dist: griffe==0.38.1; extra == "dev-no-pandas" Requires-Dist:
-polars; extra == "dev-no-pandas" Requires-Dist: pre-commit==2.15.0; extra ==
-"dev-no-pandas" Requires-Dist: pyarrow; extra == "dev-no-pandas" Requires-Dist:
+LICENSE Requires-Dist: commonmark>=0.9.1 Requires-Dist: htmltools>=0.4.1
+Requires-Dist: importlib-metadata Requires-Dist: typing_extensions>=3.10.0.0
+Requires-Dist: numpy>=1.22.4 Requires-Dist: Babel>=2.13.1 Requires-Dist:
+importlib-resources Provides-Extra: all Requires-Dist: great_tables[extra];
+extra == "all" Requires-Dist: great_tables[dev]; extra == "all" Provides-Extra:
+extra Requires-Dist: selenium>=4.18.1; extra == "extra" Requires-Dist:
+Pillow>=10.2.0; extra == "extra" Provides-Extra: dev Requires-Dist:
+great_tables[dev-no-pandas]; extra == "dev" Requires-Dist: pandas; extra ==
+"dev" Provides-Extra: dev-no-pandas Requires-Dist: black; extra == "dev-no-
+pandas" Requires-Dist: jupyter; extra == "dev-no-pandas" Requires-Dist:
+quartodoc>=0.7.1; python_version >= "3.9" and extra == "dev-no-pandas"
+Requires-Dist: griffe==0.38.1; extra == "dev-no-pandas" Requires-Dist: polars;
+extra == "dev-no-pandas" Requires-Dist: pre-commit==2.15.0; extra == "dev-no-
+pandas" Requires-Dist: pyarrow; extra == "dev-no-pandas" Requires-Dist:
 pyright>=1.1.244; extra == "dev-no-pandas" Requires-Dist: pytest>=3; extra ==
 "dev-no-pandas" Requires-Dist: pytest-cov; extra == "dev-no-pandas" Requires-
 Dist: shiny; extra == "dev-no-pandas" Requires-Dist: syrupy; extra == "dev-no-
 pandas"
  _[_._/_d_o_c_s_/_a_s_s_e_t_s_/_G_T___l_o_g_o_._s_v_g_]_Absolutely Delightful Table-making in Python_ [!
   [Python Versions](https://img.shields.io/pypi/pyversions/great_tables.svg)]
  (https://pypi.python.org/pypi/great_tables) [![PyPI](https://img.shields.io/
```

### Comparing `great_tables-0.6.0/README.md` & `great_tables-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/_extensions/machow/interlinks/interlinks.lua` & `great_tables-0.6.1/docs/_extensions/machow/interlinks/interlinks.lua`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/_quarto.yml` & `great_tables-0.6.1/docs/_quarto.yml`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/articles/intro.qmd` & `great_tables-0.6.1/docs/articles/intro.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/assets/GT_logo.svg` & `great_tables-0.6.1/docs/assets/GT_logo.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/assets/datasets.png` & `great_tables-0.6.1/docs/assets/datasets.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/assets/gt_parts_of_a_table.svg` & `great_tables-0.6.1/docs/assets/gt_parts_of_a_table.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/assets/gt_sp500_table.svg` & `great_tables-0.6.1/docs/assets/gt_sp500_table.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/assets/gt_workflow_diagram.svg` & `great_tables-0.6.1/docs/assets/gt_workflow_diagram.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/assets/tables_from_the_web.png` & `great_tables-0.6.1/docs/assets/tables_from_the_web.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/assets/the_components_of_a_table.svg` & `great_tables-0.6.1/docs/assets/the_components_of_a_table.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/blog/bring-your-own-df/index.qmd` & `great_tables-0.6.1/docs/blog/bring-your-own-df/index.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/blog/design-philosophy/a_simple_table.png` & `great_tables-0.6.1/docs/blog/design-philosophy/a_simple_table.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/blog/design-philosophy/cave_grids.png` & `great_tables-0.6.1/docs/blog/design-philosophy/cave_grids.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/blog/design-philosophy/composition_of_a_table_in_GT.png` & `great_tables-0.6.1/docs/blog/design-philosophy/composition_of_a_table_in_GT.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/blog/design-philosophy/computer_tables.png` & `great_tables-0.6.1/docs/blog/design-philosophy/computer_tables.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/blog/design-philosophy/index.qmd` & `great_tables-0.6.1/docs/blog/design-philosophy/index.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/blog/design-philosophy/nippur_cuneiform_tablet.png` & `great_tables-0.6.1/docs/blog/design-philosophy/nippur_cuneiform_tablet.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/blog/design-philosophy/snippets_from_manual_tablular_presentation.png` & `great_tables-0.6.1/docs/blog/design-philosophy/snippets_from_manual_tablular_presentation.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/blog/design-philosophy/uruk_tablet_with_annotations.png` & `great_tables-0.6.1/docs/blog/design-philosophy/uruk_tablet_with_annotations.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/blog/design-philosophy/visicalc.png` & `great_tables-0.6.1/docs/blog/design-philosophy/visicalc.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/blog/introduction-0.2.0/index.qmd` & `great_tables-0.6.1/docs/blog/introduction-0.2.0/index.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/blog/introduction-0.3.0/index.qmd` & `great_tables-0.6.1/docs/blog/introduction-0.3.0/index.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/blog/introduction-0.4.0/index.qmd` & `great_tables-0.6.1/docs/blog/introduction-0.4.0/index.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/blog/introduction_great_tables.qmd` & `great_tables-0.6.1/docs/blog/introduction_great_tables.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/blog/polars-styling/index.qmd` & `great_tables-0.6.1/docs/blog/polars-styling/index.qmd`

 * *Files 0% similar despite different names*

```diff
@@ -194,20 +194,20 @@
 time_cols = ["Year", "Month", "Day"]
 
 gt_with_spanners = (
     gt_air
 
     # Table column spanners ----
     .tab_spanner(
-        label = "Time",
-        columns = time_cols
+        label="Time",
+        columns=time_cols
     )
     .tab_spanner(
-        label = "Measurement",
-        columns = cs.all().exclude(time_cols)
+        label="Measurement",
+        columns=cs.exclude(time_cols)
     )
 )
 
 gt_with_spanners
 ```
 
 Notice that there are now labels for "Time" and "Measurement" sitting above the column names. This is useful for emphasizing columns that share something in common.
```

### Comparing `great_tables-0.6.0/docs/blog/polars-styling/table-preview.png` & `great_tables-0.6.1/docs/blog/polars-styling/table-preview.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/blog/superbowl-squares/_code.py` & `great_tables-0.6.1/docs/blog/superbowl-squares/_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 # Cross and multiply p(digit | team=KC)p(digit | team=SF) to get
 # the joint probability p(digit_KC, digit_SF | KC, SF)
 joint = (
     home.join(away, on="final_digit", how="cross")
     .with_columns(joint=pl.col("prop") * pl.col("prop_right"))
     .sort("final_digit", "final_digit_right")
     .pivot(values="joint", columns="final_digit_right", index="final_digit")
-    .with_columns((cs.all().exclude("final_digit") * 100).round(1))
+    .with_columns((cs.exclude("final_digit") * 100).round(1))
 )
 
 # Display -----
 
 (
     GT(joint, rowname_col="final_digit")
     .data_color(domain=[0, 4], palette=["red", "grey", "blue"])
```

### Comparing `great_tables-0.6.0/docs/blog/superbowl-squares/games.csv` & `great_tables-0.6.1/docs/blog/superbowl-squares/games.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/blog/superbowl-squares/index.qmd` & `great_tables-0.6.1/docs/blog/superbowl-squares/index.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/examples/_data/coffee-sales.json` & `great_tables-0.6.1/docs/examples/_data/coffee-sales.json`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/examples/_data/coffee-table-icons/aeropress.png` & `great_tables-0.6.1/docs/examples/_data/coffee-table-icons/aeropress.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/examples/_data/coffee-table-icons/cezve.png` & `great_tables-0.6.1/docs/examples/_data/coffee-table-icons/cezve.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/examples/_data/coffee-table-icons/chemex.png` & `great_tables-0.6.1/docs/examples/_data/coffee-table-icons/chemex.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/examples/_data/coffee-table-icons/cold-brew.png` & `great_tables-0.6.1/docs/examples/_data/coffee-table-icons/cold-brew.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/examples/_data/coffee-table-icons/drip-machine.png` & `great_tables-0.6.1/docs/examples/_data/coffee-table-icons/drip-machine.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/examples/_data/coffee-table-icons/espresso-machine.png` & `great_tables-0.6.1/docs/examples/_data/coffee-table-icons/espresso-machine.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/examples/_data/coffee-table-icons/filter.png` & `great_tables-0.6.1/docs/examples/_data/coffee-table-icons/filter.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/examples/_data/coffee-table-icons/french-press.png` & `great_tables-0.6.1/docs/examples/_data/coffee-table-icons/french-press.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/examples/_data/coffee-table-icons/grinder.png` & `great_tables-0.6.1/docs/examples/_data/coffee-table-icons/grinder.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/examples/_data/coffee-table-icons/kettle.png` & `great_tables-0.6.1/docs/examples/_data/coffee-table-icons/kettle.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/examples/_data/coffee-table-icons/moka-pot.png` & `great_tables-0.6.1/docs/examples/_data/coffee-table-icons/moka-pot.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/examples/_data/coffee-table-icons/noun-drip-machine-6065915.png` & `great_tables-0.6.1/docs/examples/_data/coffee-table-icons/noun-drip-machine-6065915.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/examples/_data/coffee-table-icons/pour-over.png` & `great_tables-0.6.1/docs/examples/_data/coffee-table-icons/pour-over.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/examples/_data/coffee-table-icons/scale.png` & `great_tables-0.6.1/docs/examples/_data/coffee-table-icons/scale.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/examples/_data/coffee-table-icons/total.png` & `great_tables-0.6.1/docs/examples/_data/coffee-table-icons/total.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/examples/_data/power_cie_prepared_tbl.csv` & `great_tables-0.6.1/docs/examples/_data/power_cie_prepared_tbl.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/examples/index.qmd` & `great_tables-0.6.1/docs/examples/index.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/examples/sports-earnings/basketball.png` & `great_tables-0.6.1/docs/examples/sports-earnings/basketball.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/examples/sports-earnings/boxing.png` & `great_tables-0.6.1/docs/examples/sports-earnings/boxing.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/examples/sports-earnings/golf.png` & `great_tables-0.6.1/docs/examples/sports-earnings/golf.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/examples/sports-earnings/index.ipynb` & `great_tables-0.6.1/docs/examples/sports-earnings/index.ipynb`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/examples/sports-earnings/soccer.png` & `great_tables-0.6.1/docs/examples/sports-earnings/soccer.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/examples/sports-earnings/sports_earnings.csv` & `great_tables-0.6.1/docs/examples/sports-earnings/sports_earnings.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/examples/sports-earnings/tennis.png` & `great_tables-0.6.1/docs/examples/sports-earnings/tennis.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/get-started/basic-column-labels.qmd` & `great_tables-0.6.1/docs/get-started/basic-column-labels.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/get-started/basic-formatting.qmd` & `great_tables-0.6.1/docs/get-started/basic-formatting.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/get-started/basic-header.qmd` & `great_tables-0.6.1/docs/get-started/basic-header.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/get-started/basic-stub.qmd` & `great_tables-0.6.1/docs/get-started/basic-stub.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/get-started/basic-styling.qmd` & `great_tables-0.6.1/docs/get-started/basic-styling.qmd`

 * *Files 0% similar despite different names*

```diff
@@ -218,15 +218,15 @@
 
 ```{python}
 import polars.selectors as cs
 
 gt_pl_air.tab_style(
     style=style.fill(color="yellow"),
     locations=loc.body(
-        columns=cs.all().exclude(["Month", "Day"]),
+        columns=cs.exclude(["Month", "Day"]),
         rows=pl.col("Temp") == pl.col("Temp").max()
     )
 )
 ```
 
 ## Learning more
```

### Comparing `great_tables-0.6.0/docs/get-started/colorizing-with-data.qmd` & `great_tables-0.6.1/docs/get-started/colorizing-with-data.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/get-started/column-selection.qmd` & `great_tables-0.6.1/docs/get-started/column-selection.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/get-started/index.qmd` & `great_tables-0.6.1/docs/get-started/index.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/get-started/nanoplots.qmd` & `great_tables-0.6.1/docs/get-started/nanoplots.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/get-started/overview.qmd` & `great_tables-0.6.1/docs/get-started/overview.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/get-started/row-selection.qmd` & `great_tables-0.6.1/docs/get-started/row-selection.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/get-started/table-theme-options.qmd` & `great_tables-0.6.1/docs/get-started/table-theme-options.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/get-started/table-theme-premade.qmd` & `great_tables-0.6.1/docs/get-started/table-theme-premade.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/docs/styles.css` & `great_tables-0.6.1/docs/styles.css`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/__init__.py` & `great_tables-0.6.1/great_tables/__init__.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/_boxhead.py` & `great_tables-0.6.1/great_tables/_boxhead.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/_data_color/base.py` & `great_tables-0.6.1/great_tables/_data_color/base.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/_data_color/constants.py` & `great_tables-0.6.1/great_tables/_data_color/constants.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/_data_color/palettes.py` & `great_tables-0.6.1/great_tables/_data_color/palettes.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/_databackend.py` & `great_tables-0.6.1/great_tables/_databackend.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/_export.py` & `great_tables-0.6.1/great_tables/_export.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,15 +295,15 @@
 
         # convert to other formats (e.g. pdf, bmp) using PIL
         with tempfile.TemporaryDirectory() as tmp_dir:
             fname = f"{tmp_dir}/image.png"
             el.screenshot(fname)
 
             with open(fname, "rb") as f:
-                Image.open(fp=BytesIO(f)).save(fp=path)
+                Image.open(fp=BytesIO(f.read())).save(fp=path)
 
 
 def _dump_debug_screenshot(driver, path):
     driver.execute_script(
         "document.body.style.border = '5px solid blue'; "
         "document.body.childNodes[0].style.border = '5px solid orange'; "
         "document.getElementsByTagName('table')[0].style.border = '5px solid green'; "
```

### Comparing `great_tables-0.6.0/great_tables/_formats.py` & `great_tables-0.6.1/great_tables/_formats.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/_formats_vals.py` & `great_tables-0.6.1/great_tables/_formats_vals.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/_gt_data.py` & `great_tables-0.6.1/great_tables/_gt_data.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/_heading.py` & `great_tables-0.6.1/great_tables/_heading.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/_helpers.py` & `great_tables-0.6.1/great_tables/_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import string
 from typing import Any, Callable, Literal
 
 from typing_extensions import TypeAlias
 
 from ._text import Text
 
-
 FontStackName: TypeAlias = Literal[
     "system-ui",
     "transitional",
     "old-style",
     "humanist",
     "geometric-humanist",
     "classical-humanist",
@@ -24,14 +23,137 @@
     "slab-serif",
     "antique",
     "didone",
     "handwritten",
 ]
 
 
+FONT_STACKS = {
+    "system-ui": [
+        "system-ui",
+        "sans-serif",
+    ],
+    "transitional": [
+        "Charter",
+        "Bitstream Charter",
+        "Sitka Text",
+        "Cambria",
+        "serif",
+    ],
+    "old-style": [
+        "Iowan Old Style",
+        "Palatino Linotype",
+        "URW Palladio L",
+        "P052",
+        "serif",
+    ],
+    "humanist": [
+        "Seravek",
+        "Gill Sans Nova",
+        "Ubuntu",
+        "Calibri",
+        "DejaVu Sans",
+        "source-sans-pro",
+        "sans-serif",
+    ],
+    "geometric-humanist": [
+        "Avenir",
+        "Montserrat",
+        "Corbel",
+        "URW Gothic",
+        "source-sans-pro",
+        "sans-serif",
+    ],
+    "classical-humanist": [
+        "Optima",
+        "Candara",
+        "Noto Sans",
+        "source-sans-pro",
+        "sans-serif",
+    ],
+    "neo-grotesque": [
+        "Inter",
+        "Roboto",
+        "Helvetica Neue",
+        "Arial Nova",
+        "Nimbus Sans",
+        "Arial",
+        "sans-serif",
+    ],
+    "monospace-slab-serif": [
+        "Nimbus Mono PS",
+        "Courier New",
+        "monospace",
+    ],
+    "monospace-code": [
+        "ui-monospace",
+        "Cascadia Code",
+        "Source Code Pro",
+        "Menlo",
+        "Consolas",
+        "DejaVu Sans Mono",
+        "monospace",
+    ],
+    "industrial": [
+        "Bahnschrift",
+        "DIN Alternate",
+        "Franklin Gothic Medium",
+        "Nimbus Sans Narrow",
+        "sans-serif-condensed",
+        "sans-serif",
+    ],
+    "rounded-sans": [
+        "ui-rounded",
+        "Hiragino Maru Gothic ProN",
+        "Quicksand",
+        "Comfortaa",
+        "Manjari",
+        "Arial Rounded MT",
+        "Arial Rounded MT Bold",
+        "Calibri",
+        "source-sans-pro",
+        "sans-serif",
+    ],
+    "slab-serif": [
+        "Rockwell",
+        "Rockwell Nova",
+        "Roboto Slab",
+        "DejaVu Serif",
+        "Sitka Small",
+        "serif",
+    ],
+    "antique": [
+        "Superclarendon",
+        "Bookman Old Style",
+        "URW Bookman",
+        "URW Bookman L",
+        "Georgia Pro",
+        "Georgia",
+        "serif",
+    ],
+    "didone": [
+        "Didot",
+        "Bodoni MT",
+        "Noto Serif Display",
+        "URW Palladio L",
+        "P052",
+        "Sylfaen",
+        "serif",
+    ],
+    "handwritten": [
+        "Segoe Print",
+        "Bradley Hand",
+        "Chilanka",
+        "TSCu_Comic",
+        "casual",
+        "cursive",
+    ],
+}
+
+
 def px(x: int | float) -> str:
     """
     Helper for providing a CSS length value in pixels.
 
     For certain parameters, a length value is required. Examples include the setting of font sizes
     (e.g., in `cell_text()`) and thicknesses of lines (e.g., in `cell_borders()`). Setting a length
     in pixels with `px()` allows for an absolute definition of size as opposed to the analogous
@@ -379,138 +501,19 @@
     list of font names that make up the font stack. This is exactly the type of input that the
     `table_font_names` parameter requires.
     """
     return _get_font_stack(name)
 
 
 def _get_font_stack(name: FontStackName = "system-ui", add_emoji: bool = True) -> list[str]:
-    font_stack_names = [
-        "system-ui",
-        "transitional",
-        "old-style",
-        "humanist",
-        "geometric-humanist",
-        "classical-humanist",
-        "neo-grotesque",
-        "monospace-slab-serif",
-        "monospace-code",
-        "industrial",
-        "rounded-sans",
-        "slab-serif",
-        "antique",
-        "didone",
-        "handwritten",
-    ]
+    font_stack = FONT_STACKS.get(name)
 
-    if name not in font_stack_names:
+    if font_stack is None:
         raise ValueError(f"Invalid font stack name: {name}")
 
-    if name == "system-ui":
-        font_stack = ["system-ui", "sans-serif"]
-    elif name == "transitional":
-        font_stack = ["Charter", "Bitstream Charter", "Sitka Text", "Cambria", "serif"]
-    elif name == "old-style":
-        font_stack = ["Iowan Old Style", "Palatino Linotype", "URW Palladio L", "P052", "serif"]
-    elif name == "humanist":
-        font_stack = [
-            "Seravek",
-            "Gill Sans Nova",
-            "Ubuntu",
-            "Calibri",
-            "DejaVu Sans",
-            "source-sans-pro",
-            "sans-serif",
-        ]
-    elif name == "geometric-humanist":
-        font_stack = [
-            "Avenir",
-            "Montserrat",
-            "Corbel",
-            "URW Gothic",
-            "source-sans-pro",
-            "sans-serif",
-        ]
-    elif name == "classical-humanist":
-        font_stack = ["Optima", "Candara", "Noto Sans", "source-sans-pro", "sans-serif"]
-    elif name == "neo-grotesque":
-        font_stack = [
-            "Inter",
-            "Roboto",
-            "Helvetica Neue",
-            "Arial Nova",
-            "Nimbus Sans",
-            "Arial",
-            "sans-serif",
-        ]
-    elif name == "monospace-slab-serif":
-        font_stack = ["Nimbus Mono PS", "Courier New", "monospace"]
-    elif name == "monospace-code":
-        font_stack = [
-            "ui-monospace",
-            "Cascadia Code",
-            "Source Code Pro",
-            "Menlo",
-            "Consolas",
-            "DejaVu Sans Mono",
-            "monospace",
-        ]
-    elif name == "industrial":
-        font_stack = [
-            "Bahnschrift",
-            "DIN Alternate",
-            "Franklin Gothic Medium",
-            "Nimbus Sans Narrow",
-            "sans-serif-condensed",
-            "sans-serif",
-        ]
-    elif name == "rounded-sans":
-        font_stack = [
-            "ui-rounded",
-            "Hiragino Maru Gothic ProN",
-            "Quicksand",
-            "Comfortaa",
-            "Manjari",
-            "Arial Rounded MT",
-            "Arial Rounded MT Bold",
-            "Calibri",
-            "source-sans-pro",
-            "sans-serif",
-        ]
-    elif name == "slab-serif":
-        font_stack = [
-            "Rockwell",
-            "Rockwell Nova",
-            "Roboto Slab",
-            "DejaVu Serif",
-            "Sitka Small",
-            "serif",
-        ]
-    elif name == "antique":
-        font_stack = [
-            "Superclarendon",
-            "Bookman Old Style",
-            "URW Bookman",
-            "URW Bookman L",
-            "Georgia Pro",
-            "Georgia",
-            "serif",
-        ]
-    elif name == "didone":
-        font_stack = [
-            "Didot",
-            "Bodoni MT",
-            "Noto Serif Display",
-            "URW Palladio L",
-            "P052",
-            "Sylfaen",
-            "serif",
-        ]
-    elif name == "handwritten":
-        font_stack = ["Segoe Print", "Bradley Hand", "Chilanka", "TSCu_Comic", "casual", "cursive"]
-
     if add_emoji:
         font_stack.extend(
             ["Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji"]
         )
 
     return font_stack
```

### Comparing `great_tables-0.6.0/great_tables/_locale.py` & `great_tables-0.6.1/great_tables/_locale.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/_locations.py` & `great_tables-0.6.1/great_tables/_locations.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/_options.py` & `great_tables-0.6.1/great_tables/_options.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/_render.py` & `great_tables-0.6.1/great_tables/_render.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/_scss.py` & `great_tables-0.6.1/great_tables/_scss.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/_source_notes.py` & `great_tables-0.6.1/great_tables/_source_notes.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/_spanners.py` & `great_tables-0.6.1/great_tables/_spanners.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/_stub.py` & `great_tables-0.6.1/great_tables/_stub.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/_stubhead.py` & `great_tables-0.6.1/great_tables/_stubhead.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/_styles.py` & `great_tables-0.6.1/great_tables/_styles.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/_substitution.py` & `great_tables-0.6.1/great_tables/_substitution.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/_tab_create_modify.py` & `great_tables-0.6.1/great_tables/_tab_create_modify.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/_tbl_data.py` & `great_tables-0.6.1/great_tables/_tbl_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -303,34 +303,55 @@
     raise NotImplementedError(f"Unsupported selection expr: {expr}")
 
 
 @eval_select.register
 def _(data: PlDataFrame, expr: Union[list[str], _selector_proxy_], strict: bool = True) -> _NamePos:
     # TODO: how to annotate type of a polars selector?
     # Seems to be polars.selectors._selector_proxy_.
+    import polars.selectors as cs
+
+    from functools import reduce
+    from operator import or_
     from polars import Expr
-    from polars import selectors
 
     if isinstance(expr, (str, int)):
         expr = [expr]
 
+    if isinstance(expr, list):
+        all_selectors = [
+            cs.by_name(x) if isinstance(x, str) else cs.by_index(x) if isinstance(x, int) else x
+            for x in expr
+        ]
+
+        _validate_selector_list(all_selectors)
+
+        expr = reduce(or_, all_selectors, cs.by_name())
+
     col_pos = {k: ii for ii, k in enumerate(data.columns)}
 
     # just in case _selector_proxy_ gets renamed or something
     # it inherits from Expr, so we can just use that in a pinch
-    cls_selector = getattr(selectors, "_selector_proxy_", Expr)
+    cls_selector = getattr(cs, "_selector_proxy_", Expr)
 
-    if not isinstance(expr, (list, cls_selector)):
+    if not isinstance(expr, cls_selector):
         raise TypeError(f"Unsupported selection expr type: {type(expr)}")
 
     # I don't think there's a way to get the columns w/o running the selection
-    final_columns = selectors.expand_selector(data, expr)
+    final_columns = cs.expand_selector(data, expr)
     return [(col, col_pos[col]) for col in final_columns]
 
 
+def _validate_selector_list(selectors: list):
+    from polars.selectors import is_selector
+
+    for ii, sel in enumerate(selectors):
+        if not is_selector(sel):
+            raise TypeError(f"Expected a list of selectors, but entry {ii} is type: {type(sel)}.")
+
+
 def _eval_select_from_list(
     columns: list[str], expr: list[Union[str, int]]
 ) -> list[tuple[str, int]]:
     col_pos = {k: ii for ii, k in enumerate(columns)}
 
     # TODO: should prohibit duplicate names in expr?
     res: list[tuple[str, int]] = []
```

### Comparing `great_tables-0.6.0/great_tables/_text.py` & `great_tables-0.6.1/great_tables/_text.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/_utils.py` & `great_tables-0.6.1/great_tables/_utils.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/_utils_nanoplots.py` & `great_tables-0.6.1/great_tables/_utils_nanoplots.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/_utils_render_html.py` & `great_tables-0.6.1/great_tables/_utils_render_html.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/css/gt_colors.scss` & `great_tables-0.6.1/great_tables/css/gt_colors.scss`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/css/gt_styles_default.scss` & `great_tables-0.6.1/great_tables/css/gt_styles_default.scss`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/01-countrypops.csv` & `great_tables-0.6.1/great_tables/data/01-countrypops.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/02-sza.csv` & `great_tables-0.6.1/great_tables/data/02-sza.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/03-gtcars.csv` & `great_tables-0.6.1/great_tables/data/03-gtcars.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/04-sp500.csv` & `great_tables-0.6.1/great_tables/data/04-sp500.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/05-pizzaplace.csv` & `great_tables-0.6.1/great_tables/data/05-pizzaplace.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/06-exibble.csv` & `great_tables-0.6.1/great_tables/data/06-exibble.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/07-towny.csv` & `great_tables-0.6.1/great_tables/data/07-towny.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/08-metro.csv` & `great_tables-0.6.1/great_tables/data/08-metro.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/09-constants.csv` & `great_tables-0.6.1/great_tables/data/09-constants.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/10-illness.csv` & `great_tables-0.6.1/great_tables/data/10-illness.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/11-islands.csv` & `great_tables-0.6.1/great_tables/data/11-islands.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/__init__.py` & `great_tables-0.6.1/great_tables/data/__init__.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/metro_10.svg` & `great_tables-0.6.1/great_tables/data/metro_images/metro_10.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/metro_11.svg` & `great_tables-0.6.1/great_tables/data/metro_images/metro_11.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/metro_12.svg` & `great_tables-0.6.1/great_tables/data/metro_images/metro_12.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/metro_13.svg` & `great_tables-0.6.1/great_tables/data/metro_images/metro_13.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/metro_14.svg` & `great_tables-0.6.1/great_tables/data/metro_images/metro_14.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/metro_2.svg` & `great_tables-0.6.1/great_tables/data/metro_images/metro_2.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/metro_3.svg` & `great_tables-0.6.1/great_tables/data/metro_images/metro_3.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/metro_3bis.svg` & `great_tables-0.6.1/great_tables/data/metro_images/metro_3bis.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/metro_5.svg` & `great_tables-0.6.1/great_tables/data/metro_images/metro_5.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/metro_6.svg` & `great_tables-0.6.1/great_tables/data/metro_images/metro_6.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/metro_7bis.svg` & `great_tables-0.6.1/great_tables/data/metro_images/metro_7bis.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/metro_8.svg` & `great_tables-0.6.1/great_tables/data/metro_images/metro_8.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/metro_9.svg` & `great_tables-0.6.1/great_tables/data/metro_images/metro_9.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/rer_A.svg` & `great_tables-0.6.1/great_tables/data/metro_images/rer_A.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/rer_B.svg` & `great_tables-0.6.1/great_tables/data/metro_images/rer_B.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/rer_C.svg` & `great_tables-0.6.1/great_tables/data/metro_images/rer_C.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/rer_D.svg` & `great_tables-0.6.1/great_tables/data/metro_images/rer_D.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/rer_E.svg` & `great_tables-0.6.1/great_tables/data/metro_images/rer_E.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/tram_T1.svg` & `great_tables-0.6.1/great_tables/data/metro_images/tram_T1.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/tram_T11.svg` & `great_tables-0.6.1/great_tables/data/metro_images/tram_T11.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/tram_T13.svg` & `great_tables-0.6.1/great_tables/data/metro_images/tram_T13.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/tram_T2.svg` & `great_tables-0.6.1/great_tables/data/metro_images/tram_T2.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/tram_T3a.svg` & `great_tables-0.6.1/great_tables/data/metro_images/tram_T3a.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/tram_T3b.svg` & `great_tables-0.6.1/great_tables/data/metro_images/tram_T3b.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/tram_T4.svg` & `great_tables-0.6.1/great_tables/data/metro_images/tram_T4.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/tram_T5.svg` & `great_tables-0.6.1/great_tables/data/metro_images/tram_T5.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/tram_T6.svg` & `great_tables-0.6.1/great_tables/data/metro_images/tram_T6.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/tram_T7.svg` & `great_tables-0.6.1/great_tables/data/metro_images/tram_T7.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/tram_T8.svg` & `great_tables-0.6.1/great_tables/data/metro_images/tram_T8.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/tram_T9.svg` & `great_tables-0.6.1/great_tables/data/metro_images/tram_T9.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/transilien_H.svg` & `great_tables-0.6.1/great_tables/data/metro_images/transilien_H.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/transilien_J.svg` & `great_tables-0.6.1/great_tables/data/metro_images/transilien_J.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/transilien_K.svg` & `great_tables-0.6.1/great_tables/data/metro_images/transilien_K.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/transilien_L.svg` & `great_tables-0.6.1/great_tables/data/metro_images/transilien_L.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/transilien_N.svg` & `great_tables-0.6.1/great_tables/data/metro_images/transilien_N.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/transilien_P.svg` & `great_tables-0.6.1/great_tables/data/metro_images/transilien_P.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/transilien_R.svg` & `great_tables-0.6.1/great_tables/data/metro_images/transilien_R.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/metro_images/transilien_U.svg` & `great_tables-0.6.1/great_tables/data/metro_images/transilien_U.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/x-airquality.csv` & `great_tables-0.6.1/great_tables/data/x-airquality.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/x_currencies.csv` & `great_tables-0.6.1/great_tables/data/x_currencies.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/x_default_locales.csv` & `great_tables-0.6.1/great_tables/data/x_default_locales.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/data/x_locales.csv` & `great_tables-0.6.1/great_tables/data/x_locales.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/gt.py` & `great_tables-0.6.1/great_tables/gt.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/shiny.py` & `great_tables-0.6.1/great_tables/shiny.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables/utils_render_common.py` & `great_tables-0.6.1/great_tables/utils_render_common.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/great_tables.egg-info/PKG-INFO` & `great_tables-0.6.1/great_tables.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: great-tables
-Version: 0.6.0
+Version: 0.6.1
 Summary: Easily generate information-rich, publication-quality tables from Python.
 Author-email: Richard Iannone <rich@posit.co>, Michael Chow <michael.chow@posit.co>
 License: MIT License
         
         Copyright (c) 2022-2024 Posit Software, PBC
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,15 +43,14 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-License-File: AUTHORS.rst
 Requires-Dist: commonmark>=0.9.1
 Requires-Dist: htmltools>=0.4.1
 Requires-Dist: importlib-metadata
 Requires-Dist: typing_extensions>=3.10.0.0
 Requires-Dist: numpy>=1.22.4
 Requires-Dist: Babel>=2.13.1
 Requires-Dist: importlib-resources
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: great-tables Version: 0.6.0 Summary: Easily
+Metadata-Version: 2.1 Name: great-tables Version: 0.6.1 Summary: Easily
 generate information-rich, publication-quality tables from Python. Author-
 email: Richard Iannone
 posit.co>, Michael Chow
 posit.co> License: MIT License Copyright (c) 2022-2024 Posit Software, PBC
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
@@ -27,28 +27,28 @@
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Programming Language :: Python :: Implementation :: PyPy Classifier: Topic ::
 Internet :: WWW/HTTP :: Dynamic Content Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Topic :: Text Processing
 :: Markup :: HTML Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
-LICENSE License-File: AUTHORS.rst Requires-Dist: commonmark>=0.9.1 Requires-
-Dist: htmltools>=0.4.1 Requires-Dist: importlib-metadata Requires-Dist:
-typing_extensions>=3.10.0.0 Requires-Dist: numpy>=1.22.4 Requires-Dist:
-Babel>=2.13.1 Requires-Dist: importlib-resources Provides-Extra: all Requires-
-Dist: great_tables[extra]; extra == "all" Requires-Dist: great_tables[dev];
-extra == "all" Provides-Extra: extra Requires-Dist: selenium>=4.18.1; extra ==
-"extra" Requires-Dist: Pillow>=10.2.0; extra == "extra" Provides-Extra: dev
-Requires-Dist: great_tables[dev-no-pandas]; extra == "dev" Requires-Dist:
-pandas; extra == "dev" Provides-Extra: dev-no-pandas Requires-Dist: black;
-extra == "dev-no-pandas" Requires-Dist: jupyter; extra == "dev-no-pandas"
-Requires-Dist: quartodoc>=0.7.1; python_version >= "3.9" and extra == "dev-no-
-pandas" Requires-Dist: griffe==0.38.1; extra == "dev-no-pandas" Requires-Dist:
-polars; extra == "dev-no-pandas" Requires-Dist: pre-commit==2.15.0; extra ==
-"dev-no-pandas" Requires-Dist: pyarrow; extra == "dev-no-pandas" Requires-Dist:
+LICENSE Requires-Dist: commonmark>=0.9.1 Requires-Dist: htmltools>=0.4.1
+Requires-Dist: importlib-metadata Requires-Dist: typing_extensions>=3.10.0.0
+Requires-Dist: numpy>=1.22.4 Requires-Dist: Babel>=2.13.1 Requires-Dist:
+importlib-resources Provides-Extra: all Requires-Dist: great_tables[extra];
+extra == "all" Requires-Dist: great_tables[dev]; extra == "all" Provides-Extra:
+extra Requires-Dist: selenium>=4.18.1; extra == "extra" Requires-Dist:
+Pillow>=10.2.0; extra == "extra" Provides-Extra: dev Requires-Dist:
+great_tables[dev-no-pandas]; extra == "dev" Requires-Dist: pandas; extra ==
+"dev" Provides-Extra: dev-no-pandas Requires-Dist: black; extra == "dev-no-
+pandas" Requires-Dist: jupyter; extra == "dev-no-pandas" Requires-Dist:
+quartodoc>=0.7.1; python_version >= "3.9" and extra == "dev-no-pandas"
+Requires-Dist: griffe==0.38.1; extra == "dev-no-pandas" Requires-Dist: polars;
+extra == "dev-no-pandas" Requires-Dist: pre-commit==2.15.0; extra == "dev-no-
+pandas" Requires-Dist: pyarrow; extra == "dev-no-pandas" Requires-Dist:
 pyright>=1.1.244; extra == "dev-no-pandas" Requires-Dist: pytest>=3; extra ==
 "dev-no-pandas" Requires-Dist: pytest-cov; extra == "dev-no-pandas" Requires-
 Dist: shiny; extra == "dev-no-pandas" Requires-Dist: syrupy; extra == "dev-no-
 pandas"
  _[_._/_d_o_c_s_/_a_s_s_e_t_s_/_G_T___l_o_g_o_._s_v_g_]_Absolutely Delightful Table-making in Python_ [!
   [Python Versions](https://img.shields.io/pypi/pyversions/great_tables.svg)]
  (https://pypi.python.org/pypi/great_tables) [![PyPI](https://img.shields.io/
```

### Comparing `great_tables-0.6.0/great_tables.egg-info/SOURCES.txt` & `great_tables-0.6.1/great_tables.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,9 @@
 .gitignore
 .pre-commit-config.yaml
-AUTHORS.rst
-CHANGELOG.md
-CODE_OF_CONDUCT.md
-CONTRIBUTING.md
-HISTORY.rst
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 pyproject.toml
 pyrightconfig.json
 .github/CODE_OF_CONDUCT.md
@@ -51,14 +46,16 @@
 docs/blog/design-philosophy/uruk_tablet_with_annotations.png
 docs/blog/design-philosophy/visicalc.png
 docs/blog/introduction-0.2.0/index.qmd
 docs/blog/introduction-0.3.0/index.qmd
 docs/blog/introduction-0.4.0/index.qmd
 docs/blog/polars-styling/index.qmd
 docs/blog/polars-styling/table-preview.png
+docs/blog/pycon-2024-great-tables-are-possible/index.qmd
+docs/blog/pycon-2024-great-tables-are-possible/table.html
 docs/blog/superbowl-squares/_code.py
 docs/blog/superbowl-squares/games.csv
 docs/blog/superbowl-squares/index.qmd
 docs/examples/index.qmd
 docs/examples/_data/coffee-sales.json
 docs/examples/_data/power_cie_prepared_tbl.csv
 docs/examples/_data/coffee-table-icons/aeropress.png
```

### Comparing `great_tables-0.6.0/pyproject.toml` & `great_tables-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/tests/__snapshots__/test_export.ambr` & `great_tables-0.6.1/tests/__snapshots__/test_export.ambr`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/tests/__snapshots__/test_formats.ambr` & `great_tables-0.6.1/tests/__snapshots__/test_formats.ambr`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/tests/__snapshots__/test_options.ambr` & `great_tables-0.6.1/tests/__snapshots__/test_options.ambr`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/tests/__snapshots__/test_repr.ambr` & `great_tables-0.6.1/tests/__snapshots__/test_repr.ambr`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/tests/__snapshots__/test_scss.ambr` & `great_tables-0.6.1/tests/__snapshots__/test_scss.ambr`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/tests/__snapshots__/test_utils_render_html.ambr` & `great_tables-0.6.1/tests/__snapshots__/test_utils_render_html.ambr`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/tests/data_color/__snapshots__/test_data_color.ambr` & `great_tables-0.6.1/tests/data_color/__snapshots__/test_data_color.ambr`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/tests/data_color/test_data_color.py` & `great_tables-0.6.1/tests/data_color/test_data_color.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/tests/data_color/test_data_color_utils.py` & `great_tables-0.6.1/tests/data_color/test_data_color_utils.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/tests/test__boxhead.py` & `great_tables-0.6.1/tests/test__boxhead.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,15 +64,30 @@
     aligned_table = table.cols_align()
     all_column_align = [x.column_align for x in aligned_table._boxhead._d]
 
     # Check that all columns align "left"
     assert all_column_align == ["left", "left"]
 
 
-def test_cols_align():
+def test_cols_align_columns_str():
+    df = pl.DataFrame({"A": [1, 2, 3], "B": [4, 5, 6], "C": [7.1, 8.2, 9.3]})
+    table = gt.GT(df)
+
+    # Select columns by a list of column names
+    aligned_table = table.cols_align(align="center", columns="B")
+    all_column_align = [x.column_align for x in aligned_table._boxhead._d]
+
+    assert all_column_align == [
+        "right",  # `auto_align` for `int` is "right"
+        "center",  # manually assign
+        "right",  # `auto_align` for `float` is "right"
+    ]
+
+
+def test_cols_align_columns_list_of_str():
     df = pl.DataFrame({"A": [1, 2, 3], "B": [4, 5, 6], "C": [7.1, 8.2, 9.3]})
     table = gt.GT(df)
 
     # Select columns by a list of column names
     aligned_table = table.cols_align(align="left", columns=["A"])
     all_column_align = [x.column_align for x in aligned_table._boxhead._d]
```

### Comparing `great_tables-0.6.0/tests/test__stubhead.py` & `great_tables-0.6.1/tests/test__stubhead.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/tests/test__utils_nanoplots.py` & `great_tables-0.6.1/tests/test__utils_nanoplots.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/tests/test_export.py` & `great_tables-0.6.1/tests/test_export.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,22 +29,19 @@
 
 def test_html_string_generated(gt_tbl: GT, snapshot: str):
     assert snapshot == gt_tbl.as_raw_html()
 
 
 @pytest.mark.skipif(sys.platform == "win32", reason="chrome might not be installed.")
 @pytest.mark.extra
-def test_save_image_file(gt_tbl: GT):
+def test_save_image_file(gt_tbl: GT, tmp_path):
 
-    gt_tbl.save(file="test_image.png")
+    f_path = tmp_path / "test_image.png"
+    gt_tbl.save(file=str(f_path))
 
-    # Wait for the file to be created before checking; wait up to
-    # 5 seconds for the async save to complete
-    for _ in range(5):
-        if Path("test_image.png").exists():
-            break
-        else:
-            time.sleep(1)
+    time.sleep(0.1)
+    assert f_path.exists()
 
-    assert Path("test_image.png").exists()
 
-    Path("test_image.png").unlink()
+def test_save_non_png(gt_tbl: GT, tmp_path):
+    f_path = tmp_path / "test_image.pdf"
+    gt_tbl.save(file=str(f_path))
```

### Comparing `great_tables-0.6.0/tests/test_formats.py` & `great_tables-0.6.1/tests/test_formats.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         .fmt_scientific(columns="num")
         .fmt_date(columns="date", date_style="day_month_year")
     )
 
     assert_repr_html(snapshot, new_gt)
 
 
-@pytest.mark.parametrize("expr", [[0, -1], pl.selectors.all().exclude("y")])
+@pytest.mark.parametrize("expr", [[0, -1], pl.selectors.exclude("y")])
 def test_format_col_selection_multi(expr: Any):
     df = pd.DataFrame({"x": [1], "y": [2], "z": [3]})
 
     if isinstance(expr, pl.Expr):
         gt = GT(pl.from_pandas(df))
     else:
         gt = GT(df)
```

### Comparing `great_tables-0.6.0/tests/test_formats_nanoplots.py` & `great_tables-0.6.1/tests/test_formats_nanoplots.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/tests/test_gt.py` & `great_tables-0.6.1/tests/test_gt.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/tests/test_gt_data.py` & `great_tables-0.6.1/tests/test_gt_data.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/tests/test_locations.py` & `great_tables-0.6.1/tests/test_locations.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,14 +17,21 @@
 from great_tables._styles import CellStyleText, FromColumn
 
 
 def test_resolve_vector_i():
     assert resolve_vector_i(["x", "a"], ["a", "b", "x"], "") == [0, 2]
 
 
+def test_resolve_vector_i_raises():
+    with pytest.raises(NotImplementedError) as exc_info:
+        resolve_vector_i([1, 2], ["a", "b", "x"], "")
+
+    assert "Selecting entries currently requires a list of strings." in exc_info.value.args[0]
+
+
 def test_resolve_cols_i_gt_data():
     gt = GT(pd.DataFrame(columns=["a", "b", "x"]))
     assert resolve_cols_i(gt, ["x", "a"]) == [("x", 2), ("a", 0)]
 
 
 def test_resolve_cols_i_strings():
     df = pd.DataFrame(columns=["a", "b", "x"])
@@ -32,37 +39,82 @@
 
 
 def test_resolve_cols_i_ints():
     df = pd.DataFrame(columns=["a", "b", "x"])
     assert resolve_cols_i(df, [-1, 0]) == [("x", 2), ("a", 0)]
 
 
+def test_resolve_cols_i_raises():
+    df = pd.DataFrame(columns=["a", "b", "x"])
+    assert resolve_cols_i(df, [-1, 0]) == [("x", 2), ("a", 0)]
+
+
 def test_resolve_rows_i_gt_data():
     gt = GT(pd.DataFrame({"x": ["a", "b", "c"]}), rowname_col="x")
     assert resolve_rows_i(gt, ["b", "a"]) == [("a", 0), ("b", 1)]
 
 
+def test_resolve_rows_i_gt_data_nothing():
+    gt = GT(pd.DataFrame({"x": ["a", "b", "c"]}), rowname_col="x")
+    assert resolve_rows_i(gt, null_means="nothing") == []
+
+
+@pytest.mark.parametrize("s, resolved", [("x", [("x", 1)]), ("a", [("a", 0), ("a", 2)])])
+def test_resolve_rows_i_string(s, resolved):
+    assert resolve_rows_i(["a", "x", "a", "b"], s) == resolved
+
+
 def test_resolve_rows_i_strings():
     assert resolve_rows_i(["a", "x", "a", "b"], ["x", "a"]) == [("a", 0), ("x", 1), ("a", 2)]
 
 
+@pytest.mark.parametrize("i, resolved", [(0, [("a", 0)]), (-1, [("b", 3)])])
+def test_resolve_rows_i_int(i, resolved):
+    assert resolve_rows_i(["a", "x", "a", "b"], i) == resolved
+
+
 def test_resolve_rows_i_ints():
     assert resolve_rows_i(["a", "x", "a", "b"], [0, -1]) == [("a", 0), ("b", 3)]
 
 
 def test_resolve_rows_i_polars_expr():
     gt = GT(pl.DataFrame({"x": ["a", "b", "c"]}), rowname_col="x")
     assert resolve_rows_i(gt, pl.col("x").is_in(["a", "b"])) == [("a", 0), ("b", 1)]
 
 
 def test_resolve_rows_i_func_expr():
     gt = GT(pd.DataFrame({"x": ["a", "b", "c"]}), rowname_col="x")
     assert resolve_rows_i(gt, lambda D: D["x"].isin(["a", "b"])) == [("a", 0), ("b", 1)]
 
 
+def test_resolve_rows_i_func_expr_return_non_bool_pd_series():
+    gt = GT(pd.DataFrame({"x": ["a", "b", "c"]}), rowname_col="x")
+    with pytest.raises(ValueError) as exc_info:
+        resolve_rows_i(gt, lambda D: pd.Series([4, 5, 6]))
+
+    assert (
+        "If you select rows using a callable, it must take a DataFrame, "
+        + "and return a boolean Series."
+        in exc_info.value.args[0]
+    )
+
+
+@pytest.mark.parametrize("bad_expr", [(4, 5, 6), {7, 8, 9}, {"col1": 1, "col2": 2, "col3": 3}])
+def test_resolve_rows_i_raises(bad_expr):
+    gt = GT(pd.DataFrame({"x": ["a", "b", "c"]}), rowname_col="x")
+    with pytest.raises(NotImplementedError) as exc_info:
+        resolve_rows_i(gt, bad_expr)
+
+    expected = exc_info.value.args[0]
+    assert "Currently, rows can only be selected using these approaches:" in expected
+    assert "a list of integers" in expected
+    assert "a polars expression" in expected
+    assert "a callable that takes a DataFrame and returns a boolean Series" in expected
+
+
 def test_resolve_loc_body():
     gt = GT(pd.DataFrame({"x": [1, 2], "y": [3, 4]}))
 
     cells = resolve(LocBody(["x"], [-1]), gt)
 
     assert isinstance(cells, list)
     assert len(cells) == 1
```

### Comparing `great_tables-0.6.0/tests/test_options.py` & `great_tables-0.6.1/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/tests/test_repr.py` & `great_tables-0.6.1/tests/test_repr.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/tests/test_scss.py` & `great_tables-0.6.1/tests/test_scss.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/tests/test_spanners.py` & `great_tables-0.6.1/tests/test_spanners.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/tests/test_styles.py` & `great_tables-0.6.1/tests/test_styles.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/tests/test_substitutions.py` & `great_tables-0.6.1/tests/test_substitutions.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/tests/test_tab_create_modify.py` & `great_tables-0.6.1/tests/test_tab_create_modify.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/tests/test_tbl_data.py` & `great_tables-0.6.1/tests/test_tbl_data.py`

 * *Files 27% similar despite different names*

```diff
@@ -66,22 +66,69 @@
 
     if isinstance(dst, pd.DataFrame):
         dst.index = pd.Index([0, 2])
 
     assert_frame_equal(res, dst)
 
 
-@pytest.mark.parametrize(
-    "expr", [["col2", "col1"], [1, 0], ["col2", 0], pl.selectors.all().exclude("col3")]
-)
+@pytest.mark.parametrize("expr", [["col2", "col1"], [1, 0], ["col2", 0], [1, "col1"]])
 def test_eval_select_with_list(df: DataFrameLike, expr):
-    sel = eval_select(df, ["col2", "col1"])
+    sel = eval_select(df, expr)
     assert sel == [("col2", 1), ("col1", 0)]
 
 
+@pytest.mark.parametrize(
+    "expr",
+    [
+        pl.selectors.exclude("col3"),
+        pl.selectors.starts_with("col1") | pl.selectors.starts_with("col2"),
+    ],
+)
+def test_eval_select_with_list_pl_selector(expr):
+    df = pl.DataFrame({"col1": [1, 2, 3], "col2": ["a", "b", "c"], "col3": [4.0, 5.0, 6.0]})
+    sel = eval_select(df, expr)
+    assert sel == [("col1", 0), ("col2", 1)]
+
+
+@pytest.mark.parametrize("expr", [["col2", 1.2]])
+def test_eval_select_pandas_raises1(expr):
+    df = pd.DataFrame({"col1": [1, 2, 3], "col2": ["a", "b", "c"], "col3": [4.0, 5.0, 6.0]})
+    with pytest.raises(TypeError) as exc_info:
+        eval_select(df, expr)
+
+    assert "Only int and str are supported." in str(exc_info.value.args[0])
+
+
+@pytest.mark.parametrize("expr", [3.45, {"col2"}, ("col2",)])
+def test_eval_select_pandas_raises2(expr):
+    df = pd.DataFrame({"col1": [1, 2, 3], "col2": ["a", "b", "c"], "col3": [4.0, 5.0, 6.0]})
+    with pytest.raises(NotImplementedError) as exc_info:
+        eval_select(df, expr)
+
+    assert "Unsupported selection expr: " in str(exc_info.value.args[0])
+
+
+@pytest.mark.parametrize("expr", [3.45, {6}, (7.8,)])
+def test_eval_select_polars_raises(expr):
+    df = pl.DataFrame({"col1": [1, 2, 3], "col2": ["a", "b", "c"], "col3": [4.0, 5.0, 6.0]})
+    with pytest.raises(TypeError) as exc_info:
+        eval_select(df, expr)
+
+    assert "Unsupported selection expr type:" in str(exc_info.value.args[0])
+
+
+def test_eval_selector_polars_list_raises():
+    expr = ["col1", 1.2]
+    df = pl.DataFrame({"col1": [], "col2": [], "col3": []})
+    with pytest.raises(TypeError) as exc_info:
+        eval_select(df, expr)
+
+    assert "entry 1 is type: <class 'float'>" in str(exc_info.value.args[0])
+
+
 def test_create_empty_frame(df: DataFrameLike):
     res = create_empty_frame(df)
     col = [None] * 3
 
     if isinstance(res, pd.DataFrame):
         dst = pd.DataFrame({"col1": col, "col2": col, "col3": col}, dtype="string")
     else:
```

### Comparing `great_tables-0.6.0/tests/test_utils.py` & `great_tables-0.6.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/tests/test_utils_render_common.py` & `great_tables-0.6.1/tests/test_utils_render_common.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.6.0/tests/test_utils_render_html.py` & `great_tables-0.6.1/tests/test_utils_render_html.py`

 * *Files identical despite different names*

