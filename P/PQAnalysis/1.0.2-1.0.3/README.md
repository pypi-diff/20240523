# Comparing `tmp/pqanalysis-1.0.2.tar.gz` & `tmp/pqanalysis-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqanalysis-1.0.2.tar", last modified: Mon May 13 22:28:06 2024, max compression
+gzip compressed data, was "pqanalysis-1.0.3.tar", last modified: Thu May 23 15:29:03 2024, max compression
```

## Comparing `pqanalysis-1.0.2.tar` & `pqanalysis-1.0.3.tar`

### file list

```diff
@@ -1,457 +1,457 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.812000 pqanalysis-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/.docstr.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.728000 pqanalysis-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.736000 pqanalysis-1.0.2/.github/.pylint_cache/
--rw-r--r--   0 runner    (1001) docker     (127)    16870 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/.github/.pylint_cache/PQAnalysis_1.stats
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.736000 pqanalysis-1.0.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.736000 pqanalysis-1.0.2/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/.github/scripts/parse_pylint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.736000 pqanalysis-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    22319 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/.style.yapf
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-13 22:28:06.812000 pqanalysis-1.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.740000 pqanalysis-1.0.2/PQAnalysis/
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-13 22:28:06.000000 pqanalysis-1.0.2/PQAnalysis/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.740000 pqanalysis-1.0.2/PQAnalysis/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.740000 pqanalysis-1.0.2/PQAnalysis/analysis/rdf/
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/analysis/rdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/analysis/rdf/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/analysis/rdf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    28845 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/analysis/rdf/rdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/analysis/rdf/rdf_input_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/analysis/rdf/rdf_output_file_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.740000 pqanalysis-1.0.2/PQAnalysis/atomic_system/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/atomic_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/atomic_system/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/atomic_system/_positions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/atomic_system/_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/atomic_system/_standard_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    20913 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/atomic_system/atomic_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/atomic_system/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.744000 pqanalysis-1.0.2/PQAnalysis/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/cli/_argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/cli/_cli_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7829 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/cli/add_molecules.py
--rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/cli/build_nep_traj.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/cli/continue_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/cli/gen2xyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/cli/rdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/cli/rst2xyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/cli/traj2box.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/cli/traj2qmcfc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/cli/xyz2gen.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.744000 pqanalysis-1.0.2/PQAnalysis/core/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/core/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.744000 pqanalysis-1.0.2/PQAnalysis/core/atom/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/core/atom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6910 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/core/atom/atom.py
--rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/core/atom/element.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.744000 pqanalysis-1.0.2/PQAnalysis/core/cell/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/core/cell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/core/cell/_standard_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/core/cell/cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10403 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/core/residue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/formats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.744000 pqanalysis-1.0.2/PQAnalysis/grammar/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/grammar/PQ_inputGrammar.lark
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/grammar/inputGrammar.lark
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/grammar/rules.lark
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/grammar/selection.lark
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/grammar/terminals.lark
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.748000 pqanalysis-1.0.2/PQAnalysis/io/
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/box_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7074 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/conversion_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/energy_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9726 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/formats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.748000 pqanalysis-1.0.2/PQAnalysis/io/gen_file/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/gen_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/gen_file/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/gen_file/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/gen_file/gen_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/gen_file/gen_file_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/info_file_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.748000 pqanalysis-1.0.2/PQAnalysis/io/input_file_reader/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/input_file_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/input_file_reader/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/input_file_reader/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)    17600 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/input_file_reader/input_file_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.748000 pqanalysis-1.0.2/PQAnalysis/io/input_file_reader/pq/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/input_file_reader/pq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/input_file_reader/pq/output_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     9932 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/input_file_reader/pq/pq_input_file_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.752000 pqanalysis-1.0.2/PQAnalysis/io/input_file_reader/pq_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/input_file_reader/pq_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/input_file_reader/pq_analysis/_file_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/input_file_reader/pq_analysis/_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/input_file_reader/pq_analysis/_positions_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/input_file_reader/pq_analysis/_selection_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/input_file_reader/pq_analysis/pqanalysis_input_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/moldescriptor_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.752000 pqanalysis-1.0.2/PQAnalysis/io/nep/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/nep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/nep/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    37420 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/nep/nep_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.752000 pqanalysis-1.0.2/PQAnalysis/io/restart_file/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/restart_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/restart_file/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/restart_file/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/restart_file/restart_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/restart_file/restart_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.752000 pqanalysis-1.0.2/PQAnalysis/io/topology_file/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/topology_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/topology_file/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/topology_file/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13349 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/topology_file/topology_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    13355 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/topology_file/topology_file_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.752000 pqanalysis-1.0.2/PQAnalysis/io/traj_file/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/traj_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/traj_file/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/traj_file/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12689 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/traj_file/frame_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    21253 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/traj_file/trajectory_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/traj_file/trajectory_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.756000 pqanalysis-1.0.2/PQAnalysis/io/virial/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/virial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/virial/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/virial/virial_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/io/write_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.756000 pqanalysis-1.0.2/PQAnalysis/physical_data/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/physical_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/physical_data/energy.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/physical_data/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.756000 pqanalysis-1.0.2/PQAnalysis/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17228 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/tools/add_molecule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/tools/traj_to_com_traj.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.756000 pqanalysis-1.0.2/PQAnalysis/topology/
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/topology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/topology/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.756000 pqanalysis-1.0.2/PQAnalysis/topology/bonded_topology/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/topology/bonded_topology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/topology/bonded_topology/_topology_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/topology/bonded_topology/angle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/topology/bonded_topology/bond.py
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/topology/bonded_topology/bonded_topology.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/topology/bonded_topology/dihedral.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/topology/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    23565 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/topology/selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/topology/shake_topology.py
--rw-r--r--   0 runner    (1001) docker     (127)    18093 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/topology/topology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.760000 pqanalysis-1.0.2/PQAnalysis/traj/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/traj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/traj/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/traj/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/traj/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)    12526 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/traj/trajectory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/type_checking.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.760000 pqanalysis-1.0.2/PQAnalysis/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    13171 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/utils/custom_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/PQAnalysis/utils/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.808000 pqanalysis-1.0.2/PQAnalysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-13 22:28:06.000000 pqanalysis-1.0.2/PQAnalysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15038 2024-05-13 22:28:06.000000 pqanalysis-1.0.2/PQAnalysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 22:28:06.000000 pqanalysis-1.0.2/PQAnalysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-13 22:28:06.000000 pqanalysis-1.0.2/PQAnalysis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-13 22:28:06.000000 pqanalysis-1.0.2/PQAnalysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 22:28:06.000000 pqanalysis-1.0.2/PQAnalysis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.760000 pqanalysis-1.0.2/benchmarks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.760000 pqanalysis-1.0.2/benchmarks/core/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/benchmarks/core/benchmark_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/benchmarks/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.760000 pqanalysis-1.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (127)       73 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/autodoc.sh
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.760000 pqanalysis-1.0.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.732000 pqanalysis-1.0.2/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.760000 pqanalysis-1.0.2/docs/source/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.760000 pqanalysis-1.0.2/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/_templates/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/_templates/package.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.780000 pqanalysis-1.0.2/docs/source/code/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.analysis.rdf.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.analysis.rdf.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.analysis.rdf.rdf.rst
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.analysis.rdf.rdf_input_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.analysis.rdf.rdf_output_file_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.analysis.rdf.rst
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.analysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.atomic_system.atomic_system.rst
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.atomic_system.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.atomic_system.rst
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.cli.add_molecules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.cli.build_nep_traj.rst
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.cli.continue_input.rst
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.cli.gen2xyz.rst
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.cli.rdf.rst
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.cli.rst2xyz.rst
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.cli.traj2box.rst
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.cli.traj2qmcfc.rst
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.cli.xyz2gen.rst
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.config.rst
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.core.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.core.atom.atom.rst
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.core.atom.element.rst
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.core.atom.rst
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.core.cell.cell.rst
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.core.cell.rst
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.core.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.core.residue.rst
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.core.rst
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.formats.rst
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.box_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.conversion_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.energy_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.formats.rst
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.gen_file.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.gen_file.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.gen_file.gen_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.gen_file.gen_file_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.gen_file.rst
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.info_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.input_file_reader.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.input_file_reader.formats.rst
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.input_file_reader.input_file_parser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.input_file_reader.pq.output_files.rst
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.input_file_reader.pq.pq_input_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.input_file_reader.pq.rst
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.input_file_reader.pq_analysis.pqanalysis_input_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.input_file_reader.pq_analysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.input_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.moldescriptor_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.nep.nep_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.nep.rst
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.restart_file.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.restart_file.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.restart_file.restart_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.restart_file.restart_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.restart_file.rst
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.rst
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.topology_file.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.topology_file.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.topology_file.rst
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.topology_file.topology_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.topology_file.topology_file_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.traj_file.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.traj_file.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.traj_file.frame_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.traj_file.rst
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.traj_file.trajectory_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.traj_file.trajectory_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.virial.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.virial.rst
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.virial.virial_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.write_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.physical_data.energy.rst
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.physical_data.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.physical_data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.tools.add_molecule.rst
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.tools.rst
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.tools.traj_to_com_traj.rst
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.topology.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.topology.bonded_topology.angle.rst
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.topology.bonded_topology.bond.rst
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.topology.bonded_topology.bonded_topology.rst
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.topology.bonded_topology.dihedral.rst
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.topology.bonded_topology.rst
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.topology.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.topology.rst
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.topology.selection.rst
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.topology.shake_topology.rst
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.topology.topology.rst
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.traj.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.traj.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.traj.formats.rst
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.traj.rst
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.traj.trajectory.rst
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.type_checking.rst
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.types.rst
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.utils.common.rst
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.utils.custom_logging.rst
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.utils.decorators.rst
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.utils.files.rst
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.utils.random.rst
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/PQAnalysis.utils.units.rst
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/code/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.780000 pqanalysis-1.0.2/docs/source/developerGuide/
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/developerGuide/developerGuide.rst
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.780000 pqanalysis-1.0.2/docs/source/logo/
--rw-r--r--   0 runner    (1001) docker     (127)   204575 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/logo/PQAnalysis.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.780000 pqanalysis-1.0.2/docs/source/userGuide/
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/userGuide/inputFile.rst
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/docs/source/userGuide/userGuide.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.732000 pqanalysis-1.0.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.780000 pqanalysis-1.0.2/examples/traj2box/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/examples/traj2box/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/examples/traj2box/acof_triclinic.xyz
--rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/examples/traj2box/acof_triclinic_2.xyz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.784000 pqanalysis-1.0.2/examples/traj2comtraj/
--rw-r--r--   0 runner    (1001) docker     (127)  2600700 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/examples/traj2comtraj/umcm-9-md-01.xyz
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/pytest.sh
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-13 22:28:06.812000 pqanalysis-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    29303 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/test
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.788000 pqanalysis-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.788000 pqanalysis-1.0.2/tests/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.788000 pqanalysis-1.0.2/tests/analysis/rdf/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/analysis/rdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/analysis/rdf/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    14793 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/analysis/rdf/test_rdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/analysis/rdf/test_rdfInputFileReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/analysis/rdf/test_rdfOutputFileReader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.788000 pqanalysis-1.0.2/tests/atomicSystem/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/atomicSystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23524 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/atomicSystem/test_atomic_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/atomicSystem/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/atomicSystem/test_positions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.788000 pqanalysis-1.0.2/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/cli/test_continue_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/cli/test_rst2xyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/cli/test_traj2box.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/cli/test_traj2qmcfc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.792000 pqanalysis-1.0.2/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.792000 pqanalysis-1.0.2/tests/core/atom/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/core/atom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/core/atom/test_atom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/core/atom/test_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/core/test_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/core/test_residue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.732000 pqanalysis-1.0.2/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.792000 pqanalysis-1.0.2/tests/data/inputFileReader/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.792000 pqanalysis-1.0.2/tests/data/inputFileReader/PQ_input/
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/data/inputFileReader/PQ_input/n_not_matching.in
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/data/inputFileReader/PQ_input/n_not_matching_input_file_n-08.in
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/data/inputFileReader/PQ_input/no_output_files.in
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/data/inputFileReader/PQ_input/no_start_file.in
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/data/inputFileReader/PQ_input/old_n_not_less_one_than_actual_n-09.in
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/data/inputFileReader/PQ_input/run-08.in
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/data/inputFileReader/PQ_input/run-08.rpmd.in
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/data/inputFileReader/PQ_input/run-09.in.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/data/inputFileReader/PQ_input/run-09.rpmd.in.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/data/inputFileReader/PQ_input/run-10.in.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/data/inputFileReader/PQ_input/run-10.rpmd.in.ref
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/data/inputFileReader/input.in
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/data/inputFileReader/input_PQ.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.792000 pqanalysis-1.0.2/tests/data/rdf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/data/rdf/input.in
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/data/rdf/required_keys_not_given.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.792000 pqanalysis-1.0.2/tests/data/readEnergyFile/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/data/readEnergyFile/md-01.en
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/data/readEnergyFile/md-01.info
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/data/readEnergyFile/md-01_noinfo.en
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.792000 pqanalysis-1.0.2/tests/data/readInfoFile/
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/data/readInfoFile/md-01.info
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/data/readInfoFile/md-01.qmcfc.info
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.796000 pqanalysis-1.0.2/tests/data/readMoldescriptor/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/data/readMoldescriptor/moldescriptor.dat
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/data/readMoldescriptor/moldescriptor_withError.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.796000 pqanalysis-1.0.2/tests/data/readRestartFile/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/data/readRestartFile/md-01.rst
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/data/readRestartFile/moldescriptor.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.796000 pqanalysis-1.0.2/tests/data/rst2xyz/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/data/rst2xyz/md-01.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.796000 pqanalysis-1.0.2/tests/data/traj2box/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/data/traj2box/box.dat
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/data/traj2box/box.vmd.xyz
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/data/traj2box/test.xyz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.800000 pqanalysis-1.0.2/tests/data/traj2qmcfc/
--rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/data/traj2qmcfc/acof_triclinic.xyz
--rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/data/traj2qmcfc/acof_triclinic_2.xyz
--rw-r--r--   0 runner    (1001) docker     (127)  2301740 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/data/traj2qmcfc/traj.qmcfc.xyz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.804000 pqanalysis-1.0.2/tests/io/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.804000 pqanalysis-1.0.2/tests/io/inputFileReader/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.804000 pqanalysis-1.0.2/tests/io/inputFileReader/PQ/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/io/inputFileReader/PQ/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8594 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/io/inputFileReader/PQ/test_PQ_inputFileReader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.804000 pqanalysis-1.0.2/tests/io/inputFileReader/PQAnalysis/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/io/inputFileReader/PQAnalysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/io/inputFileReader/PQAnalysis/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/io/inputFileReader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/io/inputFileReader/test_inputDictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/io/inputFileReader/test_inputFileParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/io/inputFileReader/test_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/io/inputFileReader/test_visitors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/io/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/io/test_boxWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/io/test_energyFileReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/io/test_frameReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/io/test_infoFileReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/io/test_moldescriptorReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6746 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/io/test_restartReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/io/test_restartWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)    22643 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/io/test_trajectoryReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/io/test_trajectoryWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/io/test_write_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.804000 pqanalysis-1.0.2/tests/physicalData/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/physicalData/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/physicalData/test_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/test_formats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.808000 pqanalysis-1.0.2/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/tools/test_traj_to_com_traj.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.808000 pqanalysis-1.0.2/tests/topology/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/topology/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.808000 pqanalysis-1.0.2/tests/topology/bonded_topology/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/topology/bonded_topology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/topology/bonded_topology/test_angle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/topology/bonded_topology/test_bond.py
--rw-r--r--   0 runner    (1001) docker     (127)     8111 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/topology/bonded_topology/test_bondedTopology.py
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/topology/bonded_topology/test_dihedral.py
--rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/topology/test_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/topology/test_selectionTransformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/topology/test_shakeTopology.py
--rw-r--r--   0 runner    (1001) docker     (127)    12759 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/topology/test_topology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.808000 pqanalysis-1.0.2/tests/traj/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/traj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/traj/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12440 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/traj/test_trajectory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:28:06.808000 pqanalysis-1.0.2/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/utils/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-13 22:27:52.000000 pqanalysis-1.0.2/tests/utils/test_decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.564074 pqanalysis-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/.docstr.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.480074 pqanalysis-1.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.492074 pqanalysis-1.0.3/.github/.pylint_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)    16870 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/.github/.pylint_cache/PQAnalysis_1.stats
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.492074 pqanalysis-1.0.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.492074 pqanalysis-1.0.3/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/.github/scripts/parse_pylint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.492074 pqanalysis-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    22319 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/.style.yapf
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-23 15:29:03.564074 pqanalysis-1.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.492074 pqanalysis-1.0.3/PQAnalysis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-23 15:29:03.000000 pqanalysis-1.0.3/PQAnalysis/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.496074 pqanalysis-1.0.3/PQAnalysis/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.496074 pqanalysis-1.0.3/PQAnalysis/analysis/rdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/analysis/rdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/analysis/rdf/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/analysis/rdf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28845 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/analysis/rdf/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/analysis/rdf/rdf_input_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/analysis/rdf/rdf_output_file_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.496074 pqanalysis-1.0.3/PQAnalysis/atomic_system/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/atomic_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/atomic_system/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/atomic_system/_positions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/atomic_system/_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/atomic_system/_standard_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23524 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/atomic_system/atomic_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/atomic_system/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.500074 pqanalysis-1.0.3/PQAnalysis/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/cli/_argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/cli/_cli_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7829 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/cli/add_molecules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/cli/build_nep_traj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/cli/continue_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/cli/gen2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/cli/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/cli/rst2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/cli/traj2box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/cli/traj2qmcfc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/cli/xyz2gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.500074 pqanalysis-1.0.3/PQAnalysis/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/core/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.500074 pqanalysis-1.0.3/PQAnalysis/core/atom/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/core/atom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/core/atom/atom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/core/atom/element.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.500074 pqanalysis-1.0.3/PQAnalysis/core/cell/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/core/cell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/core/cell/_standard_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/core/cell/cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10403 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/core/residue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/formats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.500074 pqanalysis-1.0.3/PQAnalysis/grammar/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/grammar/PQ_inputGrammar.lark
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/grammar/inputGrammar.lark
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/grammar/rules.lark
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/grammar/selection.lark
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/grammar/terminals.lark
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.504074 pqanalysis-1.0.3/PQAnalysis/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/box_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7074 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/conversion_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/energy_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9726 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/formats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.504074 pqanalysis-1.0.3/PQAnalysis/io/gen_file/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/gen_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/gen_file/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/gen_file/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/gen_file/gen_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/gen_file/gen_file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/info_file_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.504074 pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17742 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/input_file_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.504074 pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq/output_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9932 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq/pq_input_file_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.504074 pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq_analysis/_file_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq_analysis/_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq_analysis/_positions_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq_analysis/_selection_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq_analysis/pqanalysis_input_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/moldescriptor_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.504074 pqanalysis-1.0.3/PQAnalysis/io/nep/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/nep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/nep/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37872 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/nep/nep_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.508074 pqanalysis-1.0.3/PQAnalysis/io/restart_file/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/restart_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/restart_file/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/restart_file/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/restart_file/restart_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/restart_file/restart_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.508074 pqanalysis-1.0.3/PQAnalysis/io/topology_file/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/topology_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/topology_file/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/topology_file/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13349 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/topology_file/topology_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13355 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/topology_file/topology_file_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.508074 pqanalysis-1.0.3/PQAnalysis/io/traj_file/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/traj_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/traj_file/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/traj_file/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/traj_file/frame_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22313 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/traj_file/trajectory_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/traj_file/trajectory_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.508074 pqanalysis-1.0.3/PQAnalysis/io/virial/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/virial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/virial/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/virial/virial_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/io/write_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.508074 pqanalysis-1.0.3/PQAnalysis/physical_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/physical_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/physical_data/energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/physical_data/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.512074 pqanalysis-1.0.3/PQAnalysis/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17228 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/tools/add_molecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/tools/traj_to_com_traj.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.512074 pqanalysis-1.0.3/PQAnalysis/topology/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/topology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/topology/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.512074 pqanalysis-1.0.3/PQAnalysis/topology/bonded_topology/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/topology/bonded_topology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/topology/bonded_topology/_topology_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/topology/bonded_topology/angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/topology/bonded_topology/bond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/topology/bonded_topology/bonded_topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/topology/bonded_topology/dihedral.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/topology/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23565 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/topology/selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/topology/shake_topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18809 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/topology/topology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.512074 pqanalysis-1.0.3/PQAnalysis/traj/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/traj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/traj/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/traj/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/traj/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12838 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/traj/trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/type_checking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.512074 pqanalysis-1.0.3/PQAnalysis/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13171 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/utils/custom_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/PQAnalysis/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.560074 pqanalysis-1.0.3/PQAnalysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-23 15:29:03.000000 pqanalysis-1.0.3/PQAnalysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15074 2024-05-23 15:29:03.000000 pqanalysis-1.0.3/PQAnalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:29:03.000000 pqanalysis-1.0.3/PQAnalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-23 15:29:03.000000 pqanalysis-1.0.3/PQAnalysis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-23 15:29:03.000000 pqanalysis-1.0.3/PQAnalysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-23 15:29:03.000000 pqanalysis-1.0.3/PQAnalysis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.516074 pqanalysis-1.0.3/benchmarks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.516074 pqanalysis-1.0.3/benchmarks/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/benchmarks/core/benchmark_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/benchmarks/core/benchmark_traj_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/benchmarks/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.516074 pqanalysis-1.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)       73 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/autodoc.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.516074 pqanalysis-1.0.3/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.484073 pqanalysis-1.0.3/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.516074 pqanalysis-1.0.3/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.516074 pqanalysis-1.0.3/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/_templates/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/_templates/package.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.532074 pqanalysis-1.0.3/docs/source/code/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.analysis.rdf.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.analysis.rdf.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.analysis.rdf.rdf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.analysis.rdf.rdf_input_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.analysis.rdf.rdf_output_file_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.analysis.rdf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.atomic_system.atomic_system.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.atomic_system.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.atomic_system.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.cli.add_molecules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.cli.build_nep_traj.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.cli.continue_input.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.cli.gen2xyz.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.cli.rdf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.cli.rst2xyz.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.cli.traj2box.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.cli.traj2qmcfc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.cli.xyz2gen.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.core.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.core.atom.atom.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.core.atom.element.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.core.atom.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.core.cell.cell.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.core.cell.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.core.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.core.residue.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.core.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.formats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.box_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.conversion_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.energy_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.formats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.gen_file.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.gen_file.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.gen_file.gen_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.gen_file.gen_file_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.gen_file.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.info_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.input_file_reader.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.input_file_reader.formats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.input_file_reader.input_file_parser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.input_file_reader.pq.output_files.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.input_file_reader.pq.pq_input_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.input_file_reader.pq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.input_file_reader.pq_analysis.pqanalysis_input_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.input_file_reader.pq_analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.input_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.moldescriptor_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.nep.nep_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.nep.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.restart_file.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.restart_file.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.restart_file.restart_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.restart_file.restart_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.restart_file.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.topology_file.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.topology_file.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.topology_file.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.topology_file.topology_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.topology_file.topology_file_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.traj_file.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.traj_file.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.traj_file.frame_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.traj_file.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.traj_file.trajectory_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.traj_file.trajectory_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.virial.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.virial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.virial.virial_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.write_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.physical_data.energy.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.physical_data.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.physical_data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.tools.add_molecule.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.tools.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.tools.traj_to_com_traj.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.topology.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.topology.bonded_topology.angle.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.topology.bonded_topology.bond.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.topology.bonded_topology.bonded_topology.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.topology.bonded_topology.dihedral.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.topology.bonded_topology.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.topology.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.topology.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.topology.selection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.topology.shake_topology.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.topology.topology.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.traj.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.traj.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.traj.formats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.traj.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.traj.trajectory.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.type_checking.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.types.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.utils.common.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.utils.custom_logging.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.utils.decorators.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.utils.files.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.utils.random.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/PQAnalysis.utils.units.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/code/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.532074 pqanalysis-1.0.3/docs/source/developerGuide/
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/developerGuide/developerGuide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.532074 pqanalysis-1.0.3/docs/source/logo/
+-rw-r--r--   0 runner    (1001) docker     (127)   204575 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/logo/PQAnalysis.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.536074 pqanalysis-1.0.3/docs/source/userGuide/
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/userGuide/inputFile.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/docs/source/userGuide/userGuide.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.484073 pqanalysis-1.0.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.536074 pqanalysis-1.0.3/examples/traj2box/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/examples/traj2box/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/examples/traj2box/acof_triclinic.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/examples/traj2box/acof_triclinic_2.xyz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.536074 pqanalysis-1.0.3/examples/traj2comtraj/
+-rw-r--r--   0 runner    (1001) docker     (127)  2600700 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/examples/traj2comtraj/umcm-9-md-01.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-23 15:29:03.564074 pqanalysis-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.540074 pqanalysis-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.540074 pqanalysis-1.0.3/tests/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.544074 pqanalysis-1.0.3/tests/analysis/rdf/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/analysis/rdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/analysis/rdf/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14793 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/analysis/rdf/test_rdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/analysis/rdf/test_rdfInputFileReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/analysis/rdf/test_rdfOutputFileReader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.544074 pqanalysis-1.0.3/tests/atomicSystem/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/atomicSystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24372 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/atomicSystem/test_atomic_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/atomicSystem/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/atomicSystem/test_positions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.544074 pqanalysis-1.0.3/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/cli/test_continue_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/cli/test_rst2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/cli/test_traj2box.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/cli/test_traj2qmcfc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.544074 pqanalysis-1.0.3/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.544074 pqanalysis-1.0.3/tests/core/atom/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/core/atom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/core/atom/test_atom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/core/atom/test_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/core/test_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/core/test_residue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.488074 pqanalysis-1.0.3/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.544074 pqanalysis-1.0.3/tests/data/inputFileReader/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.548074 pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/n_not_matching.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/n_not_matching_input_file_n-08.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/no_output_files.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/no_start_file.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/old_n_not_less_one_than_actual_n-09.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/run-08.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/run-08.rpmd.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/run-09.in.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/run-09.rpmd.in.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/run-10.in.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/run-10.rpmd.in.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/inputFileReader/input.in
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/inputFileReader/input_PQ.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.548074 pqanalysis-1.0.3/tests/data/rdf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/rdf/input.in
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/rdf/required_keys_not_given.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.548074 pqanalysis-1.0.3/tests/data/readEnergyFile/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/readEnergyFile/md-01.en
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/readEnergyFile/md-01.info
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/readEnergyFile/md-01_noinfo.en
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.548074 pqanalysis-1.0.3/tests/data/readInfoFile/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/readInfoFile/md-01.info
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/readInfoFile/md-01.qmcfc.info
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.548074 pqanalysis-1.0.3/tests/data/readMoldescriptor/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/readMoldescriptor/moldescriptor.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/readMoldescriptor/moldescriptor_withError.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.548074 pqanalysis-1.0.3/tests/data/readRestartFile/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/readRestartFile/md-01.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/readRestartFile/moldescriptor.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.548074 pqanalysis-1.0.3/tests/data/rst2xyz/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/rst2xyz/md-01.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.548074 pqanalysis-1.0.3/tests/data/traj2box/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/traj2box/box.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/traj2box/box.vmd.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/traj2box/test.xyz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.552074 pqanalysis-1.0.3/tests/data/traj2qmcfc/
+-rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/traj2qmcfc/acof_triclinic.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/traj2qmcfc/acof_triclinic_2.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)  2301740 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/data/traj2qmcfc/traj.qmcfc.xyz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.556074 pqanalysis-1.0.3/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.556074 pqanalysis-1.0.3/tests/io/inputFileReader/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.556074 pqanalysis-1.0.3/tests/io/inputFileReader/PQ/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/inputFileReader/PQ/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8594 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/inputFileReader/PQ/test_PQ_inputFileReader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.560074 pqanalysis-1.0.3/tests/io/inputFileReader/PQAnalysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/inputFileReader/PQAnalysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/inputFileReader/PQAnalysis/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/inputFileReader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/inputFileReader/test_inputDictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/inputFileReader/test_inputFileParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/inputFileReader/test_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/inputFileReader/test_visitors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/test_boxWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/test_energyFileReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/test_frameReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/test_infoFileReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/test_moldescriptorReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6746 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/test_restartReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/test_restartWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23202 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/test_trajectoryReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/test_trajectoryWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/io/test_write_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.560074 pqanalysis-1.0.3/tests/physicalData/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/physicalData/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/physicalData/test_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/test_formats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.560074 pqanalysis-1.0.3/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/tools/test_traj_to_com_traj.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.560074 pqanalysis-1.0.3/tests/topology/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/topology/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.560074 pqanalysis-1.0.3/tests/topology/bonded_topology/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/topology/bonded_topology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/topology/bonded_topology/test_angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/topology/bonded_topology/test_bond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8111 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/topology/bonded_topology/test_bondedTopology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/topology/bonded_topology/test_dihedral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/topology/test_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/topology/test_selectionTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/topology/test_shakeTopology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12759 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/topology/test_topology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.560074 pqanalysis-1.0.3/tests/traj/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/traj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/traj/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12336 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/traj/test_trajectory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:29:03.560074 pqanalysis-1.0.3/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/utils/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-23 15:28:51.000000 pqanalysis-1.0.3/tests/utils/test_decorators.py
```

### Comparing `pqanalysis-1.0.2/.codecov.yml` & `pqanalysis-1.0.3/.codecov.yml`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/.github/.pylint_cache/PQAnalysis_1.stats` & `pqanalysis-1.0.3/.github/.pylint_cache/PQAnalysis_1.stats`

 * *Files 2% similar despite different names*

```diff
@@ -315,15 +315,15 @@
 000013a0: 696f 2e74 7261 6a5f 6669 6c65 2e61 7069  io.traj_file.api
 000013b0: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
 000013c0: 681b 4b00 681c 4b00 681d 4b13 681e 4b00  h.K.h.K.h.K.h.K.
 000013d0: 758c 2950 5141 6e61 6c79 7369 732e 696f  u.)PQAnalysis.io
 000013e0: 2e74 7261 6a5f 6669 6c65 2e74 7261 6a65  .traj_file.traje
 000013f0: 6374 6f72 795f 7265 6164 6572 947d 9428  ctory_reader.}.(
 00001400: 6818 4b00 6819 4b00 681a 4b00 681b 4b00  h.K.h.K.h.K.h.K.
-00001410: 681c 4b05 681d 4b9a 681e 4b02 758c 2050  h.K.h.K.h.K.u. P
+00001410: 681c 4b05 681d 4b9b 681e 4b02 758c 2050  h.K.h.K.h.K.u. P
 00001420: 5141 6e61 6c79 7369 732e 696f 2e74 7261  QAnalysis.io.tra
 00001430: 6a5f 6669 6c65 2e5f 5f69 6e69 745f 5f94  j_file.__init__.
 00001440: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
 00001450: 1b4b 0068 1c4b 0068 1d4b 0368 1e4b 0075  .K.h.K.h.K.h.K.u
 00001460: 8c29 5051 416e 616c 7973 6973 2e69 6f2e  .)PQAnalysis.io.
 00001470: 7472 616a 5f66 696c 652e 7472 616a 6563  traj_file.trajec
 00001480: 746f 7279 5f77 7269 7465 7294 7d94 2868  tory_writer.}.(h
@@ -568,197 +568,197 @@
 00002370: 6e79 2d62 7261 6e63 6865 7394 4b02 8c0e  ny-branches.K...
 00002380: 746f 6f2d 6d61 6e79 2d6c 696e 6573 944b  too-many-lines.K
 00002390: 018c 1374 6f6f 2d6d 616e 792d 7374 6174  ...too-many-stat
 000023a0: 656d 656e 7473 944b 018c 0f75 6e75 7365  ements.K...unuse
 000023b0: 642d 6172 6775 6d65 6e74 944b 018c 0e64  d-argument.K...d
 000023c0: 7570 6c69 6361 7465 2d63 6f64 6594 4b03  uplicate-code.K.
 000023d0: 758c 0f63 6f64 655f 7479 7065 5f63 6f75  u..code_type_cou
-000023e0: 6e74 947d 9428 8c04 636f 6465 944d b91d  nt.}.(..code.M..
-000023f0: 8c07 636f 6d6d 656e 7494 4d06 018c 0964  ..comment.M....d
+000023e0: 6e74 947d 9428 8c04 636f 6465 944d c01d  nt.}.(..code.M..
+000023f0: 8c07 636f 6d6d 656e 7494 4d05 018c 0964  ..comment.M....d
 00002400: 6f63 7374 7269 6e67 944d e720 8c05 656d  ocstring.M. ..em
 00002410: 7074 7994 4df0 0a8c 0574 6f74 616c 944d  pty.M....total.M
-00002420: 964a 758c 0c64 6570 656e 6465 6e63 6965  .Ju..dependencie
+00002420: 9c4a 758c 0c64 6570 656e 6465 6e63 6965  .Ju..dependencie
 00002430: 7394 7d94 288c 0d62 6561 7274 7970 652e  s.}.(..beartype.
 00002440: 636c 6177 948f 9428 6823 908c 1150 5141  claw...(h#...PQA
 00002450: 6e61 6c79 7369 732e 636f 6e66 6967 948f  nalysis.config..
-00002460: 9428 68e5 6865 68d9 68e7 68f9 68d3 68e3  .(h.heh.h.h.h.h.
-00002470: 68a5 68e1 68d5 68d7 6823 68d1 68df 68af  h.h.h.h.h#h.h.h.
-00002480: 68cf 908c 1f50 5141 6e61 6c79 7369 732e  h....PQAnalysis.
+00002460: 9428 68e3 68d3 68df 6865 68f9 68cf 68e7  .(h.h.h.heh.h.h.
+00002470: 68af 68d1 68a5 68e1 68d9 68e5 6823 68d7  h.h.h.h.h.h.h#h.
+00002480: 68d5 908c 1f50 5141 6e61 6c79 7369 732e  h....PQAnalysis.
 00002490: 7574 696c 732e 6375 7374 6f6d 5f6c 6f67  utils.custom_log
-000024a0: 6769 6e67 948f 9428 6865 68c3 6a11 0100  ging...(heh.j...
-000024b0: 0068 756a 0301 0000 68f1 683b 6853 68ed  .huj....h.h;hSh.
-000024c0: 6833 68bb 687d 68af 6871 8c48 5051 416e  h3h.h}h.hq.HPQAn
-000024d0: 616c 7973 6973 2e69 6f2e 696e 7075 745f  alysis.io.input_
-000024e0: 6669 6c65 5f72 6561 6465 722e 7071 5f61  file_reader.pq_a
-000024f0: 6e61 6c79 7369 732e 7071 616e 616c 7973  nalysis.pqanalys
-00002500: 6973 5f69 6e70 7574 5f66 696c 655f 7265  is_input_file_re
-00002510: 6164 6572 948c 2450 5141 6e61 6c79 7369  ader..$PQAnalysi
-00002520: 732e 696f 2e74 7261 6a5f 6669 6c65 2e66  s.io.traj_file.f
-00002530: 7261 6d65 5f72 6561 6465 7294 686d 8c12  rame_reader.hm..
-00002540: 5051 416e 616c 7973 6973 2e69 6f2e 6261  PQAnalysis.io.ba
-00002550: 7365 946a 1901 0000 686f 6887 68a5 6885  se.j....hoh.h.h.
-00002560: 6823 6847 6895 68a1 8c29 5051 416e 616c  h#hGh.h..)PQAnal
-00002570: 7973 6973 2e69 6f2e 7265 7374 6172 745f  ysis.io.restart_
-00002580: 6669 6c65 2e72 6573 7461 7274 5f72 6561  file.restart_rea
-00002590: 6465 7294 6869 6877 8c26 5051 416e 616c  der.hihw.&PQAnal
-000025a0: 7973 6973 2e69 6f2e 6765 6e5f 6669 6c65  ysis.io.gen_file
-000025b0: 2e67 656e 5f66 696c 655f 7265 6164 6572  .gen_file_reader
-000025c0: 946a 1301 0000 6861 6831 68c1 6825 908c  .j....hah1h.h%..
-000025d0: 0964 6563 6f72 6174 6f72 948f 9428 68f5  .decorator...(h.
-000025e0: 8c24 5051 416e 616c 7973 6973 2e61 746f  .$PQAnalysis.ato
-000025f0: 6d69 635f 7379 7374 656d 2e5f 6465 636f  mic_system._deco
-00002600: 7261 746f 7273 9468 2590 8c0d 6265 6172  rators.h%...bear
+000024a0: 6769 6e67 948f 9428 8c12 5051 416e 616c  ging...(..PQAnal
+000024b0: 7973 6973 2e69 6f2e 6261 7365 946a 1101  ysis.io.base.j..
+000024c0: 0000 8c24 5051 416e 616c 7973 6973 2e69  ...$PQAnalysis.i
+000024d0: 6f2e 7472 616a 5f66 696c 652e 6672 616d  o.traj_file.fram
+000024e0: 655f 7265 6164 6572 948c 4850 5141 6e61  e_reader..HPQAna
+000024f0: 6c79 7369 732e 696f 2e69 6e70 7574 5f66  lysis.io.input_f
+00002500: 696c 655f 7265 6164 6572 2e70 715f 616e  ile_reader.pq_an
+00002510: 616c 7973 6973 2e70 7161 6e61 6c79 7369  alysis.pqanalysi
+00002520: 735f 696e 7075 745f 6669 6c65 5f72 6561  s_input_file_rea
+00002530: 6465 7294 68a1 6869 6871 8c26 5051 416e  der.h.hihq.&PQAn
+00002540: 616c 7973 6973 2e69 6f2e 6765 6e5f 6669  alysis.io.gen_fi
+00002550: 6c65 2e67 656e 5f66 696c 655f 7265 6164  le.gen_file_read
+00002560: 6572 9468 8768 3b68 c18c 2950 5141 6e61  er.h.h;h..)PQAna
+00002570: 6c79 7369 732e 696f 2e72 6573 7461 7274  lysis.io.restart
+00002580: 5f66 696c 652e 7265 7374 6172 745f 7265  _file.restart_re
+00002590: 6164 6572 9468 7768 856a 1901 0000 68a5  ader.hwh.j....h.
+000025a0: 6847 6a13 0100 006a 0301 0000 68f1 6875  hGj....j....h.hu
+000025b0: 6853 68af 6833 6895 6823 6861 687d 6831  hSh.h3h.h#hah}h1
+000025c0: 6865 6825 68bb 68ed 686f 686d 68c3 908c  heh%h.h.hohmh...
+000025d0: 0964 6563 6f72 6174 6f72 948f 9428 8c24  .decorator...(.$
+000025e0: 5051 416e 616c 7973 6973 2e61 746f 6d69  PQAnalysis.atomi
+000025f0: 635f 7379 7374 656d 2e5f 6465 636f 7261  c_system._decora
+00002600: 746f 7273 9468 2568 f590 8c0d 6265 6172  tors.h%h....bear
 00002610: 7479 7065 2e64 6f6f 7294 8f94 2868 2590  type.door...(h%.
 00002620: 8c0f 6265 6172 7479 7065 2e74 7970 696e  ..beartype.typin
-00002630: 6794 8f94 2868 2d8c 1a50 5141 6e61 6c79  g...(h-..PQAnaly
-00002640: 7369 732e 636f 7265 2e65 7863 6570 7469  sis.core.excepti
-00002650: 6f6e 7394 6865 6837 684f 68c3 68f5 6875  ons.heh7hOh.h.hu
-00002660: 6a11 0100 006a 0301 0000 682f 68f1 683b  j....j....h/h.h;
-00002670: 685f 6853 68ed 6833 687d 68fd 68a9 6879  h_hSh.h3h}h.h.hy
-00002680: 6883 68af 6a3a 0100 006a 3b01 0000 68a3  h.h.j:...j;...h.
-00002690: 6a3c 0100 0068 f96a 0d01 0000 6a19 0100  j<...h.j....j...
-000026a0: 0068 6f68 8768 a568 8568 c968 2968 4768  .hoh.h.h.h.h)hGh
-000026b0: a18c 3850 5141 6e61 6c79 7369 732e 746f  ..8PQAnalysis.to
-000026c0: 706f 6c6f 6779 2e62 6f6e 6465 645f 746f  pology.bonded_to
-000026d0: 706f 6c6f 6779 2e5f 746f 706f 6c6f 6779  pology._topology
-000026e0: 5f70 726f 7065 7274 6965 7394 6a3d 0100  _properties.j=..
-000026f0: 0068 776a 3e01 0000 6a13 0100 006a 4101  .hwj>...j....jA.
-00002700: 0000 6831 6851 68e7 68c1 8c37 5051 416e  ..h1hQh.h..7PQAn
-00002710: 616c 7973 6973 2e69 6f2e 696e 7075 745f  alysis.io.input_
-00002720: 6669 6c65 5f72 6561 6465 722e 7071 5f61  file_reader.pq_a
-00002730: 6e61 6c79 7369 732e 5f66 696c 655f 6d69  nalysis._file_mi
-00002740: 7869 6e94 6825 908c 1550 5141 6e61 6c79  xin.h%...PQAnaly
+00002630: 6794 8f94 286a 3a01 0000 6a11 0100 0068  g...(j:...j....h
+00002640: a368 e76a 3b01 0000 6a3c 0100 0068 a16a  .h.j;...j<...h.j
+00002650: 3d01 0000 68c1 6829 683b 6887 6879 68c9  =...h.h)h;h.hyh.
+00002660: 6a3e 0100 0068 7768 8568 ed8c 1a50 5141  j>...hwh.h...PQA
+00002670: 6e61 6c79 7369 732e 636f 7265 2e65 7863  nalysis.core.exc
+00002680: 6570 7469 6f6e 7394 6a19 0100 0068 a968  eptions.j....h.h
+00002690: a568 476a 1301 0000 6a03 0100 0068 f168  .hGj....j....h.h
+000026a0: 5f68 3768 758c 3750 5141 6e61 6c79 7369  _h7hu.7PQAnalysi
+000026b0: 732e 696f 2e69 6e70 7574 5f66 696c 655f  s.io.input_file_
+000026c0: 7265 6164 6572 2e70 715f 616e 616c 7973  reader.pq_analys
+000026d0: 6973 2e5f 6669 6c65 5f6d 6978 696e 9468  is._file_mixin.h
+000026e0: 8368 5368 2f68 af68 f568 3368 4f68 5168  .hSh/h.h.h3hOhQh
+000026f0: 7d68 318c 3850 5141 6e61 6c79 7369 732e  }h1.8PQAnalysis.
+00002700: 746f 706f 6c6f 6779 2e62 6f6e 6465 645f  topology.bonded_
+00002710: 746f 706f 6c6f 6779 2e5f 746f 706f 6c6f  topology._topolo
+00002720: 6779 5f70 726f 7065 7274 6965 7394 68f9  gy_properties.h.
+00002730: 6865 6825 682d 68fd 6a41 0100 0068 6f68  heh%h-h.jA...hoh
+00002740: c36a 0d01 0000 908c 1550 5141 6e61 6c79  .j.......PQAnaly
 00002750: 7369 732e 6578 6365 7074 696f 6e73 948f  sis.exceptions..
-00002760: 9428 6a46 0100 0068 7568 8168 7b68 3b68  .(jF...huh.h{h;h
-00002770: bd68 c768 ed8c 2350 5141 6e61 6c79 7369  .h.h..#PQAnalysi
-00002780: 732e 6174 6f6d 6963 5f73 7973 7465 6d2e  s.atomic_system.
-00002790: 6578 6365 7074 696f 6e73 948c 2250 5141  exceptions.."PQA
-000027a0: 6e61 6c79 7369 732e 616e 616c 7973 6973  nalysis.analysis
-000027b0: 2e72 6466 2e65 7863 6570 7469 6f6e 7394  .rdf.exceptions.
-000027c0: 6a17 0100 0068 ef68 3368 bb68 ab68 7168  j....h.h3h.h.hqh
-000027d0: 396a 3c01 0000 68f9 6887 68a5 6885 6847  9j<...h.h.h.h.hG
-000027e0: 6895 6893 6869 689f 68b3 6825 908c 1050  h.h.hih.h.h%...P
+00002760: 9428 6a3a 0100 0068 6968 7168 8768 3b68  .(j:...hihqh.h;h
+00002770: 856a 4601 0000 68bd 8c23 5051 416e 616c  .jF...h..#PQAnal
+00002780: 7973 6973 2e61 746f 6d69 635f 7379 7374  ysis.atomic_syst
+00002790: 656d 2e65 7863 6570 7469 6f6e 7394 68a5  em.exceptions.h.
+000027a0: 6847 8c22 5051 416e 616c 7973 6973 2e61  hG."PQAnalysis.a
+000027b0: 6e61 6c79 7369 732e 7264 662e 6578 6365  nalysis.rdf.exce
+000027c0: 7074 696f 6e73 9468 9f68 7568 7b68 ef68  ptions.h.huh{h.h
+000027d0: b368 3368 9568 c768 3968 8168 ab68 9368  .h3h.h.h9h.h.h.h
+000027e0: f968 2568 bb68 ed6a 1701 0000 908c 1050  .h%h.h.j.......P
 000027f0: 5141 6e61 6c79 7369 732e 7479 7065 7394  QAnalysis.types.
-00002800: 8f94 2868 6568 3768 4f6a 0301 0000 682f  ..(heh7hOj....h/
-00002810: 683b 685f 6853 68ed 6843 6833 6845 68a9  h;h_hSh.hCh3hEh.
-00002820: 6841 68af 6a3b 0100 0068 cd6a 0d01 0000  hAh.j;...h.j....
-00002830: 6a19 0100 006a 0901 0000 6887 6885 6847  j....j....h.h.hG
-00002840: 6895 68a1 684d 6a47 0100 006a 0101 0000  h.h.hMjG...j....
-00002850: 6869 8c3c 5051 416e 616c 7973 6973 2e69  hi.<PQAnalysis.i
-00002860: 6f2e 696e 7075 745f 6669 6c65 5f72 6561  o.input_file_rea
-00002870: 6465 722e 7071 5f61 6e61 6c79 7369 732e  der.pq_analysis.
-00002880: 5f70 6f73 6974 696f 6e73 5f6d 6978 696e  _positions_mixin
-00002890: 946a 3e01 0000 6831 6851 6825 908c 056e  .j>...h1hQh%...n
-000028a0: 756d 7079 948f 9428 6865 6837 684f 6a03  umpy...(heh7hOj.
-000028b0: 0100 0068 5368 ed68 3368 bb68 fd68 af68  ...hSh.h3h.h.h.h
-000028c0: 716a 3b01 0000 68cd 6a0d 0100 006a 1901  qj;...h.j....j..
-000028d0: 0000 6a09 0100 0068 6f68 4768 2968 a16a  ..j....hohGh)h.j
-000028e0: 3d01 0000 6a01 0100 006a 3e01 0000 6a41  =...j....j>...jA
-000028f0: 0100 0068 3168 5190 8c0d 6265 6172 7479  ...h1hQ...bearty
+00002800: 8f94 286a 3b01 0000 684d 6869 68a1 6a3d  ..(j;...hMhih.j=
+00002810: 0100 0068 8768 3b68 cd68 8568 ed6a 1901  ...h.h;h.h.h.j..
+00002820: 0000 68a9 6a01 0100 0068 476a 0301 0000  ..h.j....hGj....
+00002830: 685f 6837 6843 6853 8c3c 5051 416e 616c  h_h7hChS.<PQAnal
+00002840: 7973 6973 2e69 6f2e 696e 7075 745f 6669  ysis.io.input_fi
+00002850: 6c65 5f72 6561 6465 722e 7071 5f61 6e61  le_reader.pq_ana
+00002860: 6c79 7369 732e 5f70 6f73 6974 696f 6e73  lysis._positions
+00002870: 5f6d 6978 696e 9468 2f68 af68 3368 4f68  _mixin.h/h.h3hOh
+00002880: 9568 456a 0901 0000 6831 6a48 0100 0068  .hEj....h1jH...h
+00002890: 6568 2568 4168 516a 0d01 0000 908c 056e  eh%hAhQj.......n
+000028a0: 756d 7079 948f 9428 6a3b 0100 0068 a16a  umpy...(j;...h.j
+000028b0: 3d01 0000 6871 6829 6a3e 0100 0068 cd68  =...hqh)j>...h.h
+000028c0: ed6a 1901 0000 6a01 0100 0068 476a 0301  .j....j....hGj..
+000028d0: 0000 6837 6853 68af 6833 684f 6a09 0100  ..h7hSh.h3hOj...
+000028e0: 0068 5168 3168 6568 fd68 bb6a 4101 0000  .hQh1heh.h.jA...
+000028f0: 686f 6a0d 0100 0090 8c0d 6265 6172 7479  hoj.......bearty
 00002900: 7065 2e76 616c 6594 8f94 286a 1301 0000  pe.vale...(j....
-00002910: 6a0d 0100 0068 2990 8c0b 6d75 6c74 696d  j....h)...multim
+00002910: 6829 6a0d 0100 0090 8c0b 6d75 6c74 696d  h)j.......multim
 00002920: 6574 686f 6494 8f94 2868 2b90 8c0f 5051  ethod...(h+...PQ
 00002930: 416e 616c 7973 6973 2e74 7261 6a94 8f94  Analysis.traj...
-00002940: 2868 4b68 6568 3768 7568 2f68 5d68 a968  (hKheh7huh/h]h.h
-00002950: 7968 af68 716a 3b01 0000 686d 68a3 8c1e  yh.hqj;...hmh...
-00002960: 5051 416e 616c 7973 6973 2e69 6f2e 7265  PQAnalysis.io.re
-00002970: 7374 6172 745f 6669 6c65 2e61 7069 9468  start_file.api.h
-00002980: a568 4768 a16a 3d01 0000 6877 68e7 908c  .hGh.j=...hwh...
+00002940: 2868 a368 e76a 3b01 0000 68a1 6871 6879  (h.h.j;...h.hqhy
+00002950: 6a3e 0100 0068 7768 4b68 a968 a568 4768  j>...hwhKh.h.hGh
+00002960: 3768 7568 2f68 af8c 1e50 5141 6e61 6c79  7huh/h...PQAnaly
+00002970: 7369 732e 696f 2e72 6573 7461 7274 5f66  sis.io.restart_f
+00002980: 696c 652e 6170 6994 685d 6865 686d 908c  ile.api.h]hehm..
 00002990: 0d50 5141 6e61 6c79 7369 732e 696f 948f  .PQAnalysis.io..
-000029a0: 9428 68e5 6865 68d9 6837 68cd 68d3 6861  .(h.heh.h7h.h.ha
-000029b0: 685d 68e1 682f 68d5 6847 68d1 68af 685f  h]h.h/h.hGh.h.h_
+000029a0: 9428 685d 68d3 6865 68cd 682f 68af 68d1  .(h]h.heh.h/h.h.
+000029b0: 68e1 6847 68d9 68e5 6861 685f 6837 68d5  h.hGh.h.hah_h7h.
 000029c0: 908c 1850 5141 6e61 6c79 7369 732e 7479  ...PQAnalysis.ty
-000029d0: 7065 5f63 6865 636b 696e 6794 8f94 2868  pe_checking...(h
-000029e0: 4b68 bf68 6568 3768 c36a 1101 0000 6875  Kh.heh7h.j....hu
-000029f0: 6a03 0100 0068 2f68 3b68 5f68 538c 1a50  j....h/h;h_hS..P
-00002a00: 5141 6e61 6c79 7369 732e 696f 2e67 656e  QAnalysis.io.gen
-00002a10: 5f66 696c 652e 6170 6994 68ed 685d 6843  _file.api.h.h]hC
-00002a20: 6833 68bb 6845 68a9 6879 6841 68af 6871  h3h.hEh.hyhAh.hq
-00002a30: 686d 68a3 68cd 6a58 0100 006a 0d01 0000  hmh.h.jX...j....
-00002a40: 6a19 0100 006a 0901 0000 686f 68a5 68c9  j....j....hoh.h.
-00002a50: 6847 68a1 68e9 684d 6a3d 0100 006a 0101  hGh.h.hMj=...j..
-00002a60: 0000 6869 6877 6a3e 0100 006a 1301 0000  ..hihwj>...j....
-00002a70: 6861 6831 6851 68c1 908c 1d50 5141 6e61  hah1hQh....PQAna
+000029d0: 7065 5f63 6865 636b 696e 6794 8f94 286a  pe_checking...(j
+000029e0: 1101 0000 68a3 686f 684d 6869 6871 68a1  ....h.hohMhihqh.
+000029f0: 6a3d 0100 0068 3b68 c168 7968 c96a 3e01  j=...h;h.hyh.j>.
+00002a00: 0000 68cd 6877 68ed 6a19 0100 0068 4b68  ..h.hwh.j....hKh
+00002a10: a96a 0101 0000 68a5 6847 6a13 0100 006a  .j....h.hGj....j
+00002a20: 0301 0000 68e9 8c1a 5051 416e 616c 7973  ....h...PQAnalys
+00002a30: 6973 2e69 6f2e 6765 6e5f 6669 6c65 2e61  is.io.gen_file.a
+00002a40: 7069 9468 5f68 3768 7568 4368 5368 2f68  pi.h_h7huhChSh/h
+00002a50: af68 336a 5801 0000 6845 6a09 0100 0068  .h3jX...hEj....h
+00002a60: 3168 5d68 6568 bf68 4168 bb68 5168 6168  1h]heh.hAh.hQhah
+00002a70: 6d68 c36a 0d01 0000 908c 1d50 5141 6e61  mh.j.......PQAna
 00002a80: 6c79 7369 732e 746f 706f 6c6f 6779 2e73  lysis.topology.s
 00002a90: 656c 6563 7469 6f6e 948f 9428 682f 6837  election...(h/h7
 00002aa0: 8c13 5051 416e 616c 7973 6973 2e74 6f70  ..PQAnalysis.top
 00002ab0: 6f6c 6f67 7994 908c 2250 5141 6e61 6c79  ology..."PQAnaly
 00002ac0: 7369 732e 746f 706f 6c6f 6779 2e73 6861  sis.topology.sha
 00002ad0: 6b65 5f74 6f70 6f6c 6f67 7994 8f94 2868  ke_topology...(h
 00002ae0: 2f90 8c1a 5051 416e 616c 7973 6973 2e63  /...PQAnalysis.c
 00002af0: 6f72 652e 6578 6365 7074 696f 6e73 948f  ore.exceptions..
-00002b00: 9428 6a13 0100 006a 1101 0000 6831 6a03  .(j....j....h1j.
-00002b10: 0100 008c 0f50 5141 6e61 6c79 7369 732e  .....PQAnalysis.
-00002b20: 636f 7265 9490 8c0f 5051 416e 616c 7973  core....PQAnalys
-00002b30: 6973 2e63 6f72 6594 8f94 2868 5368 6568  is.core...(hSheh
-00002b40: 4f6a 5801 0000 6a3e 0100 0068 3168 ed68  OjX...j>...h1h.h
-00002b50: 6f68 3368 a568 5168 a968 7968 a168 e968  oh3h.hQh.hyh.h.h
-00002b60: 4d6a 3b01 0000 6a3d 0100 0090 8c0a 5051  Mj;...j=......PQ
-00002b70: 416e 616c 7973 6973 948f 9428 6865 68c3  Analysis...(heh.
-00002b80: 6a11 0100 0068 756a 0301 0000 68f1 683b  j....huj....h.h;
-00002b90: 6853 68ed 6833 68bb 687d 68af 6a3a 0100  hSh.h3h.h}h.j:..
-00002ba0: 0068 716a 3b01 0000 686d 6a3c 0100 006a  .hqj;...hmj<...j
-00002bb0: 1901 0000 686f 6887 68a5 6885 6847 6895  ....hoh.h.h.hGh.
-00002bc0: 68a1 6a3d 0100 0068 6968 776a 3e01 0000  h.j=...hihwj>...
-00002bd0: 6a13 0100 0068 6168 3168 c190 8c1e 5051  j....hah1h....PQ
+00002b00: 9428 6a11 0100 008c 0f50 5141 6e61 6c79  .(j......PQAnaly
+00002b10: 7369 732e 636f 7265 946a 1301 0000 6a03  sis.core.j....j.
+00002b20: 0100 0068 3190 8c0f 5051 416e 616c 7973  ...h1...PQAnalys
+00002b30: 6973 2e63 6f72 6594 8f94 2868 a968 5368  is.core...(h.hSh
+00002b40: 656a 3b01 0000 68a5 684d 68a1 6a3d 0100  ej;...h.hMh.j=..
+00002b50: 0068 3368 4f68 e96a 5801 0000 6879 6851  .h3hOh.jX...hyhQ
+00002b60: 6a3e 0100 0068 6f68 ed68 3190 8c0a 5051  j>...hoh.h1...PQ
+00002b70: 416e 616c 7973 6973 948f 9428 6a3a 0100  Analysis...(j:..
+00002b80: 006a 1101 0000 6a3b 0100 006a 3c01 0000  .j....j;...j<...
+00002b90: 68a1 6869 6871 6a3d 0100 0068 8768 3b68  h.hihqj=...h.h;h
+00002ba0: c16a 3e01 0000 6877 6885 6a19 0100 0068  .j>...hwh.j....h
+00002bb0: a568 476a 1301 0000 6a03 0100 0068 f168  .hGj....j....h.h
+00002bc0: 7568 5368 af68 3368 9568 6168 7d68 3168  uhSh.h3h.hah}h1h
+00002bd0: 6568 bb68 ed68 6f68 6d68 c390 8c1e 5051  eh.h.hohmh....PQ
 00002be0: 416e 616c 7973 6973 2e74 6f70 6f6c 6f67  Analysis.topolog
 00002bf0: 792e 6578 6365 7074 696f 6e73 948f 9428  y.exceptions...(
-00002c00: 6831 6a60 0100 0090 8c33 5051 416e 616c  h1j`.....3PQAnal
+00002c00: 6a60 0100 0068 3190 8c33 5051 416e 616c  j`...h1..3PQAnal
 00002c10: 7973 6973 2e74 6f70 6f6c 6f67 792e 626f  ysis.topology.bo
 00002c20: 6e64 6564 5f74 6f70 6f6c 6f67 792e 626f  nded_topology.bo
 00002c30: 6e64 6564 5f74 6f70 6f6c 6f67 7994 8f94  nded_topology...
-00002c40: 2868 316a 6001 0000 908c 046c 6172 6b94  (h1j`......lark.
-00002c50: 8f94 2868 8568 3390 8c1c 5051 416e 616c  ..(h.h3...PQAnal
+00002c40: 286a 6001 0000 6831 908c 046c 6172 6b94  (j`...h1...lark.
+00002c50: 8f94 2868 3368 8590 8c1c 5051 416e 616c  ..(h3h....PQAnal
 00002c60: 7973 6973 2e74 6f70 6f6c 6f67 792e 746f  ysis.topology.to
-00002c70: 706f 6c6f 6779 948f 9428 6a60 0100 0068  pology...(j`...h
-00002c80: 3390 8c28 5051 416e 616c 7973 6973 2e74  3..(PQAnalysis.t
+00002c70: 706f 6c6f 6779 948f 9428 6833 6a60 0100  pology...(h3j`..
+00002c80: 0090 8c28 5051 416e 616c 7973 6973 2e74  ...(PQAnalysis.t
 00002c90: 6f70 6f6c 6f67 792e 626f 6e64 6564 5f74  opology.bonded_t
 00002ca0: 6f70 6f6c 6f67 792e 626f 6e64 948f 9428  opology.bond...(
-00002cb0: 683b 6a47 0100 006a 6001 0000 908c 2950  h;jG...j`.....)P
+00002cb0: 6a48 0100 0068 3b6a 6001 0000 908c 2950  jH...h;j`.....)P
 00002cc0: 5141 6e61 6c79 7369 732e 746f 706f 6c6f  QAnalysis.topolo
 00002cd0: 6779 2e62 6f6e 6465 645f 746f 706f 6c6f  gy.bonded_topolo
-00002ce0: 6779 2e61 6e67 6c65 948f 9428 683b 6a47  gy.angle...(h;jG
-00002cf0: 0100 006a 6001 0000 908c 2c50 5141 6e61  ...j`.....,PQAna
+00002ce0: 6779 2e61 6e67 6c65 948f 9428 6a48 0100  gy.angle...(jH..
+00002cf0: 0068 3b6a 6001 0000 908c 2c50 5141 6e61  .h;j`.....,PQAna
 00002d00: 6c79 7369 732e 746f 706f 6c6f 6779 2e62  lysis.topology.b
 00002d10: 6f6e 6465 645f 746f 706f 6c6f 6779 2e64  onded_topology.d
-00002d20: 6968 6564 7261 6c94 8f94 2868 3b6a 4701  ihedral...(h;jG.
-00002d30: 0000 6a60 0100 0090 8c38 5051 416e 616c  ..j`.....8PQAnal
+00002d20: 6968 6564 7261 6c94 8f94 286a 4801 0000  ihedral...(jH...
+00002d30: 683b 6a60 0100 0090 8c38 5051 416e 616c  h;j`.....8PQAnal
 00002d40: 7973 6973 2e74 6f70 6f6c 6f67 792e 626f  ysis.topology.bo
 00002d50: 6e64 6564 5f74 6f70 6f6c 6f67 792e 5f74  nded_topology._t
 00002d60: 6f70 6f6c 6f67 795f 7072 6f70 6572 7469  opology_properti
 00002d70: 6573 948f 9428 683b 908c 1550 5141 6e61  es...(h;...PQAna
 00002d80: 6c79 7369 732e 696f 2e66 6f72 6d61 7473  lysis.io.formats
-00002d90: 948f 9428 686d 68bf 68a3 6a3c 0100 006a  ...(hmh.h.j<...j
-00002da0: 5d01 0000 68c3 6875 8c0d 5051 416e 616c  ]...h.hu..PQAnal
-00002db0: 7973 6973 2e69 6f94 68bb 68d7 6847 6879  ysis.io.h.h.hGhy
-00002dc0: 68a1 68a9 68e7 908c 1850 5141 6e61 6c79  h.h.h....PQAnaly
+00002d90: 948f 9428 6a3a 0100 0068 a968 a38c 0d50  ...(j:...h.h...P
+00002da0: 5141 6e61 6c79 7369 732e 696f 9468 bf68  QAnalysis.io.h.h
+00002db0: e768 4768 a168 d76a 5d01 0000 68bb 6879  .hGh.h.j]...h.hy
+00002dc0: 686d 68c3 6875 908c 1850 5141 6e61 6c79  hmh.hu...PQAnaly
 00002dd0: 7369 732e 6174 6f6d 6963 5f73 7973 7465  sis.atomic_syste
-00002de0: 6d94 8f94 2868 a36a 5d01 0000 6a58 0100  m...(h.j]...jX..
-00002df0: 006a 3e01 0000 68ed 6875 68a5 68bb 6847  .j>...h.huh.h.hG
-00002e00: 68a1 68a9 68af 6a3b 0100 006a 3d01 0000  h.h.h.j;...j=...
+00002de0: 6d94 8f94 2868 a968 a36a 3b01 0000 68af  m...(h.h.j;...h.
+00002df0: 68a5 6847 68a1 6a3d 0100 006a 5801 0000  h.hGh.j=...jX...
+00002e00: 6a5d 0100 0068 bb68 ed6a 3e01 0000 6875  j]...h.h.j>...hu
 00002e10: 908c 2150 5141 6e61 6c79 7369 732e 746f  ..!PQAnalysis.to
 00002e20: 6f6c 732e 7472 616a 5f74 6f5f 636f 6d5f  ols.traj_to_com_
 00002e30: 7472 616a 948f 9428 8c10 5051 416e 616c  traj...(..PQAnal
 00002e40: 7973 6973 2e74 6f6f 6c73 9490 8c13 5051  ysis.tools....PQ
 00002e50: 416e 616c 7973 6973 2e74 6f70 6f6c 6f67  Analysis.topolog
-00002e60: 7994 8f94 2868 5368 bf68 6568 a368 ed68  y...(hSh.heh.h.h
-00002e70: c168 c368 5d68 a568 5168 4d6a 3b01 0000  .h.h]h.hQhMj;...
-00002e80: 6a3d 0100 0090 8c24 5051 416e 616c 7973  j=.....$PQAnalys
+00002e60: 7994 8f94 2868 5d68 5368 6568 a368 bf6a  y...(h]hSheh.h.j
+00002e70: 3b01 0000 68a5 68ed 684d 68c1 6851 6a3e  ;...h.h.hMh.hQj>
+00002e80: 0100 0068 c390 8c24 5051 416e 616c 7973  ...h...$PQAnalys
 00002e90: 6973 2e61 746f 6d69 635f 7379 7374 656d  is.atomic_system
 00002ea0: 2e5f 6465 636f 7261 746f 7273 948f 9428  ._decorators...(
-00002eb0: 684f 684d 6851 908c 2350 5141 6e61 6c79  hOhMhQ..#PQAnaly
+00002eb0: 684d 6851 684f 908c 2350 5141 6e61 6c79  hMhQhO..#PQAnaly
 00002ec0: 7369 732e 6174 6f6d 6963 5f73 7973 7465  sis.atomic_syste
 00002ed0: 6d2e 6578 6365 7074 696f 6e73 948f 9428  m.exceptions...(
-00002ee0: 684f 6a41 0100 008c 1850 5141 6e61 6c79  hOjA.....PQAnaly
-00002ef0: 7369 732e 6174 6f6d 6963 5f73 7973 7465  sis.atomic_syste
-00002f00: 6d94 6853 908c 1773 6369 7079 2e73 7061  m.hS...scipy.spa
+00002ee0: 6a41 0100 0068 4f68 538c 1850 5141 6e61  jA...hOhS..PQAna
+00002ef0: 6c79 7369 732e 6174 6f6d 6963 5f73 7973  lysis.atomic_sys
+00002f00: 7465 6d94 908c 1773 6369 7079 2e73 7061  tem....scipy.spa
 00002f10: 7469 616c 2e74 7261 6e73 666f 726d 948f  tial.transform..
 00002f20: 9428 6853 908c 1750 5141 6e61 6c79 7369  .(hS...PQAnalysi
 00002f30: 732e 7574 696c 732e 7261 6e64 6f6d 948f  s.utils.random..
-00002f40: 9428 6853 68af 908c 2450 5141 6e61 6c79  .(hSh...$PQAnaly
+00002f40: 9428 68af 6853 908c 2450 5141 6e61 6c79  .(h.hS..$PQAnaly
 00002f50: 7369 732e 6174 6f6d 6963 5f73 7973 7465  sis.atomic_syste
 00002f60: 6d2e 5f70 726f 7065 7274 6965 7394 8f94  m._properties...
 00002f70: 2868 5390 8c2d 5051 416e 616c 7973 6973  (hS..-PQAnalysis
 00002f80: 2e61 746f 6d69 635f 7379 7374 656d 2e5f  .atomic_system._
 00002f90: 7374 616e 6461 7264 5f70 726f 7065 7274  standard_propert
 00002fa0: 6965 7394 8f94 2868 5390 8c23 5051 416e  ies...(hS..#PQAn
 00002fb0: 616c 7973 6973 2e61 746f 6d69 635f 7379  alysis.atomic_sy
@@ -767,86 +767,86 @@
 00002fe0: 6973 2e61 746f 6d69 635f 7379 7374 656d  is.atomic_system
 00002ff0: 2e61 746f 6d69 635f 7379 7374 656d 948f  .atomic_system..
 00003000: 9428 6a88 0100 0090 8c17 5051 416e 616c  .(j.......PQAnal
 00003010: 7973 6973 2e61 6e61 6c79 7369 732e 7264  ysis.analysis.rd
 00003020: 6694 8f94 288c 1350 5141 6e61 6c79 7369  f...(..PQAnalysi
 00003030: 732e 616e 616c 7973 6973 9490 8c1b 5051  s.analysis....PQ
 00003040: 416e 616c 7973 6973 2e61 6e61 6c79 7369  Analysis.analysi
-00003050: 732e 7264 662e 7264 6694 8f94 286a 9701  s.rdf.rdf...(j..
-00003060: 0000 685d 8c17 5051 416e 616c 7973 6973  ..h]..PQAnalysis
-00003070: 2e61 6e61 6c79 7369 732e 7264 6694 68df  .analysis.rdf.h.
-00003080: 685f 908c 2d50 5141 6e61 6c79 7369 732e  h_..-PQAnalysis.
+00003050: 732e 7264 662e 7264 6694 8f94 2868 5d68  s.rdf.rdf...(h]h
+00003060: df68 5f8c 1750 5141 6e61 6c79 7369 732e  .h_..PQAnalysis.
+00003070: 616e 616c 7973 6973 2e72 6466 946a 9701  analysis.rdf.j..
+00003080: 0000 908c 2d50 5141 6e61 6c79 7369 732e  ....-PQAnalysis.
 00003090: 616e 616c 7973 6973 2e72 6466 2e72 6466  analysis.rdf.rdf
 000030a0: 5f69 6e70 7574 5f66 696c 655f 7265 6164  _input_file_read
-000030b0: 6572 948f 9428 68df 685d 6a9a 0100 0090  er...(h.h]j.....
+000030b0: 6572 948f 9428 685d 6a9a 0100 0068 df90  er...(h]j....h..
 000030c0: 8c2e 5051 416e 616c 7973 6973 2e61 6e61  ..PQAnalysis.ana
 000030d0: 6c79 7369 732e 7264 662e 7264 665f 6f75  lysis.rdf.rdf_ou
 000030e0: 7470 7574 5f66 696c 655f 7772 6974 6572  tput_file_writer
 000030f0: 948f 9428 685d 6a9a 0100 0090 8c10 5051  ...(h]j.......PQ
 00003100: 416e 616c 7973 6973 2e75 7469 6c73 948f  Analysis.utils..
-00003110: 9428 686d 6865 68f9 8c0e 5051 416e 616c  .(hmheh...PQAnal
-00003120: 7973 6973 2e63 6c69 9468 5f90 8c2a 5051  ysis.cli.h_..*PQ
+00003110: 9428 68f9 6865 685f 686d 8c0e 5051 416e  .(h.heh_hm..PQAn
+00003120: 616c 7973 6973 2e63 6c69 9490 8c2a 5051  alysis.cli...*PQ
 00003130: 416e 616c 7973 6973 2e69 6f2e 696e 7075  Analysis.io.inpu
 00003140: 745f 6669 6c65 5f72 6561 6465 722e 6578  t_file_reader.ex
-00003150: 6365 7074 696f 6e73 948f 9428 6887 6883  ceptions...(h.h.
-00003160: 6861 6a3a 0100 0090 8c1b 5051 416e 616c  haj:......PQAnal
+00003150: 6365 7074 696f 6e73 948f 9428 6887 6861  ceptions...(h.ha
+00003160: 6883 6a3c 0100 0090 8c1b 5051 416e 616c  h.j<......PQAnal
 00003170: 7973 6973 2e61 6e61 6c79 7369 732e 7264  ysis.analysis.rd
 00003180: 662e 6170 6994 8f94 286a 9a01 0000 906a  f.api...(j.....j
-00003190: 4c01 0000 8f94 2868 656a 9a01 0000 908c  L.....(hej......
+00003190: 4c01 0000 8f94 286a 9a01 0000 6865 908c  L.....(j....he..
 000031a0: 0974 7164 6d2e 6175 746f 948f 9428 68a5  .tqdm.auto...(h.
 000031b0: 6865 908c 1f50 5141 6e61 6c79 7369 732e  he...PQAnalysis.
 000031c0: 696f 2e69 6e70 7574 5f66 696c 655f 7265  io.input_file_re
 000031d0: 6164 6572 948f 9428 6869 6a7c 0100 0090  ader...(hij|....
 000031e0: 8c27 5051 416e 616c 7973 6973 2e69 6f2e  .'PQAnalysis.io.
 000031f0: 696e 7075 745f 6669 6c65 5f72 6561 6465  input_file_reade
-00003200: 722e 666f 726d 6174 7394 8f94 2868 6968  r.formats...(hih
-00003210: 8568 956a 3a01 0000 8c1f 5051 416e 616c  .h.j:.....PQAnal
-00003220: 7973 6973 2e69 6f2e 696e 7075 745f 6669  ysis.io.input_fi
-00003230: 6c65 5f72 6561 6465 7294 908c 1850 5141  le_reader....PQA
+00003200: 722e 666f 726d 6174 7394 8f94 286a 3c01  r.formats...(j<.
+00003210: 0000 8c1f 5051 416e 616c 7973 6973 2e69  ....PQAnalysis.i
+00003220: 6f2e 696e 7075 745f 6669 6c65 5f72 6561  o.input_file_rea
+00003230: 6465 7294 6869 6895 6885 908c 1850 5141  der.hih.h....PQA
 00003240: 6e61 6c79 7369 732e 696f 2e65 7863 6570  nalysis.io.excep
-00003250: 7469 6f6e 7394 8f94 2868 6d68 7d6a 3c01  tions...(hmh}j<.
-00003260: 0000 686f 908c 1250 5141 6e61 6c79 7369  ..ho...PQAnalysi
-00003270: 732e 696f 2e62 6173 6594 8f94 2868 6d68  s.io.base...(hmh
-00003280: 776a 3e01 0000 68c3 686f 6a7c 0100 0068  wj>...h.hoj|...h
-00003290: a568 bb68 8568 a968 a168 c168 716a 3d01  .h.h.h.h.h.hqj=.
+00003250: 7469 6f6e 7394 8f94 2868 6f68 6d6a 3a01  tions...(hohmj:.
+00003260: 0000 687d 908c 1250 5141 6e61 6c79 7369  ..h}...PQAnalysi
+00003270: 732e 696f 2e62 6173 6594 8f94 2868 a968  s.io.base...(h.h
+00003280: 8568 a568 a16a 3d01 0000 6871 68c1 68c3  .h.h.j=...hqh.h.
+00003290: 68bb 6a3e 0100 0068 6f68 6d68 776a 7c01  h.j>...hohmhwj|.
 000032a0: 0000 908c 1850 5141 6e61 6c79 7369 732e  .....PQAnalysis.
 000032b0: 7068 7973 6963 616c 5f64 6174 6194 8f94  physical_data...
 000032c0: 2868 7190 8c1e 5051 416e 616c 7973 6973  (hq...PQAnalysis
 000032d0: 2e69 6f2e 696e 666f 5f66 696c 655f 7265  .io.info_file_re
 000032e0: 6164 6572 948f 9428 6871 6a7c 0100 0090  ader...(hqj|....
 000032f0: 8c22 5051 416e 616c 7973 6973 2e69 6f2e  ."PQAnalysis.io.
 00003300: 6d6f 6c64 6573 6372 6970 746f 725f 7265  moldescriptor_re
-00003310: 6164 6572 948f 9428 6a3d 0100 006a 7c01  ader...(j=...j|.
+00003310: 6164 6572 948f 9428 6a3e 0100 006a 7c01  ader...(j>...j|.
 00003320: 0000 908c 2950 5141 6e61 6c79 7369 732e  ....)PQAnalysis.
 00003330: 696f 2e72 6573 7461 7274 5f66 696c 652e  io.restart_file.
 00003340: 7265 7374 6172 745f 7772 6974 6572 948f  restart_writer..
 00003350: 9428 8c1a 5051 416e 616c 7973 6973 2e69  .(..PQAnalysis.i
 00003360: 6f2e 7265 7374 6172 745f 6669 6c65 946a  o.restart_file.j
 00003370: 7c01 0000 908c 2950 5141 6e61 6c79 7369  |.....)PQAnalysi
 00003380: 732e 696f 2e72 6573 7461 7274 5f66 696c  s.io.restart_fil
 00003390: 652e 7265 7374 6172 745f 7265 6164 6572  e.restart_reader
-000033a0: 948f 9428 6a58 0100 006a ba01 0000 6a7c  ...(jX...j....j|
+000033a0: 948f 9428 6aba 0100 006a 5801 0000 6a7c  ...(j....jX...j|
 000033b0: 0100 0090 8c1e 5051 416e 616c 7973 6973  ......PQAnalysis
 000033c0: 2e69 6f2e 7265 7374 6172 745f 6669 6c65  .io.restart_file
 000033d0: 2e61 7069 948f 9428 6879 6a7c 0100 0090  .api...(hyj|....
 000033e0: 8c29 5051 416e 616c 7973 6973 2e69 6f2e  .)PQAnalysis.io.
 000033f0: 7472 616a 5f66 696c 652e 7472 616a 6563  traj_file.trajec
 00003400: 746f 7279 5f72 6561 6465 7294 8f94 288c  tory_reader...(.
 00003410: 1750 5141 6e61 6c79 7369 732e 696f 2e74  .PQAnalysis.io.t
 00003420: 7261 6a5f 6669 6c65 946a 7c01 0000 908c  raj_file.j|.....
 00003430: 2950 5141 6e61 6c79 7369 732e 696f 2e74  )PQAnalysis.io.t
 00003440: 7261 6a5f 6669 6c65 2e74 7261 6a65 6374  raj_file.traject
 00003450: 6f72 795f 7772 6974 6572 948f 9428 6ac1  ory_writer...(j.
 00003460: 0100 006a 7c01 0000 908c 2450 5141 6e61  ...j|.....$PQAna
 00003470: 6c79 7369 732e 696f 2e74 7261 6a5f 6669  lysis.io.traj_fi
 00003480: 6c65 2e66 7261 6d65 5f72 6561 6465 7294  le.frame_reader.
-00003490: 8f94 2868 a56a c101 0000 6a7c 0100 0090  ..(h.j....j|....
+00003490: 8f94 286a c101 0000 68a5 6a7c 0100 0090  ..(j....h.j|....
 000034a0: 8c1b 5051 416e 616c 7973 6973 2e69 6f2e  ..PQAnalysis.io.
 000034b0: 7472 616a 5f66 696c 652e 6170 6994 8f94  traj_file.api...
-000034c0: 2868 7568 796a 7c01 0000 908c 2650 5141  (huhyj|.....&PQA
+000034c0: 2868 7968 756a 7c01 0000 908c 2650 5141  (hyhuj|.....&PQA
 000034d0: 6e61 6c79 7369 732e 696f 2e67 656e 5f66  nalysis.io.gen_f
 000034e0: 696c 652e 6765 6e5f 6669 6c65 5f72 6561  ile.gen_file_rea
 000034f0: 6465 7294 8f94 288c 1650 5141 6e61 6c79  der...(..PQAnaly
 00003500: 7369 732e 696f 2e67 656e 5f66 696c 6594  sis.io.gen_file.
 00003510: 6a5d 0100 006a 7c01 0000 908c 2650 5141  j]...j|.....&PQA
 00003520: 6e61 6c79 7369 732e 696f 2e67 656e 5f66  nalysis.io.gen_f
 00003530: 696c 652e 6765 6e5f 6669 6c65 5f77 7269  ile.gen_file_wri
@@ -859,121 +859,121 @@
 000035a0: 8f94 286a 7c01 0000 908c 1f50 5141 6e61  ..(j|......PQAna
 000035b0: 6c79 7369 732e 696f 2e74 6f70 6f6c 6f67  lysis.io.topolog
 000035c0: 795f 6669 6c65 2e61 7069 948f 9428 6a7c  y_file.api...(j|
 000035d0: 0100 0090 8c20 5051 416e 616c 7973 6973  ..... PQAnalysis
 000035e0: 2e69 6f2e 656e 6572 6779 5f66 696c 655f  .io.energy_file_
 000035f0: 7265 6164 6572 948f 9428 6a7c 0100 0090  reader...(j|....
 00003600: 8c18 5051 416e 616c 7973 6973 2e69 6f2e  ..PQAnalysis.io.
-00003610: 626f 785f 7772 6974 6572 948f 9428 6875  box_writer...(hu
-00003620: 6879 6a7c 0100 0090 8c11 5051 416e 616c  hyj|......PQAnal
+00003610: 626f 785f 7772 6974 6572 948f 9428 6879  box_writer...(hy
+00003620: 6875 6a7c 0100 0090 8c11 5051 416e 616c  huj|......PQAnal
 00003630: 7973 6973 2e69 6f2e 6170 6994 8f94 286a  ysis.io.api...(j
 00003640: 7c01 0000 908c 1c50 5141 6e61 6c79 7369  |......PQAnalysi
 00003650: 732e 696f 2e63 6f6e 7665 7273 696f 6e5f  s.io.conversion_
 00003660: 6170 6994 8f94 286a 7c01 0000 908c 1750  api...(j|......P
 00003670: 5141 6e61 6c79 7369 732e 696f 2e77 7269  QAnalysis.io.wri
 00003680: 7465 5f61 7069 948f 9428 6a7c 0100 0090  te_api...(j|....
 00003690: 8c17 5051 416e 616c 7973 6973 2e69 6f2e  ..PQAnalysis.io.
-000036a0: 7472 616a 5f66 696c 6594 8f94 2868 a368  traj_file...(h.h
-000036b0: 7990 8c16 5051 416e 616c 7973 6973 2e69  y...PQAnalysis.i
+000036a0: 7472 616a 5f66 696c 6594 8f94 2868 7968  traj_file...(hyh
+000036b0: a390 8c16 5051 416e 616c 7973 6973 2e69  ....PQAnalysis.i
 000036c0: 6f2e 6765 6e5f 6669 6c65 948f 9428 6879  o.gen_file...(hy
 000036d0: 908c 1250 5141 6e61 6c79 7369 732e 666f  ...PQAnalysis.fo
 000036e0: 726d 6174 7394 8f94 2868 8368 7d68 f190  rmats...(h.h}h..
 000036f0: 8c31 5051 416e 616c 7973 6973 2e69 6f2e  .1PQAnalysis.io.
 00003700: 696e 7075 745f 6669 6c65 5f72 6561 6465  input_file_reade
 00003710: 722e 696e 7075 745f 6669 6c65 5f70 6172  r.input_file_par
-00003720: 7365 7294 8f94 2868 876a 3a01 0000 6895  ser...(h.j:...h.
+00003720: 7365 7294 8f94 2868 9568 876a 3c01 0000  ser...(h.h.j<...
 00003730: 6aad 0100 0090 8c22 5051 416e 616c 7973  j......"PQAnalys
 00003740: 6973 2e69 6f2e 696e 7075 745f 6669 6c65  is.io.input_file
 00003750: 5f72 6561 6465 722e 7071 948f 9428 6aad  _reader.pq...(j.
 00003760: 0100 0090 8c2b 5051 416e 616c 7973 6973  .....+PQAnalysis
 00003770: 2e69 6f2e 696e 7075 745f 6669 6c65 5f72  .io.input_file_r
 00003780: 6561 6465 722e 7071 5f61 6e61 6c79 7369  eader.pq_analysi
 00003790: 7394 8f94 286a ad01 0000 908c 3250 5141  s...(j......2PQA
 000037a0: 6e61 6c79 7369 732e 696f 2e69 6e70 7574  nalysis.io.input
 000037b0: 5f66 696c 655f 7265 6164 6572 2e70 715f  _file_reader.pq_
 000037c0: 616e 616c 7973 6973 2e5f 7061 7273 6594  analysis._parse.
-000037d0: 8f94 288c 3c50 5141 6e61 6c79 7369 732e  ..(.<PQAnalysis.
-000037e0: 696f 2e69 6e70 7574 5f66 696c 655f 7265  io.input_file_re
-000037f0: 6164 6572 2e70 715f 616e 616c 7973 6973  ader.pq_analysis
-00003800: 2e5f 7365 6c65 6374 696f 6e5f 6d69 7869  ._selection_mixi
-00003810: 6e94 6a4f 0100 006a 4801 0000 908c 4850  n.jO...jH.....HP
+000037d0: 8f94 286a 4f01 0000 6a47 0100 008c 3c50  ..(jO...jG....<P
+000037e0: 5141 6e61 6c79 7369 732e 696f 2e69 6e70  QAnalysis.io.inp
+000037f0: 7574 5f66 696c 655f 7265 6164 6572 2e70  ut_file_reader.p
+00003800: 715f 616e 616c 7973 6973 2e5f 7365 6c65  q_analysis._sele
+00003810: 6374 696f 6e5f 6d69 7869 6e94 908c 4850  ction_mixin...HP
 00003820: 5141 6e61 6c79 7369 732e 696f 2e69 6e70  QAnalysis.io.inp
 00003830: 7574 5f66 696c 655f 7265 6164 6572 2e70  ut_file_reader.p
 00003840: 715f 616e 616c 7973 6973 2e70 7161 6e61  q_analysis.pqana
 00003850: 6c79 7369 735f 696e 7075 745f 6669 6c65  lysis_input_file
 00003860: 5f72 6561 6465 7294 8f94 288c 2b50 5141  _reader...(.+PQA
 00003870: 6e61 6c79 7369 732e 696f 2e69 6e70 7574  nalysis.io.input
 00003880: 5f66 696c 655f 7265 6164 6572 2e70 715f  _file_reader.pq_
 00003890: 616e 616c 7973 6973 9490 8c37 5051 416e  analysis...7PQAn
 000038a0: 616c 7973 6973 2e69 6f2e 696e 7075 745f  alysis.io.input_
 000038b0: 6669 6c65 5f72 6561 6465 722e 7071 5f61  file_reader.pq_a
 000038c0: 6e61 6c79 7369 732e 5f66 696c 655f 6d69  nalysis._file_mi
-000038d0: 7869 6e94 8f94 286a 3a01 0000 908c 3c50  xin...(j:.....<P
+000038d0: 7869 6e94 8f94 286a 3c01 0000 908c 3c50  xin...(j<.....<P
 000038e0: 5141 6e61 6c79 7369 732e 696f 2e69 6e70  QAnalysis.io.inp
 000038f0: 7574 5f66 696c 655f 7265 6164 6572 2e70  ut_file_reader.p
 00003900: 715f 616e 616c 7973 6973 2e5f 7365 6c65  q_analysis._sele
 00003910: 6374 696f 6e5f 6d69 7869 6e94 8f94 286a  ction_mixin...(j
-00003920: 3a01 0000 908c 3c50 5141 6e61 6c79 7369  :.....<PQAnalysi
+00003920: 3c01 0000 908c 3c50 5141 6e61 6c79 7369  <.....<PQAnalysi
 00003930: 732e 696f 2e69 6e70 7574 5f66 696c 655f  s.io.input_file_
 00003940: 7265 6164 6572 2e70 715f 616e 616c 7973  reader.pq_analys
 00003950: 6973 2e5f 706f 7369 7469 6f6e 735f 6d69  is._positions_mi
-00003960: 7869 6e94 8f94 286a 3a01 0000 908c 2f50  xin...(j:...../P
+00003960: 7869 6e94 8f94 286a 3c01 0000 908c 2f50  xin...(j<...../P
 00003970: 5141 6e61 6c79 7369 732e 696f 2e69 6e70  QAnalysis.io.inp
 00003980: 7574 5f66 696c 655f 7265 6164 6572 2e70  ut_file_reader.p
 00003990: 712e 6f75 7470 7574 5f66 696c 6573 948f  q.output_files..
 000039a0: 9428 6895 908c 3750 5141 6e61 6c79 7369  .(h...7PQAnalysi
 000039b0: 732e 696f 2e69 6e70 7574 5f66 696c 655f  s.io.input_file_
 000039c0: 7265 6164 6572 2e70 712e 7071 5f69 6e70  reader.pq.pq_inp
 000039d0: 7574 5f66 696c 655f 7265 6164 6572 948f  ut_file_reader..
 000039e0: 9428 8c22 5051 416e 616c 7973 6973 2e69  .(."PQAnalysis.i
 000039f0: 6f2e 696e 7075 745f 6669 6c65 5f72 6561  o.input_file_rea
 00003a00: 6465 722e 7071 9490 8c25 5051 416e 616c  der.pq...%PQAnal
 00003a10: 7973 6973 2e69 6f2e 7265 7374 6172 745f  ysis.io.restart_
 00003a20: 6669 6c65 2e65 7863 6570 7469 6f6e 7394  file.exceptions.
-00003a30: 8f94 2868 a16a 3d01 0000 908c 2250 5141  ..(h.j=....."PQA
+00003a30: 8f94 2868 a16a 3e01 0000 908c 2250 5141  ..(h.j>....."PQA
 00003a40: 6e61 6c79 7369 732e 696f 2e74 7261 6a5f  nalysis.io.traj_
 00003a50: 6669 6c65 2e65 7863 6570 7469 6f6e 7394  file.exceptions.
-00003a60: 8f94 2868 a56a 3b01 0000 908c 1850 5141  ..(h.j;......PQA
+00003a60: 8f94 286a 3b01 0000 68a5 908c 1850 5141  ..(j;...h....PQA
 00003a70: 6e61 6c79 7369 732e 696f 2e76 6972 6961  nalysis.io.viria
 00003a80: 6c2e 6170 6994 8f94 2868 af90 8c16 5051  l.api...(h....PQ
 00003a90: 416e 616c 7973 6973 2e75 7469 6c73 2e75  Analysis.utils.u
 00003aa0: 6e69 7473 948f 9428 68af 908c 1650 5141  nits...(h....PQA
 00003ab0: 6e61 6c79 7369 732e 7574 696c 732e 6669  nalysis.utils.fi
 00003ac0: 6c65 7394 8f94 2868 af90 8c1c 5051 416e  les...(h....PQAn
 00003ad0: 616c 7973 6973 2e69 6f2e 6e65 702e 6578  alysis.io.nep.ex
 00003ae0: 6365 7074 696f 6e73 948f 9428 68af 908c  ceptions...(h...
 00003af0: 2150 5141 6e61 6c79 7369 732e 696f 2e67  !PQAnalysis.io.g
 00003b00: 656e 5f66 696c 652e 6578 6365 7074 696f  en_file.exceptio
-00003b10: 6e73 948f 9428 6a3e 0100 0090 8c30 5051  ns...(j>.....0PQ
+00003b10: 6e73 948f 9428 6a3d 0100 0090 8c30 5051  ns...(j=.....0PQ
 00003b20: 416e 616c 7973 6973 2e69 6f2e 746f 706f  Analysis.io.topo
 00003b30: 6c6f 6779 5f66 696c 652e 746f 706f 6c6f  logy_file.topolo
 00003b40: 6779 5f66 696c 655f 7772 6974 6572 948f  gy_file_writer..
-00003b50: 9428 8c1b 5051 416e 616c 7973 6973 2e69  .(..PQAnalysis.i
-00003b60: 6f2e 746f 706f 6c6f 6779 5f66 696c 6594  o.topology_file.
-00003b70: 68bf 908c 3050 5141 6e61 6c79 7369 732e  h...0PQAnalysis.
+00003b50: 9428 68bf 8c1b 5051 416e 616c 7973 6973  .(h...PQAnalysis
+00003b60: 2e69 6f2e 746f 706f 6c6f 6779 5f66 696c  .io.topology_fil
+00003b70: 6594 908c 3050 5141 6e61 6c79 7369 732e  e...0PQAnalysis.
 00003b80: 696f 2e74 6f70 6f6c 6f67 795f 6669 6c65  io.topology_file
 00003b90: 2e74 6f70 6f6c 6f67 795f 6669 6c65 5f72  .topology_file_r
-00003ba0: 6561 6465 7294 8f94 286a 0a02 0000 68bf  eader...(j....h.
+00003ba0: 6561 6465 7294 8f94 2868 bf6a 0a02 0000  eader...(h.j....
 00003bb0: 908c 2650 5141 6e61 6c79 7369 732e 696f  ..&PQAnalysis.io
 00003bc0: 2e74 6f70 6f6c 6f67 795f 6669 6c65 2e65  .topology_file.e
 00003bd0: 7863 6570 7469 6f6e 7394 8f94 2868 c168  xceptions...(h.h
 00003be0: c390 8c22 5051 416e 616c 7973 6973 2e69  ..."PQAnalysis.i
 00003bf0: 6f2e 7669 7269 616c 2e76 6972 6961 6c5f  o.virial.virial_
 00003c00: 7265 6164 6572 948f 9428 68c9 8c14 5051  reader...(h...PQ
 00003c10: 416e 616c 7973 6973 2e69 6f2e 7669 7269  Analysis.io.viri
 00003c20: 616c 9490 8c1c 5051 416e 616c 7973 6973  al....PQAnalysis
 00003c30: 2e69 6f2e 6e65 702e 6e65 705f 7772 6974  .io.nep.nep_writ
 00003c40: 6572 948f 9428 68cf 908c 1f50 5141 6e61  er...(h....PQAna
 00003c50: 6c79 7369 732e 636c 692e 5f61 7267 756d  lysis.cli._argum
-00003c60: 656e 745f 7061 7273 6572 948f 9428 68e5  ent_parser...(h.
-00003c70: 68d9 68d3 68e3 68e1 68d5 68d7 68d1 68df  h.h.h.h.h.h.h.h.
-00003c80: 68cf 908c 1850 5141 6e61 6c79 7369 732e  h....PQAnalysis.
+00003c60: 656e 745f 7061 7273 6572 948f 9428 68e3  ent_parser...(h.
+00003c70: 68d3 68df 68cf 68d1 68e1 68e5 68d9 68d7  h.h.h.h.h.h.h.h.
+00003c80: 68d5 908c 1850 5141 6e61 6c79 7369 732e  h....PQAnalysis.
 00003c90: 636c 692e 5f63 6c69 5f62 6173 6594 8f94  cli._cli_base...
-00003ca0: 2868 e568 d968 d368 e168 d568 d768 d168  (h.h.h.h.h.h.h.h
-00003cb0: df68 cf90 8c1d 5051 416e 616c 7973 6973  .h....PQAnalysis
+00003ca0: 2868 d368 df68 cf68 d168 e168 e568 d968  (h.h.h.h.h.h.h.h
+00003cb0: d768 d590 8c1d 5051 416e 616c 7973 6973  .h....PQAnalysis
 00003cc0: 2e74 6f6f 6c73 2e61 6464 5f6d 6f6c 6563  .tools.add_molec
 00003cd0: 756c 6594 8f94 2868 d790 8c16 5051 416e  ule...(h....PQAn
 00003ce0: 616c 7973 6973 2e63 6c69 2e78 797a 3267  alysis.cli.xyz2g
 00003cf0: 656e 948f 9428 68e3 908c 1950 5141 6e61  en...(h....PQAna
 00003d00: 6c79 7369 732e 636c 692e 7472 616a 3271  lysis.cli.traj2q
 00003d10: 6d63 6663 948f 9428 68e3 908c 1750 5141  mcfc...(h....PQA
 00003d20: 6e61 6c79 7369 732e 636c 692e 7472 616a  nalysis.cli.traj
@@ -1029,27 +1029,27 @@
 00004040: 6c65 6d65 6e74 948f 9428 6a11 0100 008c  lement...(j.....
 00004050: 1450 5141 6e61 6c79 7369 732e 636f 7265  .PQAnalysis.core
 00004060: 2e61 746f 6d94 908c 1950 5141 6e61 6c79  .atom....PQAnaly
 00004070: 7369 732e 636f 7265 2e61 746f 6d2e 6174  sis.core.atom.at
 00004080: 6f6d 948f 9428 6a4e 0200 0090 8c23 5051  om...(jN.....#PQ
 00004090: 416e 616c 7973 6973 2e70 6879 7369 6361  Analysis.physica
 000040a0: 6c5f 6461 7461 2e65 7863 6570 7469 6f6e  l_data.exception
-000040b0: 7394 8f94 286a 1901 0000 8c18 5051 416e  s...(j......PQAn
-000040c0: 616c 7973 6973 2e70 6879 7369 6361 6c5f  alysis.physical_
-000040d0: 6461 7461 9490 8c1f 5051 416e 616c 7973  data....PQAnalys
+000040b0: 7394 8f94 288c 1850 5141 6e61 6c79 7369  s...(..PQAnalysi
+000040c0: 732e 7068 7973 6963 616c 5f64 6174 6194  s.physical_data.
+000040d0: 6a19 0100 0090 8c1f 5051 416e 616c 7973  j.......PQAnalys
 000040e0: 6973 2e70 6879 7369 6361 6c5f 6461 7461  is.physical_data
 000040f0: 2e65 6e65 7267 7994 8f94 286a 5302 0000  .energy...(jS...
 00004100: 9075 8c10 6475 706c 6963 6174 6564 5f6c  .u..duplicated_l
 00004110: 696e 6573 947d 9428 8c13 6e62 5f64 7570  ines.}.(..nb_dup
 00004120: 6c69 6361 7465 645f 6c69 6e65 7394 4b00  licated_lines.K.
 00004130: 8c18 7065 7263 656e 745f 6475 706c 6963  ..percent_duplic
 00004140: 6174 6564 5f6c 696e 6573 9447 0000 0000  ated_lines.G....
 00004150: 0000 0000 758c 0a6e 6f64 655f 636f 756e  ....u..node_coun
 00004160: 7494 7d94 2868 0e4b 4b68 094b 7468 0f4d  t.}.(h.KKh.Kth.M
 00004170: 0602 6810 4b7c 758c 0c75 6e64 6f63 756d  ..h.K|u..undocum
 00004180: 656e 7465 6494 7d94 2868 0e4b 0068 094b  ented.}.(h.K.h.K
 00004190: 0068 0f4b 0068 104b 0075 6818 4b02 6819  .h.K.h.K.uh.K.h.
 000041a0: 4b00 681a 4b00 681b 4b00 681c 4b33 681d  K.h.K.h.K.h.K3h.
-000041b0: 4d72 1168 1e4b 0c8c 0b67 6c6f 6261 6c5f  Mr.h.K...global_
-000041c0: 6e6f 7465 9447 4023 b57b 3e05 bb71 6a58  note.G@#.{>..qjX
-000041d0: 0200 004b 196a 5902 0000 473f c102 6f8e  ...K.jY...G?..o.
-000041e0: 21aa 4d75 622e                           !.Mub.
+000041b0: 4d73 1168 1e4b 0c8c 0b67 6c6f 6261 6c5f  Ms.h.K...global_
+000041c0: 6e6f 7465 9447 4023 b57f 834b 973d 6a58  note.G@#...K.=jX
+000041d0: 0200 004b 196a 5902 0000 473f c101 0c25  ...K.jY...G?...%
+000041e0: d12d 7375 622e                           .-sub.
```

### Comparing `pqanalysis-1.0.2/.github/ISSUE_TEMPLATE/feature_request.md` & `pqanalysis-1.0.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/.github/scripts/parse_pylint.py` & `pqanalysis-1.0.3/.github/scripts/parse_pylint.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/.github/workflows/ci.yml` & `pqanalysis-1.0.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/.github/workflows/docs.yml` & `pqanalysis-1.0.3/.github/workflows/docs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Sample workflow for building and deploying a Jekyll site to GitHub Pages
 name: Docs
 
 on:
   # Runs on pushes targeting the default branch
   push:
-    branches: ["main"]
+    branches: 
+      - '*'
 
   # Allows you to run this workflow manually from the Actions tab
   workflow_dispatch:
 
 # Sets permissions of the GITHUB_TOKEN to allow deployment to GitHub Pages
 permissions:
   contents: write
@@ -66,7 +67,8 @@
 
       # Deployment job
       - name: deploy
         uses: JamesIves/github-pages-deploy-action@releases/v4
         with:
           branch: gh-pages # The branch the action should deploy to.
           folder: docs/build/html # The folder the action should deploy.
+        if: github.ref_name == 'main' # Only deploy on pushes to the main branch
```

### Comparing `pqanalysis-1.0.2/.github/workflows/pylint.yml` & `pqanalysis-1.0.3/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/.github/workflows/release.yml` & `pqanalysis-1.0.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/.pylintrc` & `pqanalysis-1.0.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/CODE_OF_CONDUCT.md` & `pqanalysis-1.0.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/LICENSE` & `pqanalysis-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PKG-INFO` & `pqanalysis-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PQAnalysis
-Version: 1.0.2
+Version: 1.0.3
 Summary: PQAnalysis is a python package for the analysis of PQ simulations.
 Author-email: Jakob Gamper <97gamjak@gmail.com>, "Josef M. Gallmetzer" <gallmetzer.josef@gmail.com>, "Clarissa A. Seidler" <clarissa.seidler@gmail.com>
 Project-URL: Homepage, https://github.com/MolarVerse/PQAnalysis
 Project-URL: PQ, https://github.com/MolarVerse/PQ
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pqanalysis-1.0.2/PQAnalysis/__init__.py` & `pqanalysis-1.0.3/PQAnalysis/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,16 +20,15 @@
 ##################
 # BEARTYPE SETUP #
 ##################
 
 # TODO: change the default level to "RELEASE" after all changes are implemented
 __beartype_default_level__ = "RELEASE"
 __beartype_level__ = os.getenv(
-    "PQANALYSIS_BEARTYPE_LEVEL",
-    __beartype_default_level__
+    "PQANALYSIS_BEARTYPE_LEVEL", __beartype_default_level__
 )
 
 if __beartype_level__.upper() == "DEBUG":
     beartype_this_package()
 
 #################
 # LOGGING SETUP #
@@ -39,16 +38,18 @@
 
 if logging_env_var and logging_env_var not in logging.getLevelNamesMapping():
     raise ValueError(
         f"Invalid logging level: {logging_env_var}. Valid logging "
         f"levels are: {logging.getLevelNamesMapping()}"
     )
 
-if 'execution_start_time' not in vars(
-) and 'execution_start_time' not in globals():
+if (
+    'execution_start_time' not in vars() and
+    'execution_start_time' not in globals()
+):
     execution_start_time = time.strftime('%Y-%m-%d_%H-%M-%S', time.localtime())
 
 logging.setLoggerClass(CustomLogger)
 logging.basicConfig(level=os.getenv("PQANALYSIS_LOGGING_LEVEL", "INFO"))
 package_logger = logging.getLogger(__name__)
 
 log_file_env_var = os.getenv("PQANALYSIS_LOG_FILE")
```

### Comparing `pqanalysis-1.0.2/PQAnalysis/analysis/rdf/__init__.py` & `pqanalysis-1.0.3/PQAnalysis/analysis/rdf/__init__.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/analysis/rdf/api.py` & `pqanalysis-1.0.3/PQAnalysis/analysis/rdf/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/analysis/rdf/exceptions.py` & `pqanalysis-1.0.3/PQAnalysis/analysis/rdf/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/analysis/rdf/rdf.py` & `pqanalysis-1.0.3/PQAnalysis/analysis/rdf/rdf.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/analysis/rdf/rdf_input_file_reader.py` & `pqanalysis-1.0.3/PQAnalysis/analysis/rdf/rdf_input_file_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/analysis/rdf/rdf_output_file_writer.py` & `pqanalysis-1.0.3/PQAnalysis/analysis/rdf/rdf_output_file_writer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/atomic_system/_decorators.py` & `pqanalysis-1.0.3/PQAnalysis/atomic_system/_decorators.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/atomic_system/_positions.py` & `pqanalysis-1.0.3/PQAnalysis/atomic_system/_positions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/atomic_system/_properties.py` & `pqanalysis-1.0.3/PQAnalysis/atomic_system/_properties.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 """
 from numbers import Real
 
 import numpy as np
 
 from beartype.typing import List
 
-from PQAnalysis.core import Cell
+from PQAnalysis.core import Cell, CustomElement
 from PQAnalysis.types import Np1DNumberArray
+
 from ._decorators import check_atoms_has_mass, check_atoms_pos
 from .exceptions import AtomicSystemError
 
 
 
 class _PropertiesMixin:
 
@@ -49,16 +50,16 @@
 
         if n_atoms_list.size == 0:
             return 0
 
         if not np.all(n_atoms_list == n_atoms_list[0]):
             self.logger.error(
                 (
-                "The number of atoms (or atoms in the topology), "
-                "positions, velocities, forces and charges must be equal."
+                    "The number of atoms (or atoms in the topology), "
+                    "positions, velocities, forces and charges must be equal."
                 ),
                 exception=AtomicSystemError
             )
 
         return int(n_atoms_list[0])
 
     @property
@@ -79,17 +80,15 @@
         """Np1DNumberArray: The center of mass of the system."""
         if self.n_atoms == 0:
             return np.zeros(3)
 
         relative_pos = self.cell.image(self.pos - self.pos[0]) + self.pos[0]
 
         weighted_average_pos = np.sum(
-            relative_pos * self.atomic_masses[:,
-            None],
-            axis=0
+            relative_pos * self.atomic_masses[:, None], axis=0
         ) / self.mass
 
         center_of_mass = self.cell.image(weighted_average_pos)
 
         return center_of_mass
 
     @property
@@ -97,7 +96,12 @@
         """str: The combined name of the atoms in the system."""
         return ''.join(atom.name for atom in self.atoms)
 
     @property
     def unique_element_names(self) -> List[str]:
         """List[str]: The unique element names of the atoms in the system."""
         return list({atom.element_name for atom in self.atoms})
+
+    @property
+    def build_custom_element(self) -> CustomElement:
+        """CustomElement: The custom element of the atoms in the system."""
+        return CustomElement(self.combined_name, -1, self.mass)
```

### Comparing `pqanalysis-1.0.2/PQAnalysis/atomic_system/_standard_properties.py` & `pqanalysis-1.0.3/PQAnalysis/atomic_system/_standard_properties.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             The positions of the atoms in the system.
         """
         self._pos = pos
 
     @property
     def has_pos(self) -> bool:
         """bool: A boolean indicating if the system has positions for all atoms."""
-        return len(self.pos) == self.n_atoms
+        return len(self.pos) == self.n_atoms and self.n_atoms != 0
 
     @property
     def vel(self) -> Np2DNumberArray:
         """
         Np2DNumberArray: The velocities of the atoms in the system.
 
         In order to set the velocities of the atoms in the system, 
@@ -110,15 +110,15 @@
             The velocities of the atoms in the system.
         """
         self._vel = vel
 
     @property
     def has_vel(self) -> bool:
         """bool: A boolean indicating if the system has velocities for all atoms."""
-        return len(self.vel) == self.n_atoms
+        return len(self.vel) == self.n_atoms and self.n_atoms != 0
 
     @property
     def forces(self) -> Np2DNumberArray:
         """
         Np2DNumberArray: The forces acting on the atoms in the system.
 
         In order to set the forces acting on the atoms in the system,
@@ -143,15 +143,15 @@
             The forces acting on the atoms in the system.
         """
         self._forces = forces
 
     @property
     def has_forces(self) -> bool:
         """bool: A boolean indicating if the system has forces for all atoms."""
-        return len(self.forces) == self.n_atoms
+        return len(self.forces) == self.n_atoms and self.n_atoms != 0
 
     @property
     def charges(self) -> Np1DNumberArray:
         """
         Np1DNumberArray: The charges of the atoms in the system.
 
         In order to set the charges of the atoms in the system,
@@ -176,15 +176,15 @@
             The charges of the atoms in the system.
         """
         self._charges = charges
 
     @property
     def has_charges(self) -> bool:
         """bool: A boolean indicating if the system has charges for all atoms."""
-        return len(self.charges) == self.n_atoms
+        return len(self.charges) == self.n_atoms and self.n_atoms != 0
 
     @property
     def cell(self) -> Cell:
         """Cell: The unit cell of the system."""
         return self._cell
 
     @cell.setter
```

### Comparing `pqanalysis-1.0.2/PQAnalysis/atomic_system/atomic_system.py` & `pqanalysis-1.0.3/PQAnalysis/atomic_system/atomic_system.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # just for forwardref type hinting
 from beartype.typing import List  # pylint: disable=unused-import
 
 from PQAnalysis.core import Atom, Atoms, Cell, distance
 from PQAnalysis.topology import Topology
 from PQAnalysis.types import PositiveReal, PositiveInt
 from PQAnalysis.type_checking import runtime_type_checking
+from PQAnalysis.exceptions import PQNotImplementedError
 from PQAnalysis.utils.random import get_random_seed
 from PQAnalysis.utils.custom_logging import setup_logger
 from PQAnalysis import __package_name__
 
 from PQAnalysis.types import (
     Np2DNumberArray,
     Np1DNumberArray,
@@ -31,17 +32,19 @@
 from ._properties import _PropertiesMixin
 from ._standard_properties import _StandardPropertiesMixin
 from ._positions import _PositionsMixin
 from .exceptions import AtomicSystemError
 
 
 
-class AtomicSystem(_PropertiesMixin,
+class AtomicSystem(
+    _PropertiesMixin,
     _StandardPropertiesMixin,
-    _PositionsMixin):
+    _PositionsMixin,
+):
 
     """
     A class for storing atomic systems.
 
     It contains the standard properties of an atomic system
     (i.e. positions, velocities, forces, charges, topology and cell).
     The AtomicSystem class can be used as a container for the 
@@ -165,16 +168,16 @@
         ValueError
             If both atoms and topology are given.
         """
 
         if topology is not None and atoms is not None:
             self.logger.error(
                 (
-                "Cannot initialize AtomicSystem with both atoms and topology "
-                "arguments - they are mutually exclusive."
+                    "Cannot initialize AtomicSystem with both atoms and topology "
+                    "arguments - they are mutually exclusive."
                 ),
                 exception=AtomicSystemError
             )
 
         if atoms is None and topology is None:
             topology = Topology()
         elif topology is None:
@@ -251,27 +254,27 @@
             # positions of all systems that have been fitted so far
             positions_to_fit_into = np.concatenate(
                 [system.pos for system in systems] + [self.pos]
             )
 
             self.fitting_logger.info(
                 (
-                f"Performing fitting for {i + 1}/{number_of_additions} "
-                "addition(s)."
+                    f"Performing fitting for {i + 1}/{number_of_additions} "
+                    "addition(s)."
                 )
             )
 
             systems.append(
                 self._fit_atomic_system(
-                positions_to_fit_into=positions_to_fit_into,
-                system=system,
-                max_iterations=max_iterations,
-                distance_cutoff=distance_cutoff,
-                max_displacement=max_displacement,
-                rotation_angle_step=rotation_angle_step
+                    positions_to_fit_into=positions_to_fit_into,
+                    system=system,
+                    max_iterations=max_iterations,
+                    distance_cutoff=distance_cutoff,
+                    max_displacement=max_displacement,
+                    rotation_angle_step=rotation_angle_step
                 )
             )
 
         return systems if number_of_additions > 1 else systems[0]
 
     def _fit_atomic_system(
         self,
@@ -355,15 +358,15 @@
 
             for x, y, z in itertools.product(range(0, 360, rotation_angle_step), repeat=3):
                 rotation_angles = rotation.as_euler('xyz', degrees=True)
                 rotation_angles += np.array([x, y, z])
                 rotation = Rotation.from_euler(
                     'xyz',
                     rotation_angles,
-                    degrees=True
+                    degrees=True,
                 )
                 new_pos = rotation.apply(new_pos)
 
                 distances = distance(positions_to_fit_into, new_pos, self.cell)
 
                 if np.all(distances > distance_cutoff):
                     iter_converged = _iter
@@ -383,14 +386,94 @@
         )
         system = system.copy()
         system.pos = new_pos
         system.cell = self.cell
         system.image()
         return system
 
+    @property
+    def center_of_mass_residues(self) -> "AtomicSystem":
+        """
+        Computes the center of mass of the residues in the system.
+
+        Returns
+        -------
+        AtomicSystem
+            The center of mass of the residues in the system.
+            
+        Raises:
+        -------
+        AtomicSystemError
+            If the number of residues in the system is not a 
+            multiple of the number of atoms.
+        PQNotImplementedError
+            if system has forces, velocities or charges.
+            
+        TODO:
+        -----
+        Include also center of mass velocities, forces and so on...
+        """
+        if self.has_pos:
+            residue_pos = np.zeros(
+                (len(self.topology.residue_atom_indices), 3)
+            )
+        else:
+            residue_pos = np.zeros((0, 3))
+
+        residue_atoms = []
+
+        if self.has_forces or self.has_vel or self.has_charges:
+            self.logger.error(
+                (
+                    "Center of mass of residues not implemented for "
+                    "systems with forces, velocities or charges."
+                ),
+                exception=PQNotImplementedError,
+            )
+
+        if len(self.topology.residue_ids) == 0:
+            self.logger.error(
+                "No residues in the system.",
+                exception=AtomicSystemError,
+            )
+
+        if len(self.topology.residue_ids) == 1:
+            return self.copy()
+
+        for i, residue_indices in enumerate(self.topology.residue_atom_indices):
+
+            residue_system = self[residue_indices]
+
+            # check if residue_system has more than one atom otherwise return atom element
+            if (
+                residue_system.n_atoms != 1 and
+                len(self.topology.residues) != 0
+            ):
+                custom_element = residue_system.build_custom_element
+                custom_element.symbol = self.topology.residues[i].name
+                custom_atom = Atom(custom_element)
+            else:
+                custom_atom = residue_system.atoms[0]
+
+            residue_atoms.append(custom_atom)
+
+            if residue_system.has_pos:
+                residue_pos[i] = residue_system.center_of_mass
+
+        topology = Topology(
+            atoms=residue_atoms,
+            residue_ids=self.topology.residue_ids_per_residue
+        )
+
+        return AtomicSystem(
+            pos=residue_pos,
+            cell=self.cell,
+            topology=topology,
+        )
+
     # TODO: refactor or discard this method
     def compute_com_atomic_system(self, group=None) -> "AtomicSystem":
         """
         Computes a new AtomicSystem with the center of mass of the system or groups of atoms.
 
         Parameters
         ----------
@@ -487,16 +570,15 @@
 
         if not np.allclose(self.charges, other.charges):
             return False
 
         return True
 
     def __getitem__(
-        self,
-        key: Atom | int | slice | Np1DIntArray
+        self, key: Atom | int | slice | Np1DIntArray
     ) -> "AtomicSystem":
         """
         Returns a new AtomicSystem with the given key.
 
         Examples
         --------
         >>> import numpy as np
@@ -541,16 +623,16 @@
 
         if isinstance(key, Atom):
             key = np.argwhere(np.array(self.atoms) == key).flatten()
 
         if isinstance(key, int):
             key = np.array([key])
 
-        keys = np.array(range(self.n_atoms))[key] if isinstance(key,
-            slice) else np.array(key)
+        keys = np.array(range(self.n_atoms)
+                        )[key] if isinstance(key, slice) else np.array(key)
 
         pos = self.pos[keys] if np.shape(self.pos)[0] > 0 else None
         vel = self.vel[keys] if np.shape(self.vel)[0] > 0 else None
         forces = self.forces[keys] if np.shape(self.forces)[0] > 0 else None
         charges = self.charges[keys] if np.shape(self.charges)[0] > 0 else None
 
         return AtomicSystem(
```

### Comparing `pqanalysis-1.0.2/PQAnalysis/atomic_system/exceptions.py` & `pqanalysis-1.0.3/PQAnalysis/atomic_system/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/cli/_argument_parser.py` & `pqanalysis-1.0.3/PQAnalysis/cli/_argument_parser.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/cli/_cli_base.py` & `pqanalysis-1.0.3/PQAnalysis/cli/_cli_base.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/cli/add_molecules.py` & `pqanalysis-1.0.3/PQAnalysis/cli/add_molecules.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/cli/build_nep_traj.py` & `pqanalysis-1.0.3/PQAnalysis/cli/build_nep_traj.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/cli/continue_input.py` & `pqanalysis-1.0.3/PQAnalysis/cli/continue_input.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/cli/gen2xyz.py` & `pqanalysis-1.0.3/PQAnalysis/cli/gen2xyz.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/cli/main.py` & `pqanalysis-1.0.3/PQAnalysis/cli/main.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/cli/rdf.py` & `pqanalysis-1.0.3/PQAnalysis/cli/rdf.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/cli/rst2xyz.py` & `pqanalysis-1.0.3/PQAnalysis/cli/rst2xyz.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/cli/traj2box.py` & `pqanalysis-1.0.3/PQAnalysis/cli/traj2box.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/cli/traj2qmcfc.py` & `pqanalysis-1.0.3/PQAnalysis/cli/traj2qmcfc.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/cli/xyz2gen.py` & `pqanalysis-1.0.3/PQAnalysis/cli/xyz2gen.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/core/api.py` & `pqanalysis-1.0.3/PQAnalysis/core/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/core/atom/atom.py` & `pqanalysis-1.0.3/PQAnalysis/core/atom/atom.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from numbers import Real
 
 from beartype.typing import Any, List, TypeVar
 
 from PQAnalysis import __package_name__
 from PQAnalysis.utils.custom_logging import setup_logger
 from PQAnalysis.type_checking import runtime_type_checking
+from PQAnalysis.exceptions import PQValueError
 
 from .element import Element
 from ..exceptions import AtomError
 
 #: A type hint for a list of atoms
 Atoms = TypeVar("Atoms", bound=List["PQAnalysis.core.Atom"])
 
@@ -78,51 +79,69 @@
 
     logger = logging.getLogger(__package_name__).getChild(__qualname__)
     logger = setup_logger(logger)
 
     @runtime_type_checking
     def __init__(
         self,
-        name: str | int,
+        name: str | int | Element,
         element_id: int | str | None = None,
         use_guess_element: bool = True,
         **_kwargs
     ) -> None:
         """
         Constructs all the necessary attributes for the Atom object.
 
         If use_guess_element is True, the symbol, atomic number and mass are
         determined from the name of the atom_type. If use_guess_element is
         False, the symbol, atomic number and mass are set to None, meaning that
         an empty element is created (Element()).
 
         Parameters
         ----------
-        name : str | int
+        name : str | int | Element
             The name of the atom_type (e.g. 'C1')
             If this parameter is an integer, it is interpreted as the atomic number of the 
-            element symbol and cannot be used together with the id parameter.
+            element symbol and cannot be used together with the id parameter. If the parameter
+            is an Element object, the element is set to this object and no other parameters
+            are used.
         element_id : int | str, optional
             The atomic number or element symbol of the atom_type (e.g. 6 or 'C') 
             If his parameter is not given, the name parameter is used to determine 
             the element type of the atom_type.
         use_guess_element : bool, optional
             Whether to use the guess_element function to determine
             the element type of the atom_type by its name,
             by default True
         **_kwargs
             Additional keyword arguments that are not used by the function but 
             by the runtime type checker.
 
         Raises
         ------
-        ValueError
+        PQValueError
+            If the name of the atom_type is an Element object and the id is given.
+        AtomError
             If the name of the atom_type is an integer and the id is given.
         """
 
+        if isinstance(name, Element):
+            if element_id is not None:
+                self.logger.error(
+                    (
+                    "The element of the atom_type cannot be an "
+                    "Element object if the id is given."
+                    ),
+                    exception=PQValueError
+                )
+
+            self._name = name.symbol
+            self._element = name
+            return
+
         if element_id is not None and isinstance(name, int):
 
             self.logger.error(
                 "The name of the atom_type cannot be an integer if the id is given.",
                 exception=AtomError
             )
```

### Comparing `pqanalysis-1.0.2/PQAnalysis/core/atom/element.py` & `pqanalysis-1.0.3/PQAnalysis/core/atom/element.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 
 from typing import Annotated
 from numbers import Real
 
 from beartype.typing import Any, NewType
 from beartype.vale import Is
 
-from PQAnalysis.type_checking import runtime_type_checking
+from PQAnalysis.type_checking import (
+    runtime_type_checking,
+    runtime_type_checking_setter,
+)
 from PQAnalysis.utils.custom_logging import setup_logger
 from PQAnalysis import __package_name__
 
 from ..exceptions import ElementNotFoundError
 
 
 
@@ -154,20 +157,51 @@
     @property
     def mass(self) -> Real | None:
         """Real | None: The mass of the Element."""
         return self._mass
 
 
 
+class CustomElement(Element):
+
+    """
+    A class representing a custom element it 
+    inherits from the Element class.
+    """
+
+    @runtime_type_checking
+    def __init__(self, symbol: str, atomic_number: int, mass: Real):  # pylint: disable=super-init-not-called
+        """
+        Parameters
+        ----------
+        symbol : str
+            the custom atomic symbol
+        atomic_number : int
+            the custom atomic number
+        mass : Real
+            the custom atomic mass
+        """
+
+        self._symbol = symbol
+        self._atomic_number = atomic_number
+        self._mass = mass
+
+    @Element.symbol.setter
+    @runtime_type_checking_setter
+    def symbol(self, value: str) -> None:
+        self._symbol = value
+
+
+
 #: A type hint for a list of elements
 Elements = NewType(
     "Elements",
-    Annotated[list,
-    Is[lambda list: all(isinstance(element,
-    Element) for element in list)]]
+    Annotated[
+        list,
+        Is[lambda list: all(isinstance(element, Element) for element in list)]]
 )
 
 atomicMasses = {
     "h": 1.00794,
     "d": 2.014101778,
     "t": 3.0160492675,
     "he": 4.002602,
```

### Comparing `pqanalysis-1.0.2/PQAnalysis/core/cell/_standard_properties.py` & `pqanalysis-1.0.3/PQAnalysis/core/cell/_standard_properties.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/core/cell/cell.py` & `pqanalysis-1.0.3/PQAnalysis/core/cell/cell.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/core/exceptions.py` & `pqanalysis-1.0.3/PQAnalysis/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/core/residue.py` & `pqanalysis-1.0.3/PQAnalysis/core/residue.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/exceptions.py` & `pqanalysis-1.0.3/PQAnalysis/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/formats.py` & `pqanalysis-1.0.3/PQAnalysis/formats.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/grammar/inputGrammar.lark` & `pqanalysis-1.0.3/PQAnalysis/grammar/inputGrammar.lark`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/grammar/rules.lark` & `pqanalysis-1.0.3/PQAnalysis/grammar/rules.lark`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/grammar/selection.lark` & `pqanalysis-1.0.3/PQAnalysis/grammar/selection.lark`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/__init__.py` & `pqanalysis-1.0.3/PQAnalysis/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/api.py` & `pqanalysis-1.0.3/PQAnalysis/io/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/base.py` & `pqanalysis-1.0.3/PQAnalysis/io/base.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/box_writer.py` & `pqanalysis-1.0.3/PQAnalysis/io/box_writer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/conversion_api.py` & `pqanalysis-1.0.3/PQAnalysis/io/conversion_api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/energy_file_reader.py` & `pqanalysis-1.0.3/PQAnalysis/io/energy_file_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/exceptions.py` & `pqanalysis-1.0.3/PQAnalysis/io/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/formats.py` & `pqanalysis-1.0.3/PQAnalysis/io/formats.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/gen_file/api.py` & `pqanalysis-1.0.3/PQAnalysis/io/gen_file/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/gen_file/gen_file_reader.py` & `pqanalysis-1.0.3/PQAnalysis/io/gen_file/gen_file_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/gen_file/gen_file_writer.py` & `pqanalysis-1.0.3/PQAnalysis/io/gen_file/gen_file_writer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/info_file_reader.py` & `pqanalysis-1.0.3/PQAnalysis/io/info_file_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/input_file_reader/exceptions.py` & `pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/input_file_reader/formats.py` & `pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/formats.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/input_file_reader/input_file_parser.py` & `pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/input_file_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,20 +79,25 @@
         InputDictionary: InputDictionary
             The parsed input file dictionary.
         """
         if self.input_format == InputFileFormat.PQANALYSIS:
             grammar_file = "inputGrammar.lark"
         elif self.input_format in [InputFileFormat.PQ, InputFileFormat.QMCFC]:
             grammar_file = "PQ_inputGrammar.lark"
+        else:
+            InputDictionary.logger.error(
+                f"Input file format {self.input_format} not supported.",
+                exception=PQTypeError
+            )
 
         grammar_path = __base_path__ / "grammar"
 
         parser = Lark.open(
             grammar_path / grammar_file,
-            propagate_positions=True
+            propagate_positions=True,
         )
 
         with open(self.filename, "r", encoding="utf-8") as file:
             self.raw_input_file = file.read()
 
         self.tree = parser.parse(self.raw_input_file)
 
@@ -487,20 +492,17 @@
         Returns
         -------
         Tuple[Range, str, str]
             tuple containing the range value, the string "range",
             and the line where the token was defined.
         """
 
-        return_range = range(items[0][0],
-            items[1][0]) if len(items) == 2 else range(
-            items[0][0],
-            items[2][0],
-            items[1][0]
-            )
+        return_range = range(
+            items[0][0], items[1][0]
+        ) if len(items) == 2 else range(items[0][0], items[2][0], items[1][0])
 
         return return_range, "range", str(items[0][2])
 
     def glob(self, items) -> Tuple[List[str], str, str]:
         """
         Method to transform glob values
```

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/input_file_reader/pq/output_files.py` & `pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq/output_files.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/input_file_reader/pq/pq_input_file_reader.py` & `pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq/pq_input_file_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/input_file_reader/pq_analysis/_file_mixin.py` & `pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq_analysis/_file_mixin.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/input_file_reader/pq_analysis/_parse.py` & `pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq_analysis/_parse.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/input_file_reader/pq_analysis/_positions_mixin.py` & `pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq_analysis/_positions_mixin.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/input_file_reader/pq_analysis/_selection_mixin.py` & `pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq_analysis/_selection_mixin.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/input_file_reader/pq_analysis/pqanalysis_input_file_reader.py` & `pqanalysis-1.0.3/PQAnalysis/io/input_file_reader/pq_analysis/pqanalysis_input_file_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/moldescriptor_reader.py` & `pqanalysis-1.0.3/PQAnalysis/io/moldescriptor_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/nep/nep_writer.py` & `pqanalysis-1.0.3/PQAnalysis/io/nep/nep_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,18 +232,18 @@
         virial_files = file_dict[OutputFileFormat.VIRIAL.value
                                  ] if use_virial else []
 
         if not np.isclose(test_ratio, 0.0) or total_ratios is not None:
             if self.filename is None:
                 self.logger.error(
                     (
-                    "No output filename was specified. In order to "
-                    "use the test_ratio or total_ratios splitting feature "
-                    "a filename has to be given in order to write all "
-                    "generated files."
+                        "No output filename was specified. In order to "
+                        "use the test_ratio or total_ratios splitting feature "
+                        "a filename has to be given in order to write all "
+                        "generated files."
                     ),
                     exception=NEPError
                 )
 
             self._setup_frame_splitting_for_training(test_ratio, total_ratios)
 
         self.open()
@@ -255,20 +255,18 @@
         for i, xyz_file in enumerate(xyz_files):
 
             stress = read_stress_file(stress_files[i]) if use_stress else []
             virial = read_virial_file(virial_files[i]) if use_virial else []
             energy = EnergyFileReader(en_files[i], info_files[i]).read()
 
             xyz_generator = read_trajectory_generator(
-                xyz_file,
-                traj_format=TrajectoryFormat.XYZ
+                xyz_file, traj_format=TrajectoryFormat.XYZ
             )
             force_generator = read_trajectory_generator(
-                force_files[i],
-                traj_format=TrajectoryFormat.FORCE
+                force_files[i], traj_format=TrajectoryFormat.FORCE
             ) if use_forces else None
 
             n_frames = calculate_frames_of_trajectory_file(xyz_file)
 
             n_train_max, n_test_max, _ = self._get_effective_training_portions(
                 n_frames,
                 self.test_ratio,
@@ -290,79 +288,82 @@
 
             for j, system in enumerate(xyz_generator):
                 if hasattr(energy, "qm_energy"):
                     system.energy = energy.qm_energy[j]
                 else:
                     self.logger.error(
                         (
-                        "No QM energy found in the energy file. "
-                        "The NEP builder is implemented only for QM energies. "
-                        "If there is a need for a different energy type, "
-                        "please file an issue at "
-                        f"{config.code_base_url}issues."
+                            "No QM energy found in the energy file. "
+                            "The NEP builder is implemented only for QM energies. "
+                            "If there is a need for a different energy type, "
+                            "please file an issue at "
+                            f"{config.code_base_url}issues."
                         ),
                         exception=NEPError
                     )
 
                 if use_forces:
                     force_system = next(force_generator)
                     system.forces = force_system.forces
 
                 if use_virial and virial:
                     system.virial = virial[j]
                 if use_stress and stress:
                     system.stress = stress[j]
 
                 self.write_from_atomic_system(
-                    system,
-                    self.file,
-                    use_forces,
-                    use_stress,
-                    use_virial
+                    system, self.file, use_forces, use_stress, use_virial
                 )
 
                 self.is_validation = False
 
                 if j in train_indices:
                     self.n_train_frames += 1
                     file_to_write = self.train_file
                 elif j in test_indices:
                     self.n_test_frames += 1
                     file_to_write = self.test_file
                 elif j in validation_indices:
                     self.n_validation_frames += 1
                     self.is_validation = True
                     file_to_write = self.validation_ref_file
+                else:
+                    self.logger.error(
+                        (
+                            "An error occurred during the frame splitting. "
+                            "The frame index is not in any of the training, "
+                            "testing, or validation indices. This should not "
+                            "happen. Please file an issue at "
+                            f"{config.code_base_url}issues."
+                        ),
+                        exception=NEPError
+                    )
 
                 self.write_from_atomic_system(
-                    system,
-                    file_to_write,
-                    use_forces,
-                    use_stress,
-                    use_virial
+                    system, file_to_write, use_forces, use_stress, use_virial
                 )
 
                 if self.is_validation:
                     self.write_from_atomic_system(
                         system,
                         self.validation_file,
                         use_forces=False,
                         use_stress=False,
                         use_virial=False,
                     )
 
             self.logger.info(
                 (
-                f"Processed {n_frames} frames from files:\n"
-                f"{xyz_file}, "
-                f"{en_files[i]}, "
-                f"{info_files[i]}, "
-                f"{force_files[i] if use_forces else None}, "
-                f"{stress_files[i] if use_stress else None}, "
-                f"{virial_files[i] if use_virial else None}"
+                    f"Processed {n_frames} frames from files:\n"
+                    f"{xyz_file}, "
+                    f"{en_files[i]}, "
+                    f"{info_files[i]}, "
+                    f"{force_files[i] if use_forces else None}, "
+                    f"{stress_files[i] if use_stress else None}, "
+                    f"{virial_files[i] if use_virial else None}"
                 )
             )
 
         self._close_files()
 
     def _close_files(self):
         """
@@ -426,16 +427,16 @@
         ValueError
             If validation frames are given without test frames.
         """
 
         if not np.isclose(test_ratio, 0.0) and total_ratios is not None:
             self.logger.error(
                 (
-                "The test_ratio and total_ratios keyword "
-                "arguments are mutually exclusive."
+                    "The test_ratio and total_ratios keyword "
+                    "arguments are mutually exclusive."
                 ),
                 exception=NEPError
             )
 
         if total_ratios is not None:
             ratios = total_ratios.split(":")
             if len(ratios) == 2:
@@ -445,17 +446,17 @@
             elif len(ratios) == 3:
                 n_train = float(ratios[0])
                 n_test = float(ratios[1])
                 n_validation = float(ratios[2])
             else:
                 self.logger.error(
                     (
-                    f"The total_ratios keyword argument {total_ratios} "
-                    "is not in the correct format. The correct format "
-                    "is train_ratio:test_ratio:validation_ratio."
+                        f"The total_ratios keyword argument {total_ratios} "
+                        "is not in the correct format. The correct format "
+                        "is train_ratio:test_ratio:validation_ratio."
                     ),
                     exception=NEPError
                 )
         else:
             n_train = 0.0
             n_validation = 0.0
             n_test = 0.0
@@ -464,29 +465,28 @@
 
         self.test_ratio = n_test / sum_frames
         self.validation_ratio = n_validation / sum_frames
 
         if self.test_ratio > 1.0:
             self.logger.error(
                 (
-                "The test_ratio must be between 0.0 and 1.0. "
-                "The given test_ratio "
-                f"is {self.test_ratio}."
+                    "The test_ratio must be between 0.0 and 1.0. "
+                    "The given test_ratio "
+                    f"is {self.test_ratio}."
                 ),
                 exception=NEPError
             )
 
         if np.isclose(self.test_ratio,
-            0.0) and not np.isclose(self.validation_ratio,
-            0.0):
+                      0.0) and not np.isclose(self.validation_ratio, 0.0):
             self.logger.error(
                 (
-                "It has no sense to have validation frames without test "
-                "frames. This error results from the given total_ratios "
-                f"keyword argument {total_ratios}."
+                    "It has no sense to have validation frames without test "
+                    "frames. This error results from the given total_ratios "
+                    f"keyword argument {total_ratios}."
                 ),
                 exception=NEPError
             )
 
         self.train_file = None
         self.train_writer = None
         self.train_file = None
@@ -494,46 +494,41 @@
         self.validation_file = None
         self.validation_writer = None
         self.validation_ref_file = None
         self.validation_ref_writer = None
 
         if not np.isclose(self.test_ratio, 0.0):
             self.train_writer = BaseWriter(
-                f"{self.filename}_train",
-                mode=self.original_mode
+                f"{self.filename}_train", mode=self.original_mode
             )
             self.test_writer = BaseWriter(
-                f"{self.filename}_test",
-                mode=self.original_mode
+                f"{self.filename}_test", mode=self.original_mode
             )
             self.train_writer.open()
             self.test_writer.open()
             self.train_file = self.train_writer.file
             self.test_file = self.test_writer.file
 
         if not np.isclose(self.validation_ratio, 0.0):
             self.validation_writer = BaseWriter(
-                f"{self.filename}_validation",
-                mode=self.original_mode
+                f"{self.filename}_validation", mode=self.original_mode
             )
             self.validation_writer.open()
             self.validation_ref_writer = BaseWriter(
-                f"{self.filename}_validation.ref",
-                mode=self.original_mode
+                f"{self.filename}_validation.ref", mode=self.original_mode
             )
             self.validation_ref_writer.open()
             self.validation_file = self.validation_writer.file
             self.validation_ref_file = self.validation_ref_writer.file
 
     def _determine_files(
         self,
         files: List[str],
         file_prefixes: List[str],
-    ) -> Dict[str,
-        List[str]]:
+    ) -> Dict[str, List[str]]:
         """
         Determines the files to be used for writing the NEP trajectory file.
 
         Parameters
         ----------
         files : List[str]
             The files to be used for writing the NEP trajectory file.
@@ -600,15 +595,15 @@
                 self.virial_file_extension,
                 file_prefixes
             )
 
         def raise_number_of_files_error(
             file_type: str,
             files: List[str],
-            xyz_files: List[str]
+            xyz_files: List[str],
         ):
             """
             Raises an error if the number of files does not 
             match the number of coordinate files.
 
             Parameters
             ----------
@@ -617,19 +612,19 @@
             files : List[str]
                 the files to be used for writing the NEP trajectory file
             xyz_files : List[str]
                 the coordinate files
             """
             self.logger.error(
                 (
-                f"The number of {file_type} files does not match "
-                "the number of coordinate files. The found "
-                f"{file_type} files are: {files} "
-                "and the found coordinate files are: "
-                f"{xyz_files}"
+                    f"The number of {file_type} files does not match "
+                    "the number of coordinate files. The found "
+                    f"{file_type} files are: {files} "
+                    "and the found coordinate files are: "
+                    f"{xyz_files}"
                 ),
                 exception=NEPError
             )
 
         en_files = file_dict[OutputFileFormat.ENERGY.value]
         xyz_files = file_dict[OutputFileFormat.XYZ.value]
         info_files = file_dict[OutputFileFormat.INFO.value]
@@ -703,63 +698,59 @@
             If no files with the given file prefixes were found.
         ValueError
             If no files with the given file prefixes 
             and file extension were found.
         """
 
         filtered_files = OutputFileFormat.find_matching_files(
-            files,
-            output_file_format,
-            file_extension
+            files, output_file_format, file_extension
         )
 
         if len(filtered_files) == 0:
             if file_extension is not None:
                 self.logger.error(
                     (
-                    "You did specify a file extension for the "
-                    f"{output_file_format} files, but no files with "
-                    f"the extension {file_extension} were found, "
-                    f"that match the given file prefixes {file_prefixes}."
+                        "You did specify a file extension for the "
+                        f"{output_file_format} files, but no files with "
+                        f"the extension {file_extension} were found, "
+                        f"that match the given file prefixes {file_prefixes}."
                     ),
                     exception=NEPError
                 )
             else:
                 output_file_formats = OutputFileFormat.get_file_extensions(
                     output_file_format
                 )
                 self.logger.error(
                     (
-                    f"No {output_file_format} files were found in "
-                    f"{files} that match the given file prefixes "
-                    f"{file_prefixes}. All possible file extensions are "
-                    f"{output_file_formats}. "
-                    "If the specific file extension you are looking for "
-                    "is not in the list, please specify it using the "
-                    "corresponding file_extension argument. If the "
-                    "files should be found, please check the file paths "
-                    "and the file prefixes. Additionally, if you think "
-                    "that the file extension you chose is of general "
-                    "interest and should be added to the list of "
-                    "possible file extensions, please file an issue at "
-                    f"{config.code_base_url}issues."
+                        f"No {output_file_format} files were found in "
+                        f"{files} that match the given file prefixes "
+                        f"{file_prefixes}. All possible file extensions are "
+                        f"{output_file_formats}. "
+                        "If the specific file extension you are looking for "
+                        "is not in the list, please specify it using the "
+                        "corresponding file_extension argument. If the "
+                        "files should be found, please check the file paths "
+                        "and the file prefixes. Additionally, if you think "
+                        "that the file extension you chose is of general "
+                        "interest and should be added to the list of "
+                        "possible file extensions, please file an issue at "
+                        f"{config.code_base_url}issues."
                     ),
                     exception=NEPError
                 )
 
         return sorted(filtered_files)
 
     def _get_effective_training_portions(
         self,
         n_frames: int,
         test_ratio: PositiveReal,
         validation_ratio: PositiveReal,
-    ) -> tuple[int,
-        int,
-        int]:
+    ) -> tuple[int, int, int]:
         """
         Calculates the maximum number of training, testing,
         and validation frames.
 
         By calculating the maximum number of training, testing,
         and validation frames, the number of frames to be added 
         to the training and testing files can be determined.
@@ -815,18 +806,15 @@
             Whether to write the virial tensor to the NEP trajectory file, 
             by default False
         """
 
         self.open()
         for frame in trajectory:
             self.write_from_atomic_system(
-                frame,
-                use_forces,
-                use_stress,
-                use_virial
+                frame, use_forces, use_stress, use_virial
             )
 
         self.close()
 
     @runtime_type_checking
     def write_from_atomic_system(
         self,
@@ -879,60 +867,60 @@
 
         if file is None:
             return
 
         if not system.has_pos:
             self.logger.error(
                 (
-                "The system does not have coordinates, "
-                "which are required for NEP trajectory files."
+                    "The system does not have coordinates, "
+                    "which are required for NEP trajectory files."
                 ),
                 exception=NEPError
             )
 
         if not system.has_energy:
             self.logger.error(
                 "The system does not have an energy, "
                 "which is required for NEP trajectory files.",
                 exception=NEPError
             )
 
         if use_forces and not system.has_forces:
             self.logger.error(
                 (
-                "The system does not have forces, and they were "
-                "specified to be written to the NEP trajectory file."
+                    "The system does not have forces, and they were "
+                    "specified to be written to the NEP trajectory file."
                 ),
                 exception=NEPError
             )
 
         if use_stress and use_virial:
             self.logger.error(
                 (
-                "Both the stress and the virial tensor were "
-                "specified to be written to the NEP trajectory file. "
-                "Only one of them can be written at a time."
+                    "Both the stress and the virial tensor were "
+                    "specified to be written to the NEP trajectory file. "
+                    "Only one of them can be written at a time."
                 ),
                 exception=NEPError
             )
 
         if use_stress and not system.has_stress:
             self.logger.error(
                 (
-                "The system does not have a stress tensor, "
-                "and it was specified to be written to the NEP trajectory file."
+                    "The system does not have a stress tensor, "
+                    "and it was specified to be written to the NEP trajectory file."
                 ),
                 exception=NEPError
             )
 
         if use_virial and not system.has_virial:
             self.logger.error(
                 (
-                "The system does not have a virial tensor, and "
-                "it was specified to be written to the NEP trajectory file."
+                    "The system does not have a virial tensor, and "
+                    "it was specified to be written to the NEP trajectory file."
                 ),
                 exception=NEPError
             )
 
         self._write_header(system, file, use_forces, use_stress, use_virial)
         self._write_body(system, file, use_forces)
 
@@ -1024,30 +1012,30 @@
 
         for i in range(system.n_atoms):
             symbol = system.atoms[i].symbol
             symbol = symbol[0].upper() + symbol[1:]
 
             print(
                 (
-                f"{symbol:<4} "
-                f"{system.pos[i][0]:12.8f} "
-                f"{system.pos[i][1]:12.8f} "
-                f"{system.pos[i][2]:12.8f}"
+                    f"{symbol:<4} "
+                    f"{system.pos[i][0]:12.8f} "
+                    f"{system.pos[i][1]:12.8f} "
+                    f"{system.pos[i][2]:12.8f}"
                 ),
                 file=file,
                 end=" "
             )
 
             forces = system.forces * eV / kcal_per_mol
 
             if use_forces:
                 print(
                     (
-                    f"{forces[i][0]:15.8e} "
-                    f"{forces[i][1]:15.8e} "
-                    f"{forces[i][2]:15.8e}"
+                        f"{forces[i][0]:15.8e} "
+                        f"{forces[i][1]:15.8e} "
+                        f"{forces[i][2]:15.8e}"
                     ),
                     file=file,
                     end=" "
                 )
 
             print(file=file)
```

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/restart_file/api.py` & `pqanalysis-1.0.3/PQAnalysis/io/restart_file/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/restart_file/restart_reader.py` & `pqanalysis-1.0.3/PQAnalysis/io/restart_file/restart_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/restart_file/restart_writer.py` & `pqanalysis-1.0.3/PQAnalysis/io/restart_file/restart_writer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/topology_file/api.py` & `pqanalysis-1.0.3/PQAnalysis/io/topology_file/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/topology_file/topology_file_reader.py` & `pqanalysis-1.0.3/PQAnalysis/io/topology_file/topology_file_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/topology_file/topology_file_writer.py` & `pqanalysis-1.0.3/PQAnalysis/io/topology_file/topology_file_writer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/traj_file/api.py` & `pqanalysis-1.0.3/PQAnalysis/io/traj_file/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 A module containing different API functions for reading and writing trajectory files.
 """
 
-from beartype.typing import Generator
+from beartype.typing import Generator, List
 
 from PQAnalysis.topology import Topology
 from PQAnalysis.atomic_system import AtomicSystem
 from PQAnalysis.io.formats import FileWritingMode
 from PQAnalysis.type_checking import runtime_type_checking
 
 from PQAnalysis.io.traj_file import (
@@ -58,27 +58,27 @@
     writer = TrajectoryWriter(filename, engine_format=engine_format, mode=mode)
     writer.write(traj, traj_type=traj_type)
 
 
 
 @runtime_type_checking
 def read_trajectory(
-    filename: str,
+    filename: str | List[str],
     md_format: MDEngineFormat | str = MDEngineFormat.PQ,
     traj_format: TrajectoryFormat | str = TrajectoryFormat.AUTO,
     topology: Topology | None = None,
     constant_topology: bool = True
 ) -> Trajectory:
     """
     API function for reading a trajectory from a file.
 
     Parameters
     ----------
-    filename : str
-        The name of the file to read from.
+    filename : str | List[str]
+        The name of the file to read from or a list of files to read from.
     md_format : MDEngineFormat | str, optional
         The format of the trajectory, by default MDEngineFormat.PQ
     traj_format : TrajectoryFormat | str, optional
         The format of the trajectory, by default TrajectoryFormat.AUTO.
         The format is inferred from the file extension.
     topology : Topology | None, optional
         The topology of the trajectory, by default None
```

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/traj_file/frame_reader.py` & `pqanalysis-1.0.3/PQAnalysis/io/traj_file/frame_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,16 +35,15 @@
     see :py:class:`~PQAnalysis.traj.formats.TrajectoryFormat`.
     """
 
     logger = logging.getLogger(__package_name__).getChild(__qualname__)
     logger = setup_logger(logger)
 
     def __init__(
-        self,
-        md_format: MDEngineFormat | str = MDEngineFormat.PQ
+        self, md_format: MDEngineFormat | str = MDEngineFormat.PQ
     ) -> None:
         """
         Parameters
         ----------
         md_format : MDEngineFormat | str, optional
             The format of the MD engine. Default is "PQ".
         """
@@ -210,17 +209,16 @@
         topology = self._get_topology(atoms, self.topology)
 
         return AtomicSystem(topology=topology, charges=charges, cell=cell)
 
     def _check_qmcfc(
         self,
         atoms: List[str],
-        value: Np1DNumberArray | Np2DNumberArray
-    ) -> Tuple[Np1DNumberArray | Np2DNumberArray,
-        List[str]]:
+        value: Np1DNumberArray | Np2DNumberArray,
+    ) -> Tuple[Np1DNumberArray | Np2DNumberArray, List[str]]:
         """
         Check if the first atom is X for QMCFC. If it is, remove it from the list and array.
 
         Parameters
         ----------
         atoms : List[str]
             The list of atoms.
@@ -238,28 +236,26 @@
             If the first atom is not X for QMCFC.
         """
 
         if self.md_format == MDEngineFormat.QMCFC:
             if atoms[0].upper() != 'X':
                 self.logger.error(
                     (
-                    'The first atom in one of the frames is not X. '
-                    'Please use PQ (default) md engine instead'
+                        'The first atom in one of the frames is not X. '
+                        'Please use PQ (default) md engine instead'
                     ),
                     exception=FrameReaderError
                 )
             value = value[1:]
             atoms = atoms[1:]
 
         return value, atoms
 
     def _get_topology(
-        self,
-        atoms: List[str],
-        topology: Topology | None
+        self, atoms: List[str], topology: Topology | None
     ) -> Topology:
         """
         Returns the topology of the frame.
 
         Returns
         -------
         Topology
@@ -267,28 +263,28 @@
         """
 
         if topology is None:
             try:
 
                 topology = Topology(
                     atoms=[
-                    Atom(atom,
-                    disable_type_checking=True) for atom in atoms
+                        Atom(atom, disable_type_checking=True)
+                        for atom in atoms
                     ]
                 )
 
             except ElementNotFoundError:
 
                 topology = Topology(
                     atoms=[
-                    Atom(
-                    atom,
-                    use_guess_element=False,
-                    disable_type_checking=True
-                    ) for atom in atoms
+                        Atom(
+                            atom,
+                            use_guess_element=False,
+                            disable_type_checking=True
+                        ) for atom in atoms
                     ]
                 )
 
         return topology
 
     def _read_header_line(self, header_line: str) -> Tuple[int, Cell]:
         """
@@ -334,18 +330,19 @@
             self.logger.error(
                 'Invalid file format in header line of Frame.',
                 exception=FrameReaderError
             )
 
         return n_atoms, cell
 
-    def _read_xyz(self,
+    def _read_xyz(
+        self,
         splitted_frame_string: List[str],
-        n_atoms: int) -> Tuple[Np2DNumberArray,
-        List[str]]:
+        n_atoms: int,
+    ) -> Tuple[Np2DNumberArray, List[str]]:
         """
         Reads the xyz coordinates and the atom names from the given string.
 
         Parameters
         ----------
         splitted_frame_string : str
             The string to read the xyz coordinates and the atom names from.
@@ -378,18 +375,19 @@
             return xyz, atoms
         except ValueError:
             self.logger.error(
                 'Invalid file format in xyz coordinates of Frame.',
                 exception=FrameReaderError
             )
 
-    def _read_scalar(self,
+    def _read_scalar(
+        self,
         splitted_frame_string: List[str],
-        n_atoms: int) -> Tuple[Np1DNumberArray,
-        List[str]]:
+        n_atoms: int,
+    ) -> Tuple[Np1DNumberArray, List[str]]:
         """
         Reads the scalar values and the atom names from the given string.
 
         Parameters
         ----------
         splitted_frame_string : str
             The string to read the scalar values and the atom names from.
```

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/traj_file/trajectory_reader.py` & `pqanalysis-1.0.3/PQAnalysis/io/traj_file/trajectory_reader.py`

 * *Files 5% similar despite different names*

```diff
@@ -160,15 +160,17 @@
         Yields
         ------
         Generator[AtomicSystem]
             The frames of the trajectory.
         """
 
         # Get the length of the trajectory
-        self.length_of_traj = self.calculate_number_of_frames()
+        number_of_frames = self.calculate_number_of_frames_per_file()
+
+        self.length_of_traj = sum(number_of_frames)
 
         if trajectory_stop is None:
             trajectory_stop = self.length_of_traj
 
         # If trajectory_start is less than 0 or greater than the
         # length of the trajectory, raise an IndexError
         if trajectory_start < 0 or trajectory_start > self.length_of_traj:
@@ -189,51 +191,62 @@
         # raise an IndexError
         if trajectory_start >= trajectory_stop:
             self.logger.error(
                 "start index is greater than or equal to the stop index",
                 exception=PQIndexError,
             )
 
+        # Initialize the progress bar
+        progress_bar = tqdm(
+            total=trajectory_stop - trajectory_start,
+            disable=not self.with_progress_bar
+        )
+
         # Track the number of frames that have been read
         frame_index = 0
 
         last_cell = None
 
-        for filename in self.filenames:
+        for i, filename in enumerate(self.filenames):
+
+            if trajectory_start >= frame_index + number_of_frames[i]:
+                frame_index += number_of_frames[i]
+                continue
+
+            if trajectory_stop <= frame_index:
+                break
 
             # Read the file again to get the frames
             with open(filename, "r", encoding="utf-8") as self.file:
                 frame_lines = []
 
-                progress_bar = tqdm(
-                    total=self.length_of_traj,
-                    disable=not self.with_progress_bar
-                )
-
                 # Read the lines of the file using tqdm for progress bar
                 for line in self.file:
+
                     stripped_line = line.strip()
                     if stripped_line == "" or not stripped_line[0].isdigit():
                         frame_lines.append(line)
                     else:
                         if frame_lines:
                             frame = self._read_single_frame(
                                 "".join(frame_lines),
-                                self.topology
+                                self.topology,
                             )
+
                             if frame.cell.is_vacuum and last_cell is not None:
                                 frame.cell = last_cell
+
                             last_cell = frame.cell
 
-                            # TODO: Implement the trajectory_start and trajectory_stop
-                            # more efficiently
                             # Check if the number of frames yielded is equal to the
                             # total number of frames
-                            if not (frame_index < trajectory_start or
-                                frame_index >= trajectory_stop):
+                            if not (
+                                frame_index < trajectory_start or
+                                frame_index >= trajectory_stop
+                            ):
                                 yield frame  # only yield the frame if it is within the range
                                 progress_bar.update(
                                     1
                                 )  # update the progress bar
 
                             # then increment the frame index
                             frame_index += 1
@@ -242,26 +255,27 @@
                                 self.topology = frame.topology
 
                         frame_lines = [line]
 
                 if frame_lines:
                     frame = self._read_single_frame(
                         "".join(frame_lines),
-                        self.topology
+                        self.topology,
                     )
 
                     if frame.cell.is_vacuum and last_cell is not None:
                         frame.cell = last_cell
 
                     last_cell = frame.cell
 
-                    # TODO: Implement the trajectory_start and trajectory_stop more efficiently
                     # Check if the number of frames yielded is equal to the total number of frames
-                    if not (frame_index < trajectory_start or
-                        frame_index >= trajectory_stop):
+                    if not (
+                        frame_index < trajectory_start or
+                        frame_index >= trajectory_stop
+                    ):
                         yield frame  # only yield the frame if it is within the range
                         progress_bar.update(1)  # update the progress bar
 
                     # then increment the frame index
                     frame_index += 1
 
                 if self.constant_topology and self.topology is not None:
@@ -314,15 +328,15 @@
         ------
         Generator[Trajectory]
             A generator over the windows of the trajectory with the specified
             window size and gap.
         """
 
         # Get the length of the trajectory
-        self.length_of_traj = self.calculate_number_of_frames()
+        self.length_of_traj = sum(self.calculate_number_of_frames_per_file())
 
         # If trajectory_stop is not provided, set it to the length of the trajectory
         if trajectory_stop is None:
             trajectory_stop = self.length_of_traj
 
         # If trajectory_start is less than 0 or greater than the
         # length of the trajectory, raise an IndexError
@@ -369,106 +383,137 @@
             self.logger.error(
                 "window size is greater than the trajectory_stop - trajectory_start",
                 exception=PQIndexError,
             )
 
         # Check if all frames are included in the windows
         # Length of the trajectory - window_size should be divisible by window_gap
-        if ((trajectory_stop - trajectory_start) -
-                window_size) % window_gap != 0:
+        if (
+            ((trajectory_stop - trajectory_start) - window_size) % window_gap
+            != 0
+        ):
             self.logger.warning(
                 "Not all frames are included in the windows. Check the window size and gap."
             )
 
         generator = self.frame_generator(
             trajectory_start=trajectory_start,
-            trajectory_stop=trajectory_stop
+            trajectory_stop=trajectory_stop,
         )
 
         # reads first window and converts it to a queue
         window = Trajectory(
             [
-            next(generator) for _ in range(window_size)  # pylint: disable=stop-iteration-return
+                next(generator) for _ in range(window_size)  # pylint: disable=stop-iteration-return
             ]
         )
 
         # yield the first window
         yield window.copy()
 
         # generate the rest of the windows up to trajectory_stop
-        for _ in range(trajectory_start + window_gap,
+        for _ in range(
+            trajectory_start + window_gap,
             trajectory_stop - window_size + 1,
-            window_gap):
+            window_gap
+        ):
 
             # pop the first frame and append the next frame for window_gap times to
             # get the next window
             for _ in range(window_gap):
                 window.pop(0)
                 window.append(
                     next(generator)  # pylint: disable=stop-iteration-return
                 )
 
             # yield the next window
             yield window.copy()
 
-    def calculate_number_of_frames(self) -> int:
+    def calculate_frame_size(self, filename: str = None) -> int:
         """
-        Calculates the number of frames in the trajectory file.
+        Calculates the size of the frame in the trajectory file.
 
         Returns
         -------
         int
-            The number of frames in the trajectory file.
+            The size of the frame in the trajectory file.
 
         Raises
         ------
         TrajectoryReaderError
             If the number of atoms in the first line of the file is invalid.
+        """
+
+        with open(filename, "r", encoding="utf-8") as f:
+            try:
+                n_atoms = int(f.readline().split()[0])
+            except (ValueError, IndexError):
+                self.logger.error(
+                    (
+                        "Invalid number of atoms in the first line "
+                        f"of file {filename}."
+                    ),
+                    exception=TrajectoryReaderError,
+                )
+
+        return n_atoms + 2
+
+    def calculate_number_of_frames_per_file(self) -> List[int]:
+        """
+        Calculates the number of frames for each trajectory file.
+
+        Returns
+        -------
+        List[int]
+            The number of frames in the trajectory files.
+
+        Raises
+        ------
+        TrajectoryReaderError
             If the number of lines in the file is not divisible by the number of atoms.
         """
 
-        n_frames = 0
+        n_frames_list = []
 
         for filename in self.filenames:
+            n_frames = 0
+
             with open(filename, "r", encoding="utf-8") as f:
 
                 lines = f.readlines()
                 n_lines = len(lines)
 
                 # If the file is empty, continue to the next file
                 if n_lines == 0:
                     continue
 
-                try:
-                    n_atoms = int(lines[0].split()[0])
-                except (ValueError, IndexError):
-                    self.logger.error(
-                        (
-                        "Invalid number of atoms in the first line "
-                        f"of file {filename}."
-                        ),
-                        exception=TrajectoryReaderError,
-                    )
+                # Calculate the size of the frame
+                # NOTE: this allows the user to give input which is not
+                # consistent in the number of atoms per frame in different
+                # traj files.
+                frame_size = self.calculate_frame_size(filename)
 
                 # +2 for the cell/atom_count + comment lines
-                _n_frames, remainder = divmod(n_lines, n_atoms + 2)
+                _n_frames, remainder = divmod(n_lines, frame_size)
 
                 if remainder != 0:
                     self.logger.error(
                         (
-                        "The number of lines in the file is not divisible "
-                        f"by the number of atoms {n_atoms} "
-                        "in the first line."
+                            "The number of lines in the file is not divisible "
+                            f"by the number of atoms {frame_size - 2} "
+                            "in the first line."
                         ),
                         exception=TrajectoryReaderError,
                     )
 
                 n_frames += _n_frames
 
-        return n_frames
+            n_frames_list.append(n_frames)
+
+        return n_frames_list
 
     @property
     def cells(self) -> list[Cell]:
         """
         Returns the cells of the trajectory.
 
         Returns
@@ -537,17 +582,17 @@
 
                         yield cell
 
                     else:
 
                         self.logger.error(
                             (
-                            "Invalid number of arguments for box:"
-                            f" {len(splitted_line)} encountered in file"
-                            f" {filename}:{line_number} = {stripped_line}"
+                                "Invalid number of arguments for box:"
+                                f" {len(splitted_line)} encountered in file"
+                                f" {filename}:{line_number} = {stripped_line}"
                             ),
                             exception=TrajectoryReaderError,
                         )
 
                     last_cell = cell
 
                     for _ in range(n_atoms + 1):
@@ -577,9 +622,9 @@
         ------
         TrajectoryReaderError
             If the first atom in the frame is not X for QMCFC.
         """
         return self.frame_reader.read(
             frame_string,
             traj_format=self.traj_format,
-            topology=topology
+            topology=topology,
         )
```

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/traj_file/trajectory_writer.py` & `pqanalysis-1.0.3/PQAnalysis/io/traj_file/trajectory_writer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/virial/api.py` & `pqanalysis-1.0.3/PQAnalysis/io/virial/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/virial/virial_reader.py` & `pqanalysis-1.0.3/PQAnalysis/io/virial/virial_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/io/write_api.py` & `pqanalysis-1.0.3/PQAnalysis/io/write_api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/physical_data/energy.py` & `pqanalysis-1.0.3/PQAnalysis/physical_data/energy.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/tools/add_molecule.py` & `pqanalysis-1.0.3/PQAnalysis/tools/add_molecule.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/tools/traj_to_com_traj.py` & `pqanalysis-1.0.3/PQAnalysis/tools/traj_to_com_traj.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/topology/__init__.py` & `pqanalysis-1.0.3/PQAnalysis/topology/__init__.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/topology/api.py` & `pqanalysis-1.0.3/PQAnalysis/topology/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/topology/bonded_topology/_topology_properties.py` & `pqanalysis-1.0.3/PQAnalysis/topology/bonded_topology/_topology_properties.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/topology/bonded_topology/angle.py` & `pqanalysis-1.0.3/PQAnalysis/topology/bonded_topology/angle.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/topology/bonded_topology/bond.py` & `pqanalysis-1.0.3/PQAnalysis/topology/bonded_topology/bond.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/topology/bonded_topology/bonded_topology.py` & `pqanalysis-1.0.3/PQAnalysis/topology/bonded_topology/bonded_topology.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/topology/bonded_topology/dihedral.py` & `pqanalysis-1.0.3/PQAnalysis/topology/bonded_topology/dihedral.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/topology/selection.py` & `pqanalysis-1.0.3/PQAnalysis/topology/selection.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/topology/shake_topology.py` & `pqanalysis-1.0.3/PQAnalysis/topology/shake_topology.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/topology/topology.py` & `pqanalysis-1.0.3/PQAnalysis/topology/topology.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,18 @@
 import numpy as np
 
 from PQAnalysis.core.exceptions import ResidueError
 from PQAnalysis.core import Residues, Residue, QMResidue, Atoms, Element
 from PQAnalysis.types import Np1DIntArray
 from PQAnalysis.utils.custom_logging import setup_logger
 from PQAnalysis import __package_name__
-from PQAnalysis.type_checking import runtime_type_checking, runtime_type_checking_setter
+from PQAnalysis.type_checking import (
+    runtime_type_checking,
+    runtime_type_checking_setter,
+)
 
 from .exceptions import TopologyError
 from .bonded_topology.bonded_topology import BondedTopology
 
 
 
 class Topology:
@@ -106,15 +109,15 @@
             self._atomtype_names = [atom.name for atom in atoms]
 
         if reference_residues is None:
             self._reference_residues = []
         else:
             self._reference_residues = reference_residues
 
-        if residue_ids is None:
+        if residue_ids is None or len(residue_ids) == 0:
             residue_ids = np.zeros(len(self.atoms), dtype=int)
         if len(self.atoms) != len(residue_ids):
             self.logger.error(
                 "The number of atoms does not match the number of residue ids.",
                 exception=TopologyError
             )
 
@@ -145,32 +148,33 @@
             If the reference residues are not empty and residue_ids
             with 0 don't have any element information. This problem
             can be avoided by setting 'check_residues' to False.
         """
 
         self._residue_ids = residue_ids
         self._residues, self._atoms = self._setup_residues(
-            self.residue_ids, self.atoms)
+            self.residue_ids,
+            self.atoms
+        )
 
         if not self.residues:
             self._residue_numbers = np.arange(self.n_atoms)
             self._residue_atom_indices = [
-                np.arange(i,
-                i + 1) for i in range(self.n_atoms)
+                np.arange(i, i + 1) for i in range(self.n_atoms)
             ]
         else:
             _residue_numbers = []
             self._residue_atom_indices = []
             atom_counter = 0
             for i in range(self.n_residues):
                 _residue_numbers += [i] * self.residues[i].n_atoms
                 self._residue_atom_indices.append(
                     np.arange(
-                    atom_counter,
-                    atom_counter + self.residues[i].n_atoms
+                        atom_counter,
+                        atom_counter + self.residues[i].n_atoms,
                     )
                 )
 
                 atom_counter += self.residues[i].n_atoms
             self._residue_numbers = np.array(_residue_numbers)
 
     def __eq__(self, other: Any) -> bool:
@@ -234,15 +238,15 @@
             reference_residues=self.reference_residues,
             residue_ids=residue_ids,
             check_residues=self.check_residues
         )
 
     def get_atom_indices_from_residue_names(
         self,
-        residue_name: str
+        residue_name: str,
     ) -> Np1DIntArray:
         """
         Returns the atom indices for the given residue name.
 
         Parameters
         ----------
         residue_name : str
@@ -250,44 +254,48 @@
 
         Returns
         -------
         Np1DIntArray
             The atom indices for the given residue name.
         """
         atom_indices = np.array([], dtype=int)
-        for residue, _atom_indices in zip(self.residues, self.residue_atom_indices):
+        for residue, _atom_indices in zip(self.residues,
+                                          self.residue_atom_indices):
             if residue.name.lower() == residue_name.lower():
                 atom_indices = np.append(atom_indices, _atom_indices)
 
         return atom_indices
 
     def get_atom_indices_from_residue_numbers(
         self,
-        residue_numbers: Np1DIntArray
+        residue_numbers: Np1DIntArray,
     ) -> Np1DIntArray:
         """
         Returns the atom indices for the given residue numbers.
 
         Parameters
         ----------
         residue_numbers : Np1DIntArray
             The residue numbers to get the atom indices for.
 
         Returns
         -------
         Np1DIntArray
             The atom indices for the given residue numbers.
         """
-        return np.argwhere(np.isin(self.residue_numbers,
-            residue_numbers)).flatten()
+        return np.argwhere(np.isin(
+            self.residue_numbers,
+            residue_numbers,
+        )).flatten()
 
-    def _setup_residues(self,
+    def _setup_residues(
+        self,
         residue_ids: Np1DIntArray,
-        atoms: Atoms) -> Tuple[Residues,
-        Atoms]:
+        atoms: Atoms,
+    ) -> Tuple[Residues, Atoms]:
         """
         Sets up the residues of the topology.
 
         It checks if the residue ids are contiguous and compatible with the reference residues.
         If check_residues is False, it does not check the residues and just returns an empty list.
 
         Parameters
@@ -322,16 +330,16 @@
 
         if not np.all(bool_array):
             not_found_residue_ids = np.unique(
                 residue_ids[np.argwhere(~np.array(bool_array))]
             )
             self.logger.error(
                 (
-                f"Residue ids {not_found_residue_ids} "
-                "have no corresponding reference residue."
+                    f"Residue ids {not_found_residue_ids} "
+                    "have no corresponding reference residue."
                 ),
                 exception=ResidueError
             )
 
         atom_counter = 0
         while atom_counter < len(residue_ids):
             if residue_ids[atom_counter] == 0:
@@ -346,41 +354,41 @@
                 else:
                     residues.append(QMResidue(atoms[atom_counter].element))
                     atom_counter += 1
                     continue
 
             residue = _find_residue_by_id(
                 residue_ids[atom_counter],
-                self.reference_residues
+                self.reference_residues,
             )
 
-            residue_element_counter = 0
             for i in np.arange(residue.n_atoms) + atom_counter:
-                if (atoms[i].element != Element() and atoms[i].element
-                        != residue.elements[residue_element_counter]):
+                if (
+                    atoms[i].element != Element() and
+                    atoms[i].element != residue.elements[i - atom_counter]
+                ):
                     self.logger.warning(
                         (
-                        f"The element of atom {i} ({atoms[i].element}) "
-                        "does not match the element of the reference residue "
-                        f"{residue.name} "
-                        f"({residue.elements[residue_element_counter]}). "
-                        "Therefore the element type of the residue "
-                        "description will be used within the topology format!"
+                            f"The element of atom {i} ({atoms[i].element}) "
+                            "does not match the element of the reference residue "
+                            f"{residue.name} "
+                            f"({residue.elements[i - atom_counter]}). "
+                            "Therefore the element type of the residue "
+                            "description will be used within the topology format!"
                         )
                     )
 
-                    atoms[i].element = residue.elements[residue_element_counter
-                                                        ]
+                    atoms[i].element = residue.elements[i - atom_counter]
 
                 if residue_ids[i] != residue_ids[atom_counter]:
                     self.logger.error(
                         (
-                        "The residue ids are not contiguous. Problems with residue "
-                        f"{residue.name} with indices {atom_counter}-"
-                        f"{atom_counter + residue.n_atoms-1}"
+                            "The residue ids are not contiguous. Problems with residue "
+                            f"{residue.name} with indices {atom_counter}-"
+                            f"{atom_counter + residue.n_atoms-1}"
                         ),
                         exception=ResidueError
                     )
 
             residues.append(residue)
 
             atom_counter += residue.n_atoms
@@ -422,15 +430,15 @@
 
     @check_residues.setter
     @runtime_type_checking_setter
     def check_residues(self, value: bool) -> None:
         self._check_residues = value
         self._residues, self._atoms = self._setup_residues(
             self.residue_ids,
-            self.atoms
+            self.atoms,
         )
 
     @property
     def reference_residue_ids(self) -> Np1DIntArray:
         """Np1DIntArray: The residue ids of the reference residues."""
         return np.array([residue.id for residue in self.reference_residues])
 
@@ -475,17 +483,16 @@
         return len(self.residues)
 
     @property
     def n_qm_residues(self) -> int:
         """int: The number of QM residues in the topology."""
         return len(
             [
-            residue for residue in self.residues
-            if isinstance(residue,
-            QMResidue)
+                residue for residue in self.residues
+                if isinstance(residue, QMResidue)
             ]
         )
 
     @property
     def n_mm_residues(self) -> int:
         """int: The number of MM residues in the topology."""
         return self.n_residues - self.n_qm_residues
@@ -501,14 +508,34 @@
         return self._residue_numbers
 
     @property
     def residue_atom_indices(self) -> List[Np1DIntArray]:
         """List[Np1DIntArray]: The residue atom indices of the topology."""
         return self._residue_atom_indices
 
+    @property
+    def n_atoms_per_residue(self) -> Np1DIntArray:
+        """Np1DIntArray: The number of atoms per residue."""
+        return np.array(
+            [len(indices) for indices in self.residue_atom_indices]
+        )
+
+    @property
+    def residue_ids_per_residue(self) -> Np1DIntArray:
+        """List[Np1DIntArray]: The residue ids per residue."""
+        residue_ids_per_residue = []
+
+        if len(self.residue_ids) == 0:
+            return residue_ids_per_residue
+
+        for i in np.cumsum(self.n_atoms_per_residue):
+            residue_ids_per_residue.append(self.residue_ids[i - 1])
+
+        return np.array(residue_ids_per_residue)
+
 
 
 def _find_residue_by_id(res_id: Integral, residues: Residues) -> Residue:
     """
     Finds a residue by its id.
 
     Parameters
@@ -533,22 +560,20 @@
     bool_array = np.array([residue.id == res_id for residue in residues])
 
     residues = np.array(residues)
     residue = residues[np.argwhere(bool_array)].flatten()
 
     if len(residue) > 1:
         Topology.logger.error(
-            f"The residue id {res_id} is not unique.",
-            exception=ResidueError
+            f"The residue id {res_id} is not unique.", exception=ResidueError
         )
 
     if len(residue) == 0:
         Topology.logger.error(
-            f"The residue id {res_id} was not found.",
-            exception=ResidueError
+            f"The residue id {res_id} was not found.", exception=ResidueError
         )
 
     return residue[0]
 
 
 
 def _unique_residues_(residues: Residues) -> Residues:
```

### Comparing `pqanalysis-1.0.2/PQAnalysis/traj/api.py` & `pqanalysis-1.0.3/PQAnalysis/traj/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/traj/exceptions.py` & `pqanalysis-1.0.3/PQAnalysis/traj/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/traj/formats.py` & `pqanalysis-1.0.3/PQAnalysis/traj/formats.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/traj/trajectory.py` & `pqanalysis-1.0.3/PQAnalysis/traj/trajectory.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,18 @@
 from PQAnalysis.topology import Topology
 from PQAnalysis.types import Np2DNumberArray, Np1DNumberArray
 from PQAnalysis.exceptions import PQIndexError, PQTypeError
 from PQAnalysis.core import Cell
 from PQAnalysis.atomic_system import AtomicSystem
 from PQAnalysis.utils.custom_logging import setup_logger
 from PQAnalysis import __package_name__
-from PQAnalysis.type_checking import runtime_type_checking, runtime_type_checking_setter
+from PQAnalysis.type_checking import (
+    runtime_type_checking,
+    runtime_type_checking_setter,
+)
 
 
 
 class Trajectory:
 
     """
     A trajectory object is a sequence of frames.
@@ -32,15 +35,15 @@
     """
 
     logger = logging.getLogger(__package_name__).getChild(__qualname__)
 
     @runtime_type_checking
     def __init__(
         self,
-        frames: List[AtomicSystem] | AtomicSystem | None = None
+        frames: List[AtomicSystem] | AtomicSystem | None = None,
     ) -> None:
         """
         Parameters
         ----------
         frames : AtomicSystem | None, optional
             The list of atomic systems in the trajectory.
             If frames is an AtomicSystem, it is first converted to list of frames.
@@ -276,24 +279,28 @@
             self.logger.error(
                 "window size is greater than the trajectory_stop - trajectory_start",
                 exception=PQIndexError,
             )
 
         # Check if all frames are included in the windows
         # Length of the trajectory - window_size should be divisible by window_gap
-        if ((trajectory_stop - trajectory_start) -
-                window_size) % window_gap != 0:
+        if (
+            ((trajectory_stop - trajectory_start) - window_size) % window_gap
+            != 0
+        ):
             self.logger.warning(
                 "Not all frames are included in the windows. Check the window size and gap."
             )
 
         # generate the window of the trajectory
-        for i in range(trajectory_start,
+        for i in range(
+            trajectory_start,
             trajectory_stop - window_size + 1,
-            window_gap):
+            window_gap,
+        ):
             yield self[i:i + window_size]
 
     @runtime_type_checking
     def __contains__(self, item: AtomicSystem) -> bool:
         """
         This method allows a frame to be checked for membership in a trajectory.
 
@@ -394,7 +401,15 @@
         if len(self.frames) != 0:
             self.frames[0].topology = topology
 
     @property
     def cells(self) -> List[Cell]:
         """List[Cell]: The cells of the trajectory."""
         return [frame.cell for frame in self.frames]
+
+    @property
+    def com_residue_traj(self) -> "Trajectory":
+        """Trajectory: The trajectory with the center of mass of the residues."""
+
+        frames = [frame.center_of_mass_residues for frame in self.frames]
+
+        return Trajectory(frames)
```

### Comparing `pqanalysis-1.0.2/PQAnalysis/type_checking.py` & `pqanalysis-1.0.3/PQAnalysis/type_checking.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/types.py` & `pqanalysis-1.0.3/PQAnalysis/types.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/utils/common.py` & `pqanalysis-1.0.3/PQAnalysis/utils/common.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/utils/custom_logging.py` & `pqanalysis-1.0.3/PQAnalysis/utils/custom_logging.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/utils/decorators.py` & `pqanalysis-1.0.3/PQAnalysis/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/utils/files.py` & `pqanalysis-1.0.3/PQAnalysis/utils/files.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis/utils/random.py` & `pqanalysis-1.0.3/PQAnalysis/utils/random.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/PQAnalysis.egg-info/PKG-INFO` & `pqanalysis-1.0.3/PQAnalysis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PQAnalysis
-Version: 1.0.2
+Version: 1.0.3
 Summary: PQAnalysis is a python package for the analysis of PQ simulations.
 Author-email: Jakob Gamper <97gamjak@gmail.com>, "Josef M. Gallmetzer" <gallmetzer.josef@gmail.com>, "Clarissa A. Seidler" <clarissa.seidler@gmail.com>
 Project-URL: Homepage, https://github.com/MolarVerse/PQAnalysis
 Project-URL: PQ, https://github.com/MolarVerse/PQ
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pqanalysis-1.0.2/PQAnalysis.egg-info/SOURCES.txt` & `pqanalysis-1.0.3/PQAnalysis.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 CODE_OF_CONDUCT.md
 LICENSE
 README.md
 pyproject.toml
 pytest.ini
 pytest.sh
 setup.cfg
-test
 .github/.pylint_cache/PQAnalysis_1.stats
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/scripts/parse_pylint.py
 .github/workflows/ci.yml
 .github/workflows/docs.yml
 .github/workflows/pylint.yml
@@ -153,14 +152,15 @@
 PQAnalysis/utils/custom_logging.py
 PQAnalysis/utils/decorators.py
 PQAnalysis/utils/files.py
 PQAnalysis/utils/random.py
 PQAnalysis/utils/units.py
 benchmarks/pytest.ini
 benchmarks/core/benchmark_cell.py
+benchmarks/core/benchmark_traj_reader.py
 docs/Makefile
 docs/autodoc.sh
 docs/make.bat
 docs/source/conf.py
 docs/source/index.rst
 docs/source/_static/css/custom.css
 docs/source/_templates/module.rst
```

### Comparing `pqanalysis-1.0.2/README.md` & `pqanalysis-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/docs/Makefile` & `pqanalysis-1.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/docs/make.bat` & `pqanalysis-1.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/docs/source/_templates/module.rst` & `pqanalysis-1.0.3/docs/source/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/docs/source/_templates/package.rst` & `pqanalysis-1.0.3/docs/source/_templates/package.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/docs/source/code/PQAnalysis.atomic_system.exceptions.rst` & `pqanalysis-1.0.3/docs/source/code/PQAnalysis.atomic_system.exceptions.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.exceptions.rst` & `pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.exceptions.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.input_file_reader.exceptions.rst` & `pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.input_file_reader.exceptions.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.input_file_reader.input_file_parser.rst` & `pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.input_file_reader.input_file_parser.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.input_file_reader.pq_analysis.pqanalysis_input_file_reader.rst` & `pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.input_file_reader.pq_analysis.pqanalysis_input_file_reader.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.input_file_reader.rst` & `pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.input_file_reader.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.rst` & `pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.topology_file.topology_file_writer.rst` & `pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.topology_file.topology_file_writer.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/docs/source/code/PQAnalysis.io.traj_file.api.rst` & `pqanalysis-1.0.3/docs/source/code/PQAnalysis.io.traj_file.api.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/docs/source/code/PQAnalysis.rst` & `pqanalysis-1.0.3/docs/source/code/PQAnalysis.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/docs/source/code/PQAnalysis.tools.add_molecule.rst` & `pqanalysis-1.0.3/docs/source/code/PQAnalysis.tools.add_molecule.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/docs/source/code/PQAnalysis.topology.api.rst` & `pqanalysis-1.0.3/docs/source/code/PQAnalysis.topology.api.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/docs/source/code/PQAnalysis.utils.custom_logging.rst` & `pqanalysis-1.0.3/docs/source/code/PQAnalysis.utils.custom_logging.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/docs/source/conf.py` & `pqanalysis-1.0.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/docs/source/developerGuide/developerGuide.rst` & `pqanalysis-1.0.3/docs/source/developerGuide/developerGuide.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/docs/source/logo/PQAnalysis.png` & `pqanalysis-1.0.3/docs/source/logo/PQAnalysis.png`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/docs/source/userGuide/inputFile.rst` & `pqanalysis-1.0.3/docs/source/userGuide/inputFile.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/docs/source/userGuide/userGuide.rst` & `pqanalysis-1.0.3/docs/source/userGuide/userGuide.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/examples/traj2box/acof_triclinic.xyz` & `pqanalysis-1.0.3/examples/traj2box/acof_triclinic.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/examples/traj2box/acof_triclinic_2.xyz` & `pqanalysis-1.0.3/examples/traj2box/acof_triclinic_2.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/examples/traj2comtraj/umcm-9-md-01.xyz` & `pqanalysis-1.0.3/examples/traj2comtraj/umcm-9-md-01.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/pyproject.toml` & `pqanalysis-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/analysis/rdf/test_api.py` & `pqanalysis-1.0.3/tests/analysis/rdf/test_api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/analysis/rdf/test_rdf.py` & `pqanalysis-1.0.3/tests/analysis/rdf/test_rdf.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/analysis/rdf/test_rdfInputFileReader.py` & `pqanalysis-1.0.3/tests/analysis/rdf/test_rdfInputFileReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/analysis/rdf/test_rdfOutputFileReader.py` & `pqanalysis-1.0.3/tests/analysis/rdf/test_rdfOutputFileReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/atomicSystem/test_decorators.py` & `pqanalysis-1.0.3/tests/atomicSystem/test_decorators.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/atomicSystem/test_positions.py` & `pqanalysis-1.0.3/tests/atomicSystem/test_positions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/cli/test_continue_input.py` & `pqanalysis-1.0.3/tests/cli/test_continue_input.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/cli/test_rst2xyz.py` & `pqanalysis-1.0.3/tests/cli/test_rst2xyz.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/cli/test_traj2box.py` & `pqanalysis-1.0.3/tests/cli/test_traj2box.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/cli/test_traj2qmcfc.py` & `pqanalysis-1.0.3/tests/cli/test_traj2qmcfc.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/conftest.py` & `pqanalysis-1.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/core/atom/test_atom.py` & `pqanalysis-1.0.3/tests/core/atom/test_atom.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,17 +54,15 @@
             'C1'
         )
 
         assert_logging_with_exception(
             caplog,
             "TypeChecking",
             "ERROR",
-            get_type_error_message("name",
-            1.2,
-            str | int),
+            get_type_error_message("name", 1.2, str | int | Element),
             PQTypeError,
             Atom,
             1.2
         )
 
         assert_logging_with_exception(
             caplog,
```

### Comparing `pqanalysis-1.0.2/tests/core/atom/test_element.py` & `pqanalysis-1.0.3/tests/core/atom/test_element.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/core/test_cell.py` & `pqanalysis-1.0.3/tests/core/test_cell.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/core/test_residue.py` & `pqanalysis-1.0.3/tests/core/test_residue.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/data/inputFileReader/PQ_input/n_not_matching.in` & `pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/n_not_matching.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/data/inputFileReader/PQ_input/n_not_matching_input_file_n-08.in` & `pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/n_not_matching_input_file_n-08.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/data/inputFileReader/PQ_input/no_output_files.in` & `pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/no_output_files.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/data/inputFileReader/PQ_input/no_start_file.in` & `pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/no_start_file.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/data/inputFileReader/PQ_input/old_n_not_less_one_than_actual_n-09.in` & `pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/old_n_not_less_one_than_actual_n-09.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/data/inputFileReader/PQ_input/run-08.in` & `pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/run-08.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/data/inputFileReader/PQ_input/run-08.rpmd.in` & `pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/run-08.rpmd.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/data/inputFileReader/PQ_input/run-09.in.ref` & `pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/run-09.in.ref`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/data/inputFileReader/PQ_input/run-09.rpmd.in.ref` & `pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/run-09.rpmd.in.ref`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/data/inputFileReader/PQ_input/run-10.in.ref` & `pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/run-10.in.ref`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/data/inputFileReader/PQ_input/run-10.rpmd.in.ref` & `pqanalysis-1.0.3/tests/data/inputFileReader/PQ_input/run-10.rpmd.in.ref`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/data/readEnergyFile/md-01.info` & `pqanalysis-1.0.3/tests/data/readEnergyFile/md-01.info`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/data/readInfoFile/md-01.info` & `pqanalysis-1.0.3/tests/data/readInfoFile/md-01.info`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/data/readInfoFile/md-01.qmcfc.info` & `pqanalysis-1.0.3/tests/data/readInfoFile/md-01.qmcfc.info`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/data/traj2qmcfc/acof_triclinic.xyz` & `pqanalysis-1.0.3/tests/data/traj2qmcfc/acof_triclinic.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/data/traj2qmcfc/acof_triclinic_2.xyz` & `pqanalysis-1.0.3/tests/data/traj2qmcfc/acof_triclinic_2.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/data/traj2qmcfc/traj.qmcfc.xyz` & `pqanalysis-1.0.3/tests/data/traj2qmcfc/traj.qmcfc.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/io/inputFileReader/PQ/test_PQ_inputFileReader.py` & `pqanalysis-1.0.3/tests/io/inputFileReader/PQ/test_PQ_inputFileReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/io/inputFileReader/PQAnalysis/test_parse.py` & `pqanalysis-1.0.3/tests/io/inputFileReader/PQAnalysis/test_parse.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/io/inputFileReader/test_inputDictionary.py` & `pqanalysis-1.0.3/tests/io/inputFileReader/test_inputDictionary.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/io/inputFileReader/test_inputFileParser.py` & `pqanalysis-1.0.3/tests/io/inputFileReader/test_inputFileParser.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/io/inputFileReader/test_transformers.py` & `pqanalysis-1.0.3/tests/io/inputFileReader/test_transformers.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/io/inputFileReader/test_visitors.py` & `pqanalysis-1.0.3/tests/io/inputFileReader/test_visitors.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/io/test_base.py` & `pqanalysis-1.0.3/tests/io/test_base.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/io/test_boxWriter.py` & `pqanalysis-1.0.3/tests/io/test_boxWriter.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/io/test_energyFileReader.py` & `pqanalysis-1.0.3/tests/io/test_energyFileReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/io/test_frameReader.py` & `pqanalysis-1.0.3/tests/io/test_frameReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/io/test_infoFileReader.py` & `pqanalysis-1.0.3/tests/io/test_infoFileReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/io/test_moldescriptorReader.py` & `pqanalysis-1.0.3/tests/io/test_moldescriptorReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/io/test_restartReader.py` & `pqanalysis-1.0.3/tests/io/test_restartReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/io/test_restartWriter.py` & `pqanalysis-1.0.3/tests/io/test_restartWriter.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/io/test_trajectoryReader.py` & `pqanalysis-1.0.3/tests/io/test_trajectoryReader.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,30 +53,20 @@
         print(traj[1].topology.atoms)
         # traj[] can also return an AtomicSystem
         print(traj[0].cell)  # pylint: disable=no-member
         print(traj[1].cell)  # pylint: disable=no-member
 
         frame1 = AtomicSystem(
             atoms=atoms,
-            pos=np.array([[0.0,
-            0.0,
-            0.0],
-            [0.0,
-            1.0,
-            0.0]]),
+            pos=np.array([[0.0, 0.0, 0.0], [0.0, 1.0, 0.0]]),
             cell=cell
         )
         frame2 = AtomicSystem(
             atoms=atoms,
-            pos=np.array([[1.0,
-            0.0,
-            0.0],
-            [0.0,
-            1.0,
-            1.0]]),
+            pos=np.array([[1.0, 0.0, 0.0], [0.0, 1.0, 1.0]]),
             cell=cell
         )
 
         assert traj[0] == frame1
         # NOTE: here cell is not none because of the consecutive reading of frames
         # Cell will be taken from the previous frame
         assert traj[1] == frame2
@@ -141,44 +131,34 @@
         reader = TrajectoryReader("tmp.xyz")
 
         cell = Cell(1.0, 1.0, 1.0)
         atoms = [Atom(atom) for atom in ["h", "o"]]
 
         frame1 = AtomicSystem(
             atoms=atoms,
-            pos=np.array([[0.0,
-            0.0,
-            0.0],
-            [0.0,
-            1.0,
-            0.0]]),
+            pos=np.array([[0.0, 0.0, 0.0], [0.0, 1.0, 0.0]]),
             cell=cell
         )
         frame2 = AtomicSystem(
             atoms=atoms,
-            pos=np.array([[1.0,
-            0.0,
-            0.0],
-            [0.0,
-            1.0,
-            1.0]]),
+            pos=np.array([[1.0, 0.0, 0.0], [0.0, 1.0, 1.0]]),
             cell=cell
         )
 
         test_frames = [frame for frame in reader.frame_generator()]
         assert test_frames == [frame1, frame2]
 
         reader = TrajectoryReader(["tmp.xyz", "tmp.xyz"])
 
         test_frames = [frame for frame in reader.frame_generator()]
         assert test_frames == [frame1, frame2, frame1, frame2]
 
         # vacuum cell
         file = open("tmp2.xyz", "w")
-        print("2", file=file)
+        print("2 1.0 1.0 1.0", file=file)
         print("", file=file)
         print("h 0.0 0.0 0.0", file=file)
         print("o 0.0 1.0 0.0", file=file)
         print("2", file=file)
         print("", file=file)
         print("h 1.0 0.0 0.0", file=file)
         print("o 0.0 1.0 1.0", file=file)
@@ -195,14 +175,24 @@
         assert test_frames == [frame2, frame1, frame2]
 
         test_frames = [
             frame for frame in reader.frame_generator(trajectory_stop=3)
         ]
         assert test_frames == [frame1, frame2, frame1]
 
+        test_frames = [
+            frame for frame in reader.frame_generator(trajectory_start=2)
+        ]
+        assert test_frames == [frame1, frame2]
+
+        test_frames = [
+            frame for frame in reader.frame_generator(trajectory_stop=2)
+        ]
+        assert test_frames == [frame1, frame2]
+
         # Check file change after setting the reader
         file = open("tmp2.xyz", "w")
         print("2 1.0 1.0 1.0", file=file)
         print("", file=file)
         print("h 0.0 0.0 0.0", file=file)
         print("o 0.0 1.0 0.0", file=file)
         file.close()
@@ -226,41 +216,40 @@
 
         assert_logging_with_exception(
             caplog,
             TrajectoryReader.__qualname__,
             exception=PQIndexError,
             logging_level="ERROR",
             message_to_test=(
-            "start index is less than 0 or greater than the length of the trajectory"
+                "start index is less than 0 or greater than the length of the trajectory"
             ),
             function=reader.frame_generator(trajectory_start=-1).__next__,
         )
 
         assert_logging_with_exception(
             caplog,
             TrajectoryReader.__qualname__,
             exception=PQIndexError,
             logging_level="ERROR",
             message_to_test=(
-            "stop index is less than 0 or greater than the length of the trajectory"
+                "stop index is less than 0 or greater than the length of the trajectory"
             ),
             function=reader.frame_generator(trajectory_stop=-1).__next__,
         )
 
         assert_logging_with_exception(
             caplog,
             TrajectoryReader.__qualname__,
             exception=PQIndexError,
             logging_level="ERROR",
             message_to_test=(
-            "start index is greater than or equal to the stop index"
+                "start index is greater than or equal to the stop index"
             ),
             function=reader.frame_generator(
-            trajectory_start=1,
-            trajectory_stop=1
+                trajectory_start=1, trajectory_stop=1
             ).__next__,
         )
 
     # -------------------------------------------------------------------------------- #
 
     @pytest.mark.usefixtures("tmpdir")
     def test_window_generator(self, caplog):
@@ -279,74 +268,77 @@
         reader = TrajectoryReader(filenames)
 
         cell = Cell(1.0, 1.0, 1.0)
         atoms = [Atom(atom) for atom in ["h", "o"]]
 
         frame1 = AtomicSystem(
             atoms=atoms,
-            pos=np.array([[0.0,
-            0.0,
-            0.0],
-            [0.0,
-            1.0,
-            0.0]]),
+            pos=np.array([[0.0, 0.0, 0.0], [0.0, 1.0, 0.0]]),
             cell=cell
         )
         frame2 = AtomicSystem(
             atoms=atoms,
-            pos=np.array([[1.0,
-            0.0,
-            0.0],
-            [0.0,
-            1.0,
-            1.0]]),
+            pos=np.array([[1.0, 0.0, 0.0], [0.0, 1.0, 1.0]]),
             cell=cell
         )
 
         test_frames = list(reader.window_generator(window_size=1))
         assert test_frames == [
             Trajectory([frame1]),
             Trajectory([frame2]),
             Trajectory([frame1]),
             Trajectory([frame2]),
         ]
 
         test_frames = list(reader.window_generator(window_size=2))
         assert test_frames == [
-            Trajectory([frame1,
-            frame2]),
-            Trajectory([frame2,
-            frame1]),
-            Trajectory([frame1,
-            frame2]),
+            Trajectory([frame1, frame2]),
+            Trajectory([frame2, frame1]),
+            Trajectory([frame1, frame2]),
         ]
 
         test_frames = list(reader.window_generator(window_size=4))
         assert test_frames == [Trajectory([frame1, frame2, frame1, frame2])]
 
         test_frames = list(
-            reader.window_generator(window_size=2,
-            window_gap=2)
+            reader.window_generator(window_size=2, window_gap=2)
         )
         assert test_frames == [
-            Trajectory([frame1,
-            frame2]),
-            Trajectory([frame1,
-            frame2]),
+            Trajectory([frame1, frame2]),
+            Trajectory([frame1, frame2]),
         ]
 
         test_frames = list(
             reader.window_generator(
-            window_size=2,
-            window_gap=1,
-            trajectory_start=1,
-            trajectory_stop=3
+                window_size=2,
+                window_gap=1,
+                trajectory_start=1,
+                trajectory_stop=3
             )
         )
         assert test_frames == [Trajectory([frame2, frame1])]
+        test_frames = list(
+            reader.window_generator(
+                window_size=2,
+                window_gap=1,
+                trajectory_start=2,
+                trajectory_stop=4
+            )
+        )
+        assert test_frames == [Trajectory([frame1, frame2])]
+
+        filenames = ["tmp.xyz", "tmp.xyz", "tmp.xyz"]
+        reader = TrajectoryReader(filenames)
+
+        test_frames = list(
+            reader.window_generator(
+                window_size=2, window_gap=1, trajectory_stop=2
+            )
+        )
+        assert test_frames == [Trajectory([frame1, frame2])]
 
         # Test file change after setting the reader
         file = open("tmp.xyz", "w")
         print("2 1.0 1.0 1.0", file=file)
         print("", file=file)
         print("h 0.0 0.0 0.0", file=file)
         print("o 0.0 1.0 0.0", file=file)
@@ -356,14 +348,17 @@
         print("o 0.0 1.0 1.0", file=file)
         print("2", file=file)
         print("", file=file)
         print("h 0.0 0.0 0.0", file=file)
         print("o 0.0 1.0 0.0", file=file)
         file.close()
 
+        filenames = ["tmp.xyz", "tmp.xyz"]
+        reader = TrajectoryReader(filenames)
+
         test_frames = list(reader.window_generator(1))
         assert test_frames == [
             Trajectory([frame1]),
             Trajectory([frame2]),
             Trajectory([frame1]),
             Trajectory([frame1]),
             Trajectory([frame2]),
@@ -383,174 +378,154 @@
         file.close()
 
         assert_logging(
             caplog,
             TrajectoryReader.__qualname__,
             "WARNING",
             "Not all frames are included in the windows. Check the window size and gap.",
-            reader.window_generator(1,
-            2).__next__,
+            reader.window_generator(1, 2).__next__,
         )
 
         assert_logging_with_exception(
             caplog,
             TrajectoryReader.__qualname__,
             exception=PQIndexError,
             logging_level="ERROR",
             message_to_test=(
-            "window size can not be less than 1 or greater than the length of the trajectory"
+                "window size can not be less than 1 or greater than the length of the trajectory"
             ),
             function=reader.window_generator(0).__next__,
         )
 
         assert_logging_with_exception(
             caplog,
             TrajectoryReader.__qualname__,
             exception=PQIndexError,
             logging_level="ERROR",
             message_to_test=(
-            "window size can not be less than 1 or greater than the length of the trajectory"
+                "window size can not be less than 1 or greater than the length of the trajectory"
             ),
             function=reader.window_generator(5).__next__,
         )
 
         assert_logging_with_exception(
             caplog,
             TrajectoryReader.__qualname__,
             exception=PQIndexError,
             logging_level="ERROR",
             message_to_test=(
-            "window gap can not be less than 1 or greater than the length of the trajectory"
+                "window gap can not be less than 1 or greater than the length of the trajectory"
             ),
-            function=reader.window_generator(3,
-            0).__next__,
+            function=reader.window_generator(3, 0).__next__,
         )
 
         assert_logging_with_exception(
             caplog,
             TrajectoryReader.__qualname__,
             exception=PQIndexError,
             logging_level="ERROR",
             message_to_test=(
-            "window gap can not be less than 1 or greater than the length of the trajectory"
+                "window gap can not be less than 1 or greater than the length of the trajectory"
             ),
-            function=reader.window_generator(3,
-            5).__next__,
+            function=reader.window_generator(3, 5).__next__,
         )
 
         assert_logging_with_exception(
             caplog,
             TrajectoryReader.__qualname__,
             exception=PQIndexError,
             logging_level="ERROR",
             message_to_test=(
-            "start index is less than 0 or greater than the length of the trajectory"
+                "start index is less than 0 or greater than the length of the trajectory"
             ),
-            function=reader.window_generator(1,
-            1,
-            trajectory_start=-1).__next__,
+            function=reader.window_generator(1, 1,
+                                             trajectory_start=-1).__next__,
         )
 
         assert_logging_with_exception(
             caplog,
             TrajectoryReader.__qualname__,
             exception=PQIndexError,
             logging_level="ERROR",
             message_to_test=(
-            "start index is less than 0 or greater than the length of the trajectory"
+                "start index is less than 0 or greater than the length of the trajectory"
             ),
             function=reader.window_generator(
-            1,
-            1,
-            trajectory_start=5,
-            trajectory_stop=6
+                1, 1, trajectory_start=5, trajectory_stop=6
             ).__next__,
         )
 
         assert_logging_with_exception(
             caplog,
             TrajectoryReader.__qualname__,
             exception=PQIndexError,
             logging_level="ERROR",
             message_to_test=(
-            "stop index is less than 0 or greater than the length of the trajectory"
+                "stop index is less than 0 or greater than the length of the trajectory"
             ),
-            function=reader.window_generator(1,
-            1,
-            trajectory_stop=-1).__next__,
+            function=reader.window_generator(1, 1,
+                                             trajectory_stop=-1).__next__,
         )
 
         assert_logging_with_exception(
             caplog,
             TrajectoryReader.__qualname__,
             exception=PQIndexError,
             logging_level="ERROR",
             message_to_test=(
-            "stop index is less than 0 or greater than the length of the trajectory"
+                "stop index is less than 0 or greater than the length of the trajectory"
             ),
             function=reader.window_generator(
-            1,
-            1,
-            trajectory_start=0,
-            trajectory_stop=6
+                1, 1, trajectory_start=0, trajectory_stop=6
             ).__next__,
         )
 
         assert_logging_with_exception(
             caplog,
             TrajectoryReader.__qualname__,
             exception=PQIndexError,
             logging_level="ERROR",
             message_to_test=(
-            "start index is greater than or equal to the stop index"
+                "start index is greater than or equal to the stop index"
             ),
             function=reader.window_generator(
-            1,
-            1,
-            trajectory_start=1,
-            trajectory_stop=0
+                1, 1, trajectory_start=1, trajectory_stop=0
             ).__next__,
         )
 
         assert_logging_with_exception(
             caplog,
             TrajectoryReader.__qualname__,
             exception=PQIndexError,
             logging_level="ERROR",
             message_to_test=(
-            "start index is greater than or equal to the stop index"
+                "start index is greater than or equal to the stop index"
             ),
             function=reader.window_generator(
-            1,
-            1,
-            trajectory_start=1,
-            trajectory_stop=1
+                1, 1, trajectory_start=1, trajectory_stop=1
             ).__next__,
         )
 
         assert_logging_with_exception(
             caplog,
             TrajectoryReader.__qualname__,
             exception=PQIndexError,
             logging_level="ERROR",
             message_to_test=(
-            "window size is greater than the trajectory_stop - trajectory_start"
+                "window size is greater than the trajectory_stop - trajectory_start"
             ),
             function=reader.window_generator(
-            4,
-            1,
-            trajectory_start=0,
-            trajectory_stop=2
+                4, 1, trajectory_start=0, trajectory_stop=2
             ).__next__,
         )
 
     # -------------------------------------------------------------------------------- #
 
     @pytest.mark.usefixtures("tmpdir")
-    def test_calculate_number_of_frames(self, caplog):
+    def test_calculate_number_of_frames_per_file(self, caplog):
         file = open("tmp.xyz", "w")
         print("2 1.0 1.0 1.0", file=file)
         print("", file=file)
         print("h 0.0 0.0 0.0", file=file)
         print("o 0.0 1.0 0.0", file=file)
         print("2", file=file)
         print("", file=file)
@@ -560,15 +535,15 @@
 
         file = open("tmp2.xyz", "w")
         file.close()
 
         filenames = ["tmp.xyz", "tmp2.xyz"]
         reader = TrajectoryReader(filenames)
 
-        assert reader.calculate_number_of_frames() == 2
+        assert sum(reader.calculate_number_of_frames_per_file()) == 2
 
         file = open("tmp2.xyz", "w")
         print("str 1.0 1.0 1.0", file=file)
         print("", file=file)
         print("h 0.0 0.0 0.0", file=file)
         print("o 0.0 1.0 0.0", file=file)
         print("2", file=file)
@@ -581,17 +556,17 @@
 
         assert_logging_with_exception(
             caplog,
             TrajectoryReader.__qualname__,
             exception=TrajectoryReaderError,
             logging_level="ERROR",
             message_to_test=(
-            "Invalid number of atoms in the first line of file tmp2.xyz."
+                "Invalid number of atoms in the first line of file tmp2.xyz."
             ),
-            function=reader.calculate_number_of_frames,
+            function=reader.calculate_number_of_frames_per_file,
         )
 
         file = open("tmp2.xyz", "w")
         print("", file=file)
         print("", file=file)
         print("h 0.0 0.0 0.0", file=file)
         print("o 0.0 1.0 0.0", file=file)
@@ -604,17 +579,17 @@
 
         assert_logging_with_exception(
             caplog,
             TrajectoryReader.__qualname__,
             exception=TrajectoryReaderError,
             logging_level="ERROR",
             message_to_test=(
-            "Invalid number of atoms in the first line of file tmp2.xyz."
+                "Invalid number of atoms in the first line of file tmp2.xyz."
             ),
-            function=reader.calculate_number_of_frames,
+            function=reader.calculate_number_of_frames_per_file,
         )
 
         file = open("tmp2.xyz", "w")
         print("2", file=file)
         print("", file=file)
         print("h 0.0 0.0 0.0", file=file)
         print("o 0.0 1.0 0.0", file=file)
@@ -627,18 +602,18 @@
 
         assert_logging_with_exception(
             caplog,
             TrajectoryReader.__qualname__,
             exception=TrajectoryReaderError,
             logging_level="ERROR",
             message_to_test=(
-            "The number of lines in the file is not divisible "
-            "by the number of atoms 2 in the first line."
+                "The number of lines in the file is not divisible "
+                "by the number of atoms 2 in the first line."
             ),
-            function=reader.calculate_number_of_frames,
+            function=reader.calculate_number_of_frames_per_file,
         )
 
     # -------------------------------------------------------------------------------- #
     @pytest.mark.usefixtures("tmpdir")
     def test_cells(self, caplog):
         file = open("tmp.xyz", "w")
         print("2", file=file)
@@ -725,12 +700,12 @@
 
         assert_logging_with_exception(
             caplog,
             TrajectoryReader.__qualname__,
             exception=TrajectoryReaderError,
             logging_level="ERROR",
             message_to_test=(
-            "Invalid number of arguments for box: 8 encountered "
-            "in file tmp.xyz:1 = 2 1.0 1.0 1.0 90.0 90.0 90.0 0.0"
+                "Invalid number of arguments for box: 8 encountered "
+                "in file tmp.xyz:1 = 2 1.0 1.0 1.0 90.0 90.0 90.0 0.0"
             ),
             function=reader._cell_generator().__next__,
         )
```

### Comparing `pqanalysis-1.0.2/tests/io/test_trajectoryWriter.py` & `pqanalysis-1.0.3/tests/io/test_trajectoryWriter.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/io/test_write_api.py` & `pqanalysis-1.0.3/tests/io/test_write_api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/physicalData/test_energy.py` & `pqanalysis-1.0.3/tests/physicalData/test_energy.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/tools/test_traj_to_com_traj.py` & `pqanalysis-1.0.3/tests/tools/test_traj_to_com_traj.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/topology/bonded_topology/test_angle.py` & `pqanalysis-1.0.3/tests/topology/bonded_topology/test_angle.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/topology/bonded_topology/test_bond.py` & `pqanalysis-1.0.3/tests/topology/bonded_topology/test_bond.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/topology/bonded_topology/test_bondedTopology.py` & `pqanalysis-1.0.3/tests/topology/bonded_topology/test_bondedTopology.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/topology/bonded_topology/test_dihedral.py` & `pqanalysis-1.0.3/tests/topology/bonded_topology/test_dihedral.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/topology/test_selection.py` & `pqanalysis-1.0.3/tests/topology/test_selection.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/topology/test_selectionTransformer.py` & `pqanalysis-1.0.3/tests/topology/test_selectionTransformer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/topology/test_shakeTopology.py` & `pqanalysis-1.0.3/tests/topology/test_shakeTopology.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/topology/test_topology.py` & `pqanalysis-1.0.3/tests/topology/test_topology.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/traj/test_api.py` & `pqanalysis-1.0.3/tests/traj/test_api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/traj/test_trajectory.py` & `pqanalysis-1.0.3/tests/traj/test_trajectory.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,29 +47,21 @@
 
     def test_check_PBC(self):
         traj = Trajectory(self.frames)
         assert traj.check_pbc() == False
 
         system1 = AtomicSystem(
             atoms=self.atoms1,
-            pos=np.array([[0,
-            1,
-            2]]),
-            cell=Cell(10,
-            10,
-            10)
+            pos=np.array([[0, 1, 2]]),
+            cell=Cell(10, 10, 10)
         )
         system2 = AtomicSystem(
             atoms=self.atoms2,
-            pos=np.array([[1,
-            1,
-            2]]),
-            cell=Cell(10,
-            10,
-            10)
+            pos=np.array([[1, 1, 2]]),
+            cell=Cell(10, 10, 10)
         )
         frame1 = system1
         frame2 = system2
         frames = [frame1, frame2]
 
         traj = Trajectory(frames)
         assert traj.check_pbc() == True
@@ -87,29 +79,21 @@
 
     def test_check_vacuum(self):
         traj = Trajectory(self.frames)
         assert traj.check_vacuum() == True
 
         system1 = AtomicSystem(
             atoms=self.atoms1,
-            pos=np.array([[0,
-            1,
-            2]]),
-            cell=Cell(10,
-            10,
-            10)
+            pos=np.array([[0, 1, 2]]),
+            cell=Cell(10, 10, 10)
         )
         system2 = AtomicSystem(
             atoms=self.atoms2,
-            pos=np.array([[1,
-            1,
-            2]]),
-            cell=Cell(10,
-            10,
-            10)
+            pos=np.array([[1, 1, 2]]),
+            cell=Cell(10, 10, 10)
         )
         frame1 = system1
         frame2 = system2
         frames = [frame1, frame2]
 
         traj = Trajectory(frames)
         assert traj.check_vacuum() == False
@@ -126,29 +110,21 @@
         traj = Trajectory(self.frames)
         assert traj.box_volumes[0] > 10**10
         assert traj.box_volumes[1] > 10**10
         assert traj.box_volumes[2] > 10**10
 
         system1 = AtomicSystem(
             atoms=self.atoms1,
-            pos=np.array([[0,
-            1,
-            2]]),
-            cell=Cell(10,
-            10,
-            10)
+            pos=np.array([[0, 1, 2]]),
+            cell=Cell(10, 10, 10)
         )
         system2 = AtomicSystem(
             atoms=self.atoms2,
-            pos=np.array([[1,
-            1,
-            2]]),
-            cell=Cell(11,
-            11,
-            11)
+            pos=np.array([[1, 1, 2]]),
+            cell=Cell(11, 11, 11)
         )
         frame1 = system1
         frame2 = system2
         frames = [frame1, frame2]
 
         traj = Trajectory(frames)
         assert np.allclose(traj.box_volumes, np.array([1000, 11 * 11 * 11]))
@@ -179,141 +155,124 @@
         traj = Trajectory(self.frames)
 
         test_frames = [traj.frames for traj in traj.window(1, 2)]
         assert test_frames == [[self.frame1], [self.frame3]]
 
         test_frames = [traj.frames for traj in traj.window(2, 1)]
         assert test_frames == [
-            [self.frame1,
-            self.frame2],
-            [self.frame2,
-            self.frame3]
+            [self.frame1, self.frame2], [self.frame2, self.frame3]
         ]
 
         test_frames = [traj.frames for traj in traj.window(2)]
         assert test_frames == [
-            [self.frame1,
-            self.frame2],
-            [self.frame2,
-            self.frame3]
+            [self.frame1, self.frame2], [self.frame2, self.frame3]
         ]
 
         test_frames = [traj.frames for traj in traj.window(1)]
         assert test_frames == [[self.frame1], [self.frame2], [self.frame3]]
 
         test_frames = [traj.frames for traj in traj.window(2, 2)]
         assert test_frames == [[self.frame1, self.frame2]]
 
         assert_logging(
             caplog,
             Trajectory.__qualname__,
             "WARNING",
             "Not all frames are included in the windows. Check the window size and gap.",
-            traj.window(2,
-            2).__next__,
+            traj.window(2, 2).__next__,
         )
 
         assert_logging_with_exception(
             caplog,
             Trajectory.__qualname__,
             exception=PQIndexError,
             logging_level="ERROR",
             message_to_test=(
-            "window size can not be less than 1 or greater than the length of the trajectory"
+                "window size can not be less than 1 or greater than the length of the trajectory"
             ),
             function=traj.window(0).__next__,
         )
 
         assert_logging_with_exception(
             caplog,
             Trajectory.__qualname__,
             exception=PQIndexError,
             logging_level="ERROR",
             message_to_test=(
-            "window size can not be less than 1 or greater than the length of the trajectory"
+                "window size can not be less than 1 or greater than the length of the trajectory"
             ),
             function=traj.window(4).__next__,
         )
 
         assert_logging_with_exception(
             caplog,
             Trajectory.__qualname__,
             exception=PQIndexError,
             logging_level="ERROR",
             message_to_test=(
-            "window gap can not be less than 1 or greater than the length of the trajectory"
+                "window gap can not be less than 1 or greater than the length of the trajectory"
             ),
-            function=traj.window(1,
-            0).__next__,
+            function=traj.window(1, 0).__next__,
         )
 
         assert_logging_with_exception(
             caplog,
             Trajectory.__qualname__,
             exception=PQIndexError,
             logging_level="ERROR",
             message_to_test=(
-            "window gap can not be less than 1 or greater than the length of the trajectory"
+                "window gap can not be less than 1 or greater than the length of the trajectory"
             ),
-            function=traj.window(1,
-            4).__next__,
+            function=traj.window(1, 4).__next__,
         )
 
         assert_logging_with_exception(
             caplog,
             Trajectory.__qualname__,
             exception=PQIndexError,
             logging_level="ERROR",
             message_to_test=(
-            "start index is less than 0 or greater than the length of the trajectory"
+                "start index is less than 0 or greater than the length of the trajectory"
             ),
-            function=traj.window(1,
-            1,
-            trajectory_start=-1).__next__,
+            function=traj.window(1, 1, trajectory_start=-1).__next__,
         )
 
         assert_logging_with_exception(
             caplog,
             Trajectory.__qualname__,
             exception=PQIndexError,
             logging_level="ERROR",
             message_to_test=(
-            "stop index is less than 0 or greater than the length of the trajectory"
+                "stop index is less than 0 or greater than the length of the trajectory"
             ),
-            function=traj.window(1,
-            1,
-            trajectory_stop=-1).__next__,
+            function=traj.window(1, 1, trajectory_stop=-1).__next__,
         )
 
         assert_logging_with_exception(
             caplog,
             Trajectory.__qualname__,
             exception=PQIndexError,
             logging_level="ERROR",
             message_to_test=(
-            "start index is greater than or equal to the stop index"
+                "start index is greater than or equal to the stop index"
             ),
-            function=traj.window(1,
-            1,
-            trajectory_start=2,
-            trajectory_stop=1).__next__,
+            function=traj.window(1, 1, trajectory_start=2,
+                                 trajectory_stop=1).__next__,
         )
 
         assert_logging_with_exception(
             caplog,
             Trajectory.__qualname__,
             exception=PQIndexError,
             logging_level="ERROR",
             message_to_test=(
-            "window size is greater than the trajectory_stop - trajectory_start"
+                "window size is greater than the trajectory_stop - trajectory_start"
             ),
-            function=traj.window(3,
-            1,
-            trajectory_start=1,
-            trajectory_stop=3).__next__,
+            function=traj.window(3, 1, trajectory_start=1,
+                                 trajectory_stop=3).__next__,
         )
 
     def test__iter__(self):
         traj = Trajectory(self.frames)
         assert [frame for frame in traj] == self.frames
 
         assert [frame for frame in Trajectory()] == []
@@ -390,37 +349,27 @@
 
         max_float = sys.float_info.max
 
         traj = Trajectory([frame1, frame2])
         assert np.allclose(
             traj.box_lengths,
             np.array(
-            [
-            [max_float,
-            max_float,
-            max_float],
-            [max_float,
-            max_float,
-            max_float]
-            ]
+                [
+                    [max_float, max_float, max_float],
+                    [max_float, max_float, max_float]
+                ]
             ),
         )
 
         frame1 = AtomicSystem(cell=Cell(10, 10, 10))
         frame2 = AtomicSystem(cell=Cell(11, 11, 11))
 
         traj = Trajectory([frame1, frame2])
         assert np.allclose(
-            traj.box_lengths,
-            np.array([[10,
-            10,
-            10],
-            [11,
-            11,
-            11]])
+            traj.box_lengths, np.array([[10, 10, 10], [11, 11, 11]])
         )
 
     def test_property_cells(self):
         frame1 = AtomicSystem()
         frame2 = AtomicSystem()
 
         traj = Trajectory([frame1, frame2])
@@ -436,7 +385,20 @@
 
     def test_str_repr(self):
         traj = Trajectory(self.frames)
         assert str(traj) == "Trajectory with 3 frames"
         assert repr(traj) == "Trajectory with 3 frames"
         assert str(Trajectory()) == "Trajectory with 0 frames"
         assert repr(Trajectory()) == "Trajectory with 0 frames"
+
+    def test_com_residue_traj(self):
+        traj = Trajectory(self.frames)
+        assert traj.com_residue_traj == Trajectory(
+            [
+                self.system1.center_of_mass_residues,
+                self.system2.center_of_mass_residues,
+                self.system3.center_of_mass_residues
+            ]
+        )
+
+        traj = Trajectory()
+        assert traj.com_residue_traj == Trajectory()
```

### Comparing `pqanalysis-1.0.2/tests/utils/test_common.py` & `pqanalysis-1.0.3/tests/utils/test_common.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.2/tests/utils/test_decorators.py` & `pqanalysis-1.0.3/tests/utils/test_decorators.py`

 * *Files identical despite different names*

