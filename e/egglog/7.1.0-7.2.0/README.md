# Comparing `tmp/egglog-7.1.0.tar.gz` & `tmp/egglog-7.2.0.tar.gz`

## Comparing `egglog-7.1.0.tar` & `egglog-7.2.0.tar`

### file list

```diff
@@ -1,115 +1,116 @@
--rw-r--r--   0        0        0     1356 1970-01-01 00:00:00.000000 egglog-7.1.0/Cargo.toml
--rw-r--r--   0     1001      127      640 2024-05-03 20:47:31.000000 egglog-7.1.0/.github/dependabot.yml
--rw-r--r--   0     1001      127     2147 2024-05-03 20:47:31.000000 egglog-7.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      127     3872 2024-05-03 20:47:31.000000 egglog-7.1.0/.github/workflows/version.yml
--rw-r--r--   0     1001      127      776 2024-05-03 20:47:31.000000 egglog-7.1.0/.gitignore
--rw-r--r--   0     1001      127     1000 2024-05-03 20:47:31.000000 egglog-7.1.0/.pre-commit-config.yaml
--rw-r--r--   0     1001      127      825 2024-05-03 20:47:31.000000 egglog-7.1.0/.readthedocs.yaml
--rw-r--r--   0     1001      127     1438 2024-05-03 20:47:31.000000 egglog-7.1.0/CITATION.cff
--rw-r--r--   0     1001      127     1070 2024-05-03 20:47:31.000000 egglog-7.1.0/LICENSE
--rw-r--r--   0     1001      127     1417 2024-05-03 20:47:31.000000 egglog-7.1.0/README.md
--rw-r--r--   0     1001      127      388 2024-05-03 20:47:31.000000 egglog-7.1.0/conftest.py
--rw-r--r--   0     1001      127       71 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/.gitignore
--rw-r--r--   0     1001      127      484 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/_templates/comments.html
--rw-r--r--   0     1001      127    14715 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/changelog.md
--rw-r--r--   0     1001      127     5603 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/conf.py
--rw-r--r--   0     1001      127      149 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/environment.yml
--rw-r--r--   0     1001      127       13 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/.gitignore
--rw-r--r--   0     1001      127  1093641 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/2023_07_presentation.ipynb
--rw-r--r--   0     1001      127   114752 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/2023_11_09_portland_state.ipynb
--rw-r--r--   0     1001      127   260924 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/2023_11_17_pytensor.ipynb
--rw-r--r--   0     1001      127   789680 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/2023_11_pydata_lightning_talk.ipynb
--rw-r--r--   0     1001      127    72312 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/2023_12_02_congruence_closure-1.png
--rw-r--r--   0     1001      127   193296 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/2023_12_02_congruence_closure-2.png
--rw-r--r--   0     1001      127     8470 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/2023_12_02_congruence_closure.md
--rw-r--r--   0     1001      127  1048406 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/2024_03_17_community_talk.ipynb
--rw-r--r--   0     1001      127   288149 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/2024_03_17_map.svg
--rw-r--r--   0     1001      127    30290 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/big_graph.svg
--rw-r--r--   0     1001      127     1402 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/define_and_define.md
--rw-r--r--   0     1001      127   657446 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/ecosystem-graph.png
--rw-r--r--   0     1001      127   184123 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/egg.png
--rw-r--r--   0     1001      127    64006 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/indexing_pushdown.ipynb
--rw-r--r--   0     1001      127   117358 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/moa.png
--rw-r--r--   0     1001      127     1551 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/optional_values.md
--rw-r--r--   0     1001      127   420307 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation/pldi_2023_presentation.ipynb
--rw-r--r--   0     1001      127      121 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/explanation.md
--rw-r--r--   0     1001      127      807 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/how-to-guides.md
--rw-r--r--   0     1001      127     1924 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/index.md
--rw-r--r--   0     1001      127     1226 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/reference/bindings.md
--rw-r--r--   0     1001      127      708 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/reference/contributing.md
--rw-r--r--   0     1001      127    16713 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/reference/egglog-translation.md
--rw-r--r--   0     1001      127     1555 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/reference/high-level.md
--rw-r--r--   0     1001      127    12708 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/reference/python-integration.md
--rw-r--r--   0     1001      127     1188 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/reference/usage.md
--rw-r--r--   0     1001      127      594 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/reference.md
--rw-r--r--   0     1001      127    75257 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/tutorials/getting-started.ipynb
--rw-r--r--   0     1001      127    14545 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/tutorials/screenshot-1.png
--rw-r--r--   0     1001      127    91888 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/tutorials/screenshot-2.png
--rw-r--r--   0     1001      127   801962 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/tutorials/sklearn.ipynb
--rw-r--r--   0     1001      127       94 2024-05-03 20:47:31.000000 egglog-7.1.0/docs/tutorials.md
--rw-r--r--   0     1001      127     2623 2024-05-03 20:47:31.000000 egglog-7.1.0/increment_version.py
--rw-r--r--   0     1001      127     5077 2024-05-03 20:47:31.000000 egglog-7.1.0/pyproject.toml
--rw-r--r--   0     1001      127      237 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/__init__.py
--rw-r--r--   0     1001      127    11237 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/bindings.pyi
--rw-r--r--   0     1001      127    12617 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/builtins.py
--rw-r--r--   0     1001      127      168 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/config.py
--rw-r--r--   0     1001      127     6151 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/conversion.py
--rw-r--r--   0     1001      127    15559 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/declarations.py
--rw-r--r--   0     1001      127    64303 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/egraph.py
--rw-r--r--   0     1001      127    19618 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/egraph_state.py
--rw-r--r--   0     1001      127      232 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/examples/README.rst
--rw-r--r--   0     1001      127       31 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/examples/__init__.py
--rw-r--r--   0     1001      127      695 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/examples/bool.py
--rw-r--r--   0     1001      127      966 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/examples/eqsat_basic.py
--rw-r--r--   0     1001      127      492 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/examples/fib.py
--rw-r--r--   0     1001      127     8208 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/examples/lambda_.py
--rw-r--r--   0     1001      127     4961 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/examples/matrix.py
--rw-r--r--   0     1001      127     4042 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/examples/ndarrays.py
--rw-r--r--   0     1001      127     2119 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/examples/resolution.py
--rw-r--r--   0     1001      127      618 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/examples/schedule_demo.py
--rw-r--r--   0     1001      127       49 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/exp/__init__.py
--rw-r--r--   0     1001      127    40040 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/exp/array_api.py
--rw-r--r--   0     1001      127     1250 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/exp/array_api_jit.py
--rw-r--r--   0     1001      127     2852 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/exp/array_api_numba.py
--rw-r--r--   0     1001      127    19209 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/exp/array_api_program_gen.py
--rw-r--r--   0     1001      127    11874 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/exp/program_gen.py
--rw-r--r--   0     1001      127      749 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/exp/siu_examples.py
--rw-r--r--   0     1001      127     1305 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/graphviz_widget.py
--rw-r--r--   0     1001      127     1213 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/ipython_magic.py
--rw-r--r--   0     1001      127    18607 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/pretty.py
--rw-r--r--   0     1001      127        0 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/py.typed
--rw-r--r--   0     1001      127    22465 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/runtime.py
--rw-r--r--   0     1001      127     1823 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/thunk.py
--rw-r--r--   0     1001      127     5550 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/type_constraint_solver.py
--rw-r--r--   0     1001      127       96 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/widget.css
--rw-r--r--   0     1001      127     1971 2024-05-03 20:47:31.000000 egglog-7.1.0/python/egglog/widget.js
--rw-r--r--   0     1001      127       24 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/__init__.py
--rw-r--r--   0     1001      127     4324 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/__snapshots__/test_array_api/TestLDA.test_optimize.py
--rw-r--r--   0     1001      127     1978 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/__snapshots__/test_array_api/TestLDA.test_source_optimized.py
--rw-r--r--   0     1001      127     4399 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/__snapshots__/test_array_api/TestLDA.test_trace.py
--rw-r--r--   0     1001      127      110 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/__snapshots__/test_program_gen/test_to_string.py
--rw-r--r--   0     1001      127      606 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/conftest.py
--rw-r--r--   0     1001      127     5485 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/test_array_api.py
--rw-r--r--   0     1001      127     7775 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/test_bindings.py
--rw-r--r--   0     1001      127     2100 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/test_convert.py
--rw-r--r--   0     1001      127    16272 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/test_high_level.py
--rw-r--r--   0     1001      127     1020 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/test_modules.py
--rw-r--r--   0     1001      127     4810 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/test_pretty.py
--rw-r--r--   0     1001      127     2178 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/test_program_gen.py
--rw-r--r--   0     1001      127     3552 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/test_py_object_sort.py
--rw-r--r--   0     1001      127     3629 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/test_runtime.py
--rw-r--r--   0     1001      127     1999 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/test_type_constraint_solver.py
--rw-r--r--   0     1001      127     1126 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/test_typing.py
--rw-r--r--   0     1001      127     4292 2024-05-03 20:47:31.000000 egglog-7.1.0/python/tests/test_unstable_fn.py
--rw-r--r--   0     1001      127       31 2024-05-03 20:47:31.000000 egglog-7.1.0/rust-toolchain.toml
--rw-r--r--   0     1001      127    23443 2024-05-03 20:47:31.000000 egglog-7.1.0/src/conversions.rs
--rw-r--r--   0     1001      127     7760 2024-05-03 20:47:31.000000 egglog-7.1.0/src/egraph.rs
--rw-r--r--   0     1001      127     1516 2024-05-03 20:47:31.000000 egglog-7.1.0/src/error.rs
--rw-r--r--   0     1001      127      945 2024-05-03 20:47:31.000000 egglog-7.1.0/src/lib.rs
--rw-r--r--   0     1001      127    19045 2024-05-03 20:47:31.000000 egglog-7.1.0/src/py_object_sort.rs
--rw-r--r--   0     1001      127     1010 2024-05-03 20:47:31.000000 egglog-7.1.0/src/serialize.rs
--rw-r--r--   0     1001      127     7878 2024-05-03 20:47:31.000000 egglog-7.1.0/src/utils.rs
--rw-r--r--   0     1001      127      323 2024-05-03 20:47:31.000000 egglog-7.1.0/stubtest_allow
--rw-r--r--   0     1001      127      464 2024-05-03 20:47:31.000000 egglog-7.1.0/test-data/unit/check-high-level.test
--rw-r--r--   0     1001      127    35419 2024-05-03 20:48:21.000000 egglog-7.1.0/Cargo.lock
--rw-r--r--   0        0        0     3819 1970-01-01 00:00:00.000000 egglog-7.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1356 1970-01-01 00:00:00.000000 egglog-7.2.0/Cargo.toml
+-rw-r--r--   0     1001      127      640 2024-05-23 15:45:56.000000 egglog-7.2.0/.github/dependabot.yml
+-rw-r--r--   0     1001      127     2147 2024-05-23 15:45:56.000000 egglog-7.2.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127     3880 2024-05-23 15:45:56.000000 egglog-7.2.0/.github/workflows/version.yml
+-rw-r--r--   0     1001      127      776 2024-05-23 15:45:56.000000 egglog-7.2.0/.gitignore
+-rw-r--r--   0     1001      127     1000 2024-05-23 15:45:56.000000 egglog-7.2.0/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127      825 2024-05-23 15:45:56.000000 egglog-7.2.0/.readthedocs.yaml
+-rw-r--r--   0     1001      127     1438 2024-05-23 15:45:56.000000 egglog-7.2.0/CITATION.cff
+-rw-r--r--   0     1001      127     1070 2024-05-23 15:45:56.000000 egglog-7.2.0/LICENSE
+-rw-r--r--   0     1001      127     1417 2024-05-23 15:45:56.000000 egglog-7.2.0/README.md
+-rw-r--r--   0     1001      127      388 2024-05-23 15:45:56.000000 egglog-7.2.0/conftest.py
+-rw-r--r--   0     1001      127       71 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/.gitignore
+-rw-r--r--   0     1001      127      484 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/_templates/comments.html
+-rw-r--r--   0     1001      127    14983 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/changelog.md
+-rw-r--r--   0     1001      127     5603 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/conf.py
+-rw-r--r--   0     1001      127      149 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/environment.yml
+-rw-r--r--   0     1001      127       13 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/explanation/.gitignore
+-rw-r--r--   0     1001      127  1093641 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/explanation/2023_07_presentation.ipynb
+-rw-r--r--   0     1001      127   114752 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/explanation/2023_11_09_portland_state.ipynb
+-rw-r--r--   0     1001      127   260924 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/explanation/2023_11_17_pytensor.ipynb
+-rw-r--r--   0     1001      127   789680 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/explanation/2023_11_pydata_lightning_talk.ipynb
+-rw-r--r--   0     1001      127    72312 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/explanation/2023_12_02_congruence_closure-1.png
+-rw-r--r--   0     1001      127   193296 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/explanation/2023_12_02_congruence_closure-2.png
+-rw-r--r--   0     1001      127     8470 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/explanation/2023_12_02_congruence_closure.md
+-rw-r--r--   0     1001      127  1048406 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/explanation/2024_03_17_community_talk.ipynb
+-rw-r--r--   0     1001      127   288149 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/explanation/2024_03_17_map.svg
+-rw-r--r--   0     1001      127    30290 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/explanation/big_graph.svg
+-rw-r--r--   0     1001      127     1402 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/explanation/define_and_define.md
+-rw-r--r--   0     1001      127   657446 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/explanation/ecosystem-graph.png
+-rw-r--r--   0     1001      127   184123 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/explanation/egg.png
+-rw-r--r--   0     1001      127    64006 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/explanation/indexing_pushdown.ipynb
+-rw-r--r--   0     1001      127   117358 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/explanation/moa.png
+-rw-r--r--   0     1001      127     1551 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/explanation/optional_values.md
+-rw-r--r--   0     1001      127   420307 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/explanation/pldi_2023_presentation.ipynb
+-rw-r--r--   0     1001      127      121 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/explanation.md
+-rw-r--r--   0     1001      127      807 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/how-to-guides.md
+-rw-r--r--   0     1001      127     1924 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/index.md
+-rw-r--r--   0     1001      127     1226 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/reference/bindings.md
+-rw-r--r--   0     1001      127     2876 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/reference/contributing.md
+-rw-r--r--   0     1001      127    16713 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/reference/egglog-translation.md
+-rw-r--r--   0     1001      127     1555 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/reference/high-level.md
+-rw-r--r--   0     1001      127    15069 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/reference/python-integration.md
+-rw-r--r--   0     1001      127     1188 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/reference/usage.md
+-rw-r--r--   0     1001      127      594 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/reference.md
+-rw-r--r--   0     1001      127    75257 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/tutorials/getting-started.ipynb
+-rw-r--r--   0     1001      127    14545 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/tutorials/screenshot-1.png
+-rw-r--r--   0     1001      127    91888 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/tutorials/screenshot-2.png
+-rw-r--r--   0     1001      127   801962 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/tutorials/sklearn.ipynb
+-rw-r--r--   0     1001      127       94 2024-05-23 15:45:56.000000 egglog-7.2.0/docs/tutorials.md
+-rw-r--r--   0     1001      127     2623 2024-05-23 15:45:56.000000 egglog-7.2.0/increment_version.py
+-rw-r--r--   0     1001      127     5077 2024-05-23 15:45:56.000000 egglog-7.2.0/pyproject.toml
+-rw-r--r--   0     1001      127      237 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/__init__.py
+-rw-r--r--   0     1001      127    11237 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/bindings.pyi
+-rw-r--r--   0     1001      127    12617 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/builtins.py
+-rw-r--r--   0     1001      127      168 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/config.py
+-rw-r--r--   0     1001      127     6151 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/conversion.py
+-rw-r--r--   0     1001      127    17884 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/declarations.py
+-rw-r--r--   0     1001      127    66696 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/egraph.py
+-rw-r--r--   0     1001      127    21315 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/egraph_state.py
+-rw-r--r--   0     1001      127      232 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/examples/README.rst
+-rw-r--r--   0     1001      127       31 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/examples/__init__.py
+-rw-r--r--   0     1001      127      695 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/examples/bool.py
+-rw-r--r--   0     1001      127      966 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/examples/eqsat_basic.py
+-rw-r--r--   0     1001      127      492 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/examples/fib.py
+-rw-r--r--   0     1001      127     1153 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/examples/higher_order_functions.py
+-rw-r--r--   0     1001      127     8208 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/examples/lambda_.py
+-rw-r--r--   0     1001      127     4961 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/examples/matrix.py
+-rw-r--r--   0     1001      127     4042 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/examples/ndarrays.py
+-rw-r--r--   0     1001      127     2119 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/examples/resolution.py
+-rw-r--r--   0     1001      127      618 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/examples/schedule_demo.py
+-rw-r--r--   0     1001      127       49 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/exp/__init__.py
+-rw-r--r--   0     1001      127    40099 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/exp/array_api.py
+-rw-r--r--   0     1001      127     1250 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/exp/array_api_jit.py
+-rw-r--r--   0     1001      127     2852 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/exp/array_api_numba.py
+-rw-r--r--   0     1001      127    19209 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/exp/array_api_program_gen.py
+-rw-r--r--   0     1001      127    11874 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/exp/program_gen.py
+-rw-r--r--   0     1001      127      749 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/exp/siu_examples.py
+-rw-r--r--   0     1001      127     1305 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/graphviz_widget.py
+-rw-r--r--   0     1001      127     1213 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/ipython_magic.py
+-rw-r--r--   0     1001      127    19087 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/pretty.py
+-rw-r--r--   0     1001      127        0 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/py.typed
+-rw-r--r--   0     1001      127    22623 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/runtime.py
+-rw-r--r--   0     1001      127     2087 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/thunk.py
+-rw-r--r--   0     1001      127     5693 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/type_constraint_solver.py
+-rw-r--r--   0     1001      127       96 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/widget.css
+-rw-r--r--   0     1001      127     1971 2024-05-23 15:45:56.000000 egglog-7.2.0/python/egglog/widget.js
+-rw-r--r--   0     1001      127       24 2024-05-23 15:45:56.000000 egglog-7.2.0/python/tests/__init__.py
+-rw-r--r--   0     1001      127     4324 2024-05-23 15:45:56.000000 egglog-7.2.0/python/tests/__snapshots__/test_array_api/TestLDA.test_optimize.py
+-rw-r--r--   0     1001      127     1978 2024-05-23 15:45:56.000000 egglog-7.2.0/python/tests/__snapshots__/test_array_api/TestLDA.test_source_optimized.py
+-rw-r--r--   0     1001      127     4399 2024-05-23 15:45:56.000000 egglog-7.2.0/python/tests/__snapshots__/test_array_api/TestLDA.test_trace.py
+-rw-r--r--   0     1001      127      110 2024-05-23 15:45:56.000000 egglog-7.2.0/python/tests/__snapshots__/test_program_gen/test_to_string.py
+-rw-r--r--   0     1001      127      743 2024-05-23 15:45:56.000000 egglog-7.2.0/python/tests/conftest.py
+-rw-r--r--   0     1001      127     5485 2024-05-23 15:45:56.000000 egglog-7.2.0/python/tests/test_array_api.py
+-rw-r--r--   0     1001      127     7775 2024-05-23 15:45:56.000000 egglog-7.2.0/python/tests/test_bindings.py
+-rw-r--r--   0     1001      127     2100 2024-05-23 15:45:56.000000 egglog-7.2.0/python/tests/test_convert.py
+-rw-r--r--   0     1001      127    18791 2024-05-23 15:45:56.000000 egglog-7.2.0/python/tests/test_high_level.py
+-rw-r--r--   0     1001      127     1020 2024-05-23 15:45:56.000000 egglog-7.2.0/python/tests/test_modules.py
+-rw-r--r--   0     1001      127     4810 2024-05-23 15:45:56.000000 egglog-7.2.0/python/tests/test_pretty.py
+-rw-r--r--   0     1001      127     2178 2024-05-23 15:45:56.000000 egglog-7.2.0/python/tests/test_program_gen.py
+-rw-r--r--   0     1001      127     3552 2024-05-23 15:45:56.000000 egglog-7.2.0/python/tests/test_py_object_sort.py
+-rw-r--r--   0     1001      127     3635 2024-05-23 15:45:56.000000 egglog-7.2.0/python/tests/test_runtime.py
+-rw-r--r--   0     1001      127     1999 2024-05-23 15:45:56.000000 egglog-7.2.0/python/tests/test_type_constraint_solver.py
+-rw-r--r--   0     1001      127     1126 2024-05-23 15:45:56.000000 egglog-7.2.0/python/tests/test_typing.py
+-rw-r--r--   0     1001      127     4292 2024-05-23 15:45:56.000000 egglog-7.2.0/python/tests/test_unstable_fn.py
+-rw-r--r--   0     1001      127       31 2024-05-23 15:45:56.000000 egglog-7.2.0/rust-toolchain.toml
+-rw-r--r--   0     1001      127    23443 2024-05-23 15:45:56.000000 egglog-7.2.0/src/conversions.rs
+-rw-r--r--   0     1001      127     7760 2024-05-23 15:45:56.000000 egglog-7.2.0/src/egraph.rs
+-rw-r--r--   0     1001      127     1516 2024-05-23 15:45:56.000000 egglog-7.2.0/src/error.rs
+-rw-r--r--   0     1001      127      945 2024-05-23 15:45:56.000000 egglog-7.2.0/src/lib.rs
+-rw-r--r--   0     1001      127    19045 2024-05-23 15:45:56.000000 egglog-7.2.0/src/py_object_sort.rs
+-rw-r--r--   0     1001      127     1010 2024-05-23 15:45:56.000000 egglog-7.2.0/src/serialize.rs
+-rw-r--r--   0     1001      127     7878 2024-05-23 15:45:56.000000 egglog-7.2.0/src/utils.rs
+-rw-r--r--   0     1001      127      323 2024-05-23 15:45:56.000000 egglog-7.2.0/stubtest_allow
+-rw-r--r--   0     1001      127      464 2024-05-23 15:45:56.000000 egglog-7.2.0/test-data/unit/check-high-level.test
+-rw-r--r--   0     1001      127    35419 2024-05-23 15:46:41.000000 egglog-7.2.0/Cargo.lock
+-rw-r--r--   0        0        0     3819 1970-01-01 00:00:00.000000 egglog-7.2.0/PKG-INFO
```

### Comparing `egglog-7.1.0/Cargo.toml` & `egglog-7.2.0/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "egglog-python"
-version = "7.1.0"
+version = "7.2.0"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "egglog_python"
 crate-type = ["cdylib"]
```

### Comparing `egglog-7.1.0/.github/dependabot.yml` & `egglog-7.2.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/.github/workflows/CI.yml` & `egglog-7.2.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/.github/workflows/version.yml` & `egglog-7.2.0/.github/workflows/version.yml`

 * *Files 5% similar despite different names*

```diff
@@ -124,11 +124,11 @@
     steps:
       - uses: actions/checkout@v4
         with:
           ref: version-${{ needs.bump.outputs.version }}
       - run: |
           git tag "v$VERSION"
           git push --tags
-          gh pr merge --admin --delete-branch
+          gh pr merge --admin --delete-branch --merge
         env:
           VERSION: ${{ needs.bump.outputs.version }}
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `egglog-7.1.0/.gitignore` & `egglog-7.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/.pre-commit-config.yaml` & `egglog-7.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/.readthedocs.yaml` & `egglog-7.2.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/CITATION.cff` & `egglog-7.2.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/LICENSE` & `egglog-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/README.md` & `egglog-7.2.0/README.md`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/docs/changelog.md` & `egglog-7.2.0/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # Changelog
 
 _This project uses semantic versioning_
 
 ## UNRELEASED
 
+## 7.2.0 (2024-05-23)
+
+- Adds ability to use function bodies as default rewrites ([#167](https://github.com/egraphs-good/egglog-python/pull/167))
+- Fixed bug with creating empty maps and adding to maps ([#168](https://github.com/egraphs-good/egglog-python/pull/168))
+
 ## 7.1.0 (2024-05-03)
 
 ## New Feaatures
 
 - Upgrade [egglog](https://github.com/egraphs-good/egglog/compare/0113af1d6476b75d4319591cc3d675f96a71cdc5...fb4a9f114f9bb93154d6eff0dbab079b5cb4ebb6) ([#143](https://github.com/egraphs-good/egglog-python/pull/143))
   - Adds `bindings.UnstableCombinedRulset` to commands
   - Adds `UnstableFn` sort
```

### Comparing `egglog-7.1.0/docs/conf.py` & `egglog-7.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/docs/explanation/2023_07_presentation.ipynb` & `egglog-7.2.0/docs/explanation/2023_07_presentation.ipynb`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/docs/explanation/2023_11_09_portland_state.ipynb` & `egglog-7.2.0/docs/explanation/2023_11_09_portland_state.ipynb`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/docs/explanation/2023_11_17_pytensor.ipynb` & `egglog-7.2.0/docs/explanation/2023_11_17_pytensor.ipynb`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/docs/explanation/2023_11_pydata_lightning_talk.ipynb` & `egglog-7.2.0/docs/explanation/2023_11_pydata_lightning_talk.ipynb`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/docs/explanation/2023_12_02_congruence_closure-1.png` & `egglog-7.2.0/docs/explanation/2023_12_02_congruence_closure-1.png`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/docs/explanation/2023_12_02_congruence_closure-2.png` & `egglog-7.2.0/docs/explanation/2023_12_02_congruence_closure-2.png`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/docs/explanation/2023_12_02_congruence_closure.md` & `egglog-7.2.0/docs/explanation/2023_12_02_congruence_closure.md`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/docs/explanation/2024_03_17_community_talk.ipynb` & `egglog-7.2.0/docs/explanation/2024_03_17_community_talk.ipynb`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/docs/explanation/2024_03_17_map.svg` & `egglog-7.2.0/docs/explanation/2024_03_17_map.svg`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/docs/explanation/big_graph.svg` & `egglog-7.2.0/docs/explanation/big_graph.svg`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/docs/explanation/define_and_define.md` & `egglog-7.2.0/docs/explanation/define_and_define.md`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/docs/explanation/ecosystem-graph.png` & `egglog-7.2.0/docs/explanation/ecosystem-graph.png`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/docs/explanation/egg.png` & `egglog-7.2.0/docs/explanation/egg.png`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/docs/explanation/indexing_pushdown.ipynb` & `egglog-7.2.0/docs/explanation/indexing_pushdown.ipynb`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/docs/explanation/moa.png` & `egglog-7.2.0/docs/explanation/moa.png`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/docs/explanation/optional_values.md` & `egglog-7.2.0/docs/explanation/optional_values.md`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/docs/explanation/pldi_2023_presentation.ipynb` & `egglog-7.2.0/docs/explanation/pldi_2023_presentation.ipynb`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/docs/how-to-guides.md` & `egglog-7.2.0/docs/how-to-guides.md`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/docs/index.md` & `egglog-7.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/docs/reference/bindings.md` & `egglog-7.2.0/docs/reference/bindings.md`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/docs/reference/egglog-translation.md` & `egglog-7.2.0/docs/reference/egglog-translation.md`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/docs/reference/high-level.md` & `egglog-7.2.0/docs/reference/high-level.md`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/docs/reference/python-integration.md` & `egglog-7.2.0/docs/reference/python-integration.md`

 * *Files 14% similar despite different names*

```diff
@@ -131,14 +131,15 @@
 class Math(Expr):
     def __init__(self, x: i64Like) -> None: ...
 
     @classmethod
     def var(cls, name: StringLike) -> Math: ...
 
     def __add__(self, other: Math) -> Math: ...
+    def __mul__(self, other: Math) -> Math: ...
 
 converter(i64, Math, Math)
 converter(String, Math, Math.var)
 
 Math(2) + i64(30) + String("x")
 # equal to
 Math(2) + Math(i64(30)) + Math.var(String("x"))
@@ -422,7 +423,90 @@
 
 check_eq(added_two, MathList.EMPTY.append(Math(2) + Math(1)), math_list_ruleset.saturate())
 ```
 
 Note that this is all built on the [unstable function support added as a sort to egglog](https://github.com/egraphs-good/egglog/pull/348).
 While this sort is exposed directly at the high level with the `UnstableFn` class, we don't reccomend depending on it directly, and instead
 using the builtin Python type annotations. This will allow us to change the implementation in the future without breaking user code.
+
+## Default Replacements
+
+When defining a function or a constant, you can also provide a default replacement value. This is useful when
+you might want both the original value and the replaced value in the e-graph, so that later rules could reference either.
+
+```{code-cell} python
+@function
+def math_float(f: f64Like) -> Math:
+    ...
+
+
+# Can add a default replacement value for a constants
+pi = constant("pi", Math, math_float(3.14))
+
+
+# or for a function by providing a body
+@function
+def square(x: Math) -> Math:
+    return x * x
+
+# thse rewrites will be added to the e-graph under the default ruleset
+egraph = EGraph()
+egraph.register(pi)
+egraph.register(square(Math.var('x')))
+egraph.run(1)
+egraph.check(eq(pi).to(math_float(3.14)))
+egraph.check(eq(square(Math.var('x'))).to(Math.var('x') * Math.var('x')))
+egraph
+```
+
+This is equivalent to adding the rewrite rules to the e-graph directly, like this, but just more succinct:
+
+```python
+x  = var("x", Math)
+egraph.register(rewrite(pi).to(math_float(3.14)))
+egraph.register(rewrite(square(x)).to(x * x))
+```
+
+You can also specify a ruleset to add the rewrites to, by passing in the `ruleset` keyword argument:
+
+```{code-cell} python
+math_ruleset = ruleset()
+
+e_constant = constant("e", Math, math_float(2.71), ruleset=math_ruleset)
+
+@function(ruleset=math_ruleset)
+def cube(x: Math) -> Math:
+    return x * x * x
+
+
+egraph.register(e_constant)
+egraph.register(cube(Math.var('x')))
+egraph.run(math_ruleset)
+egraph.check(eq(e_constant).to(math_float(2.71)))
+egraph.check(eq(cube(Math.var('x'))).to(Math.var('x') * Math.var('x') * Math.var('x')))
+```
+
+### Default Replacement for Classes
+
+In classes, you can also provide a default replacement value for constants and methods, and an optional ruleset on the class constructor:
+
+```{code-cell} python
+other_math_ruleset = ruleset()
+
+
+class WrappedMath(Expr, ruleset=other_math_ruleset):
+    PI: ClassVar[Math] = math_float(3.14)
+
+    def __init__(self, x: Math) -> None: ...
+
+    def double(self) -> WrappedMath:
+        return self + self
+
+    def __add__(self, other: WrappedMath) -> WrappedMath: ...
+
+x = WrappedMath(WrappedMath.PI).double()
+egraph = EGraph()
+egraph.register(x)
+egraph.run(other_math_ruleset * 2)
+egraph.check(eq(x).to(WrappedMath(math_float(3.14)) + WrappedMath(math_float(3.14))))
+egraph
+```
```

### Comparing `egglog-7.1.0/docs/reference/usage.md` & `egglog-7.2.0/docs/reference/usage.md`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/docs/reference.md` & `egglog-7.2.0/docs/reference.md`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/docs/tutorials/getting-started.ipynb` & `egglog-7.2.0/docs/tutorials/getting-started.ipynb`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/docs/tutorials/screenshot-1.png` & `egglog-7.2.0/docs/tutorials/screenshot-1.png`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/docs/tutorials/screenshot-2.png` & `egglog-7.2.0/docs/tutorials/screenshot-2.png`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/docs/tutorials/sklearn.ipynb` & `egglog-7.2.0/docs/tutorials/sklearn.ipynb`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/increment_version.py` & `egglog-7.2.0/increment_version.py`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/pyproject.toml` & `egglog-7.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/python/egglog/bindings.pyi` & `egglog-7.2.0/python/egglog/bindings.pyi`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/python/egglog/builtins.py` & `egglog-7.2.0/python/egglog/builtins.py`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/python/egglog/conversion.py` & `egglog-7.2.0/python/egglog/conversion.py`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/python/egglog/declarations.py` & `egglog-7.2.0/python/egglog/declarations.py`

 * *Files 10% similar despite different names*

```diff
@@ -67,24 +67,32 @@
     "BiRewriteDecl",
     "RuleDecl",
     "RewriteOrRuleDecl",
     "ActionCommandDecl",
     "CommandDecl",
     "SpecialFunctions",
     "FunctionSignature",
+    "DefaultRewriteDecl",
+    "InitRef",
 ]
 
 
 @dataclass
 class DelayedDeclerations:
     __egg_decls_thunk__: Callable[[], Declarations]
 
     @property
     def __egg_decls__(self) -> Declarations:
-        return self.__egg_decls_thunk__()
+        try:
+            return self.__egg_decls_thunk__()
+        # Catch attribute error, so that it isn't bubbled up as a missing attribute and fallbacks on `__getattr__`
+        # instead raise explicitly
+        except AttributeError as err:
+            msg = "Error resolving declerations"
+            raise RuntimeError(msg) from err
 
 
 @runtime_checkable
 class HasDeclerations(Protocol):
     @property
     def __egg_decls__(self) -> Declarations: ...
 
@@ -109,29 +117,35 @@
 @dataclass
 class Declarations:
     _functions: dict[str, FunctionDecl | RelationDecl] = field(default_factory=dict)
     _constants: dict[str, ConstantDecl] = field(default_factory=dict)
     _classes: dict[str, ClassDecl] = field(default_factory=dict)
     _rulesets: dict[str, RulesetDecl | CombinedRulesetDecl] = field(default_factory=lambda: {"": RulesetDecl([])})
 
+    @property
+    def default_ruleset(self) -> RulesetDecl:
+        ruleset = self._rulesets[""]
+        assert isinstance(ruleset, RulesetDecl)
+        return ruleset
+
     @classmethod
     def create(cls, *others: DeclerationsLike) -> Declarations:
         others = upcast_declerations(others)
         if not others:
             return Declarations()
         first, *rest = others
         if not rest:
             return first
         new = first.copy()
         new.update(*rest)
         return new
 
     def copy(self) -> Declarations:
         new = Declarations()
-        new |= self
+        self.update_other(new)
         return new
 
     def update(self, *others: DeclerationsLike) -> None:
         for other in others:
             self |= other
 
     def __or__(self, other: DeclerationsLike) -> Declarations:
@@ -150,49 +164,82 @@
     def update_other(self, other: Declarations) -> None:
         """
         Updates the other decl with these values in palce.
         """
         other._functions |= self._functions
         other._classes |= self._classes
         other._constants |= self._constants
+        # Must combine rulesets bc the empty ruleset might be different, bc DefaultRewriteDecl
+        # is added to functions.
+        combined_default_rules: set[RewriteOrRuleDecl] = {*self.default_ruleset.rules, *other.default_ruleset.rules}
         other._rulesets |= self._rulesets
+        other._rulesets[""] = RulesetDecl(list(combined_default_rules))
 
-    def get_callable_decl(self, ref: CallableRef) -> CallableDecl:
+    def get_callable_decl(self, ref: CallableRef) -> CallableDecl:  # noqa: PLR0911
         match ref:
             case FunctionRef(name):
                 return self._functions[name]
             case ConstantRef(name):
                 return self._constants[name]
             case MethodRef(class_name, method_name):
                 return self._classes[class_name].methods[method_name]
             case ClassVariableRef(class_name, name):
                 return self._classes[class_name].class_variables[name]
             case ClassMethodRef(class_name, name):
                 return self._classes[class_name].class_methods[name]
             case PropertyRef(class_name, property_name):
                 return self._classes[class_name].properties[property_name]
+            case InitRef(class_name):
+                init_fn = self._classes[class_name].init
+                assert init_fn
+                return init_fn
         assert_never(ref)
 
+    def set_function_decl(
+        self, ref: FunctionRef | MethodRef | ClassMethodRef | PropertyRef | InitRef, decl: FunctionDecl
+    ) -> None:
+        match ref:
+            case FunctionRef(name):
+                self._functions[name] = decl
+            case MethodRef(class_name, method_name):
+                self._classes[class_name].methods[method_name] = decl
+            case ClassMethodRef(class_name, name):
+                self._classes[class_name].class_methods[name] = decl
+            case PropertyRef(class_name, property_name):
+                self._classes[class_name].properties[property_name] = decl
+            case InitRef(class_name):
+                self._classes[class_name].init = decl
+            case _:
+                assert_never(ref)
+
     def has_method(self, class_name: str, method_name: str) -> bool | None:
         """
         Returns whether the given class has the given method, or None if we cant find the class.
         """
         if class_name in self._classes:
             return method_name in self._classes[class_name].methods
         return None
 
     def get_class_decl(self, name: str) -> ClassDecl:
         return self._classes[name]
 
+    def get_paramaterized_class(self, name: str) -> TypeRefWithVars:
+        """
+        Returns a class reference with type parameters, if the class is paramaterized.
+        """
+        type_vars = self._classes[name].type_vars
+        return TypeRefWithVars(name, tuple(map(ClassTypeVarRef, type_vars)))
+
 
 @dataclass
 class ClassDecl:
     egg_name: str | None = None
     type_vars: tuple[str, ...] = ()
     builtin: bool = False
+    init: FunctionDecl | None = None
     class_methods: dict[str, FunctionDecl] = field(default_factory=dict)
     # These have to be seperate from class_methods so that printing them can be done easily
     class_variables: dict[str, ConstantDecl] = field(default_factory=dict)
     methods: dict[str, FunctionDecl] = field(default_factory=dict)
     properties: dict[str, FunctionDecl] = field(default_factory=dict)
     preserved_methods: dict[str, Callable] = field(default_factory=dict)
 
@@ -290,26 +337,33 @@
 @dataclass(frozen=True)
 class ClassMethodRef:
     class_name: str
     method_name: str
 
 
 @dataclass(frozen=True)
+class InitRef:
+    class_name: str
+
+
+@dataclass(frozen=True)
 class ClassVariableRef:
     class_name: str
     var_name: str
 
 
 @dataclass(frozen=True)
 class PropertyRef:
     class_name: str
     property_name: str
 
 
-CallableRef: TypeAlias = FunctionRef | ConstantRef | MethodRef | ClassMethodRef | ClassVariableRef | PropertyRef
+CallableRef: TypeAlias = (
+    FunctionRef | ConstantRef | MethodRef | ClassMethodRef | InitRef | ClassVariableRef | PropertyRef
+)
 
 
 ##
 # Callables
 ##
 
 
@@ -374,15 +428,14 @@
     def mutates(self) -> bool:
         return self.return_type is None
 
 
 @dataclass(frozen=True)
 class FunctionDecl:
     signature: FunctionSignature | SpecialFunctions = field(default_factory=FunctionSignature)
-
     # Egg params
     builtin: bool = False
     egg_name: str | None = None
     cost: int | None = None
     default: ExprDecl | None = None
     on_merge: tuple[ActionDecl, ...] = ()
     merge: ExprDecl | None = None
@@ -454,15 +507,15 @@
     # TODO: Can I make these not typed expressions?
     args: tuple[TypedExprDecl, ...] = ()
     # type parameters that were bound to the callable, if it is a classmethod
     # Used for pretty printing classmethod calls with type parameters
     bound_tp_params: tuple[JustTypeRef, ...] | None = None
 
     def __post_init__(self) -> None:
-        if self.bound_tp_params and not isinstance(self.callable, ClassMethodRef):
+        if self.bound_tp_params and not isinstance(self.callable, ClassMethodRef | InitRef):
             msg = "Cannot bind type parameters to a non-class method callable."
             raise ValueError(msg)
 
     def __hash__(self) -> int:
         return self._cached_hash
 
     @cached_property
@@ -625,15 +678,21 @@
 @dataclass(frozen=True)
 class RuleDecl:
     head: tuple[ActionDecl, ...]
     body: tuple[FactDecl, ...]
     name: str | None
 
 
-RewriteOrRuleDecl: TypeAlias = RewriteDecl | BiRewriteDecl | RuleDecl
+@dataclass(frozen=True)
+class DefaultRewriteDecl:
+    ref: CallableRef
+    expr: ExprDecl
+
+
+RewriteOrRuleDecl: TypeAlias = RewriteDecl | BiRewriteDecl | RuleDecl | DefaultRewriteDecl
 
 
 @dataclass(frozen=True)
 class ActionCommandDecl:
     action: ActionDecl
```

### Comparing `egglog-7.1.0/python/egglog/egraph.py` & `egglog-7.2.0/python/egglog/egraph.py`

 * *Files 3% similar despite different names*

```diff
@@ -348,15 +348,15 @@
         """
 
         Defines a named constant of a certain type.
 
         This is the same as defining a nullary function with a high cost.
         # TODO: Rename as declare to match eggglog?
         """
-        return constant(name, tp, egg_name)
+        return constant(name, tp, egg_name=egg_name)
 
     def register(
         self,
         /,
         command_or_generator: ActionLike | RewriteOrRule | RewriteOrRuleGenerator,
         *command_likes: ActionLike | RewriteOrRule,
     ) -> None:
@@ -448,14 +448,15 @@
     def __new__(  # type: ignore[misc]
         cls: type[_ExprMetaclass],
         name: str,
         bases: tuple[type, ...],
         namespace: dict[str, Any],
         egg_sort: str | None = None,
         builtin: bool = False,
+        ruleset: Ruleset | None = None,
     ) -> RuntimeClass | type:
         # If this is the Expr subclass, just return the class
         if not bases:
             return super().__new__(cls, name, bases, namespace)
         # TODO: Raise error on subclassing or multiple inheritence
 
         frame = currentframe()
@@ -463,24 +464,36 @@
         prev_frame = frame.f_back
         assert prev_frame
 
         # Store frame so that we can get live access to updated locals/globals
         # Otherwise, f_locals returns a copy
         # https://peps.python.org/pep-0667/
         decls_thunk = Thunk.fn(
-            _generate_class_decls, namespace, prev_frame, builtin, egg_sort, name, fallback=Declarations
+            _generate_class_decls,
+            namespace,
+            prev_frame,
+            builtin,
+            egg_sort,
+            name,
+            ruleset,
+            fallback=Declarations,
         )
         return RuntimeClass(decls_thunk, TypeRefWithVars(name))
 
     def __instancecheck__(cls, instance: object) -> bool:
         return isinstance(instance, RuntimeExpr)
 
 
-def _generate_class_decls(  # noqa: C901
-    namespace: dict[str, Any], frame: FrameType, builtin: bool, egg_sort: str | None, cls_name: str
+def _generate_class_decls(
+    namespace: dict[str, Any],
+    frame: FrameType,
+    builtin: bool,
+    egg_sort: str | None,
+    cls_name: str,
+    ruleset: Ruleset | None,
 ) -> Declarations:
     """
     Lazy constructor for class declerations to support classes with methods whose types are not yet defined.
     """
     parameters: list[TypeVar] = (
         # Get the generic params from the orig bases generic class
         namespace["__orig_bases__"][1].__parameters__ if "__orig_bases__" in namespace else []
@@ -494,33 +507,35 @@
     # Register class variables
     ##
     # Create a dummy type to pass to get_type_hints to resolve the annotations we have
     _Dummytype = type("_DummyType", (), {"__annotations__": namespace.get("__annotations__", {})})
     for k, v in get_type_hints(_Dummytype, globalns=frame.f_globals, localns=frame.f_locals).items():
         if getattr(v, "__origin__", None) == ClassVar:
             (inner_tp,) = v.__args__
-            type_ref = resolve_type_annotation(decls, inner_tp).to_just()
-            cls_decl.class_variables[k] = ConstantDecl(type_ref)
-
+            type_ref = resolve_type_annotation(decls, inner_tp)
+            cls_decl.class_variables[k] = ConstantDecl(type_ref.to_just())
+            _add_default_rewrite(decls, ClassVariableRef(cls_name, k), type_ref, namespace.pop(k, None), ruleset)
         else:
             msg = f"On class {cls_name}, for attribute '{k}', expected a ClassVar, but got {v}"
             raise NotImplementedError(msg)
 
     ##
     # Register methods, classmethods, preserved methods, and properties
     ##
 
     # The type ref of self is paramterized by the type vars
-    slf_type_ref = TypeRefWithVars(cls_name, tuple(map(ClassTypeVarRef, type_vars)))
+    TypeRefWithVars(cls_name, tuple(map(ClassTypeVarRef, type_vars)))
 
     # Get all the methods from the class
     filtered_namespace: list[tuple[str, Any]] = [
         (k, v) for k, v in namespace.items() if k not in IGNORED_ATTRIBUTES or isinstance(v, _WrappedMethod)
     ]
 
+    # all methods we should try adding default functions for
+    default_function_refs: dict[ClassMethodRef | MethodRef | PropertyRef, Callable] = {}
     # Then register each of its methods
     for method_name, method in filtered_namespace:
         is_init = method_name == "__init__"
         # Don't register the init methods for literals, since those don't use the type checking mechanisms
         if is_init and cls_name in LIT_CLASS_NAMES:
             continue
         match method:
@@ -532,51 +547,34 @@
                 unextractable, preserve = False, False
                 mutates = method_name in ALWAYS_MUTATES_SELF
         if preserve:
             cls_decl.preserved_methods[method_name] = fn
             continue
         locals = frame.f_locals
 
-        def create_decl(fn: object, first: Literal["cls"] | TypeRefWithVars) -> FunctionDecl:
-            special_function_name: SpecialFunctions | None = (
-                "fn-partial" if egg_fn == "unstable-fn" else "fn-app" if egg_fn == "unstable-app" else None  # noqa: B023
-            )
-            if special_function_name:
-                return FunctionDecl(
-                    special_function_name,
-                    builtin=True,
-                    egg_name=egg_fn,  # noqa: B023
-                )
-
-            return _fn_decl(
-                decls,
-                egg_fn,  # noqa: B023
-                fn,
-                locals,  # noqa: B023
-                default,  # noqa: B023
-                cost,  # noqa: B023
-                merge,  # noqa: B023
-                on_merge,  # noqa: B023
-                mutates,  # noqa: B023
-                builtin,
-                first,
-                is_init,  # noqa: B023
-                unextractable,  # noqa: B023
-            )
-
+        ref: ClassMethodRef | MethodRef | PropertyRef | InitRef
         match fn:
             case classmethod():
-                cls_decl.class_methods[method_name] = create_decl(fn.__func__, "cls")
+                ref = ClassMethodRef(cls_name, method_name)
+                fn = fn.__func__
             case property():
-                cls_decl.properties[method_name] = create_decl(fn.fget, slf_type_ref)
+                ref = PropertyRef(cls_name, method_name)
+                fn = fn.fget
             case _:
-                if is_init:
-                    cls_decl.class_methods[method_name] = create_decl(fn, slf_type_ref)
-                else:
-                    cls_decl.methods[method_name] = create_decl(fn, slf_type_ref)
+                ref = InitRef(cls_name) if is_init else MethodRef(cls_name, method_name)
+
+        _fn_decl(decls, egg_fn, ref, fn, locals, default, cost, merge, on_merge, mutates, builtin, unextractable)
+
+        if not builtin and not isinstance(ref, InitRef) and not mutates:
+            default_function_refs[ref] = fn
+
+    # Add all rewrite methods at the end so that all methods are registered first and can be accessed
+    # in the bodies
+    for ref, fn in default_function_refs.items():
+        _add_default_rewrite_function(decls, ref, fn, ruleset)
 
     return decls
 
 
 @overload
 def function(fn: CALLABLE, /) -> CALLABLE: ...
 
@@ -587,27 +585,29 @@
     egg_fn: str | None = None,
     cost: int | None = None,
     merge: Callable[[Any, Any], Any] | None = None,
     on_merge: Callable[[Any, Any], Iterable[ActionLike]] | None = None,
     mutates_first_arg: bool = False,
     unextractable: bool = False,
     builtin: bool = False,
+    ruleset: Ruleset | None = None,
 ) -> Callable[[CALLABLE], CALLABLE]: ...
 
 
 @overload
 def function(
     *,
     egg_fn: str | None = None,
     cost: int | None = None,
     default: EXPR | None = None,
     merge: Callable[[EXPR, EXPR], EXPR] | None = None,
     on_merge: Callable[[EXPR, EXPR], Iterable[ActionLike]] | None = None,
     mutates_first_arg: bool = False,
     unextractable: bool = False,
+    ruleset: Ruleset | None = None,
 ) -> Callable[[Callable[P, EXPR]], Callable[P, EXPR]]: ...
 
 
 def function(*args, **kwargs) -> Any:
     """
     Defined by a unique name and a typing relation that will specify the return type based on the types of the argument expressions.
 
@@ -630,104 +630,114 @@
     mutates_first_arg: bool = False
     egg_fn: str | None = None
     cost: int | None = None
     default: RuntimeExpr | None = None
     merge: Callable[[RuntimeExpr, RuntimeExpr], RuntimeExpr] | None = None
     on_merge: Callable[[RuntimeExpr, RuntimeExpr], Iterable[ActionLike]] | None = None
     unextractable: bool = False
+    ruleset: Ruleset | None = None
 
     def __call__(self, fn: Callable[..., RuntimeExpr]) -> RuntimeFunction:
         return RuntimeFunction(Thunk.fn(self.create_decls, fn), FunctionRef(fn.__name__))
 
     def create_decls(self, fn: Callable[..., RuntimeExpr]) -> Declarations:
         decls = Declarations()
-        decls._functions[fn.__name__] = _fn_decl(
+        _fn_decl(
             decls,
             self.egg_fn,
+            (ref := FunctionRef(fn.__name__)),
             fn,
             self.hint_locals,
             self.default,
             self.cost,
             self.merge,
             self.on_merge,
             self.mutates_first_arg,
             self.builtin,
             unextractable=self.unextractable,
         )
+        _add_default_rewrite_function(decls, ref, fn, self.ruleset)
         return decls
 
 
 def _fn_decl(
     decls: Declarations,
     egg_name: str | None,
+    ref: FunctionRef | MethodRef | PropertyRef | ClassMethodRef | InitRef,
     fn: object,
     # Pass in the locals, retrieved from the frame when wrapping,
     # so that we support classes and function defined inside of other functions (which won't show up in the globals)
     hint_locals: dict[str, Any],
     default: RuntimeExpr | None,
     cost: int | None,
     merge: Callable[[RuntimeExpr, RuntimeExpr], RuntimeExpr] | None,
     on_merge: Callable[[RuntimeExpr, RuntimeExpr], Iterable[ActionLike]] | None,
     mutates_first_arg: bool,
     is_builtin: bool,
-    # The first arg is either cls, for a classmethod, a self type, or none for a function
-    first_arg: Literal["cls"] | TypeOrVarRef | None = None,
-    is_init: bool = False,
     unextractable: bool = False,
-) -> FunctionDecl:
+) -> None:
+    """
+    Sets the function decl for the function object.
+    """
     if not isinstance(fn, FunctionType):
         raise NotImplementedError(f"Can only generate function decls for functions not {fn}  {type(fn)}")
 
+    # partial function creation and calling are handled with a special case in the type checker, so don't
+    # use the normal logic
+    special_function_name: SpecialFunctions | None = (
+        "fn-partial" if egg_name == "unstable-fn" else "fn-app" if egg_name == "unstable-app" else None
+    )
+    if special_function_name:
+        decls.set_function_decl(ref, FunctionDecl(special_function_name, builtin=True, egg_name=egg_name))
+        return
+
     hint_globals = fn.__globals__.copy()
     # Copy Callable into global if not present bc sometimes it gets automatically removed by ruff to type only block
     # https://docs.astral.sh/ruff/rules/typing-only-standard-library-import/
     if "Callable" not in hint_globals:
         hint_globals["Callable"] = Callable
 
     hints = get_type_hints(fn, hint_globals, hint_locals)
 
     params = list(signature(fn).parameters.values())
 
-    # If this is an init function, or a classmethod, remove the first arg name
-    if is_init or first_arg == "cls":
+    # If this is an init function, or a classmethod, the first arg is not used
+    if isinstance(ref, ClassMethodRef | InitRef):
         params = params[1:]
 
     if _last_param_variable(params):
         *params, var_arg_param = params
         # For now, we don't use the variable arg name
         var_arg_type = resolve_type_annotation(decls, hints[var_arg_param.name])
     else:
         var_arg_type = None
     arg_types = tuple(
-        first_arg
-        # If the first arg is a self, and this not an __init__ fn, add this as a typeref
-        if i == 0 and isinstance(first_arg, ClassTypeVarRef | TypeRefWithVars) and not is_init
+        decls.get_paramaterized_class(ref.class_name)
+        if i == 0 and isinstance(ref, MethodRef | PropertyRef)
         else resolve_type_annotation(decls, hints[t.name])
         for i, t in enumerate(params)
     )
 
     # Resolve all default values as arg types
     arg_defaults = [
         resolve_literal(t, p.default) if p.default is not Parameter.empty else None
         for (t, p) in zip(arg_types, params, strict=True)
     ]
 
     decls.update(*arg_defaults)
 
-    # If this is an init fn use the first arg as the return type
-    if is_init:
-        assert not mutates_first_arg
-        if not isinstance(first_arg, ClassTypeVarRef | TypeRefWithVars):
-            msg = "Init function must have a self type"
-            raise ValueError(msg)
-        return_type = first_arg
-    elif mutates_first_arg:
-        return_type = arg_types[0]
-    else:
-        return_type = resolve_type_annotation(decls, hints["return"])
+    return_type = (
+        decls.get_paramaterized_class(ref.class_name)
+        if isinstance(ref, InitRef)
+        else arg_types[0]
+        if mutates_first_arg
+        else resolve_type_annotation(decls, hints["return"])
+    )
+
+    arg_names = tuple(t.name for t in params)
 
     decls |= default
     merged = (
         None
         if merge is None
         else merge(
             RuntimeExpr.__from_value__(decls, TypedExprDecl(return_type.to_just(), VarDecl("old"))),
@@ -743,30 +753,31 @@
             on_merge(
                 RuntimeExpr.__from_value__(decls, TypedExprDecl(return_type.to_just(), VarDecl("old"))),
                 RuntimeExpr.__from_value__(decls, TypedExprDecl(return_type.to_just(), VarDecl("new"))),
             )
         )
     )
     decls.update(*merge_action)
-    return FunctionDecl(
+    decl = FunctionDecl(
         FunctionSignature(
             return_type=None if mutates_first_arg else return_type,
             var_arg_type=var_arg_type,
             arg_types=arg_types,
-            arg_names=tuple(t.name for t in params),
+            arg_names=arg_names,
             arg_defaults=tuple(a.__egg_typed_expr__.expr if a is not None else None for a in arg_defaults),
         ),
         cost=cost,
         egg_name=egg_name,
         merge=merged.__egg_typed_expr__.expr if merged is not None else None,
         unextractable=unextractable,
         builtin=is_builtin,
         default=None if default is None else default.__egg_typed_expr__.expr,
         on_merge=tuple(a.action for a in merge_action),
     )
+    decls.set_function_decl(ref, decl)
 
 
 # Overload to support aritys 0-4 until variadic generic support map, so we can map from type to value
 @overload
 def relation(
     name: str, tp1: type[E1], tp2: type[E2], tp3: type[E3], tp4: type[E4], /
 ) -> Callable[[E1, E2, E3, E4], Unit]: ...
@@ -800,27 +811,81 @@
     decls = Declarations()
     decls |= cast(RuntimeClass, Unit)
     arg_types = tuple(resolve_type_annotation(decls, tp).to_just() for tp in tps)
     decls._functions[name] = RelationDecl(arg_types, tuple(None for _ in tps), egg_fn)
     return decls
 
 
-def constant(name: str, tp: type[EXPR], egg_name: str | None = None) -> EXPR:
+def constant(
+    name: str,
+    tp: type[EXPR],
+    default_replacement: EXPR | None = None,
+    /,
+    *,
+    egg_name: str | None = None,
+    ruleset: Ruleset | None = None,
+) -> EXPR:
     """
     A "constant" is implemented as the instantiation of a value that takes no args.
     This creates a function with `name` and return type `tp` and returns a value of it being called.
     """
-    return cast(EXPR, RuntimeExpr(Thunk.fn(_constant_thunk, name, tp, egg_name)))
+    return cast(EXPR, RuntimeExpr(Thunk.fn(_constant_thunk, name, tp, egg_name, default_replacement, ruleset)))
 
 
-def _constant_thunk(name: str, tp: type, egg_name: str | None) -> tuple[Declarations, TypedExprDecl]:
+def _constant_thunk(
+    name: str, tp: type, egg_name: str | None, default_replacement: object, ruleset: Ruleset | None
+) -> tuple[Declarations, TypedExprDecl]:
     decls = Declarations()
-    type_ref = resolve_type_annotation(decls, tp).to_just()
-    decls._constants[name] = ConstantDecl(type_ref, egg_name)
-    return decls, TypedExprDecl(type_ref, CallDecl(ConstantRef(name)))
+    type_ref = resolve_type_annotation(decls, tp)
+    callable_ref = ConstantRef(name)
+    decls._constants[name] = ConstantDecl(type_ref.to_just(), egg_name)
+    _add_default_rewrite(decls, callable_ref, type_ref, default_replacement, ruleset)
+    return decls, TypedExprDecl(type_ref.to_just(), CallDecl(callable_ref))
+
+
+def _add_default_rewrite_function(decls: Declarations, ref: CallableRef, fn: Callable, ruleset: Ruleset | None) -> None:
+    """
+    Adds a default rewrite for a function, by calling the functions with vars and adding it if it is not None.
+    """
+    callable_decl = decls.get_callable_decl(ref)
+    assert isinstance(callable_decl, FunctionDecl)
+    signature = callable_decl.signature
+    assert isinstance(signature, FunctionSignature)
+
+    var_args: list[object] = [
+        RuntimeExpr.__from_value__(decls, TypedExprDecl(tp.to_just(), VarDecl(_rule_var_name(name))))
+        for name, tp in zip(signature.arg_names, signature.arg_types, strict=False)
+    ]
+    # If this is a classmethod, add the class as the first arg
+    if isinstance(ref, ClassMethodRef):
+        tp = decls.get_paramaterized_class(ref.class_name)
+        var_args.insert(0, RuntimeClass(Thunk.value(decls), tp))
+    _add_default_rewrite(decls, ref, signature.semantic_return_type, fn(*var_args), ruleset)
+
+
+def _add_default_rewrite(
+    decls: Declarations, ref: CallableRef, type_ref: TypeOrVarRef, default_rewrite: object, ruleset: Ruleset | None
+) -> None:
+    """
+    Adds a default rewrite for the callable, if the default rewrite is not None
+
+    Will add it to the ruleset if it is passed in, or add it to the default ruleset on the passed in decls if not.
+    """
+    if default_rewrite is None:
+        return
+    resolved_value = resolve_literal(type_ref, default_rewrite)
+    rewrite_decl = DefaultRewriteDecl(ref, resolved_value.__egg_typed_expr__.expr)
+    if ruleset:
+        ruleset_decls = ruleset._current_egg_decls
+        ruleset_decl = ruleset.__egg_ruleset__
+    else:
+        ruleset_decls = decls
+        ruleset_decl = decls.default_ruleset
+    ruleset_decl.rules.append(rewrite_decl)
+    ruleset_decls |= resolved_value
 
 
 def _last_param_variable(params: list[Parameter]) -> bool:
     """
     Checks if the last paramater is a variable arg.
 
     Raises an error if any of the other params are not positional or keyword.
@@ -987,14 +1052,15 @@
     def let(self, name: str, expr: EXPR) -> EXPR:
         """
         Define a new expression in the egraph and return a reference to it.
         """
         action = let(name, expr)
         self.register(action)
         runtime_expr = to_runtime_expr(expr)
+        self._add_decls(runtime_expr)
         return cast(
             EXPR,
             RuntimeExpr.__from_value__(
                 self.__egg_decls__, TypedExprDecl(runtime_expr.__egg_typed_expr__.tp, VarDecl(name))
             ),
         )
 
@@ -1012,15 +1078,16 @@
         """
         schedule = run(ruleset, *until) * limit_or_schedule if isinstance(limit_or_schedule, int) else limit_or_schedule
         del limit_or_schedule, until, ruleset
         runtime_expr = to_runtime_expr(expr)
         self._add_decls(runtime_expr, schedule)
         egg_schedule = self._state.schedule_to_egg(schedule.schedule)
         typed_expr = runtime_expr.__egg_typed_expr__
-        egg_expr = self._state.expr_to_egg(typed_expr.expr)
+        # Must also register type
+        egg_expr = self._state.typed_expr_to_egg(typed_expr)
         self._egraph.run_program(bindings.Simplify(egg_expr, egg_schedule))
         extract_report = self._egraph.extract_report()
         if not isinstance(extract_report, bindings.Best):
             msg = "No extract report saved"
             raise ValueError(msg)  # noqa: TRY004
         (new_typed_expr,) = self._state.exprs_from_egg(extract_report.termdag, [extract_report.term], typed_expr.tp)
         return cast(EXPR, RuntimeExpr.__from_value__(self.__egg_decls__, new_typed_expr))
@@ -1117,16 +1184,15 @@
         if not isinstance(extract_report, bindings.Variants):
             msg = "Wrong extract report type"
             raise ValueError(msg)  # noqa: TRY004
         new_exprs = self._state.exprs_from_egg(extract_report.termdag, extract_report.terms, typed_expr.tp)
         return [cast(EXPR, RuntimeExpr.__from_value__(self.__egg_decls__, expr)) for expr in new_exprs]
 
     def _run_extract(self, typed_expr: TypedExprDecl, n: int) -> bindings._ExtractReport:
-        self._state.type_ref_to_egg(typed_expr.tp)
-        expr = self._state.expr_to_egg(typed_expr.expr)
+        expr = self._state.typed_expr_to_egg(typed_expr)
         self._egraph.run_program(bindings.ActionCommand(bindings.Extract(expr, bindings.Lit(bindings.Int(n)))))
         extract_report = self._egraph.extract_report()
         if not extract_report:
             msg = "No extract report saved"
             raise ValueError(msg)
         return extract_report
 
@@ -1177,15 +1243,15 @@
     def eval(self, expr: Expr) -> object:
         """
         Evaluates the given expression (which must be a primitive type), returning the result.
         """
         runtime_expr = to_runtime_expr(expr)
         self._add_decls(runtime_expr)
         typed_expr = runtime_expr.__egg_typed_expr__
-        egg_expr = self._state.expr_to_egg(typed_expr.expr)
+        egg_expr = self._state.typed_expr_to_egg(typed_expr)
         match typed_expr.tp:
             case JustTypeRef("i64"):
                 return self._egraph.eval_i64(egg_expr)
             case JustTypeRef("f64"):
                 return self._egraph.eval_f64(egg_expr)
             case JustTypeRef("Bool"):
                 return self._egraph.eval_bool(egg_expr)
@@ -1874,15 +1940,15 @@
     """
     # Get the local scope from where the function is defined, so that we can get any type hints that are in the scope
     # but not in the globals
     globals = gen.__globals__.copy()
     if "Callable" not in globals:
         globals["Callable"] = Callable
     hints = get_type_hints(gen, globals, frame.f_locals)
-    args = [_var(p.name, hints[p.name]) for p in signature(gen).parameters.values()]
+    args = [_var(_rule_var_name(p.name), hints[p.name]) for p in signature(gen).parameters.values()]
     return list(gen(*args))  # type: ignore[misc]
 
 
 FactLike = Fact | Expr
 
 
 def _fact_likes(fact_likes: Iterable[FactLike]) -> tuple[Fact, ...]:
```

### Comparing `egglog-7.1.0/python/egglog/egraph_state.py` & `egglog-7.2.0/python/egglog/egraph_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from .declarations import *
 from .pretty import *
 from .type_constraint_solver import TypeConstraintError, TypeConstraintSolver
 
 if TYPE_CHECKING:
     from collections.abc import Iterable
 
-__all__ = ["EGraphState", "GLOBAL_PY_OBJECT_SORT"]
+__all__ = ["EGraphState", "GLOBAL_PY_OBJECT_SORT", "_rule_var_name"]
 
 # Create a global sort for python objects, so we can store them without an e-graph instance
 # Needed when serializing commands to egg commands when creating modules
 GLOBAL_PY_OBJECT_SORT = bindings.PyObjectSort()
 
 
 @dataclass
@@ -94,15 +94,16 @@
                         self.egraph.run_program(bindings.AddRuleset(name))
                     added_rules = self.rulesets[name] = set()
                 else:
                     added_rules = self.rulesets[name]
                 for rule in rules:
                     if rule in added_rules:
                         continue
-                    self.egraph.run_program(self.command_to_egg(rule, name))
+                    cmd = self.command_to_egg(rule, name)
+                    self.egraph.run_program(cmd)
                     added_rules.add(rule)
             case CombinedRulesetDecl(rulesets):
                 if name in self.rulesets:
                     return
                 self.rulesets[name] = set()
                 for ruleset in rulesets:
                     self.ruleset_to_egg(ruleset)
@@ -111,67 +112,77 @@
     def command_to_egg(self, cmd: CommandDecl, ruleset: str) -> bindings._Command:
         match cmd:
             case ActionCommandDecl(action):
                 return bindings.ActionCommand(self.action_to_egg(action))
             case RewriteDecl(tp, lhs, rhs, conditions) | BiRewriteDecl(tp, lhs, rhs, conditions):
                 self.type_ref_to_egg(tp)
                 rewrite = bindings.Rewrite(
-                    self.expr_to_egg(lhs),
-                    self.expr_to_egg(rhs),
+                    self._expr_to_egg(lhs),
+                    self._expr_to_egg(rhs),
                     [self.fact_to_egg(c) for c in conditions],
                 )
                 return (
                     bindings.RewriteCommand(ruleset, rewrite, cmd.subsume)
                     if isinstance(cmd, RewriteDecl)
                     else bindings.BiRewriteCommand(ruleset, rewrite)
                 )
             case RuleDecl(head, body, name):
                 rule = bindings.Rule(
                     [self.action_to_egg(a) for a in head],
                     [self.fact_to_egg(f) for f in body],
                 )
                 return bindings.RuleCommand(name or "", ruleset, rule)
+            case DefaultRewriteDecl(ref, expr):
+                decl = self.__egg_decls__.get_callable_decl(ref).to_function_decl()
+                sig = decl.signature
+                assert isinstance(sig, FunctionSignature)
+                args = tuple(
+                    TypedExprDecl(tp.to_just(), VarDecl(_rule_var_name(name)))
+                    for name, tp in zip(sig.arg_names, sig.arg_types, strict=False)
+                )
+                rewrite_decl = RewriteDecl(sig.semantic_return_type.to_just(), CallDecl(ref, args), expr, (), False)
+                return self.command_to_egg(rewrite_decl, ruleset)
             case _:
                 assert_never(cmd)
 
     def action_to_egg(self, action: ActionDecl) -> bindings._Action:
         match action:
             case LetDecl(name, typed_expr):
                 return bindings.Let(name, self.typed_expr_to_egg(typed_expr))
             case SetDecl(tp, call, rhs):
                 self.type_ref_to_egg(tp)
-                call_ = self.expr_to_egg(call)
-                return bindings.Set(call_.name, call_.args, self.expr_to_egg(rhs))
+                call_ = self._expr_to_egg(call)
+                return bindings.Set(call_.name, call_.args, self._expr_to_egg(rhs))
             case ExprActionDecl(typed_expr):
                 return bindings.Expr_(self.typed_expr_to_egg(typed_expr))
             case ChangeDecl(tp, call, change):
                 self.type_ref_to_egg(tp)
-                call_ = self.expr_to_egg(call)
+                call_ = self._expr_to_egg(call)
                 egg_change: bindings._Change
                 match change:
                     case "delete":
                         egg_change = bindings.Delete()
                     case "subsume":
                         egg_change = bindings.Subsume()
                     case _:
                         assert_never(change)
                 return bindings.Change(egg_change, call_.name, call_.args)
             case UnionDecl(tp, lhs, rhs):
                 self.type_ref_to_egg(tp)
-                return bindings.Union(self.expr_to_egg(lhs), self.expr_to_egg(rhs))
+                return bindings.Union(self._expr_to_egg(lhs), self._expr_to_egg(rhs))
             case PanicDecl(name):
                 return bindings.Panic(name)
             case _:
                 assert_never(action)
 
     def fact_to_egg(self, fact: FactDecl) -> bindings._Fact:
         match fact:
             case EqDecl(tp, exprs):
                 self.type_ref_to_egg(tp)
-                return bindings.Eq([self.expr_to_egg(e) for e in exprs])
+                return bindings.Eq([self._expr_to_egg(e) for e in exprs])
             case ExprFactDecl(typed_expr):
                 return bindings.Fact(self.typed_expr_to_egg(typed_expr))
             case _:
                 assert_never(fact)
 
     def callable_ref_to_egg(self, ref: CallableRef) -> str:
         """
@@ -197,16 +208,16 @@
                     assert isinstance(signature, FunctionSignature), "Cannot turn special function to egg"
                     egg_fn_decl = bindings.FunctionDecl(
                         egg_name,
                         bindings.Schema(
                             [self.type_ref_to_egg(a.to_just()) for a in signature.arg_types],
                             self.type_ref_to_egg(signature.semantic_return_type.to_just()),
                         ),
-                        self.expr_to_egg(decl.default) if decl.default else None,
-                        self.expr_to_egg(decl.merge) if decl.merge else None,
+                        self._expr_to_egg(decl.default) if decl.default else None,
+                        self._expr_to_egg(decl.merge) if decl.merge else None,
                         [self.action_to_egg(a) for a in decl.on_merge],
                         decl.cost,
                         decl.unextractable,
                     )
                     self.egraph.run_program(bindings.Function(egg_fn_decl))
             case _:
                 assert_never(decl)
@@ -241,14 +252,16 @@
             self.egraph.run_program(bindings.Sort(egg_name, args))
         # For builtin classes, let's also make sure we have the mapping of all egg fn names for class methods, because
         # these can be created even without adding them to the e-graph, like `vec-empty` which can be extracted
         # even if you never use that function.
         if decl.builtin:
             for method in decl.class_methods:
                 self.callable_ref_to_egg(ClassMethodRef(ref.name, method))
+            if decl.init:
+                self.callable_ref_to_egg(InitRef(ref.name))
 
         return egg_name
 
     def op_mapping(self) -> dict[str, str]:
         """
         Create a mapping of egglog function name to Python function name, for use in the serialized format
         for better visualization.
@@ -257,23 +270,23 @@
             k: pretty_callable_ref(self.__egg_decls__, next(iter(v)))
             for k, v in self.egg_fn_to_callable_refs.items()
             if len(v) == 1
         }
 
     def typed_expr_to_egg(self, typed_expr_decl: TypedExprDecl) -> bindings._Expr:
         self.type_ref_to_egg(typed_expr_decl.tp)
-        return self.expr_to_egg(typed_expr_decl.expr)
+        return self._expr_to_egg(typed_expr_decl.expr)
 
     @overload
-    def expr_to_egg(self, expr_decl: CallDecl) -> bindings.Call: ...
+    def _expr_to_egg(self, expr_decl: CallDecl) -> bindings.Call: ...
 
     @overload
-    def expr_to_egg(self, expr_decl: ExprDecl) -> bindings._Expr: ...
+    def _expr_to_egg(self, expr_decl: ExprDecl) -> bindings._Expr: ...
 
-    def expr_to_egg(self, expr_decl: ExprDecl) -> bindings._Expr:
+    def _expr_to_egg(self, expr_decl: ExprDecl) -> bindings._Expr:
         """
         Convert an ExprDecl to an egg expression.
 
         Cached using weakrefs to avoid memory leaks.
         """
         try:
             return self.expr_to_egg_cache[expr_decl]
@@ -303,15 +316,15 @@
             case CallDecl(ref, args, _):
                 egg_fn = self.callable_ref_to_egg(ref)
                 egg_args = [self.typed_expr_to_egg(a) for a in args]
                 res = bindings.Call(egg_fn, egg_args)
             case PyObjectDecl(value):
                 res = GLOBAL_PY_OBJECT_SORT.store(value)
             case PartialCallDecl(call_decl):
-                egg_fn_call = self.expr_to_egg(call_decl)
+                egg_fn_call = self._expr_to_egg(call_decl)
                 res = bindings.Call("unstable-fn", [bindings.Lit(bindings.String(egg_fn_call.name)), *egg_fn_call.args])
             case _:
                 assert_never(expr_decl.expr)
 
         self.expr_to_egg_cache[expr_decl] = res
         return res
 
@@ -351,14 +364,16 @@
         case (
             MethodRef(cls_name, name)
             | ClassMethodRef(cls_name, name)
             | ClassVariableRef(cls_name, name)
             | PropertyRef(cls_name, name)
         ):
             return f"{cls_name}_{name}"
+        case InitRef(cls_name):
+            return f"{cls_name}___init__"
         case _:
             assert_never(ref)
 
 
 @dataclass
 class FromEggState:
     """
@@ -423,34 +438,50 @@
         # Find the first callable ref that matches the call
         for callable_ref in self.state.egg_fn_to_callable_refs[term.name]:
             # If this is a classmethod, we might need the type params that were bound for this type
             # This could be multiple types if the classmethod is ambiguous, like map create.
             possible_types: Iterable[JustTypeRef | None]
             signature = self.decls.get_callable_decl(callable_ref).to_function_decl().signature
             assert isinstance(signature, FunctionSignature)
-            if isinstance(callable_ref, ClassMethodRef):
-                possible_types = self.state._get_possible_types(callable_ref.class_name)
+            if isinstance(callable_ref, ClassMethodRef | InitRef | MethodRef):
+                # Need OR in case we have class method whose class whas never added as a sort, which would happen
+                # if the class method didn't return that type and no other function did. In this case, we don't need
+                # to care about the type vars and we we don't need to bind any possible type.
+                possible_types = self.state._get_possible_types(callable_ref.class_name) or [None]
                 cls_name = callable_ref.class_name
             else:
                 possible_types = [None]
                 cls_name = None
             for possible_type in possible_types:
                 tcs = TypeConstraintSolver(self.decls)
                 if possible_type and possible_type.args:
                     tcs.bind_class(possible_type)
-
                 try:
                     arg_types, bound_tp_params = tcs.infer_arg_types(
                         signature.arg_types, signature.semantic_return_type, signature.var_arg_type, tp, cls_name
                     )
                 except TypeConstraintError:
                     continue
                 args = tuple(self.resolve_term(a, tp) for a, tp in zip(term.args, arg_types, strict=False))
-                return CallDecl(callable_ref, args, bound_tp_params)
+
+                return CallDecl(
+                    callable_ref,
+                    args,
+                    # Don't include bound type params if this is just a method, we only needed them for type resolution
+                    # but dont need to store them
+                    bound_tp_params if isinstance(callable_ref, ClassMethodRef | InitRef) else None,
+                )
         raise ValueError(f"Could not find callable ref for call {term}")
 
     def resolve_term(self, term_id: int, tp: JustTypeRef) -> TypedExprDecl:
         try:
             return self.cache[term_id]
         except KeyError:
             res = self.cache[term_id] = self.from_expr(tp, self.termdag.nodes[term_id])
             return res
+
+
+def _rule_var_name(s: str) -> str:
+    """
+    Create a hidden variable name, for rewrites, so that let bindings or function won't conflict with it
+    """
+    return f"__var__{s}"
```

### Comparing `egglog-7.1.0/python/egglog/examples/bool.py` & `egglog-7.2.0/python/egglog/examples/bool.py`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/python/egglog/examples/eqsat_basic.py` & `egglog-7.2.0/python/egglog/examples/eqsat_basic.py`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/python/egglog/examples/lambda_.py` & `egglog-7.2.0/python/egglog/examples/lambda_.py`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/python/egglog/examples/matrix.py` & `egglog-7.2.0/python/egglog/examples/matrix.py`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/python/egglog/examples/ndarrays.py` & `egglog-7.2.0/python/egglog/examples/ndarrays.py`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/python/egglog/examples/resolution.py` & `egglog-7.2.0/python/egglog/examples/resolution.py`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/python/egglog/examples/schedule_demo.py` & `egglog-7.2.0/python/egglog/examples/schedule_demo.py`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/python/egglog/exp/array_api.py` & `egglog-7.2.0/python/egglog/exp/array_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -878,15 +878,18 @@
 
 converter(type(None), OptionalIntOrTuple, lambda _: OptionalIntOrTuple.none)
 converter(IntOrTuple, OptionalIntOrTuple, OptionalIntOrTuple.some)
 
 
 @function
 def asarray(
-    a: NDArray, dtype: OptionalDType = OptionalDType.none, copy: OptionalBool = OptionalBool.none
+    a: NDArray,
+    dtype: OptionalDType = OptionalDType.none,
+    copy: OptionalBool = OptionalBool.none,
+    device: OptionalDevice = OptionalDevice.none,
 ) -> NDArray: ...
 
 
 @array_api_ruleset.register
 def _assarray(a: NDArray, d: OptionalDType, ob: OptionalBool):
     yield rewrite(asarray(a, d, ob).ndim).to(a.ndim)  # asarray doesn't change ndim
     yield rewrite(asarray(a)).to(a)
```

### Comparing `egglog-7.1.0/python/egglog/exp/array_api_jit.py` & `egglog-7.2.0/python/egglog/exp/array_api_jit.py`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/python/egglog/exp/array_api_numba.py` & `egglog-7.2.0/python/egglog/exp/array_api_numba.py`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/python/egglog/exp/array_api_program_gen.py` & `egglog-7.2.0/python/egglog/exp/array_api_program_gen.py`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/python/egglog/exp/program_gen.py` & `egglog-7.2.0/python/egglog/exp/program_gen.py`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/python/egglog/exp/siu_examples.py` & `egglog-7.2.0/python/egglog/exp/siu_examples.py`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/python/egglog/graphviz_widget.py` & `egglog-7.2.0/python/egglog/graphviz_widget.py`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/python/egglog/ipython_magic.py` & `egglog-7.2.0/python/egglog/ipython_magic.py`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/python/egglog/pretty.py` & `egglog-7.2.0/python/egglog/pretty.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,26 +162,30 @@
                 self(d.expr)
             case ChangeDecl(_, d, _) | SaturateDecl(d) | RepeatDecl(d, _) | ActionCommandDecl(d):
                 self(d)
             case PanicDecl(_) | VarDecl(_) | LitDecl(_) | PyObjectDecl(_):
                 pass
             case EqDecl(_, decls) | SequenceDecl(decls) | RulesetDecl(decls):
                 for de in decls:
+                    if isinstance(de, DefaultRewriteDecl):
+                        continue
                     self(de)
             case CallDecl(_, exprs, _):
                 for e in exprs:
                     self(e.expr)
             case RunDecl(_, until):
                 if until:
                     for f in until:
                         self(f)
             case PartialCallDecl(c):
                 self(c)
             case CombinedRulesetDecl(_):
                 pass
+            case DefaultRewriteDecl():
+                pass
             case _:
                 assert_never(decl)
 
         self._seen.add(decl)
 
 
 @dataclass
@@ -272,15 +276,15 @@
                 return f"panic({s!r})", "action"
             case EqDecl(_, exprs):
                 first, *rest = exprs
                 return f"eq({self(first)}).to({', '.join(map(self, rest))})", "fact"
             case RulesetDecl(rules):
                 if ruleset_name:
                     return f"ruleset(name={ruleset_name!r})", f"ruleset_{ruleset_name}"
-                args = ", ".join(map(self, rules))
+                args = ", ".join(self(r) for r in rules if not isinstance(r, DefaultRewriteDecl))
                 return f"ruleset({args})", "ruleset"
             case CombinedRulesetDecl(rulesets):
                 if ruleset_name:
                     rulesets = (*rulesets, f"name={ruleset_name!r})")
                 return f"unstable_combine_rulesets({', '.join(rulesets)})", "combined_ruleset"
             case SaturateDecl(schedule):
                 return f"{self(schedule, parens=True)}.saturate()", "schedule"
@@ -294,14 +298,17 @@
             case RunDecl(ruleset_name, until):
                 ruleset = self.decls._rulesets[ruleset_name]
                 ruleset_str = self(ruleset, ruleset_name=ruleset_name)
                 if not until:
                     return ruleset_str, "schedule"
                 args = ", ".join(map(self, until))
                 return f"run({ruleset_str}, {args})", "schedule"
+            case DefaultRewriteDecl():
+                msg = "default rewrites should not be pretty printed"
+                raise TypeError(msg)
         assert_never(decl)
 
     def _call(
         self,
         decl: CallDecl,
         parens: bool,
     ) -> tuple[str, str]:
@@ -366,18 +373,16 @@
         """
         Pretty print the call, returning either the full function call or a tuple of the function and the args.
         """
         match ref:
             case FunctionRef(name):
                 return name, args
             case ClassMethodRef(class_name, method_name):
-                fn_str = str(JustTypeRef(class_name, bound_tp_params or ()))
-                if method_name != "__init__":
-                    fn_str += f".{method_name}"
-                return fn_str, args
+                tp_ref = JustTypeRef(class_name, bound_tp_params or ())
+                return f"{tp_ref}.{method_name}", args
             case MethodRef(_class_name, method_name):
                 slf, *args = args
                 slf = self(slf, parens=True)
                 match method_name:
                     case _ if method_name in UNARY_METHODS:
                         expr = f"{UNARY_METHODS[method_name]}{slf}"
                         return f"({expr})" if parens else expr
@@ -396,14 +401,17 @@
                         return f"{slf}.{method_name}", args
             case ConstantRef(name):
                 return name
             case ClassVariableRef(class_name, variable_name):
                 return f"{class_name}.{variable_name}"
             case PropertyRef(_class_name, property_name):
                 return f"{self(args[0], parens=True)}.{property_name}"
+            case InitRef(class_name):
+                tp_ref = JustTypeRef(class_name, bound_tp_params or ())
+                return str(tp_ref), args
         assert_never(ref)
 
     def _generate_name(self, typ: str) -> str:
         self._gen_name_types[typ] += 1
         return f"_{typ}_{self._gen_name_types[typ]}"
 
     def _name_expr(self, tp_name: str, expr_str: str, copy_identifier: bool) -> str:
@@ -430,14 +438,16 @@
             return name
         case (
             ClassMethodRef(class_name, method_name)
             | MethodRef(class_name, method_name)
             | PropertyRef(class_name, method_name)
         ):
             return f"{class_name}.{method_name}"
+        case InitRef(class_name):
+            return class_name
         case ConstantRef(_):
             msg = "Constants should not be callable"
             raise NotImplementedError(msg)
         case ClassVariableRef(_, _):
             msg = "Class variables should not be callable"
             raise NotADirectoryError(msg)
     assert_never(ref)
```

### Comparing `egglog-7.1.0/python/egglog/runtime.py` & `egglog-7.2.0/python/egglog/runtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,18 +159,16 @@
                 self.__egg_decls__, TypedExprDecl(self.__egg_tp__.to_just(), LitDecl(args[0]))
             )
         if name == UNIT_CLASS_NAME:
             assert len(args) == 0
             return RuntimeExpr.__from_value__(
                 self.__egg_decls__, TypedExprDecl(self.__egg_tp__.to_just(), LitDecl(None))
             )
-
-        return RuntimeFunction(
-            Thunk.value(self.__egg_decls__), ClassMethodRef(name, "__init__"), self.__egg_tp__.to_just()
-        )(*args, **kwargs)  # type: ignore[arg-type]
+        fn = RuntimeFunction(Thunk.value(self.__egg_decls__), InitRef(name), self.__egg_tp__.to_just())
+        return fn(*args, **kwargs)  # type: ignore[arg-type]
 
     def __dir__(self) -> list[str]:
         cls_decl = self.__egg_decls__.get_class_decl(self.__egg_tp__.name)
         possible_methods = (
             list(cls_decl.class_methods) + list(cls_decl.class_variables) + list(cls_decl.preserved_methods)
         )
         if "__init__" in possible_methods:
@@ -273,15 +271,18 @@
             )
         else:
             function_value = None
             assert isinstance(signature, FunctionSignature)
 
         # Turn all keyword args into positional args
         py_signature = to_py_signature(signature, self.__egg_decls__, _egg_partial_function)
-        bound = py_signature.bind(*args, **kwargs)
+        try:
+            bound = py_signature.bind(*args, **kwargs)
+        except TypeError as err:
+            raise TypeError(f"Failed to call {self} with args {args} and kwargs {kwargs}") from err
         del kwargs
         bound.apply_defaults()
         assert not bound.kwargs
         args = bound.args
 
         upcasted_args = [
             resolve_literal(cast(TypeOrVarRef, tp), arg)
@@ -306,15 +307,17 @@
             tcs.bind_class(bound_tp)
         arg_exprs = tuple(arg.__egg_typed_expr__ for arg in upcasted_args)
         arg_types = [expr.tp for expr in arg_exprs]
         cls_name = bound_tp.name if bound_tp else None
         return_tp = tcs.infer_return_type(
             signature.arg_types, signature.semantic_return_type, signature.var_arg_type, arg_types, cls_name
         )
-        bound_params = cast(JustTypeRef, bound_tp).args if isinstance(self.__egg_ref__, ClassMethodRef) else None
+        bound_params = (
+            cast(JustTypeRef, bound_tp).args if isinstance(self.__egg_ref__, ClassMethodRef | InitRef) else None
+        )
         # If we were using unstable-app to call a funciton, add that function back as the first arg.
         if function_value:
             arg_exprs = (function_value, *arg_exprs)
         expr_decl = CallDecl(self.__egg_ref__, arg_exprs, bound_params)
         typed_expr_decl = TypedExprDecl(return_tp, expr_decl)
         # If there is not return type, we are mutating the first arg
         if not signature.return_type:
```

### Comparing `egglog-7.1.0/python/egglog/thunk.py` & `egglog-7.2.0/python/egglog/thunk.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 @dataclass
 class Thunk(Generic[T, Unpack[TS]]):
     """
     Cached delayed function call.
     """
 
-    state: Resolved[T] | Unresolved[T, Unpack[TS]] | Resolving[T]
+    state: Resolved[T] | Unresolved[T, Unpack[TS]] | Resolving[T] | Error
 
     @classmethod
     def fn(
         cls, fn: Callable[[Unpack[TS]], T], *args: Unpack[TS], fallback: Callable[[], T] | None = None
     ) -> Thunk[T, Unpack[TS]]:
         """
         Create a thunk based on some functions and some partial args.
@@ -40,22 +40,29 @@
 
     def __call__(self) -> T:
         match self.state:
             case Resolved(value):
                 return value
             case Unresolved(fn, args, fallback):
                 self.state = Resolving(fallback)
-                res = fn(*args)
-                self.state = Resolved(res)
-                return res
+                try:
+                    res = fn(*args)
+                except Exception as e:
+                    self.state = Error(e)
+                    raise
+                else:
+                    self.state = Resolved(res)
+                    return res
             case Resolving(fallback):
                 if fallback is None:
                     msg = "Recursively resolving thunk without fallback"
                     raise ValueError(msg)
                 return fallback()
+            case Error(e):
+                raise e
 
 
 @dataclass
 class Resolved(Generic[T]):
     value: T
 
 
@@ -65,7 +72,12 @@
     args: tuple[Unpack[TS]]
     fallback: Callable[[], T] | None
 
 
 @dataclass
 class Resolving(Generic[T]):
     fallback: Callable[[], T] | None
+
+
+@dataclass
+class Error:
+    e: Exception
```

### Comparing `egglog-7.1.0/python/egglog/type_constraint_solver.py` & `egglog-7.2.0/python/egglog/type_constraint_solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,17 +75,18 @@
     ) -> tuple[Iterable[JustTypeRef], tuple[JustTypeRef, ...] | None]:
         """
         Given a return type, infer the argument types. If there is a variable arg, it returns an infinite iterable.
 
         Also returns the bound type params if the class name is passed in.
         """
         self._infer_typevars(fn_return, return_, cls_name)
-        arg_types = (
-            self._subtitute_typevars(a, cls_name) for a in chain(fn_args, repeat(fn_var_args) if fn_var_args else [])
-        )
+        arg_types: Iterable[JustTypeRef] = [self._subtitute_typevars(a, cls_name) for a in fn_args]
+        if fn_var_args:
+            # Need to be generator so it can be infinite for variable args
+            arg_types = chain(arg_types, repeat(self._subtitute_typevars(fn_var_args, cls_name)))
         bound_typevars = (
             tuple(
                 v
                 # Sort by the index of the typevar in the class
                 for _, v in sorted(
                     self._cls_typevar_index_to_type[cls_name].items(),
                     key=lambda kv: self._decls.get_class_decl(cls_name).type_vars.index(kv[0]),
@@ -128,15 +129,15 @@
                     class_typevars[typevar] = arg
             case _:
                 assert_never(fn_arg)
 
     def _subtitute_typevars(self, tp: TypeOrVarRef, cls_name: str | None) -> JustTypeRef:
         match tp:
             case ClassTypeVarRef(name):
+                assert cls_name is not None
                 try:
-                    assert cls_name is not None
                     return self._cls_typevar_index_to_type[cls_name][name]
                 except KeyError as e:
                     raise TypeConstraintError(f"Not enough bound typevars for {tp}") from e
             case TypeRefWithVars(name, args):
                 return JustTypeRef(name, tuple(self._subtitute_typevars(arg, name) for arg in args))
         assert_never(tp)
```

### Comparing `egglog-7.1.0/python/egglog/widget.js` & `egglog-7.2.0/python/egglog/widget.js`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/python/tests/__snapshots__/test_array_api/TestLDA.test_optimize.py` & `egglog-7.2.0/python/tests/__snapshots__/test_array_api/TestLDA.test_optimize.py`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/python/tests/__snapshots__/test_array_api/TestLDA.test_source_optimized.py` & `egglog-7.2.0/python/tests/__snapshots__/test_array_api/TestLDA.test_source_optimized.py`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/python/tests/__snapshots__/test_array_api/TestLDA.test_trace.py` & `egglog-7.2.0/python/tests/__snapshots__/test_array_api/TestLDA.test_trace.py`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/python/tests/conftest.py` & `egglog-7.2.0/python/tests/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 
 
 @pytest.fixture(autouse=True)
 def _reset_conversions():
     import egglog.conversion
 
     old_conversions = copy.copy(egglog.conversion.CONVERSIONS)
+    old_conversion_decls = copy.copy(egglog.conversion.CONVERSIONS_DECLS)
     yield
     egglog.conversion.CONVERSIONS = old_conversions
+    egglog.conversion.CONVERSIONS_DECLS = old_conversion_decls
 
 
 class PythonSnapshotExtension(SingleFileSnapshotExtension):
     _file_extension = "py"
 
     def serialize(self, data, **kwargs) -> bytes:
         return str(data).encode()
```

### Comparing `egglog-7.1.0/python/tests/test_array_api.py` & `egglog-7.2.0/python/tests/test_array_api.py`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/python/tests/test_bindings.py` & `egglog-7.2.0/python/tests/test_bindings.py`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/python/tests/test_convert.py` & `egglog-7.2.0/python/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/python/tests/test_high_level.py` & `egglog-7.2.0/python/tests/test_high_level.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # mypy: disable-error-code="empty-body"
 from __future__ import annotations
 
 import importlib
 import pathlib
 from copy import copy
-from typing import ClassVar, Union
+from typing import ClassVar, TypeAlias, Union
 
 import pytest
 
 from egglog import *
 from egglog.declarations import (
     CallDecl,
     FunctionRef,
@@ -479,15 +479,15 @@
     # i.e. Int(x) + NDArray(y) -> NDArray(Int(x)) + NDArray(y) instead of Int(x) + NDArray(y).to_int()
 
     class Int(Expr):
         def __init__(self, name: StringLike) -> None: ...
 
         def __add__(self, other: Int) -> Int: ...
 
-    NDArrayLike = Union[Int, "NDArray"]
+    NDArrayLike: TypeAlias = Union[Int, "NDArray"]
 
     class NDArray(Expr):
         def __init__(self, name: StringLike) -> None: ...
 
         def __add__(self, other: NDArrayLike) -> NDArray: ...
 
         def __radd__(self, other: NDArrayLike) -> NDArray: ...
@@ -644,7 +644,120 @@
     class A(Expr):
         def __init__(self) -> None: ...
 
         @property
         def b(self) -> i64: ...
 
     assert expr_parts(A.b(A())) == expr_parts(A().b)
+
+
+class A(Expr):
+    def __init__(self) -> None: ...
+
+
+class TestDefaultReplacements:
+    def test_function(self):
+        @function
+        def f() -> A:
+            return A()
+
+        check_eq(f(), A(), run())
+
+    def test_function_ruleset(self):
+        r = ruleset()
+
+        @function(ruleset=r)
+        def f() -> A:
+            return A()
+
+        check_eq(f(), A(), r)
+
+    def test_constant(self):
+        a = constant("a", A, A())
+        check_eq(a, A(), run())
+
+    def test_constant_ruleset(self):
+        r = ruleset()
+        a = constant("a", A, A(), ruleset=r)
+
+        check_eq(a, A(), r)
+
+    def test_method(self):
+        class B(Expr):
+            def __init__(self) -> None: ...
+            def f(self) -> A:
+                return A()
+
+        check_eq(B().f(), A(), run())
+
+    def test_method_ruleset(self):
+        r = ruleset()
+
+        class B(Expr, ruleset=r):
+            def __init__(self) -> None: ...
+            def f(self) -> A:
+                return A()
+
+        check_eq(B().f(), A(), r)
+
+    def test_classmethod(self):
+        class B(Expr):
+            @classmethod
+            def f(cls) -> A:
+                return A()
+
+        check_eq(B.f(), A(), run())
+
+    def test_classmethod_ruleset(self):
+        r = ruleset()
+
+        class B(Expr, ruleset=r):
+            @classmethod
+            def f(cls) -> A:
+                return A()
+
+        check_eq(B.f(), A(), r)
+
+    def test_classvar(self):
+        class B(Expr):
+            a: ClassVar[A] = A()
+
+        check_eq(B.a, A(), run())
+
+    def test_classvar_ruleset(self):
+        r = ruleset()
+
+        class B(Expr, ruleset=r):
+            a: ClassVar[A] = A()
+
+        check_eq(B.a, A(), r)
+
+    def test_method_refer_to_later(self):
+        """
+        Verify that an earlier method body can refer to values defined in later ones
+        """
+
+        class B(Expr):
+            def __init__(self) -> None: ...
+            def f(self) -> A:
+                return self.g()
+
+            def g(self) -> A: ...
+
+        B()
+        left = B().f()
+        right = B().g()
+        check_eq(left, right, run())
+
+
+class TestIssue166:
+    """
+    Raised by @cgyurgyik in https://github.com/egraphs-good/egglog-python/issues/166
+    """
+
+    def test_inserting_map(self):
+        egraph = EGraph()
+        m = egraph.let("map", Map[String, i64].empty().insert(String("a"), i64(42)))
+        egraph.simplify(m, 5)
+
+    def test_creating_map(self):
+        EGraph().simplify(Map[String, i64].empty(), 1)
```

### Comparing `egglog-7.1.0/python/tests/test_modules.py` & `egglog-7.2.0/python/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/python/tests/test_pretty.py` & `egglog-7.2.0/python/tests/test_pretty.py`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/python/tests/test_program_gen.py` & `egglog-7.2.0/python/tests/test_program_gen.py`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/python/tests/test_py_object_sort.py` & `egglog-7.2.0/python/tests/test_py_object_sort.py`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/python/tests/test_runtime.py` & `egglog-7.2.0/python/tests/test_runtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,14 @@
         ),
     )
 
 
 def test_class_variable():
     decls = Declarations(
         _classes={
-            "i64": ClassDecl(class_variables={"one": ConstantDecl(JustTypeRef("i64"))}),
+            "i64": ClassDecl(class_variables={"one": ConstantDecl(JustTypeRef("i64"), None)}),
         },
     )
     i64 = RuntimeClass(Thunk.value(decls), TypeRefWithVars("i64"))
     one = i64.one
     assert isinstance(one, RuntimeExpr)
     assert one.__egg_typed_expr__ == TypedExprDecl(JustTypeRef("i64"), CallDecl(ClassVariableRef("i64", "one")))
```

### Comparing `egglog-7.1.0/python/tests/test_type_constraint_solver.py` & `egglog-7.2.0/python/tests/test_type_constraint_solver.py`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/python/tests/test_typing.py` & `egglog-7.2.0/python/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/python/tests/test_unstable_fn.py` & `egglog-7.2.0/python/tests/test_unstable_fn.py`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/src/conversions.rs` & `egglog-7.2.0/src/conversions.rs`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/src/egraph.rs` & `egglog-7.2.0/src/egraph.rs`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/src/error.rs` & `egglog-7.2.0/src/error.rs`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/src/lib.rs` & `egglog-7.2.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/src/py_object_sort.rs` & `egglog-7.2.0/src/py_object_sort.rs`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/src/serialize.rs` & `egglog-7.2.0/src/serialize.rs`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/src/utils.rs` & `egglog-7.2.0/src/utils.rs`

 * *Files identical despite different names*

### Comparing `egglog-7.1.0/Cargo.lock` & `egglog-7.2.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -308,15 +308,15 @@
  "smallvec",
  "symbol_table",
  "thiserror",
 ]
 
 [[package]]
 name = "egglog-python"
-version = "7.1.0"
+version = "7.2.0"
 dependencies = [
  "egglog",
  "egraph-serialize",
  "lalrpop-util",
  "log",
  "num-rational",
  "ordered-float",
```

### Comparing `egglog-7.1.0/PKG-INFO` & `egglog-7.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: egglog
-Version: 7.1.0
+Version: 7.2.0
 Classifier: Environment :: MacOS X
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -26,35 +26,35 @@
 Requires-Dist: pytest-codspeed; extra == 'test'
 Requires-Dist: pytest-benchmark; extra == 'test'
 Requires-Dist: pytest-xdist; extra == 'test'
 Requires-Dist: scikit-learn; extra == 'array'
 Requires-Dist: array_api_compat; extra == 'array'
 Requires-Dist: numba==0.59.1; extra == 'array'
 Requires-Dist: llvmlite==0.42.0; extra == 'array'
+Requires-Dist: pre-commit; extra == 'dev'
+Requires-Dist: ruff; extra == 'dev'
+Requires-Dist: mypy; extra == 'dev'
+Requires-Dist: anywidget[dev]; extra == 'dev'
+Requires-Dist: egglog[docs,test]; extra == 'dev'
 Requires-Dist: pydata-sphinx-theme; extra == 'docs'
 Requires-Dist: myst-nb; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints; extra == 'docs'
 Requires-Dist: sphinx-gallery; extra == 'docs'
 Requires-Dist: nbconvert; extra == 'docs'
 Requires-Dist: matplotlib; extra == 'docs'
 Requires-Dist: anywidget; extra == 'docs'
 Requires-Dist: seaborn; extra == 'docs'
 Requires-Dist: egglog[array]; extra == 'docs'
 Requires-Dist: line-profiler; extra == 'docs'
 Requires-Dist: sphinxcontrib-mermaid; extra == 'docs'
 Requires-Dist: ablog; extra == 'docs'
-Requires-Dist: pre-commit; extra == 'dev'
-Requires-Dist: ruff; extra == 'dev'
-Requires-Dist: mypy; extra == 'dev'
-Requires-Dist: anywidget[dev]; extra == 'dev'
-Requires-Dist: egglog[docs,test]; extra == 'dev'
 Provides-Extra: test
 Provides-Extra: array
-Provides-Extra: docs
 Provides-Extra: dev
+Provides-Extra: docs
 License-File: LICENSE
 Summary: e-graphs in Python built around the the egglog rust library
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # `egglog` Python wrapper
```

