# Comparing `tmp/aind_metadata_mapper-0.8.0.tar.gz` & `tmp/aind_metadata_mapper-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_metadata_mapper-0.8.0.tar", last modified: Wed May 22 00:06:41 2024, max compression
+gzip compressed data, was "aind_metadata_mapper-0.9.0.tar", last modified: Wed May 22 21:57:54 2024, max compression
```

## Comparing `aind_metadata_mapper-0.8.0.tar` & `aind_metadata_mapper-0.9.0.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.526428 aind_metadata_mapper-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.502428 aind_metadata_mapper-0.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.506428 aind_metadata_mapper-0.8.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.506428 aind_metadata_mapper-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/.github/workflows/test_and_lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-05-22 00:06:41.526428 aind_metadata_mapper-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.506428 aind_metadata_mapper-0.8.0/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.510428 aind_metadata_mapper-0.8.0/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.510428 aind_metadata_mapper-0.8.0/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/doc_template/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.510428 aind_metadata_mapper-0.8.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/examples/bergamo_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.510428 aind_metadata_mapper-0.8.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/scripts/singularity_build.def
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 00:06:41.526428 aind_metadata_mapper-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.502428 aind_metadata_mapper-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.510428 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-22 00:06:31.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.510428 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/bergamo/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/bergamo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23425 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/bergamo/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.510428 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/dynamic_routing/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/dynamic_routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/dynamic_routing/mvr_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/dynamic_routing/neuropixels_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/dynamic_routing/sync_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/dynamic_routing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.510428 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/exaspim/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/exaspim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.514428 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/fip/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/fip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/fip/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    12051 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/gather_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.514428 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/mesoscope/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/mesoscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/mesoscope/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.514428 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/open_ephys/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/open_ephys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/open_ephys/rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/open_ephys/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.514428 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/smartspim/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/smartspim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.526428 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-05-22 00:06:41.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-22 00:06:41.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 00:06:41.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-22 00:06:41.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 00:06:41.000000 aind_metadata_mapper-0.8.0/src/aind_metadata_mapper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.514428 aind_metadata_mapper-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.506428 aind_metadata_mapper-0.8.0/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.514428 aind_metadata_mapper-0.8.0/tests/resources/bergamo/
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/bergamo/cropped_neuron50_00001.tif
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/bergamo/example_description0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    76696 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/bergamo/example_metadata.txt.gz
--rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/bergamo/expected_session.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.514428 aind_metadata_mapper-0.8.0/tests/resources/dynamic_routing/
--rw-r--r--   0 runner    (1001) docker     (127)    39424 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/dynamic_routing/base-missing-probe_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)    40853 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/dynamic_routing/base_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/dynamic_routing/mvr.ini
--rw-r--r--   0 runner    (1001) docker     (127)    42611 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/dynamic_routing/mvr_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/dynamic_routing/sync.yml
--rw-r--r--   0 runner    (1001) docker     (127)    46653 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/dynamic_routing/sync_rig.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.518428 aind_metadata_mapper-0.8.0/tests/resources/fip/
--rw-r--r--   0 runner    (1001) docker     (127)    15663 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/fip/000000_ophys_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/fip/000000_ophys_session.json
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/fip/example_from_teensy.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.518428 aind_metadata_mapper-0.8.0/tests/resources/gather_metadata_job/
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/gather_metadata_job/example_funding_multiple_response.json
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/gather_metadata_job/example_funding_response.json
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/gather_metadata_job/example_procedures_response.json
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/gather_metadata_job/example_subject_response.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.518428 aind_metadata_mapper-0.8.0/tests/resources/gather_metadata_job/metadata_files/
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/gather_metadata_job/metadata_files/data_description.json
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/gather_metadata_job/metadata_files/procedures.json
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/gather_metadata_job/metadata_files/processing.json
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/gather_metadata_job/metadata_files/subject.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.518428 aind_metadata_mapper-0.8.0/tests/resources/mesoscope/
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/mesoscope/0123456789_Face_20240212T091444.json
--rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/mesoscope/example_extract.json
--rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/mesoscope/example_platform.json
--rw-r--r--   0 runner    (1001) docker     (127)    12605 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/mesoscope/expected_session.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.522428 aind_metadata_mapper-0.8.0/tests/resources/open_ephys/
--rw-r--r--   0 runner    (1001) docker     (127)    11653 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/open_ephys/ephys_session.json
--rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/open_ephys/newscale_main.csv
--rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/open_ephys/newscale_surface_finding.csv
--rw-r--r--   0 runner    (1001) docker     (127)    42283 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/open_ephys/open-ephys-inferred_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)    42266 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/open_ephys/open-ephys_rig.json
--rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/open_ephys/settings.mislabeled-probes-0.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/open_ephys/settings.mislabeled-probes-1.xml
--rw-r--r--   0 runner    (1001) docker     (127)   132751 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/open_ephys/settings.xml
--rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/open_ephys/settings_main.xml
--rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/resources/open_ephys/settings_surface_finding.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.522428 aind_metadata_mapper-0.8.0/tests/test_bergamo/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/test_bergamo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13922 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/test_bergamo/test_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.522428 aind_metadata_mapper-0.8.0/tests/test_dynamic_routing/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/test_dynamic_routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/test_dynamic_routing/test_mvr_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/test_dynamic_routing/test_neuropixels_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/test_dynamic_routing/test_sync_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/test_dynamic_routing/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.522428 aind_metadata_mapper-0.8.0/tests/test_fip/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/test_fip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/test_fip/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)    18232 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/test_gather_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/test_legacy_core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.522428 aind_metadata_mapper-0.8.0/tests/test_mesoscope/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/test_mesoscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7761 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/test_mesoscope/test_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:06:41.522428 aind_metadata_mapper-0.8.0/tests/test_open_ephys/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/test_open_ephys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/test_open_ephys/test_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     9935 2024-05-22 00:06:30.000000 aind_metadata_mapper-0.8.0/tests/test_open_ephys/test_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:57:54.715367 aind_metadata_mapper-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:57:54.691367 aind_metadata_mapper-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:57:54.695367 aind_metadata_mapper-0.9.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:57:54.695367 aind_metadata_mapper-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/.github/workflows/test_and_lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-05-22 21:57:54.711367 aind_metadata_mapper-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:57:54.695367 aind_metadata_mapper-0.9.0/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:57:54.695367 aind_metadata_mapper-0.9.0/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:57:54.699367 aind_metadata_mapper-0.9.0/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/doc_template/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:57:54.699367 aind_metadata_mapper-0.9.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/examples/bergamo_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:57:54.699367 aind_metadata_mapper-0.9.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/scripts/singularity_build.def
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 21:57:54.715367 aind_metadata_mapper-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:57:54.691367 aind_metadata_mapper-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:57:54.699367 aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:57:54.699367 aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/bergamo/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/bergamo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23425 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/bergamo/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:57:54.699367 aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/dynamic_routing/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/dynamic_routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/dynamic_routing/mvr_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/dynamic_routing/neuropixels_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/dynamic_routing/sync_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/dynamic_routing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:57:54.699367 aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/exaspim/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/exaspim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:57:54.699367 aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/fip/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/fip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/fip/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12051 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/gather_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:57:54.699367 aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/mesoscope/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/mesoscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/mesoscope/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:57:54.703367 aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/open_ephys/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/open_ephys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/open_ephys/rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/open_ephys/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:57:54.703367 aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/smartspim/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/smartspim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:57:54.711367 aind_metadata_mapper-0.9.0/src/aind_metadata_mapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-05-22 21:57:54.000000 aind_metadata_mapper-0.9.0/src/aind_metadata_mapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-22 21:57:54.000000 aind_metadata_mapper-0.9.0/src/aind_metadata_mapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 21:57:54.000000 aind_metadata_mapper-0.9.0/src/aind_metadata_mapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-22 21:57:54.000000 aind_metadata_mapper-0.9.0/src/aind_metadata_mapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 21:57:54.000000 aind_metadata_mapper-0.9.0/src/aind_metadata_mapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:57:54.703367 aind_metadata_mapper-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:57:54.695367 aind_metadata_mapper-0.9.0/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:57:54.703367 aind_metadata_mapper-0.9.0/tests/resources/bergamo/
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/bergamo/cropped_neuron50_00001.tif
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/bergamo/example_description0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    76696 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/bergamo/example_metadata.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/bergamo/expected_session.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:57:54.703367 aind_metadata_mapper-0.9.0/tests/resources/dynamic_routing/
+-rw-r--r--   0 runner    (1001) docker     (127)    39424 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/dynamic_routing/base-missing-probe_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)    40853 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/dynamic_routing/base_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/dynamic_routing/mvr.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    42611 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/dynamic_routing/mvr_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/dynamic_routing/sync.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    46653 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/dynamic_routing/sync_rig.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:57:54.703367 aind_metadata_mapper-0.9.0/tests/resources/fip/
+-rw-r--r--   0 runner    (1001) docker     (127)    15663 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/fip/000000_ophys_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/fip/000000_ophys_session.json
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/fip/example_from_teensy.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:57:54.703367 aind_metadata_mapper-0.9.0/tests/resources/gather_metadata_job/
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/gather_metadata_job/example_funding_multiple_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/gather_metadata_job/example_funding_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/gather_metadata_job/example_procedures_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/gather_metadata_job/example_subject_response.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:57:54.707367 aind_metadata_mapper-0.9.0/tests/resources/gather_metadata_job/metadata_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/gather_metadata_job/metadata_files/data_description.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/gather_metadata_job/metadata_files/procedures.json
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/gather_metadata_job/metadata_files/processing.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/gather_metadata_job/metadata_files/subject.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:57:54.707367 aind_metadata_mapper-0.9.0/tests/resources/mesoscope/
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/mesoscope/0123456789_Face_20240212T091444.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/mesoscope/example_extract.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/mesoscope/example_platform.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12605 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/mesoscope/expected_session.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:57:54.707367 aind_metadata_mapper-0.9.0/tests/resources/open_ephys/
+-rw-r--r--   0 runner    (1001) docker     (127)    11653 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/open_ephys/ephys_session.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/open_ephys/newscale_main.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/open_ephys/newscale_surface_finding.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    42283 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/open_ephys/open-ephys-inferred_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)    42266 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/open_ephys/open-ephys_rig.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/open_ephys/settings.mislabeled-probes-0.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/open_ephys/settings.mislabeled-probes-1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   132751 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/open_ephys/settings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/open_ephys/settings_main.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/resources/open_ephys/settings_surface_finding.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:57:54.711367 aind_metadata_mapper-0.9.0/tests/test_bergamo/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/test_bergamo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13922 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/test_bergamo/test_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:57:54.711367 aind_metadata_mapper-0.9.0/tests/test_dynamic_routing/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/test_dynamic_routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/test_dynamic_routing/test_mvr_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/test_dynamic_routing/test_neuropixels_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/test_dynamic_routing/test_sync_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/test_dynamic_routing/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:57:54.711367 aind_metadata_mapper-0.9.0/tests/test_fip/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/test_fip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/test_fip/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18232 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/test_gather_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/test_legacy_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:57:54.711367 aind_metadata_mapper-0.9.0/tests/test_mesoscope/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/test_mesoscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7761 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/test_mesoscope/test_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:57:54.711367 aind_metadata_mapper-0.9.0/tests/test_open_ephys/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/test_open_ephys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/test_open_ephys/test_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9935 2024-05-22 21:57:44.000000 aind_metadata_mapper-0.9.0/tests/test_open_ephys/test_session.py
```

### Comparing `aind_metadata_mapper-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_metadata_mapper-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_metadata_mapper-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/.github/ISSUE_TEMPLATE/user-story.md` & `aind_metadata_mapper-0.9.0/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/.github/workflows/tag_and_publish.yml` & `aind_metadata_mapper-0.9.0/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/.github/workflows/test_and_lint.yml` & `aind_metadata_mapper-0.9.0/.github/workflows/test_and_lint.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/.gitignore` & `aind_metadata_mapper-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/CONTRIBUTING.md` & `aind_metadata_mapper-0.9.0/CONTRIBUTING.md`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 ### Testing
 
 Testing is required to open a PR in this repository to ensure robustness and reliability of our codebase. 
 - **1:1 Correspondence:** Structure unit tests in a manner that mirrors the module structure. 
   - For every package in the src directory, there should be a corresponding test package.
   - For every module in a package, there should be a corresponding unit test module.
   - For every method in a module, there should be a corresponding unit test.
+- **Mocking Writes**: Your unit tests should not write anything out. You can use the `unittest.mock` library to intercept file operations and test your method without actually creating a file.
 - **Test Coverage:** Aim for comprehensive test coverage to validate all critical paths and edge cases within the module. To open a PR, you will need at least 80% coverage. 
   - Please test your changes using the **coverage** library, which will run the tests and log a coverage report:
     ```bash
     coverage run -m unittest discover && coverage report
     ```
     To open the coverage report in a browser, you can run
     ```bash
```

### Comparing `aind_metadata_mapper-0.8.0/LICENSE` & `aind_metadata_mapper-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/PKG-INFO` & `aind_metadata_mapper-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-metadata-mapper
-Version: 0.8.0
+Version: 0.9.0
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_metadata_mapper-0.8.0/README.md` & `aind_metadata_mapper-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/doc_template/Makefile` & `aind_metadata_mapper-0.9.0/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/doc_template/make.bat` & `aind_metadata_mapper-0.9.0/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/doc_template/source/_static/dark-logo.svg` & `aind_metadata_mapper-0.9.0/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/doc_template/source/_static/favicon.ico` & `aind_metadata_mapper-0.9.0/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/doc_template/source/_static/light-logo.svg` & `aind_metadata_mapper-0.9.0/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/doc_template/source/conf.py` & `aind_metadata_mapper-0.9.0/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/examples/bergamo_session.py` & `aind_metadata_mapper-0.9.0/examples/bergamo_session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/pyproject.toml` & `aind_metadata_mapper-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/bergamo/session.py` & `aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/bergamo/session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/core.py` & `aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/core.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/dynamic_routing/mvr_rig.py` & `aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/dynamic_routing/mvr_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/dynamic_routing/neuropixels_rig.py` & `aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/dynamic_routing/neuropixels_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/dynamic_routing/sync_rig.py` & `aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/dynamic_routing/sync_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/dynamic_routing/utils.py` & `aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/dynamic_routing/utils.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/fip/session.py` & `aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/fip/session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/gather_metadata.py` & `aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/gather_metadata.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/mesoscope/session.py` & `aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/mesoscope/session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/open_ephys/rig.py` & `aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/open_ephys/rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/src/aind_metadata_mapper/open_ephys/session.py` & `aind_metadata_mapper-0.9.0/src/aind_metadata_mapper/open_ephys/session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/src/aind_metadata_mapper.egg-info/PKG-INFO` & `aind_metadata_mapper-0.9.0/src/aind_metadata_mapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-metadata-mapper
-Version: 0.8.0
+Version: 0.9.0
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_metadata_mapper-0.8.0/src/aind_metadata_mapper.egg-info/SOURCES.txt` & `aind_metadata_mapper-0.9.0/src/aind_metadata_mapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/bergamo/cropped_neuron50_00001.tif` & `aind_metadata_mapper-0.9.0/tests/resources/bergamo/cropped_neuron50_00001.tif`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/bergamo/example_description0.txt` & `aind_metadata_mapper-0.9.0/tests/resources/bergamo/example_description0.txt`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/bergamo/example_metadata.txt.gz` & `aind_metadata_mapper-0.9.0/tests/resources/bergamo/example_metadata.txt.gz`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/bergamo/expected_session.json` & `aind_metadata_mapper-0.9.0/tests/resources/bergamo/expected_session.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/dynamic_routing/base-missing-probe_rig.json` & `aind_metadata_mapper-0.9.0/tests/resources/dynamic_routing/base-missing-probe_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/dynamic_routing/base_rig.json` & `aind_metadata_mapper-0.9.0/tests/resources/dynamic_routing/base_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/dynamic_routing/mvr.ini` & `aind_metadata_mapper-0.9.0/tests/resources/dynamic_routing/mvr.ini`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/dynamic_routing/mvr_rig.json` & `aind_metadata_mapper-0.9.0/tests/resources/dynamic_routing/mvr_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/dynamic_routing/sync.yml` & `aind_metadata_mapper-0.9.0/tests/resources/dynamic_routing/sync.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/dynamic_routing/sync_rig.json` & `aind_metadata_mapper-0.9.0/tests/resources/dynamic_routing/sync_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/fip/000000_ophys_rig.json` & `aind_metadata_mapper-0.9.0/tests/resources/fip/000000_ophys_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/fip/000000_ophys_session.json` & `aind_metadata_mapper-0.9.0/tests/resources/fip/000000_ophys_session.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/gather_metadata_job/example_funding_multiple_response.json` & `aind_metadata_mapper-0.9.0/tests/resources/gather_metadata_job/example_funding_multiple_response.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/gather_metadata_job/example_procedures_response.json` & `aind_metadata_mapper-0.9.0/tests/resources/gather_metadata_job/example_procedures_response.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/gather_metadata_job/example_subject_response.json` & `aind_metadata_mapper-0.9.0/tests/resources/gather_metadata_job/example_subject_response.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/gather_metadata_job/metadata_files/data_description.json` & `aind_metadata_mapper-0.9.0/tests/resources/gather_metadata_job/metadata_files/data_description.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/gather_metadata_job/metadata_files/procedures.json` & `aind_metadata_mapper-0.9.0/tests/resources/gather_metadata_job/metadata_files/procedures.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/gather_metadata_job/metadata_files/processing.json` & `aind_metadata_mapper-0.9.0/tests/resources/gather_metadata_job/metadata_files/processing.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/gather_metadata_job/metadata_files/subject.json` & `aind_metadata_mapper-0.9.0/tests/resources/gather_metadata_job/metadata_files/subject.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json` & `aind_metadata_mapper-0.9.0/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json` & `aind_metadata_mapper-0.9.0/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/mesoscope/0123456789_Face_20240212T091444.json` & `aind_metadata_mapper-0.9.0/tests/resources/mesoscope/0123456789_Face_20240212T091444.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/mesoscope/example_extract.json` & `aind_metadata_mapper-0.9.0/tests/resources/mesoscope/example_extract.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/mesoscope/example_platform.json` & `aind_metadata_mapper-0.9.0/tests/resources/mesoscope/example_platform.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/mesoscope/expected_session.json` & `aind_metadata_mapper-0.9.0/tests/resources/mesoscope/expected_session.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/open_ephys/ephys_session.json` & `aind_metadata_mapper-0.9.0/tests/resources/open_ephys/ephys_session.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/open_ephys/newscale_main.csv` & `aind_metadata_mapper-0.9.0/tests/resources/open_ephys/newscale_main.csv`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/open_ephys/newscale_surface_finding.csv` & `aind_metadata_mapper-0.9.0/tests/resources/open_ephys/newscale_surface_finding.csv`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/open_ephys/open-ephys-inferred_rig.json` & `aind_metadata_mapper-0.9.0/tests/resources/open_ephys/open-ephys-inferred_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/open_ephys/open-ephys_rig.json` & `aind_metadata_mapper-0.9.0/tests/resources/open_ephys/open-ephys_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/open_ephys/settings.mislabeled-probes-0.xml` & `aind_metadata_mapper-0.9.0/tests/resources/open_ephys/settings.mislabeled-probes-0.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/open_ephys/settings.mislabeled-probes-1.xml` & `aind_metadata_mapper-0.9.0/tests/resources/open_ephys/settings.mislabeled-probes-1.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/open_ephys/settings.xml` & `aind_metadata_mapper-0.9.0/tests/resources/open_ephys/settings.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/open_ephys/settings_main.xml` & `aind_metadata_mapper-0.9.0/tests/resources/open_ephys/settings_main.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/resources/open_ephys/settings_surface_finding.xml` & `aind_metadata_mapper-0.9.0/tests/resources/open_ephys/settings_surface_finding.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/test_bergamo/test_session.py` & `aind_metadata_mapper-0.9.0/tests/test_bergamo/test_session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/test_dynamic_routing/test_mvr_rig.py` & `aind_metadata_mapper-0.9.0/tests/test_dynamic_routing/test_mvr_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/test_dynamic_routing/test_neuropixels_rig.py` & `aind_metadata_mapper-0.9.0/tests/test_dynamic_routing/test_neuropixels_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/test_dynamic_routing/test_sync_rig.py` & `aind_metadata_mapper-0.9.0/tests/test_dynamic_routing/test_sync_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/test_dynamic_routing/test_utils.py` & `aind_metadata_mapper-0.9.0/tests/test_dynamic_routing/test_utils.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/test_fip/test_session.py` & `aind_metadata_mapper-0.9.0/tests/test_fip/test_session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/test_gather_metadata.py` & `aind_metadata_mapper-0.9.0/tests/test_gather_metadata.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/test_legacy_core.py` & `aind_metadata_mapper-0.9.0/tests/test_legacy_core.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/test_mesoscope/test_session.py` & `aind_metadata_mapper-0.9.0/tests/test_mesoscope/test_session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/test_open_ephys/test_rig.py` & `aind_metadata_mapper-0.9.0/tests/test_open_ephys/test_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.8.0/tests/test_open_ephys/test_session.py` & `aind_metadata_mapper-0.9.0/tests/test_open_ephys/test_session.py`

 * *Files identical despite different names*

