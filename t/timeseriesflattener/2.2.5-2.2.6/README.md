# Comparing `tmp/timeseriesflattener-2.2.5.tar.gz` & `tmp/timeseriesflattener-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeseriesflattener-2.2.5.tar", last modified: Wed May 22 07:30:38 2024, max compression
+gzip compressed data, was "timeseriesflattener-2.2.6.tar", last modified: Thu May 23 10:58:11 2024, max compression
```

## Comparing `timeseriesflattener-2.2.5.tar` & `timeseriesflattener-2.2.6.tar`

### file list

```diff
@@ -1,213 +1,213 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.516650 timeseriesflattener-2.2.5/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.448650 timeseriesflattener-2.2.5/.devcontainer/
--rw-r--r--   0 root         (0) root         (0)     1639 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.devcontainer/devcontainer.json
--rw-r--r--   0 root         (0) root         (0)      148 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.devcontainer/post-start.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.452650 timeseriesflattener-2.2.5/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.440650 timeseriesflattener-2.2.5/.github/actions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.452650 timeseriesflattener-2.2.5/.github/actions/test/
--rw-r--r--   0 root         (0) root         (0)      901 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.github/actions/test/action.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.452650 timeseriesflattener-2.2.5/.github/actions/test_tutorials/
--rw-r--r--   0 root         (0) root         (0)      885 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.github/actions/test_tutorials/action.yml
--rw-r--r--   0 root         (0) root         (0)      529 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.github/dependabot.yml
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.github/pull_request_template.md
--rw-r--r--   0 root         (0) root         (0)     1689 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.github/recommended_repo_setup.md
--rw-r--r--   0 root         (0) root         (0)      465 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.github/setup_ci.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.452650 timeseriesflattener-2.2.5/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      636 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.github/workflows/benchmark.yml
--rw-r--r--   0 root         (0) root         (0)      720 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.github/workflows/check_for_rej.yml
--rw-r--r--   0 root         (0) root         (0)      849 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)      898 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)      727 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.github/workflows/generate_paper_pdf.yml
--rw-r--r--   0 root         (0) root         (0)     1939 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.github/workflows/main_test_and_release.yml
--rw-r--r--   0 root         (0) root         (0)     1025 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.github/workflows/pre-commit.yml
--rw-r--r--   0 root         (0) root         (0)     1132 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.github/workflows/stalebot.yml
--rw-r--r--   0 root         (0) root         (0)      788 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.github/workflows/static_type_checks.yml
--rw-r--r--   0 root         (0) root         (0)     2885 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.gitignore
--rw-r--r--   0 root         (0) root         (0)      697 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)        7 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.python-version
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.452650 timeseriesflattener-2.2.5/.vscode/
--rw-r--r--   0 root         (0) root         (0)      346 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.vscode/extensions.json
--rw-r--r--   0 root         (0) root         (0)      249 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.vscode/settings.json
--rw-r--r--   0 root         (0) root         (0)     1373 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.vscode/tasks.json
--rw-r--r--   0 root         (0) root         (0)     1286 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/.zenodo.json
--rw-r--r--   0 root         (0) root         (0)    75066 2024-05-22 07:30:32.000000 timeseriesflattener-2.2.5/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     5238 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     4474 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)     1031 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/Dockerfile
--rw-r--r--   0 root         (0) root         (0)     1087 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      262 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/Makefile
--rw-r--r--   0 root         (0) root         (0)    11525 2024-05-22 07:30:38.516650 timeseriesflattener-2.2.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7649 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/README.md
--rw-r--r--   0 root         (0) root         (0)     1763 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/citation.cff
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.456650 timeseriesflattener-2.2.5/docs/
--rw-r--r--   0 root         (0) root         (0)      633 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.456650 timeseriesflattener-2.2.5/docs/_static/
--rw-r--r--   0 root         (0) root         (0)    15406 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/_static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)    49714 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)    49714 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/_static/icon_dark.png
--rw-r--r--   0 root         (0) root         (0)   424821 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/_static/terminology_figure.png
--rw-r--r--   0 root         (0) root         (0)      291 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/aggregators.rst
--rw-r--r--   0 root         (0) root         (0)     4115 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     2097 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/faq.rst
--rw-r--r--   0 root         (0) root         (0)     1013 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/feature_specifications.rst
--rw-r--r--   0 root         (0) root         (0)      295 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/flattener.rst
--rw-r--r--   0 root         (0) root         (0)     5165 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      299 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/installation.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.456650 timeseriesflattener-2.2.5/docs/tutorials/
--rw-r--r--   0 root         (0) root         (0)   128585 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/tutorials/01_basic.ipynb
--rw-r--r--   0 root         (0) root         (0)    50850 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/tutorials/02_advanced.ipynb
--rw-r--r--   0 root         (0) root         (0)    29677 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/tutorials/03_text.ipynb
--rw-r--r--   0 root         (0) root         (0)     5314 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/tutorials/04_from_legacy.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.460650 timeseriesflattener-2.2.5/docs/tutorials/img/
--rw-r--r--   0 root         (0) root         (0)    78953 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/tutorials/img/term_a.png
--rw-r--r--   0 root         (0) root         (0)   109486 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/tutorials/img/term_b.png
--rw-r--r--   0 root         (0) root         (0)   107613 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/tutorials/img/term_c.png
--rw-r--r--   0 root         (0) root         (0)   250306 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/tutorials/img/term_d.png
--rw-r--r--   0 root         (0) root         (0)      404 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/docs/tutorials.rst
--rw-r--r--   0 root         (0) root         (0)     1833 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/example.py
--rw-r--r--   0 root         (0) root         (0)    49714 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/icon.png
--rw-r--r--   0 root         (0) root         (0)      426 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/lefthook.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.460650 timeseriesflattener-2.2.5/paper/
--rw-r--r--   0 root         (0) root         (0)    14392 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/paper/paper.bib
--rw-r--r--   0 root         (0) root         (0)     9344 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/paper/paper.md
--rw-r--r--   0 root         (0) root         (0)     4633 2024-05-22 07:30:32.000000 timeseriesflattener-2.2.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2520 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/requirements-dev.lock
--rw-r--r--   0 root         (0) root         (0)     1474 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/requirements.lock
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 07:30:38.516650 timeseriesflattener-2.2.5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.460650 timeseriesflattener-2.2.5/src/
--rw-r--r--   0 root         (0) root         (0)     1379 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/conftest.py
--rw-r--r--   0 root         (0) root         (0)     5193 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/test_benchmark.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.464650 timeseriesflattener-2.2.5/src/timeseriesflattener/
--rw-r--r--   0 root         (0) root         (0)      776 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1467 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/_frame_validator.py
--rw-r--r--   0 root         (0) root         (0)     3705 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/_intermediary_frames.py
--rw-r--r--   0 root         (0) root         (0)     3922 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/aggregators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.464650 timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3708 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/from_legacy.py
--rw-r--r--   0 root         (0) root         (0)     2602 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/meta.py
--rw-r--r--   0 root         (0) root         (0)     2658 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/outcome.py
--rw-r--r--   0 root         (0) root         (0)     1784 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/prediction_times.py
--rw-r--r--   0 root         (0) root         (0)     1504 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/predictor.py
--rw-r--r--   0 root         (0) root         (0)     1367 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/static.py
--rw-r--r--   0 root         (0) root         (0)     1349 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/test_from_legacy.py
--rw-r--r--   0 root         (0) root         (0)     1917 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/test_specs.py
--rw-r--r--   0 root         (0) root         (0)     2148 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/timedelta.py
--rw-r--r--   0 root         (0) root         (0)     1170 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/timestamp_frame.py
--rw-r--r--   0 root         (0) root         (0)     7279 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/flattener.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.468650 timeseriesflattener-2.2.5/src/timeseriesflattener/frame_utilities/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/frame_utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      505 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/frame_utilities/_horisontally_concat.py
--rw-r--r--   0 root         (0) root         (0)      614 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/frame_utilities/anyframe_to_lazyframe.py
--rw-r--r--   0 root         (0) root         (0)     1042 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/process_spec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.468650 timeseriesflattener-2.2.5/src/timeseriesflattener/spec_processors/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/spec_processors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1043 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/spec_processors/static.py
--rw-r--r--   0 root         (0) root         (0)    10312 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/spec_processors/temporal.py
--rw-r--r--   0 root         (0) root         (0)     1864 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/spec_processors/test_static.py
--rw-r--r--   0 root         (0) root         (0)    10592 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/spec_processors/test_temporal.py
--rw-r--r--   0 root         (0) root         (0)     1542 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/spec_processors/timedelta.py
--rw-r--r--   0 root         (0) root         (0)     5207 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/test_aggregators.py
--rw-r--r--   0 root         (0) root         (0)    12858 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/test_flattener.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.468650 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/
--rw-r--r--   0 root         (0) root         (0)     1519 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/load_synth_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.468650 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/synth_data_generator/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/synth_data_generator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5619 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py
--rw-r--r--   0 root         (0) root         (0)     2746 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py
--rw-r--r--   0 root         (0) root         (0)     1958 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py
--rw-r--r--   0 root         (0) root         (0)      983 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/synth_data_generator/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.444650 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.444650 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/flattened/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.468650 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/
--rw-r--r--   0 root         (0) root         (0)     1494 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
--rw-r--r--   0 root         (0) root         (0)   864795 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.484650 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/
--rw-r--r--   0 root         (0) root         (0)      754 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/create_synth_birthdays.py
--rw-r--r--   0 root         (0) root         (0)      744 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py
--rw-r--r--   0 root         (0) root         (0)      830 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py
--rw-r--r--   0 root         (0) root         (0)      807 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py
--rw-r--r--   0 root         (0) root         (0)      731 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/create_synth_txt_data.py
--rw-r--r--   0 root         (0) root         (0)   200734 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/synth_birthdays.csv
--rw-r--r--   0 root         (0) root         (0)   248865 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv
--rw-r--r--   0 root         (0) root         (0)   268962 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv
--rw-r--r--   0 root         (0) root         (0)   268904 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv
--rw-r--r--   0 root         (0) root         (0)  4316151 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv
--rw-r--r--   0 root         (0) root         (0)  4315816 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv
--rw-r--r--   0 root         (0) root         (0)    68900 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv
--rw-r--r--   0 root         (0) root         (0)    84570 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv
--rw-r--r--   0 root         (0) root         (0)     5511 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/testing/utils_for_testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.488650 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/
--rw-r--r--   0 root         (0) root         (0)      264 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2855 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/aggregation_fns.py
--rw-r--r--   0 root         (0) root         (0)     1070 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/df_transforms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.488650 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/feature_cache/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/feature_cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2016 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/feature_cache/abstract_feature_cache.py
--rw-r--r--   0 root         (0) root         (0)     6160 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/feature_cache/cache_to_disk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.488650 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/feature_specs/
--rw-r--r--   0 root         (0) root         (0)     5548 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/feature_specs/group_specs.py
--rw-r--r--   0 root         (0) root         (0)     7846 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/feature_specs/single_specs.py
--rw-r--r--   0 root         (0) root         (0)    35315 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/flattened_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2150 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/flattened_ds_validator.py
--rw-r--r--   0 root         (0) root         (0)     2229 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/logger.py
--rw-r--r--   0 root         (0) root         (0)     7546 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/misc_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.488650 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/
--rw-r--r--   0 root         (0) root         (0)     2981 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/load_synth_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.492650 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/synth_data_generator/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/synth_data_generator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5527 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/synth_data_generator/synth_col_generators.py
--rw-r--r--   0 root         (0) root         (0)     2697 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/synth_data_generator/synth_prediction_times_generator.py
--rw-r--r--   0 root         (0) root         (0)     1962 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/synth_data_generator/synth_txt_data_generator.py
--rw-r--r--   0 root         (0) root         (0)      923 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/synth_data_generator/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.444650 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.444650 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/flattened/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.492650 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/
--rw-r--r--   0 root         (0) root         (0)     1461 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
--rw-r--r--   0 root         (0) root         (0)   864795 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.492650 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/models/
--rw-r--r--   0 root         (0) root         (0)     1877 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/models/create_bow_and_pca_model.py
--rw-r--r--   0 root         (0) root         (0)    25543 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/models/synth_bow_model.pkl
--rw-r--r--   0 root         (0) root         (0)     1015 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/models/synth_pca_model.pkl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.508650 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/
--rw-r--r--   0 root         (0) root         (0)      709 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_prediction_times.py
--rw-r--r--   0 root         (0) root         (0)      795 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_binary.py
--rw-r--r--   0 root         (0) root         (0)      772 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_float.py
--rw-r--r--   0 root         (0) root         (0)      696 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_sex.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_txt_data.py
--rw-r--r--   0 root         (0) root         (0)   200734 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/synth_birthdays.csv
--rw-r--r--   0 root         (0) root         (0)   248865 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/synth_prediction_times.csv
--rw-r--r--   0 root         (0) root         (0)   268962 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_1.csv
--rw-r--r--   0 root         (0) root         (0)   268904 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_2.csv
--rw-r--r--   0 root         (0) root         (0)  4316151 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_1.csv
--rw-r--r--   0 root         (0) root         (0)  4315816 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_2.csv
--rw-r--r--   0 root         (0) root         (0)    68900 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/synth_sex.csv
--rw-r--r--   0 root         (0) root         (0)    84570 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/synth_text_data.csv
--rw-r--r--   0 root         (0) root         (0)     5464 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/utils_for_testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.508650 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.508650 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_feature_cache/
--rw-r--r--   0 root         (0) root         (0)     3308 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_feature_cache/test_cache_to_disk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.508650 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13595 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_aggregation_fns.py
--rw-r--r--   0 root         (0) root         (0)     1295 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_df_transforms.py
--rw-r--r--   0 root         (0) root         (0)     3399 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_feature_spec_objects.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.512650 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23392 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
--rw-r--r--   0 root         (0) root         (0)     2663 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
--rw-r--r--   0 root         (0) root         (0)     2308 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
--rw-r--r--   0 root         (0) root         (0)     2321 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
--rw-r--r--   0 root         (0) root         (0)     5796 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2420 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.512650 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/utils/
--rw-r--r--   0 root         (0) root         (0)      984 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/src/timeseriesflattener/v1/utils/pydantic_basemodel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 07:30:38.512650 timeseriesflattener-2.2.5/src/timeseriesflattener.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11525 2024-05-22 07:30:38.000000 timeseriesflattener-2.2.5/src/timeseriesflattener.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8475 2024-05-22 07:30:38.000000 timeseriesflattener-2.2.5/src/timeseriesflattener.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 07:30:38.000000 timeseriesflattener-2.2.5/src/timeseriesflattener.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      650 2024-05-22 07:30:38.000000 timeseriesflattener-2.2.5/src/timeseriesflattener.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       44 2024-05-22 07:30:38.000000 timeseriesflattener-2.2.5/src/timeseriesflattener.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     8330 2024-05-22 07:30:31.000000 timeseriesflattener-2.2.5/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.886716 timeseriesflattener-2.2.6/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.822715 timeseriesflattener-2.2.6/.devcontainer/
+-rw-r--r--   0 root         (0) root         (0)     1639 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/.devcontainer/devcontainer.json
+-rw-r--r--   0 root         (0) root         (0)      148 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/.devcontainer/post-start.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.822715 timeseriesflattener-2.2.6/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.810715 timeseriesflattener-2.2.6/.github/actions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.822715 timeseriesflattener-2.2.6/.github/actions/test/
+-rw-r--r--   0 root         (0) root         (0)      901 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/.github/actions/test/action.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.822715 timeseriesflattener-2.2.6/.github/actions/test_tutorials/
+-rw-r--r--   0 root         (0) root         (0)      885 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/.github/actions/test_tutorials/action.yml
+-rw-r--r--   0 root         (0) root         (0)      529 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/.github/dependabot.yml
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/.github/pull_request_template.md
+-rw-r--r--   0 root         (0) root         (0)     1689 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/.github/recommended_repo_setup.md
+-rw-r--r--   0 root         (0) root         (0)      465 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/.github/setup_ci.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.826715 timeseriesflattener-2.2.6/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      636 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/.github/workflows/benchmark.yml
+-rw-r--r--   0 root         (0) root         (0)      720 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/.github/workflows/check_for_rej.yml
+-rw-r--r--   0 root         (0) root         (0)      849 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)      898 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)      727 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/.github/workflows/generate_paper_pdf.yml
+-rw-r--r--   0 root         (0) root         (0)     1939 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/.github/workflows/main_test_and_release.yml
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/.github/workflows/pre-commit.yml
+-rw-r--r--   0 root         (0) root         (0)     1132 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/.github/workflows/stalebot.yml
+-rw-r--r--   0 root         (0) root         (0)      788 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/.github/workflows/static_type_checks.yml
+-rw-r--r--   0 root         (0) root         (0)     2885 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      697 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/.python-version
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.826715 timeseriesflattener-2.2.6/.vscode/
+-rw-r--r--   0 root         (0) root         (0)      346 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/.vscode/extensions.json
+-rw-r--r--   0 root         (0) root         (0)      249 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/.vscode/settings.json
+-rw-r--r--   0 root         (0) root         (0)     1373 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/.vscode/tasks.json
+-rw-r--r--   0 root         (0) root         (0)     1286 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/.zenodo.json
+-rw-r--r--   0 root         (0) root         (0)    75600 2024-05-23 10:58:06.000000 timeseriesflattener-2.2.6/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     5238 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     4474 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)     1031 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)     1087 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      262 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/Makefile
+-rw-r--r--   0 root         (0) root         (0)    11525 2024-05-23 10:58:11.886716 timeseriesflattener-2.2.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7649 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/README.md
+-rw-r--r--   0 root         (0) root         (0)     1763 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/citation.cff
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.826715 timeseriesflattener-2.2.6/docs/
+-rw-r--r--   0 root         (0) root         (0)      633 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.830715 timeseriesflattener-2.2.6/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)    15406 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/docs/_static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)    49714 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)    49714 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/docs/_static/icon_dark.png
+-rw-r--r--   0 root         (0) root         (0)   424821 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/docs/_static/terminology_figure.png
+-rw-r--r--   0 root         (0) root         (0)      291 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/docs/aggregators.rst
+-rw-r--r--   0 root         (0) root         (0)     4115 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     2097 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/docs/faq.rst
+-rw-r--r--   0 root         (0) root         (0)     1013 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/docs/feature_specifications.rst
+-rw-r--r--   0 root         (0) root         (0)      295 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/docs/flattener.rst
+-rw-r--r--   0 root         (0) root         (0)     5165 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      299 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/docs/installation.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.830715 timeseriesflattener-2.2.6/docs/tutorials/
+-rw-r--r--   0 root         (0) root         (0)   128585 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/docs/tutorials/01_basic.ipynb
+-rw-r--r--   0 root         (0) root         (0)    50850 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/docs/tutorials/02_advanced.ipynb
+-rw-r--r--   0 root         (0) root         (0)    29677 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/docs/tutorials/03_text.ipynb
+-rw-r--r--   0 root         (0) root         (0)     5366 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/docs/tutorials/04_from_legacy.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.830715 timeseriesflattener-2.2.6/docs/tutorials/img/
+-rw-r--r--   0 root         (0) root         (0)    78953 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/docs/tutorials/img/term_a.png
+-rw-r--r--   0 root         (0) root         (0)   109486 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/docs/tutorials/img/term_b.png
+-rw-r--r--   0 root         (0) root         (0)   107613 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/docs/tutorials/img/term_c.png
+-rw-r--r--   0 root         (0) root         (0)   250306 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/docs/tutorials/img/term_d.png
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/docs/tutorials.rst
+-rw-r--r--   0 root         (0) root         (0)     1833 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/example.py
+-rw-r--r--   0 root         (0) root         (0)    49714 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/icon.png
+-rw-r--r--   0 root         (0) root         (0)      426 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/lefthook.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.834715 timeseriesflattener-2.2.6/paper/
+-rw-r--r--   0 root         (0) root         (0)    14392 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/paper/paper.bib
+-rw-r--r--   0 root         (0) root         (0)     9344 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/paper/paper.md
+-rw-r--r--   0 root         (0) root         (0)     4633 2024-05-23 10:58:06.000000 timeseriesflattener-2.2.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2520 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/requirements-dev.lock
+-rw-r--r--   0 root         (0) root         (0)     1474 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/requirements.lock
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-23 10:58:11.886716 timeseriesflattener-2.2.6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.834715 timeseriesflattener-2.2.6/src/
+-rw-r--r--   0 root         (0) root         (0)     1379 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     5193 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/test_benchmark.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.834715 timeseriesflattener-2.2.6/src/timeseriesflattener/
+-rw-r--r--   0 root         (0) root         (0)      776 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1467 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/_frame_validator.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/_intermediary_frames.py
+-rw-r--r--   0 root         (0) root         (0)     4680 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/aggregators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.838715 timeseriesflattener-2.2.6/src/timeseriesflattener/feature_specs/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/feature_specs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3708 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/feature_specs/from_legacy.py
+-rw-r--r--   0 root         (0) root         (0)     2602 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/feature_specs/meta.py
+-rw-r--r--   0 root         (0) root         (0)     3100 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/feature_specs/outcome.py
+-rw-r--r--   0 root         (0) root         (0)     1784 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/feature_specs/prediction_times.py
+-rw-r--r--   0 root         (0) root         (0)     1763 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/feature_specs/predictor.py
+-rw-r--r--   0 root         (0) root         (0)     1368 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/feature_specs/static.py
+-rw-r--r--   0 root         (0) root         (0)     1328 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/feature_specs/test_from_legacy.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/feature_specs/test_specs.py
+-rw-r--r--   0 root         (0) root         (0)     2148 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/feature_specs/timedelta.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/feature_specs/timestamp_frame.py
+-rw-r--r--   0 root         (0) root         (0)     7269 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/flattener.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.838715 timeseriesflattener-2.2.6/src/timeseriesflattener/frame_utilities/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/frame_utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      505 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/frame_utilities/_horisontally_concat.py
+-rw-r--r--   0 root         (0) root         (0)      614 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/frame_utilities/anyframe_to_lazyframe.py
+-rw-r--r--   0 root         (0) root         (0)     1042 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/process_spec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.842715 timeseriesflattener-2.2.6/src/timeseriesflattener/spec_processors/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/spec_processors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1043 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/spec_processors/static.py
+-rw-r--r--   0 root         (0) root         (0)    10312 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/spec_processors/temporal.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/spec_processors/test_static.py
+-rw-r--r--   0 root         (0) root         (0)    10592 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/spec_processors/test_temporal.py
+-rw-r--r--   0 root         (0) root         (0)     1542 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/spec_processors/timedelta.py
+-rw-r--r--   0 root         (0) root         (0)     6125 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/test_aggregators.py
+-rw-r--r--   0 root         (0) root         (0)    12858 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/test_flattener.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.842715 timeseriesflattener-2.2.6/src/timeseriesflattener/testing/
+-rw-r--r--   0 root         (0) root         (0)     1519 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/testing/load_synth_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.842715 timeseriesflattener-2.2.6/src/timeseriesflattener/testing/synth_data_generator/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/testing/synth_data_generator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5619 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py
+-rw-r--r--   0 root         (0) root         (0)     2746 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py
+-rw-r--r--   0 root         (0) root         (0)     1958 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py
+-rw-r--r--   0 root         (0) root         (0)      983 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/testing/synth_data_generator/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.814715 timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.814715 timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/flattened/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.842715 timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/
+-rw-r--r--   0 root         (0) root         (0)     1494 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
+-rw-r--r--   0 root         (0) root         (0)   864795 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.858715 timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/raw/
+-rw-r--r--   0 root         (0) root         (0)      754 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/raw/create_synth_birthdays.py
+-rw-r--r--   0 root         (0) root         (0)      744 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py
+-rw-r--r--   0 root         (0) root         (0)      830 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py
+-rw-r--r--   0 root         (0) root         (0)      807 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py
+-rw-r--r--   0 root         (0) root         (0)      731 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/raw/create_synth_txt_data.py
+-rw-r--r--   0 root         (0) root         (0)   200734 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/raw/synth_birthdays.csv
+-rw-r--r--   0 root         (0) root         (0)   248865 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv
+-rw-r--r--   0 root         (0) root         (0)   268962 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv
+-rw-r--r--   0 root         (0) root         (0)   268904 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv
+-rw-r--r--   0 root         (0) root         (0)  4316151 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv
+-rw-r--r--   0 root         (0) root         (0)  4315816 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv
+-rw-r--r--   0 root         (0) root         (0)    68900 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv
+-rw-r--r--   0 root         (0) root         (0)    84570 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv
+-rw-r--r--   0 root         (0) root         (0)     5511 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/testing/utils_for_testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.862715 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/
+-rw-r--r--   0 root         (0) root         (0)      264 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2855 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/aggregation_fns.py
+-rw-r--r--   0 root         (0) root         (0)     1070 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/df_transforms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.862715 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/feature_cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/feature_cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2016 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/feature_cache/abstract_feature_cache.py
+-rw-r--r--   0 root         (0) root         (0)     6160 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/feature_cache/cache_to_disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.862715 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/feature_specs/
+-rw-r--r--   0 root         (0) root         (0)     5548 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/feature_specs/group_specs.py
+-rw-r--r--   0 root         (0) root         (0)     7846 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/feature_specs/single_specs.py
+-rw-r--r--   0 root         (0) root         (0)    35315 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/flattened_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2150 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/flattened_ds_validator.py
+-rw-r--r--   0 root         (0) root         (0)     2229 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/logger.py
+-rw-r--r--   0 root         (0) root         (0)     7546 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/misc_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.862715 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/
+-rw-r--r--   0 root         (0) root         (0)     2981 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/load_synth_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.862715 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/synth_data_generator/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/synth_data_generator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5527 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/synth_data_generator/synth_col_generators.py
+-rw-r--r--   0 root         (0) root         (0)     2697 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/synth_data_generator/synth_prediction_times_generator.py
+-rw-r--r--   0 root         (0) root         (0)     1962 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/synth_data_generator/synth_txt_data_generator.py
+-rw-r--r--   0 root         (0) root         (0)      923 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/synth_data_generator/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.818715 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.814715 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/flattened/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.862715 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/
+-rw-r--r--   0 root         (0) root         (0)     1461 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
+-rw-r--r--   0 root         (0) root         (0)   864795 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.866715 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/models/
+-rw-r--r--   0 root         (0) root         (0)     1877 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/models/create_bow_and_pca_model.py
+-rw-r--r--   0 root         (0) root         (0)    25543 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/models/synth_bow_model.pkl
+-rw-r--r--   0 root         (0) root         (0)     1015 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/models/synth_pca_model.pkl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.882716 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/raw/
+-rw-r--r--   0 root         (0) root         (0)      709 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_prediction_times.py
+-rw-r--r--   0 root         (0) root         (0)      795 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_binary.py
+-rw-r--r--   0 root         (0) root         (0)      772 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_float.py
+-rw-r--r--   0 root         (0) root         (0)      696 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_sex.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_txt_data.py
+-rw-r--r--   0 root         (0) root         (0)   200734 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/raw/synth_birthdays.csv
+-rw-r--r--   0 root         (0) root         (0)   248865 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/raw/synth_prediction_times.csv
+-rw-r--r--   0 root         (0) root         (0)   268962 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_1.csv
+-rw-r--r--   0 root         (0) root         (0)   268904 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_2.csv
+-rw-r--r--   0 root         (0) root         (0)  4316151 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_1.csv
+-rw-r--r--   0 root         (0) root         (0)  4315816 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_2.csv
+-rw-r--r--   0 root         (0) root         (0)    68900 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/raw/synth_sex.csv
+-rw-r--r--   0 root         (0) root         (0)    84570 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/raw/synth_text_data.csv
+-rw-r--r--   0 root         (0) root         (0)     5464 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/utils_for_testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.882716 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.882716 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/tests/test_feature_cache/
+-rw-r--r--   0 root         (0) root         (0)     3308 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/tests/test_feature_cache/test_cache_to_disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.882716 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/tests/test_timeseriesflattener/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/tests/test_timeseriesflattener/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13595 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_aggregation_fns.py
+-rw-r--r--   0 root         (0) root         (0)     1295 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_df_transforms.py
+-rw-r--r--   0 root         (0) root         (0)     3399 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_feature_spec_objects.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.882716 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23392 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
+-rw-r--r--   0 root         (0) root         (0)     2663 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
+-rw-r--r--   0 root         (0) root         (0)     2308 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
+-rw-r--r--   0 root         (0) root         (0)     2321 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
+-rw-r--r--   0 root         (0) root         (0)     5796 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2420 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.882716 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/utils/
+-rw-r--r--   0 root         (0) root         (0)      984 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/src/timeseriesflattener/v1/utils/pydantic_basemodel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:58:11.886716 timeseriesflattener-2.2.6/src/timeseriesflattener.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11525 2024-05-23 10:58:11.000000 timeseriesflattener-2.2.6/src/timeseriesflattener.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8475 2024-05-23 10:58:11.000000 timeseriesflattener-2.2.6/src/timeseriesflattener.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 10:58:11.000000 timeseriesflattener-2.2.6/src/timeseriesflattener.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      650 2024-05-23 10:58:11.000000 timeseriesflattener-2.2.6/src/timeseriesflattener.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2024-05-23 10:58:11.000000 timeseriesflattener-2.2.6/src/timeseriesflattener.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     8330 2024-05-23 10:58:05.000000 timeseriesflattener-2.2.6/tasks.py
```

### Comparing `timeseriesflattener-2.2.5/.devcontainer/devcontainer.json` & `timeseriesflattener-2.2.6/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/.github/actions/test/action.yml` & `timeseriesflattener-2.2.6/.github/actions/test/action.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/.github/actions/test_tutorials/action.yml` & `timeseriesflattener-2.2.6/.github/actions/test_tutorials/action.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/.github/dependabot.yml` & `timeseriesflattener-2.2.6/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/.github/recommended_repo_setup.md` & `timeseriesflattener-2.2.6/.github/recommended_repo_setup.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/.github/workflows/benchmark.yml` & `timeseriesflattener-2.2.6/.github/workflows/benchmark.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/.github/workflows/check_for_rej.yml` & `timeseriesflattener-2.2.6/.github/workflows/check_for_rej.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/.github/workflows/dependabot_automerge.yml` & `timeseriesflattener-2.2.6/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/.github/workflows/documentation.yml` & `timeseriesflattener-2.2.6/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/.github/workflows/generate_paper_pdf.yml` & `timeseriesflattener-2.2.6/.github/workflows/generate_paper_pdf.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/.github/workflows/main_test_and_release.yml` & `timeseriesflattener-2.2.6/.github/workflows/main_test_and_release.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/.github/workflows/pre-commit.yml` & `timeseriesflattener-2.2.6/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/.github/workflows/stalebot.yml` & `timeseriesflattener-2.2.6/.github/workflows/stalebot.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/.github/workflows/static_type_checks.yml` & `timeseriesflattener-2.2.6/.github/workflows/static_type_checks.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/.gitignore` & `timeseriesflattener-2.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/.pre-commit-config.yaml` & `timeseriesflattener-2.2.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/.vscode/tasks.json` & `timeseriesflattener-2.2.6/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/.zenodo.json` & `timeseriesflattener-2.2.6/.zenodo.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/CHANGELOG.md` & `timeseriesflattener-2.2.6/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v2.2.6 (2024-05-23)
+
+### Fix
+
+* Change to type instead of instantiated type ([`e327665`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/e3276650ad1751d4c325256b91856c94b1567b99))
+* Misc ([`46c6707`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/46c670727c25ae8e5552a412e867f2e3791dc473))
+* Validate fallback is compatible with output of aggregator ([`6fe230b`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/6fe230bd5889e4a89215a08c4e0b9130c105f920))
+
 ## v2.2.5 (2024-05-22)
 
 ### Fix
 
 * Use Union in pydantic basemodels ([`a80a9c2`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/a80a9c24c6eb7e0ceadba021eb4474325b560a38))
 
 ## v2.2.4 (2024-05-17)
```

### Comparing `timeseriesflattener-2.2.5/CODE_OF_CONDUCT.md` & `timeseriesflattener-2.2.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/CONTRIBUTING.md` & `timeseriesflattener-2.2.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/Dockerfile` & `timeseriesflattener-2.2.6/Dockerfile`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/LICENSE` & `timeseriesflattener-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/PKG-INFO` & `timeseriesflattener-2.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseriesflattener
-Version: 2.2.5
+Version: 2.2.6
 Summary: A package for converting time series data from e.g. electronic health records into wide format data.
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>, Jakob Grøhn Damgaard <bokajgd@gmail.com>, Martin Bernstorff <martinbernstorff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 PSYCOP Group, Aarhus University
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: timeseriesflattener Version: 2.2.5 Summary: A
+Metadata-Version: 2.1 Name: timeseriesflattener Version: 2.2.6 Summary: A
 package for converting time series data from e.g. electronic health records
 into wide format data. Author: Kenneth Enevoldsen Author-email: Lasse Hansen
 gmail.com>, Jakob GrÃ¸hn Damgaard
 gmail.com>, Martin Bernstorff
 gmail.com> License: MIT License Copyright (c) 2022 PSYCOP Group, Aarhus
 University Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
```

### Comparing `timeseriesflattener-2.2.5/README.md` & `timeseriesflattener-2.2.6/README.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/citation.cff` & `timeseriesflattener-2.2.6/citation.cff`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/docs/Makefile` & `timeseriesflattener-2.2.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/docs/_static/favicon.ico` & `timeseriesflattener-2.2.6/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/docs/_static/icon.png` & `timeseriesflattener-2.2.6/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/docs/_static/icon_dark.png` & `timeseriesflattener-2.2.6/docs/_static/icon_dark.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/docs/_static/terminology_figure.png` & `timeseriesflattener-2.2.6/docs/_static/terminology_figure.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/docs/conf.py` & `timeseriesflattener-2.2.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/docs/faq.rst` & `timeseriesflattener-2.2.6/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/docs/feature_specifications.rst` & `timeseriesflattener-2.2.6/docs/feature_specifications.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/docs/index.rst` & `timeseriesflattener-2.2.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/docs/tutorials/01_basic.ipynb` & `timeseriesflattener-2.2.6/docs/tutorials/01_basic.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/docs/tutorials/02_advanced.ipynb` & `timeseriesflattener-2.2.6/docs/tutorials/02_advanced.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/docs/tutorials/03_text.ipynb` & `timeseriesflattener-2.2.6/docs/tutorials/03_text.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/docs/tutorials/04_from_legacy.ipynb` & `timeseriesflattener-2.2.6/docs/tutorials/04_from_legacy.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997137176238738%*

 * *Differences: {"'cells'": "{3: {'source': {delete: [4]}}, 4: {'source': {insert: [(24, '        # boolean, "*

 * *            "requires the fallback to be a bool\\n')], delete: [24]}}, 6: {'source': {insert: "*

 * *            "[(29, '        # boolean, requires the fallback to be a bool\\n')], delete: [29]}}}"}*

```diff
@@ -37,15 +37,14 @@
                 }
             ],
             "source": [
                 "from __future__ import annotations\n",
                 "\n",
                 "import pandas as pd\n",
                 "from timeseriesflattener.v1.aggregation_fns import (\n",
-                "    boolean,\n",
                 "    change_per_day,\n",
                 "    count,\n",
                 "    earliest,\n",
                 "    latest,\n",
                 "    maximum,\n",
                 "    mean,\n",
                 "    minimum,\n",
@@ -80,15 +79,15 @@
                 "        earliest,\n",
                 "        maximum,\n",
                 "        minimum,\n",
                 "        mean,\n",
                 "        summed,\n",
                 "        count,\n",
                 "        variance,\n",
-                "        boolean,\n",
+                "        # boolean, requires the fallback to be a bool\n",
                 "        change_per_day,\n",
                 "    ],\n",
                 "    fallback=[0],\n",
                 ").create_combinations()\n",
                 "\n",
                 "print(f\"The generated specs are for version 1: {isinstance(legacy_spec[0], Version1PredictorSpec)}\")"
             ]
@@ -140,15 +139,15 @@
                 "        earliest,\n",
                 "        maximum,\n",
                 "        minimum,\n",
                 "        mean,\n",
                 "        summed,\n",
                 "        count,\n",
                 "        variance,\n",
-                "        boolean,\n",
+                "        # boolean, requires the fallback to be a bool\n",
                 "        change_per_day,\n",
                 "    ],\n",
                 "    fallback=[0],\n",
                 ").create_combinations()\n",
                 "\n",
                 "print(f\"The generated specs are for version 2: {isinstance(new_specs[0], Version2PredictorSpec)}\")"
             ]
```

### Comparing `timeseriesflattener-2.2.5/docs/tutorials/img/term_a.png` & `timeseriesflattener-2.2.6/docs/tutorials/img/term_a.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/docs/tutorials/img/term_b.png` & `timeseriesflattener-2.2.6/docs/tutorials/img/term_b.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/docs/tutorials/img/term_c.png` & `timeseriesflattener-2.2.6/docs/tutorials/img/term_c.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/docs/tutorials/img/term_d.png` & `timeseriesflattener-2.2.6/docs/tutorials/img/term_d.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/example.py` & `timeseriesflattener-2.2.6/example.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/icon.png` & `timeseriesflattener-2.2.6/icon.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/paper/paper.bib` & `timeseriesflattener-2.2.6/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/paper/paper.md` & `timeseriesflattener-2.2.6/paper/paper.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/pyproject.toml` & `timeseriesflattener-2.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "timeseriesflattener"
-version = "2.2.5"
+version = "2.2.6"
 authors = [
   { name = "Lasse Hansen", email = "lasseh0310@gmail.com" },
   { name = "Jakob Grøhn Damgaard", email = "bokajgd@gmail.com" },
   { name = "Kenneth Enevoldsen" },
   { name = "Martin Bernstorff", email = "martinbernstorff@gmail.com" },
 ]
 description = "A package for converting time series data from e.g. electronic health records into wide format data."
```

### Comparing `timeseriesflattener-2.2.5/requirements-dev.lock` & `timeseriesflattener-2.2.6/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/requirements.lock` & `timeseriesflattener-2.2.6/requirements.lock`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/conftest.py` & `timeseriesflattener-2.2.6/src/conftest.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/test_benchmark.py` & `timeseriesflattener-2.2.6/src/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/__init__.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/__init__.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/_frame_validator.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/_frame_validator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/_intermediary_frames.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/_intermediary_frames.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/aggregators.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/aggregators.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,67 +3,84 @@
 import datetime as dt
 from abc import ABC, abstractmethod
 
 import polars as pl
 from attr import dataclass
 
 
+def _validate_compatible_fallback_type_for_aggregator(
+    aggregator: Aggregator, fallback: str | int | float | None
+) -> None:
+    try:
+        pl.Series([aggregator.output_type()]).fill_null(fallback)
+    except:
+        raise ValueError(
+            f"Invalid fallback value {fallback} for aggregator {aggregator.__class__.__name__}. Fallback of type {type(fallback)} is not compatible with the aggregator's output type of {type(aggregator.output_type)}."
+        )
+
+
 class Aggregator(ABC):
     name: str
+    output_type: type[float | int | bool]
 
     @abstractmethod
     def __call__(self, column_name: str) -> pl.Expr:
         ...
 
     def new_col_name(self, previous_col_name: str) -> str:
         return f"{previous_col_name}_{self.name}"
 
 
 class MinAggregator(Aggregator):
     """Returns the minimum value in the look window."""
 
     name: str = "min"
+    output_type = float
 
     def __call__(self, column_name: str) -> pl.Expr:
         return pl.col(column_name).min().alias(self.new_col_name(column_name))
 
 
 class MaxAggregator(Aggregator):
     """Returns the maximum value in the look window."""
 
     name: str = "max"
+    output_type = float
 
     def __call__(self, column_name: str) -> pl.Expr:
         return pl.col(column_name).max().alias(self.new_col_name(column_name))
 
 
 class MeanAggregator(Aggregator):
     """Returns the mean value in the look window."""
 
     name: str = "mean"
+    output_type = float
 
     def __call__(self, column_name: str) -> pl.Expr:
         return pl.col(column_name).mean().alias(self.new_col_name(column_name))
 
 
 class CountAggregator(Aggregator):
     """Returns the count of non-null values in the look window."""
 
     name: str = "count"
+    output_type = int
 
     def __call__(self, column_name: str) -> pl.Expr:
         return pl.col(column_name).count().alias(self.new_col_name(column_name))
 
 
 @dataclass(frozen=True)
 class EarliestAggregator(Aggregator):
     """Returns the earliest value in the look window."""
 
     timestamp_col_name: str
     name: str = "earliest"
+    output_type = float
 
     def __call__(self, column_name: str) -> pl.Expr:
         return (
             pl.col(column_name)
             .filter(pl.col(self.timestamp_col_name) == pl.col(self.timestamp_col_name).min())
             .first()
             .alias(self.new_col_name(column_name))
@@ -72,46 +89,50 @@
 
 @dataclass(frozen=True)
 class LatestAggregator(Aggregator):
     """Returns the latest value in the look window"""
 
     timestamp_col_name: str
     name: str = "latest"
+    output_type = float
 
     def __call__(self, column_name: str) -> pl.Expr:
         return (
             pl.col(column_name)
             .filter(pl.col(self.timestamp_col_name) == pl.col(self.timestamp_col_name).max())
             .first()
             .alias(self.new_col_name(column_name))
         )
 
 
 class SumAggregator(Aggregator):
     """Returns the sum of all values in the look window."""
 
     name: str = "sum"
+    output_type = float
 
     def __call__(self, column_name: str) -> pl.Expr:
         return pl.col(column_name).sum().alias(self.new_col_name(column_name))
 
 
 class VarianceAggregator(Aggregator):
     """Returns the variance of the values in the look window"""
 
     name: str = "var"
+    output_type = float
 
     def __call__(self, column_name: str) -> pl.Expr:
         return pl.col(column_name).var().alias(self.new_col_name(column_name))
 
 
 class HasValuesAggregator(Aggregator):
-    """Examines whether any values exist in the column. If so, returns 1, else 0."""
+    """Examines whether any values exist in the column. If so, returns True, else False."""
 
     name: str = "bool"
+    output_type = bool
 
     def __call__(self, column_name: str) -> pl.Expr:
         return (
             pl.when(pl.col(column_name).is_not_null())
             .then(1)
             .otherwise(0)
             .cast(pl.Boolean)
@@ -122,14 +143,15 @@
 
 @dataclass(frozen=True)
 class SlopeAggregator(Aggregator):
     """Returns the slope (i.e. the correlation between the timestamp and the value) in the look window."""
 
     timestamp_col_name: str
     name: str = "slope"
+    output_type = float
 
     def __call__(self, column_name: str) -> pl.Expr:
         # Convert to days for the slope. Arbitrarily chosen to be the number of days since 1970-01-01.
         x_col = (pl.col(self.timestamp_col_name) - dt.datetime(1970, 1, 1)).dt.days()
         y_col = pl.col(column_name)
 
         numerator = pl.corr(x_col, y_col, propagate_nans=True) * y_col.std()
```

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/from_legacy.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/feature_specs/from_legacy.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/meta.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/feature_specs/meta.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/outcome.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/feature_specs/outcome.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from dataclasses import InitVar, dataclass
 from typing import TYPE_CHECKING
 
 import polars as pl
 
 from .._frame_validator import _validate_col_name_columns_exist
 from .meta import ValueFrame, _lookdistance_to_normalised_lookperiod
+from ..aggregators import _validate_compatible_fallback_type_for_aggregator
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
     from ..aggregators import Aggregator
     from .timestamp_frame import TimestampValueFrame
 
@@ -30,14 +31,18 @@
         self, lookahead_distances: Sequence[dt.timedelta | tuple[dt.timedelta, dt.timedelta]]
     ):
         self.normalised_lookperiod = [
             _lookdistance_to_normalised_lookperiod(lookdistance=lookdistance, direction="ahead")
             for lookdistance in lookahead_distances
         ]
         _validate_col_name_columns_exist(obj=self)
+        for aggregator in self.aggregators:
+            _validate_compatible_fallback_type_for_aggregator(
+                aggregator=aggregator, fallback=self.fallback
+            )
 
     @property
     def df(self) -> pl.LazyFrame:
         return self.value_frame.df
 
 
 @dataclass
@@ -58,14 +63,18 @@
     def __post_init__(self, init_frame: TimestampValueFrame):
         self.normalised_lookperiod = [
             _lookdistance_to_normalised_lookperiod(lookdistance=lookdistance, direction="ahead")
             for lookdistance in self.lookahead_distances
         ]
 
         self.fallback = 0
+        for aggregator in self.aggregators:
+            _validate_compatible_fallback_type_for_aggregator(
+                aggregator=aggregator, fallback=self.fallback
+            )
 
         self.value_frame = ValueFrame(
             init_df=init_frame.df.with_columns((pl.lit(1)).alias(self.output_name)),
             entity_id_col_name=init_frame.entity_id_col_name,
             value_timestamp_col_name=init_frame.value_timestamp_col_name,
         )
```

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/prediction_times.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/feature_specs/prediction_times.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/predictor.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/feature_specs/predictor.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import datetime as dt
 from dataclasses import InitVar, dataclass
 from typing import TYPE_CHECKING
 
 from .._frame_validator import _validate_col_name_columns_exist
 from .meta import ValueFrame, _lookdistance_to_normalised_lookperiod
+from ..aggregators import _validate_compatible_fallback_type_for_aggregator
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
     import polars as pl
 
     from ..aggregators import Aggregator
@@ -35,11 +36,15 @@
         self, lookbehind_distances: Sequence[dt.timedelta | tuple[dt.timedelta, dt.timedelta]]
     ):
         self.normalised_lookperiod = [
             _lookdistance_to_normalised_lookperiod(lookdistance=lookdistance, direction="behind")
             for lookdistance in lookbehind_distances
         ]
         _validate_col_name_columns_exist(obj=self)
+        for aggregator in self.aggregators:
+            _validate_compatible_fallback_type_for_aggregator(
+                aggregator=aggregator, fallback=self.fallback
+            )
 
     @property
     def df(self) -> pl.LazyFrame:
         return self.value_frame.df
```

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/static.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/feature_specs/static.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,13 +28,13 @@
 
 @dataclass(frozen=True)
 class StaticSpec:
     """Specification for a static feature, e.g. the sex of a person.
 
     The value_frame must contain columns:
         entity_id_col_name: The name of the column containing the entity ids. Must be a string, and the column's values must be strings which are unique.
-        additional columns containing the values of the static feature. The name of the columns will be used for feature naming.
+        additional columns containing the values of the static feature. The names of the columns will be used for feature naming.
     """
 
     value_frame: StaticFrame
     column_prefix: str
     fallback: int | float | str | None
```

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/test_from_legacy.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/feature_specs/test_from_legacy.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,15 +37,14 @@
             earliest,
             maximum,
             minimum,
             mean,
             summed,
             count,
             variance,
-            boolean,
             change_per_day,
         ],
         fallback=[0],
     )
 
     new_specs = legacy_spec.create_combinations()
```

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/test_specs.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/feature_specs/test_specs.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/timedelta.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/feature_specs/timedelta.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/feature_specs/timestamp_frame.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/feature_specs/timestamp_frame.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/flattener.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/flattener.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,19 +106,19 @@
             If None, multiprocessing will be handled entirely by polars, otherwise, 
             specify the number of workers to use with joblib. """
 
     def aggregate_timeseries(
         self, specs: Sequence[ValueSpecification], step_size: dt.timedelta | None = None
     ) -> AggregatedFrame:
         """Perform the aggregation/flattening.
-        
+
         Args:
             specs: The specifications for the features to be created.
-            step_size: The step size for the aggregation. 
-                If not None, will aggregate prediction times in chunks of step_size. 
+            step_size: The step size for the aggregation.
+                If not None, will aggregate prediction times in chunks of step_size.
                 Reduce if you encounter memory issues."""
         if self.compute_lazily:
             print(
                 "We have encountered performance issues on Windows when using lazy evaluation. If you encounter performance issues, try setting lazy=False."
             )
 
         # Check for conflicts in the specs
```

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/frame_utilities/anyframe_to_lazyframe.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/frame_utilities/anyframe_to_lazyframe.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/process_spec.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/process_spec.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/spec_processors/static.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/spec_processors/static.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/spec_processors/temporal.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/spec_processors/temporal.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/spec_processors/test_static.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/spec_processors/test_static.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/spec_processors/test_temporal.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/spec_processors/test_temporal.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/spec_processors/timedelta.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/spec_processors/timedelta.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/test_aggregators.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/test_aggregators.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     LatestAggregator,
     MaxAggregator,
     MeanAggregator,
     MinAggregator,
     SlopeAggregator,
     SumAggregator,
     VarianceAggregator,
+    _validate_compatible_fallback_type_for_aggregator,
 )
 from .spec_processors.temporal import _aggregate_masked_frame
 from .test_flattener import assert_frame_equal
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
@@ -87,15 +88,18 @@
         SingleVarAggregatorExample(
             aggregator=SumAggregator(), input_values=[1, 2], expected_output_values=[3]
         ),
         SingleVarAggregatorExample(
             aggregator=VarianceAggregator(), input_values=[1, 2], expected_output_values=[0.5]
         ),
         SingleVarAggregatorExample(
-            aggregator=HasValuesAggregator(), input_values=[1, 2], expected_output_values=[1], fallback_str="False"
+            aggregator=HasValuesAggregator(),
+            input_values=[1, 2],
+            expected_output_values=[1],
+            fallback_str="False",
         ),
         SingleVarAggregatorExample(
             aggregator=HasValuesAggregator(),
             input_values=[None],  # type: ignore
             expected_output_values=[0],
             fallback_str="False",
         ),
@@ -155,7 +159,34 @@
             timestamp_col_name="timestamp",
         ),
         aggregators=[example.aggregator],
         fallback=np.nan if example.aggregator.name != "bool" else False,
     )
 
     assert_frame_equal(result.collect(), example.expected_output)
+
+
+@pytest.mark.parametrize(
+    ("aggregator", "fallback", "valid_fallback"),
+    [
+        (MeanAggregator(), 1, True),
+        (MeanAggregator(), np.nan, True),
+        (HasValuesAggregator(), np.nan, False),
+        (HasValuesAggregator(), False, True),
+        (HasValuesAggregator(), 1, False),
+    ],
+)
+def test_valid_fallback_for_aggregator(
+    aggregator: Aggregator, fallback: float | int | bool | None, valid_fallback: bool
+):
+    if valid_fallback:
+        assert (
+            _validate_compatible_fallback_type_for_aggregator(
+                aggregator=aggregator, fallback=fallback
+            )
+            is None
+        )
+    else:
+        with pytest.raises(ValueError):
+            _validate_compatible_fallback_type_for_aggregator(
+                aggregator=aggregator, fallback=fallback
+            )
```

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/test_flattener.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/test_flattener.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/load_synth_data.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/testing/load_synth_data.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/synth_data_generator/utils.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/testing/synth_data_generator/utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv` & `timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/create_synth_birthdays.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/raw/create_synth_birthdays.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/synth_birthdays.csv` & `timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/raw/synth_birthdays.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv` & `timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv` & `timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv` & `timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv` & `timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv` & `timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv` & `timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv` & `timeseriesflattener-2.2.6/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/testing/utils_for_testing.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/testing/utils_for_testing.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/aggregation_fns.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/aggregation_fns.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/df_transforms.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/df_transforms.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/feature_cache/abstract_feature_cache.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/feature_cache/abstract_feature_cache.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/feature_cache/cache_to_disk.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/feature_cache/cache_to_disk.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/feature_specs/group_specs.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/feature_specs/group_specs.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/feature_specs/single_specs.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/feature_specs/single_specs.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/flattened_dataset.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/flattened_dataset.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/flattened_ds_validator.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/flattened_ds_validator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/logger.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/logger.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/misc_utils.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/misc_utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/load_synth_data.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/load_synth_data.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/synth_data_generator/synth_col_generators.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/synth_data_generator/synth_col_generators.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/synth_data_generator/synth_prediction_times_generator.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/synth_data_generator/synth_prediction_times_generator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/synth_data_generator/synth_txt_data_generator.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/synth_data_generator/synth_txt_data_generator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/synth_data_generator/utils.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/synth_data_generator/utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/models/create_bow_and_pca_model.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/models/create_bow_and_pca_model.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/models/synth_bow_model.pkl` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/models/synth_bow_model.pkl`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/models/synth_pca_model.pkl` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/models/synth_pca_model.pkl`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_prediction_times.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_prediction_times.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_binary.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_binary.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_float.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_float.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_sex.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_sex.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/synth_birthdays.csv` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/raw/synth_birthdays.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/synth_prediction_times.csv` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/raw/synth_prediction_times.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_1.csv` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_2.csv` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_1.csv` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_2.csv` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/synth_sex.csv` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/raw/synth_sex.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/test_data/raw/synth_text_data.csv` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/test_data/raw/synth_text_data.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/testing/utils_for_testing.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/testing/utils_for_testing.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_feature_cache/test_cache_to_disk.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/tests/test_feature_cache/test_cache_to_disk.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_aggregation_fns.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_aggregation_fns.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_df_transforms.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_df_transforms.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_feature_spec_objects.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_feature_spec_objects.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/utils.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener/v1/utils/pydantic_basemodel.py` & `timeseriesflattener-2.2.6/src/timeseriesflattener/v1/utils/pydantic_basemodel.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener.egg-info/PKG-INFO` & `timeseriesflattener-2.2.6/src/timeseriesflattener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseriesflattener
-Version: 2.2.5
+Version: 2.2.6
 Summary: A package for converting time series data from e.g. electronic health records into wide format data.
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>, Jakob Grøhn Damgaard <bokajgd@gmail.com>, Martin Bernstorff <martinbernstorff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 PSYCOP Group, Aarhus University
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: timeseriesflattener Version: 2.2.5 Summary: A
+Metadata-Version: 2.1 Name: timeseriesflattener Version: 2.2.6 Summary: A
 package for converting time series data from e.g. electronic health records
 into wide format data. Author: Kenneth Enevoldsen Author-email: Lasse Hansen
 gmail.com>, Jakob GrÃ¸hn Damgaard
 gmail.com>, Martin Bernstorff
 gmail.com> License: MIT License Copyright (c) 2022 PSYCOP Group, Aarhus
 University Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
```

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener.egg-info/SOURCES.txt` & `timeseriesflattener-2.2.6/src/timeseriesflattener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/src/timeseriesflattener.egg-info/requires.txt` & `timeseriesflattener-2.2.6/src/timeseriesflattener.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.5/tasks.py` & `timeseriesflattener-2.2.6/tasks.py`

 * *Files identical despite different names*

