# Comparing `tmp/sqlfluff-3.0.6.tar.gz` & `tmp/sqlfluff-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlfluff-3.0.6.tar", last modified: Mon May  6 19:38:40 2024, max compression
+gzip compressed data, was "sqlfluff-3.0.7.tar", last modified: Thu May 23 09:39:51 2024, max compression
```

## Comparing `sqlfluff-3.0.6.tar` & `sqlfluff-3.0.7.tar`

### file list

```diff
@@ -1,273 +1,273 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.983252 sqlfluff-3.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)   507355 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-05-06 19:38:40.983252 sqlfluff-3.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     8367 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 19:38:40.983252 sqlfluff-3.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.927252 sqlfluff-3.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.931252 sqlfluff-3.0.6/src/sqlfluff/
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.935252 sqlfluff-3.0.6/src/sqlfluff/api/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/api/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/api/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.935252 sqlfluff-3.0.6/src/sqlfluff/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/cli/autocomplete.py
--rw-r--r--   0 runner    (1001) docker     (127)    51559 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    26128 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/cli/formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/cli/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/cli/outputstream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.939252 sqlfluff-3.0.6/src/sqlfluff/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45221 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12738 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/default_config.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.939252 sqlfluff-3.0.6/src/sqlfluff/core/dialects/
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/dialects/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/dialects/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    12243 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.939252 sqlfluff-3.0.6/src/sqlfluff/core/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/helpers/dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/helpers/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/helpers/slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/helpers/string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.939252 sqlfluff-3.0.6/src/sqlfluff/core/linter/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/linter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/linter/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/linter/fix.py
--rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/linter/linted_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)    17070 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/linter/linted_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    47948 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/linter/linter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/linter/linting_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    12847 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/linter/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/linter/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.943252 sqlfluff-3.0.6/src/sqlfluff/core/parser/
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13372 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.943252 sqlfluff-3.0.6/src/sqlfluff/core/parser/grammar/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/grammar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11911 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/grammar/anyof.py
--rw-r--r--   0 runner    (1001) docker     (127)    19771 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/grammar/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/grammar/conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/grammar/delimited.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/grammar/noncode.py
--rw-r--r--   0 runner    (1001) docker     (127)    26538 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/grammar/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    36075 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/lexer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9730 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/markers.py
--rw-r--r--   0 runner    (1001) docker     (127)    28332 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/match_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)    11753 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/match_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/matchable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    11439 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.947252 sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49362 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/bracketed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/keyword.py
--rw-r--r--   0 runner    (1001) docker     (127)     9440 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/raw.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/parser/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.947252 sqlfluff-3.0.6/src/sqlfluff/core/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/plugin/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/plugin/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/plugin/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.951252 sqlfluff-3.0.6/src/sqlfluff/core/rules/
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48881 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/rules/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8938 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/rules/config_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/rules/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/rules/crawlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/rules/doc_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    17908 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/rules/fix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/rules/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    13500 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/rules/noqa.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/rules/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.951252 sqlfluff-3.0.6/src/sqlfluff/core/templaters/
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/templaters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23058 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/templaters/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    45600 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/templaters/jinja.py
--rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/templaters/placeholder.py
--rw-r--r--   0 runner    (1001) docker     (127)    46401 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/templaters/python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.951252 sqlfluff-3.0.6/src/sqlfluff/core/templaters/slicers/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/templaters/slicers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35992 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/templaters/slicers/tracer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/core/timing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.963252 sqlfluff-3.0.6/src/sqlfluff/dialects/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   139271 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_ansi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_ansi_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    22826 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_athena.py
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_athena_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    82970 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_bigquery_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    40104 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_clickhouse_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)     8751 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_databricks.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_databricks_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    17402 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_db2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_db2_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    18370 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_duckdb.py
--rw-r--r--   0 runner    (1001) docker     (127)    93480 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_exasol.py
--rw-r--r--   0 runner    (1001) docker     (127)    15655 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_exasol_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    19408 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_greenplum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_greenplum_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    33399 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_hive.py
--rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_hive_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    29892 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_materialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_materialize_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    82604 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_mysql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    28793 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_oracle.py
--rw-r--r--   0 runner    (1001) docker     (127)   192309 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)    37092 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_postgres_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    73019 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_redshift.py
--rw-r--r--   0 runner    (1001) docker     (127)     9669 2024-05-06 19:38:30.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_redshift_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)   242793 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_snowflake.py
--rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_snowflake_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_soql.py
--rw-r--r--   0 runner    (1001) docker     (127)   105781 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_sparksql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_sparksql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    20606 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_sqlite_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    28146 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_teradata.py
--rw-r--r--   0 runner    (1001) docker     (127)    11953 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_trino.py
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_trino_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)   194021 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_tsql.py
--rw-r--r--   0 runner    (1001) docker     (127)    12783 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_tsql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    66185 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_vertica.py
--rw-r--r--   0 runner    (1001) docker     (127)     6277 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_vertica_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/diff_quality_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.963252 sqlfluff-3.0.6/src/sqlfluff/rules/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.963252 sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/
--rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL01.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL02.py
--rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL03.py
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL04.py
--rw-r--r--   0 runner    (1001) docker     (127)    11267 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL05.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL06.py
--rw-r--r--   0 runner    (1001) docker     (127)    10982 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL07.py
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL08.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL09.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.967252 sqlfluff-3.0.6/src/sqlfluff/rules/ambiguous/
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/ambiguous/AM01.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/ambiguous/AM02.py
--rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/ambiguous/AM03.py
--rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/ambiguous/AM04.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/ambiguous/AM05.py
--rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/ambiguous/AM06.py
--rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/ambiguous/AM07.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/ambiguous/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.967252 sqlfluff-3.0.6/src/sqlfluff/rules/capitalisation/
--rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/capitalisation/CP01.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/capitalisation/CP02.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/capitalisation/CP03.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/capitalisation/CP04.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/capitalisation/CP05.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/capitalisation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.971252 sqlfluff-3.0.6/src/sqlfluff/rules/convention/
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV01.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV02.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV03.py
--rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV04.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV05.py
--rw-r--r--   0 runner    (1001) docker     (127)    14963 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV06.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV07.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV08.py
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV09.py
--rw-r--r--   0 runner    (1001) docker     (127)    11947 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV10.py
--rw-r--r--   0 runner    (1001) docker     (127)    16354 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV11.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/convention/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.971252 sqlfluff-3.0.6/src/sqlfluff/rules/jinja/
--rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/jinja/JJ01.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/jinja/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.971252 sqlfluff-3.0.6/src/sqlfluff/rules/layout/
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT01.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT02.py
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT03.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT04.py
--rw-r--r--   0 runner    (1001) docker     (127)     6092 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT05.py
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT06.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT07.py
--rw-r--r--   0 runner    (1001) docker     (127)     8279 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT08.py
--rw-r--r--   0 runner    (1001) docker     (127)    16989 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT09.py
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT10.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT11.py
--rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT12.py
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT13.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/layout/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.975252 sqlfluff-3.0.6/src/sqlfluff/rules/references/
--rw-r--r--   0 runner    (1001) docker     (127)     9008 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/references/RF01.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/references/RF02.py
--rw-r--r--   0 runner    (1001) docker     (127)    11350 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/references/RF03.py
--rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/references/RF04.py
--rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/references/RF05.py
--rw-r--r--   0 runner    (1001) docker     (127)     8506 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/references/RF06.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/references/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.975252 sqlfluff-3.0.6/src/sqlfluff/rules/structure/
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST01.py
--rw-r--r--   0 runner    (1001) docker     (127)    10049 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST02.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST03.py
--rw-r--r--   0 runner    (1001) docker     (127)     9713 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST04.py
--rw-r--r--   0 runner    (1001) docker     (127)    20587 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST05.py
--rw-r--r--   0 runner    (1001) docker     (127)     9623 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST06.py
--rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST07.py
--rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST08.py
--rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST09.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/structure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.975252 sqlfluff-3.0.6/src/sqlfluff/rules/tsql/
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/tsql/TQ01.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/rules/tsql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.979252 sqlfluff-3.0.6/src/sqlfluff/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.979252 sqlfluff-3.0.6/src/sqlfluff/utils/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16342 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/analysis/query.py
--rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/analysis/select.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.979252 sqlfluff-3.0.6/src/sqlfluff/utils/functional/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/functional/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/functional/raw_file_slice_predicates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/functional/raw_file_slices.py
--rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/functional/segment_predicates.py
--rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/functional/segments.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/functional/templated_file_slice_predicates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/functional/templated_file_slices.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/identifers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.983252 sqlfluff-3.0.6/src/sqlfluff/utils/reflow/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/reflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/reflow/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7051 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/reflow/depthmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    32545 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/reflow/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/reflow/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    23067 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/reflow/rebreak.py
--rw-r--r--   0 runner    (1001) docker     (127)    94663 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/reflow/reindent.py
--rw-r--r--   0 runner    (1001) docker     (127)    24129 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/reflow/respace.py
--rw-r--r--   0 runner    (1001) docker     (127)    25529 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/reflow/sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.983252 sqlfluff-3.0.6/src/sqlfluff/utils/testing/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/testing/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/testing/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     8794 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/src/sqlfluff/utils/testing/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.983252 sqlfluff-3.0.6/src/sqlfluff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-05-06 19:38:40.000000 sqlfluff-3.0.6/src/sqlfluff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-05-06 19:38:40.000000 sqlfluff-3.0.6/src/sqlfluff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 19:38:40.000000 sqlfluff-3.0.6/src/sqlfluff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-06 19:38:40.000000 sqlfluff-3.0.6/src/sqlfluff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-06 19:38:40.000000 sqlfluff-3.0.6/src/sqlfluff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-06 19:38:40.000000 sqlfluff-3.0.6/src/sqlfluff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:38:40.983252 sqlfluff-3.0.6/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-06 19:38:31.000000 sqlfluff-3.0.6/test/testing_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:51.480547 sqlfluff-3.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)   510086 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11986 2024-05-23 09:39:51.480547 sqlfluff-3.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8558 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 09:39:51.480547 sqlfluff-3.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:51.424546 sqlfluff-3.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:51.428546 sqlfluff-3.0.7/src/sqlfluff/
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:51.432546 sqlfluff-3.0.7/src/sqlfluff/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/api/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/api/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:51.432546 sqlfluff-3.0.7/src/sqlfluff/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/cli/autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51559 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26128 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/cli/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/cli/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/cli/outputstream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:51.436546 sqlfluff-3.0.7/src/sqlfluff/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45221 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12738 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/default_config.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:51.436546 sqlfluff-3.0.7/src/sqlfluff/core/dialects/
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/dialects/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/dialects/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12243 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:51.436546 sqlfluff-3.0.7/src/sqlfluff/core/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/helpers/dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/helpers/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/helpers/slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/helpers/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:51.440546 sqlfluff-3.0.7/src/sqlfluff/core/linter/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/linter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/linter/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/linter/fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9624 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/linter/linted_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17070 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/linter/linted_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47948 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/linter/linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/linter/linting_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12847 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/linter/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/linter/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:51.440546 sqlfluff-3.0.7/src/sqlfluff/core/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13372 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/parser/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:51.444546 sqlfluff-3.0.7/src/sqlfluff/core/parser/grammar/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/parser/grammar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11911 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/parser/grammar/anyof.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19771 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/parser/grammar/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/parser/grammar/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/parser/grammar/delimited.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/parser/grammar/noncode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26538 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/parser/grammar/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/parser/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36075 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/parser/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9730 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/parser/markers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28332 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/parser/match_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11753 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/parser/match_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/parser/matchable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11439 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/parser/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:51.444546 sqlfluff-3.0.7/src/sqlfluff/core/parser/segments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/parser/segments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49362 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/parser/segments/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/parser/segments/bracketed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/parser/segments/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/parser/segments/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/parser/segments/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/parser/segments/keyword.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9440 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/parser/segments/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/parser/segments/raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/parser/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:51.444546 sqlfluff-3.0.7/src/sqlfluff/core/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/plugin/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/plugin/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/plugin/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:51.448546 sqlfluff-3.0.7/src/sqlfluff/core/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48881 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/rules/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8938 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/rules/config_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/rules/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/rules/crawlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/rules/doc_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17908 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/rules/fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/rules/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13500 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/rules/noqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/rules/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:51.448546 sqlfluff-3.0.7/src/sqlfluff/core/templaters/
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/templaters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23058 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/templaters/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45600 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/templaters/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/templaters/placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46401 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/templaters/python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:51.448546 sqlfluff-3.0.7/src/sqlfluff/core/templaters/slicers/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/templaters/slicers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35992 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/templaters/slicers/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/core/timing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:51.460547 sqlfluff-3.0.7/src/sqlfluff/dialects/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   139271 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_ansi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_ansi_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22826 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_athena.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_athena_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86952 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_bigquery_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40101 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_clickhouse_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8751 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_databricks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_databricks_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17402 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_db2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_db2_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18370 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93480 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_exasol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15655 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_exasol_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19408 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_greenplum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_greenplum_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33399 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_hive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_hive_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29892 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_materialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_materialize_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83191 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_mysql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28845 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_oracle.py
+-rw-r--r--   0 runner    (1001) docker     (127)   192309 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37092 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_postgres_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73019 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_redshift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9669 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_redshift_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)   242793 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_snowflake_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_soql.py
+-rw-r--r--   0 runner    (1001) docker     (127)   105781 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_sparksql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_sparksql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24586 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_sqlite_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28146 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_teradata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11953 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_trino.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_trino_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)   194021 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_tsql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12783 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_tsql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66185 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_vertica.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6277 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_vertica_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/diff_quality_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:51.460547 sqlfluff-3.0.7/src/sqlfluff/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:51.464547 sqlfluff-3.0.7/src/sqlfluff/rules/aliasing/
+-rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/aliasing/AL01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/aliasing/AL02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/aliasing/AL03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/aliasing/AL04.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11267 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/aliasing/AL05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/aliasing/AL06.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10982 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/aliasing/AL07.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/aliasing/AL08.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/aliasing/AL09.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/aliasing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:51.464547 sqlfluff-3.0.7/src/sqlfluff/rules/ambiguous/
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/ambiguous/AM01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/ambiguous/AM02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/ambiguous/AM03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/ambiguous/AM04.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/ambiguous/AM05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/ambiguous/AM06.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/ambiguous/AM07.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/ambiguous/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:51.464547 sqlfluff-3.0.7/src/sqlfluff/rules/capitalisation/
+-rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/capitalisation/CP01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/capitalisation/CP02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/capitalisation/CP03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/capitalisation/CP04.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/capitalisation/CP05.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/capitalisation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:51.468547 sqlfluff-3.0.7/src/sqlfluff/rules/convention/
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/convention/CV01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/convention/CV02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/convention/CV03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/convention/CV04.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/convention/CV05.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14963 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/convention/CV06.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/convention/CV07.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/convention/CV08.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/convention/CV09.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11947 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/convention/CV10.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16354 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/convention/CV11.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/convention/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:51.468547 sqlfluff-3.0.7/src/sqlfluff/rules/jinja/
+-rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/jinja/JJ01.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/jinja/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:51.472547 sqlfluff-3.0.7/src/sqlfluff/rules/layout/
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/layout/LT01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/layout/LT02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/layout/LT03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/layout/LT04.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6092 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/layout/LT05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/layout/LT06.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/layout/LT07.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8279 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/layout/LT08.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16989 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/layout/LT09.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/layout/LT10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/layout/LT11.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/layout/LT12.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/layout/LT13.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/layout/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:51.472547 sqlfluff-3.0.7/src/sqlfluff/rules/references/
+-rw-r--r--   0 runner    (1001) docker     (127)     9008 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/references/RF01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/references/RF02.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11350 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/references/RF03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/references/RF04.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/references/RF05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8506 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/references/RF06.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/references/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:51.476547 sqlfluff-3.0.7/src/sqlfluff/rules/structure/
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/structure/ST01.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10049 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/structure/ST02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/structure/ST03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9713 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/structure/ST04.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20587 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/structure/ST05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9623 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/structure/ST06.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/structure/ST07.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/structure/ST08.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/structure/ST09.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/structure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:51.476547 sqlfluff-3.0.7/src/sqlfluff/rules/tsql/
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/tsql/TQ01.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/rules/tsql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:51.476547 sqlfluff-3.0.7/src/sqlfluff/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:51.476547 sqlfluff-3.0.7/src/sqlfluff/utils/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/utils/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16342 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/utils/analysis/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/utils/analysis/select.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:51.476547 sqlfluff-3.0.7/src/sqlfluff/utils/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/utils/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/utils/functional/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/utils/functional/raw_file_slice_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/utils/functional/raw_file_slices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/utils/functional/segment_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8234 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/utils/functional/segments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/utils/functional/templated_file_slice_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/utils/functional/templated_file_slices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/utils/identifers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:51.480547 sqlfluff-3.0.7/src/sqlfluff/utils/reflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/utils/reflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/utils/reflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7051 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/utils/reflow/depthmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32545 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/utils/reflow/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/utils/reflow/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23067 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/utils/reflow/rebreak.py
+-rw-r--r--   0 runner    (1001) docker     (127)    94663 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/utils/reflow/reindent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24129 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/utils/reflow/respace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25529 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/utils/reflow/sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:51.480547 sqlfluff-3.0.7/src/sqlfluff/utils/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/utils/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/utils/testing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/utils/testing/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8794 2024-05-23 09:39:40.000000 sqlfluff-3.0.7/src/sqlfluff/utils/testing/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:51.480547 sqlfluff-3.0.7/src/sqlfluff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11986 2024-05-23 09:39:51.000000 sqlfluff-3.0.7/src/sqlfluff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-05-23 09:39:51.000000 sqlfluff-3.0.7/src/sqlfluff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 09:39:51.000000 sqlfluff-3.0.7/src/sqlfluff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-23 09:39:51.000000 sqlfluff-3.0.7/src/sqlfluff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-23 09:39:51.000000 sqlfluff-3.0.7/src/sqlfluff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-23 09:39:51.000000 sqlfluff-3.0.7/src/sqlfluff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:39:51.480547 sqlfluff-3.0.7/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-23 09:39:41.000000 sqlfluff-3.0.7/test/testing_test.py
```

### Comparing `sqlfluff-3.0.6/CHANGELOG.md` & `sqlfluff-3.0.7/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,48 @@
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 <!--
 Note: Changes are now automatically tracked in [GitHub](https://github.com/sqlfluff/sqlfluff/releases) and will be copied in here on each release (please remember to update the issues and contributors to links!). There is no need to manually edit this file going forward.
 -->
 <!--Start Of Releases (DO NOT DELETE THIS LINE)-->
 
+## [3.0.7] - 2024-05-23
+
+## Highlights
+
+This is primarily a fix for compatibility with dbt 1.8+. Beyond
+that it also brings several dialect improvements to SQLite, Bigquery,
+MySQL, Oracle & Clickhouse.
+
+Thanks also to the **five** new contributors whose work was included
+in this release! 🎉🎉🏆🎉🎉
+
+## What’s Changed
+
+* Add more minor features and fixes to sqlite dialect [#5894](https://github.com/sqlfluff/sqlfluff/pull/5894) [@Enduriel](https://github.com/Enduriel)
+* Fix Clickhouse identifiers format [#5890](https://github.com/sqlfluff/sqlfluff/pull/5890) [@Pavel-Strybuk](https://github.com/Pavel-Strybuk)
+* Add full support for on conflict clause in SQLite [#5888](https://github.com/sqlfluff/sqlfluff/pull/5888) [@Enduriel](https://github.com/Enduriel)
+* dbt Templater Plugin: dbt 1.8 support [#5892](https://github.com/sqlfluff/sqlfluff/pull/5892) [@keraion](https://github.com/keraion)
+* Added support for oracle materialized view [#5883](https://github.com/sqlfluff/sqlfluff/pull/5883) [@harshsoni2024](https://github.com/harshsoni2024)
+* BigQuery: Support ALTER TABLE ADD KEY statements [#5881](https://github.com/sqlfluff/sqlfluff/pull/5881) [@kzosabe](https://github.com/kzosabe)
+* MySQL: Support DIV and MOD operators [#5879](https://github.com/sqlfluff/sqlfluff/pull/5879) [@kzosabe](https://github.com/kzosabe)
+* Update documentation to include all templaters [#5873](https://github.com/sqlfluff/sqlfluff/pull/5873) [@timchurch](https://github.com/timchurch)
+* MySQL: Define date part function names [#5874](https://github.com/sqlfluff/sqlfluff/pull/5874) [@kzosabe](https://github.com/kzosabe)
+* Remove typing_extensions requirement [#5860](https://github.com/sqlfluff/sqlfluff/pull/5860) [@qarkai](https://github.com/qarkai)
+* BigQuery: Fix EXPORT DATA statement [#5859](https://github.com/sqlfluff/sqlfluff/pull/5859) [@kzosabe](https://github.com/kzosabe)
+* BigQuery: Support CREATE INDEX statements [#5858](https://github.com/sqlfluff/sqlfluff/pull/5858) [@kzosabe](https://github.com/kzosabe)
+
+## New Contributors
+
+* [@qarkai](https://github.com/qarkai) made their first contribution in [#5860](https://github.com/sqlfluff/sqlfluff/pull/5860)
+* [@timchurch](https://github.com/timchurch) made their first contribution in [#5873](https://github.com/sqlfluff/sqlfluff/pull/5873)
+* [@harshsoni2024](https://github.com/harshsoni2024) made their first contribution in [#5883](https://github.com/sqlfluff/sqlfluff/pull/5883)
+* [@Enduriel](https://github.com/Enduriel) made their first contribution in [#5888](https://github.com/sqlfluff/sqlfluff/pull/5888)
+* [@Pavel-Strybuk](https://github.com/Pavel-Strybuk) made their first contribution in [#5890](https://github.com/sqlfluff/sqlfluff/pull/5890)
+
 ## [3.0.6] - 2024-05-06
 
 ## Highlights
 
 This release primarily fixes an issue introduced by the recent dbt 1.7.14 release,
 and better support for dbt 1.7+. It also includes a range of dialect improvements
 and CLI refinements.
```

### Comparing `sqlfluff-3.0.6/LICENSE.md` & `sqlfluff-3.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/PKG-INFO` & `sqlfluff-3.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff
-Version: 3.0.6
+Version: 3.0.7
 Summary: The SQL Linter for Humans
 Author-email: Alan Cruickshank <alan@designingoverload.com>
 License: MIT License
         
         Copyright (c) 2023 Alan Cruickshank
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -65,15 +65,14 @@
 Requires-Dist: pathspec
 Requires-Dist: pytest
 Requires-Dist: pyyaml>=5.1
 Requires-Dist: regex
 Requires-Dist: tblib
 Requires-Dist: toml; python_version < "3.11"
 Requires-Dist: tqdm
-Requires-Dist: typing_extensions
 
 ![SQLFluff](https://raw.githubusercontent.com/sqlfluff/sqlfluff/main/images/sqlfluff-wide.png)
 
 # The SQL Linter for Humans
 
 [![PyPi Version](https://img.shields.io/pypi/v/sqlfluff.svg?style=flat-square&logo=PyPi)](https://pypi.org/project/sqlfluff/)
 [![PyPi License](https://img.shields.io/pypi/l/sqlfluff.svg?style=flat-square)](https://pypi.org/project/sqlfluff/)
@@ -138,15 +137,18 @@
 
 SQL itself does not lend itself well to [modularity](https://docs.getdbt.com/docs/viewpoint#section-modularity),
 so to introduce some flexibility and reusability it is often [templated](https://en.wikipedia.org/wiki/Template_processor)
 as discussed more in [our modularity documentation](https://docs.sqlfluff.com/en/stable/realworld.html#modularity).
 
 **SQLFluff** supports the following templates:
 - [Jinja](https://jinja.palletsprojects.com/) (aka Jinja2)
-- [dbt](https://www.getdbt.com/)
+- SQL placeholders (e.g. SQLAlchemy parameters)
+- [Python format strings](https://docs.python.org/3/library/string.html#format-string-syntax)
+- [dbt](https://www.getdbt.com/) (requires plugin)
+
 
 Again, please raise issues if you wish to support more templating languages/syntaxes.
 
 ## VS Code Extension
 
 We also have a VS Code extension:
```

### Comparing `sqlfluff-3.0.6/README.md` & `sqlfluff-3.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,18 @@
 
 SQL itself does not lend itself well to [modularity](https://docs.getdbt.com/docs/viewpoint#section-modularity),
 so to introduce some flexibility and reusability it is often [templated](https://en.wikipedia.org/wiki/Template_processor)
 as discussed more in [our modularity documentation](https://docs.sqlfluff.com/en/stable/realworld.html#modularity).
 
 **SQLFluff** supports the following templates:
 - [Jinja](https://jinja.palletsprojects.com/) (aka Jinja2)
-- [dbt](https://www.getdbt.com/)
+- SQL placeholders (e.g. SQLAlchemy parameters)
+- [Python format strings](https://docs.python.org/3/library/string.html#format-string-syntax)
+- [dbt](https://www.getdbt.com/) (requires plugin)
+
 
 Again, please raise issues if you wish to support more templating languages/syntaxes.
 
 ## VS Code Extension
 
 We also have a VS Code extension:
```

### Comparing `sqlfluff-3.0.6/pyproject.toml` & `sqlfluff-3.0.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=40.8.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "sqlfluff"
-version = "3.0.6"
+version = "3.0.7"
 description = "The SQL Linter for Humans"
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.8"
 authors = [
   {name = "Alan Cruickshank", email = "alan@designingoverload.com"},
 ]
 license = {file = "LICENSE.md"}
@@ -87,16 +87,14 @@
     "regex",
     # For returning exceptions from multiprocessing.Pool.map()
     "tblib",
     # For parsing pyproject.toml
     "toml; python_version < '3.11'",
     # For handling progress bars
     "tqdm",
-    # Literals and TypedDicts
-    "typing_extensions",
 ]
 
 [project.urls]
 Homepage = "https://www.sqlfluff.com"
 Documentation = "https://docs.sqlfluff.com"
 Source = "https://github.com/sqlfluff/sqlfluff"
 Changes = "https://github.com/sqlfluff/sqlfluff/blob/main/CHANGELOG.md"
@@ -125,15 +123,15 @@
 sqlfluff_rules_convention = "sqlfluff.rules.convention"
 sqlfluff_rules_jinja = "sqlfluff.rules.jinja"
 sqlfluff_rules_tsql = "sqlfluff.rules.tsql"
 
 
 [tool.sqlfluff_docs]
 # NOTE: Stable version is used by docs/conf.py
-stable_version = "3.0.6"
+stable_version = "3.0.7"
 
 
 [tool.setuptools.package-data]
 sqlfluff = ["core/default_config.cfg", "py.typed"]
 
 
 [tool.importlinter]
```

### Comparing `sqlfluff-3.0.6/src/sqlfluff/__init__.py` & `sqlfluff-3.0.7/src/sqlfluff/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/api/simple.py` & `sqlfluff-3.0.7/src/sqlfluff/api/simple.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/cli/autocomplete.py` & `sqlfluff-3.0.7/src/sqlfluff/cli/autocomplete.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/cli/commands.py` & `sqlfluff-3.0.7/src/sqlfluff/cli/commands.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/cli/formatters.py` & `sqlfluff-3.0.7/src/sqlfluff/cli/formatters.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/cli/helpers.py` & `sqlfluff-3.0.7/src/sqlfluff/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/cli/outputstream.py` & `sqlfluff-3.0.7/src/sqlfluff/cli/outputstream.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/__init__.py` & `sqlfluff-3.0.7/src/sqlfluff/core/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/config.py` & `sqlfluff-3.0.7/src/sqlfluff/core/config.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/default_config.cfg` & `sqlfluff-3.0.7/src/sqlfluff/core/default_config.cfg`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/dialects/__init__.py` & `sqlfluff-3.0.7/src/sqlfluff/core/dialects/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/dialects/base.py` & `sqlfluff-3.0.7/src/sqlfluff/core/dialects/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/dialects/common.py` & `sqlfluff-3.0.7/src/sqlfluff/core/dialects/common.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/enums.py` & `sqlfluff-3.0.7/src/sqlfluff/core/enums.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/errors.py` & `sqlfluff-3.0.7/src/sqlfluff/core/errors.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/helpers/dict.py` & `sqlfluff-3.0.7/src/sqlfluff/core/helpers/dict.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/helpers/file.py` & `sqlfluff-3.0.7/src/sqlfluff/core/helpers/file.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/helpers/slice.py` & `sqlfluff-3.0.7/src/sqlfluff/core/helpers/slice.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/helpers/string.py` & `sqlfluff-3.0.7/src/sqlfluff/core/helpers/string.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/linter/common.py` & `sqlfluff-3.0.7/src/sqlfluff/core/linter/common.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/linter/fix.py` & `sqlfluff-3.0.7/src/sqlfluff/core/linter/fix.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/linter/linted_dir.py` & `sqlfluff-3.0.7/src/sqlfluff/core/linter/linted_dir.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """Defines the LintedDir class.
 
 This stores the idea of a collection of linted files at a single start path
 
 """
 
-from typing import Any, Dict, List, Optional, Tuple, Union, overload
-
-from typing_extensions import Literal, TypedDict
+from typing import Any, Dict, List, Literal, Optional, Tuple, TypedDict, Union, overload
 
 from sqlfluff.core.errors import CheckTuple, SQLLintError
 from sqlfluff.core.linter.linted_file import TMP_PRS_ERROR_TYPES, LintedFile
 from sqlfluff.core.parser.segments.base import BaseSegment
 
 LintingRecord = TypedDict(
     "LintingRecord",
```

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/linter/linted_file.py` & `sqlfluff-3.0.7/src/sqlfluff/core/linter/linted_file.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/linter/linter.py` & `sqlfluff-3.0.7/src/sqlfluff/core/linter/linter.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/linter/linting_result.py` & `sqlfluff-3.0.7/src/sqlfluff/core/linter/linting_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 """Defines the linter class."""
 
 import csv
 import time
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Set, Tuple, Union, overload
-
-from typing_extensions import Literal
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Dict,
+    List,
+    Literal,
+    Optional,
+    Set,
+    Tuple,
+    Union,
+    overload,
+)
 
 from sqlfluff.core.errors import CheckTuple
 from sqlfluff.core.linter.linted_dir import LintedDir, LintingRecord
 from sqlfluff.core.timing import RuleTimingSummary, TimingSummary
 
 if TYPE_CHECKING:  # pragma: no cover
     from sqlfluff.core.parser.segments.base import BaseSegment
```

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/linter/patch.py` & `sqlfluff-3.0.7/src/sqlfluff/core/linter/patch.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/linter/runner.py` & `sqlfluff-3.0.7/src/sqlfluff/core/linter/runner.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/parser/__init__.py` & `sqlfluff-3.0.7/src/sqlfluff/core/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/parser/context.py` & `sqlfluff-3.0.7/src/sqlfluff/core/parser/context.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/parser/grammar/__init__.py` & `sqlfluff-3.0.7/src/sqlfluff/core/parser/grammar/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/parser/grammar/anyof.py` & `sqlfluff-3.0.7/src/sqlfluff/core/parser/grammar/anyof.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/parser/grammar/base.py` & `sqlfluff-3.0.7/src/sqlfluff/core/parser/grammar/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/parser/grammar/conditional.py` & `sqlfluff-3.0.7/src/sqlfluff/core/parser/grammar/conditional.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/parser/grammar/delimited.py` & `sqlfluff-3.0.7/src/sqlfluff/core/parser/grammar/delimited.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/parser/grammar/noncode.py` & `sqlfluff-3.0.7/src/sqlfluff/core/parser/grammar/noncode.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/parser/grammar/sequence.py` & `sqlfluff-3.0.7/src/sqlfluff/core/parser/grammar/sequence.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/parser/helpers.py` & `sqlfluff-3.0.7/src/sqlfluff/core/parser/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/parser/lexer.py` & `sqlfluff-3.0.7/src/sqlfluff/core/parser/lexer.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/parser/markers.py` & `sqlfluff-3.0.7/src/sqlfluff/core/parser/markers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/parser/match_algorithms.py` & `sqlfluff-3.0.7/src/sqlfluff/core/parser/match_algorithms.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/parser/match_result.py` & `sqlfluff-3.0.7/src/sqlfluff/core/parser/match_result.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/parser/matchable.py` & `sqlfluff-3.0.7/src/sqlfluff/core/parser/matchable.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/parser/parser.py` & `sqlfluff-3.0.7/src/sqlfluff/core/parser/parser.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/parser/parsers.py` & `sqlfluff-3.0.7/src/sqlfluff/core/parser/parsers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/__init__.py` & `sqlfluff-3.0.7/src/sqlfluff/core/parser/segments/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/base.py` & `sqlfluff-3.0.7/src/sqlfluff/core/parser/segments/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/bracketed.py` & `sqlfluff-3.0.7/src/sqlfluff/core/parser/segments/bracketed.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/common.py` & `sqlfluff-3.0.7/src/sqlfluff/core/parser/segments/common.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/file.py` & `sqlfluff-3.0.7/src/sqlfluff/core/parser/segments/file.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/generator.py` & `sqlfluff-3.0.7/src/sqlfluff/core/parser/segments/generator.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/keyword.py` & `sqlfluff-3.0.7/src/sqlfluff/core/parser/segments/keyword.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/meta.py` & `sqlfluff-3.0.7/src/sqlfluff/core/parser/segments/meta.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/parser/segments/raw.py` & `sqlfluff-3.0.7/src/sqlfluff/core/parser/segments/raw.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/parser/types.py` & `sqlfluff-3.0.7/src/sqlfluff/core/parser/types.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/plugin/hookspecs.py` & `sqlfluff-3.0.7/src/sqlfluff/core/plugin/hookspecs.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/plugin/host.py` & `sqlfluff-3.0.7/src/sqlfluff/core/plugin/host.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/plugin/lib.py` & `sqlfluff-3.0.7/src/sqlfluff/core/plugin/lib.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/rules/__init__.py` & `sqlfluff-3.0.7/src/sqlfluff/core/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/rules/base.py` & `sqlfluff-3.0.7/src/sqlfluff/core/rules/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/rules/config_info.py` & `sqlfluff-3.0.7/src/sqlfluff/core/rules/config_info.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/rules/context.py` & `sqlfluff-3.0.7/src/sqlfluff/core/rules/context.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/rules/crawlers.py` & `sqlfluff-3.0.7/src/sqlfluff/core/rules/crawlers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/rules/doc_decorators.py` & `sqlfluff-3.0.7/src/sqlfluff/core/rules/doc_decorators.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/rules/fix.py` & `sqlfluff-3.0.7/src/sqlfluff/core/rules/fix.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/rules/loader.py` & `sqlfluff-3.0.7/src/sqlfluff/core/rules/loader.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/rules/noqa.py` & `sqlfluff-3.0.7/src/sqlfluff/core/rules/noqa.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/rules/reference.py` & `sqlfluff-3.0.7/src/sqlfluff/core/rules/reference.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/templaters/__init__.py` & `sqlfluff-3.0.7/src/sqlfluff/core/templaters/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/templaters/base.py` & `sqlfluff-3.0.7/src/sqlfluff/core/templaters/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/templaters/jinja.py` & `sqlfluff-3.0.7/src/sqlfluff/core/templaters/jinja.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/templaters/placeholder.py` & `sqlfluff-3.0.7/src/sqlfluff/core/templaters/placeholder.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/templaters/python.py` & `sqlfluff-3.0.7/src/sqlfluff/core/templaters/python.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/templaters/slicers/tracer.py` & `sqlfluff-3.0.7/src/sqlfluff/core/templaters/slicers/tracer.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/core/timing.py` & `sqlfluff-3.0.7/src/sqlfluff/core/timing.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_ansi.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_ansi.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_ansi_keywords.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_ansi_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_athena.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_athena.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_athena_keywords.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_athena_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_bigquery.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_bigquery.py`

 * *Files 0% similar despite different names*

```diff
@@ -512,14 +512,16 @@
             Ref("AlterSchemaStatementSegment"),
             Ref("CreateMaterializedViewStatementSegment"),
             Ref("CreateMaterializedViewAsReplicaOfStatementSegment"),
             Ref("AlterMaterializedViewStatementSegment"),
             Ref("DropMaterializedViewStatementSegment"),
             Ref("DropProcedureStatementSegment"),
             Ref("UndropSchemaStatementSegment"),
+            Ref("CreateSearchIndexStatementSegment"),
+            Ref("CreateVectorIndexStatementSegment"),
             Ref("CreateRowAccessPolicyStatementSegment"),
             Ref("CreateCapacityStatementSegment"),
             Ref("CreateReservationStatementSegment"),
             Ref("CreateAssignmentStatementSegment"),
         ],
     )
 
@@ -1768,14 +1770,58 @@
                     "ADD",
                     "COLUMN",
                     Ref("IfNotExistsGrammar", optional=True),
                     Ref("ColumnDefinitionSegment"),
                 ),
                 allow_trailing=True,
             ),
+            # https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#alter_table_add_foreign_key_statement
+            # https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#alter_table_add_primary_key_statement
+            Delimited(
+                OneOf(
+                    Sequence(
+                        "ADD",
+                        Sequence(
+                            "CONSTRAINT",
+                            Ref("IfNotExistsGrammar", optional=True),
+                            Ref("SingleIdentifierGrammar"),
+                            optional=True,
+                        ),
+                        "FOREIGN",
+                        "KEY",
+                        Bracketed(
+                            Delimited(
+                                Ref("SingleIdentifierGrammar"),
+                            ),
+                        ),
+                        "REFERENCES",
+                        Ref("TableReferenceSegment"),
+                        Bracketed(
+                            Delimited(
+                                Ref("SingleIdentifierGrammar"),
+                            ),
+                        ),
+                        "NOT",
+                        "ENFORCED",
+                    ),
+                    Sequence(
+                        "ADD",
+                        "PRIMARY",
+                        "KEY",
+                        Bracketed(
+                            Delimited(
+                                Ref("SingleIdentifierGrammar"),
+                            ),
+                        ),
+                        "NOT",
+                        "ENFORCED",
+                    ),
+                ),
+                allow_trailing=True,
+            ),
             # https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#alter_table_rename_to_statement
             Sequence(
                 "RENAME",
                 "TO",
                 Ref("TableReferenceSegment"),
             ),
             # https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#alter_table_rename_column_statement
@@ -2411,21 +2457,36 @@
                         ),
                         StringParser(
                             "format",
                             CodeSegment,
                             type="export_option",
                         ),
                         StringParser(
+                            "header",
+                            CodeSegment,
+                            type="export_option",
+                        ),
+                        StringParser(
+                            "overwrite",
+                            CodeSegment,
+                            type="export_option",
+                        ),
+                        StringParser(
                             "uri",
                             CodeSegment,
                             type="export_option",
                         ),
+                        StringParser(
+                            "use_avro_logical_types",
+                            CodeSegment,
+                            type="export_option",
+                        ),
                     ),
                     Ref("EqualsSegment"),
-                    Ref("QuotedLiteralSegment"),
+                    Ref("BaseExpressionElementGrammar"),
                 ),
                 # Bool options
                 # Note: adding as own type, rather than keywords as convention with
                 # Bigquery, as per the docs, is to put Keywords in uppercase, and these
                 # in lowercase.
                 Sequence(
                     OneOf(
@@ -2598,14 +2659,66 @@
             Ref("EqualsSegment"),
             Ref("ExpressionSegment"),
             optional=True,
         ),
     )
 
 
+class CreateSearchIndexStatementSegment(BaseSegment):
+    """A `CREATE SEARCH INDEX` statement.
+
+    https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#create_search_index_statement
+    """
+
+    type = "create_search_index_statement"
+    match_grammar: Matchable = Sequence(
+        "CREATE",
+        "SEARCH",
+        "INDEX",
+        Ref("IfNotExistsGrammar", optional=True),
+        Ref("IndexReferenceSegment"),
+        "ON",
+        Ref("TableReferenceSegment"),
+        Bracketed(
+            OneOf(
+                Sequence("ALL", "COLUMNS"),
+                Delimited(
+                    Ref("IndexColumnDefinitionSegment"),
+                ),
+            )
+        ),
+        Ref("OptionsSegment", optional=True),
+    )
+
+
+class CreateVectorIndexStatementSegment(BaseSegment):
+    """A `CREATE VECTOR INDEX` statement.
+
+    https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#create_vector_index_statement
+    """
+
+    type = "create_vector_index_statement"
+    match_grammar: Matchable = Sequence(
+        "CREATE",
+        Ref("OrReplaceGrammar", optional=True),
+        "VECTOR",
+        "INDEX",
+        Ref("IfNotExistsGrammar", optional=True),
+        Ref("IndexReferenceSegment"),
+        "ON",
+        Ref("TableReferenceSegment"),
+        Bracketed(
+            Delimited(
+                Ref("IndexColumnDefinitionSegment"),
+            ),
+        ),
+        Ref("OptionsSegment"),
+    )
+
+
 class CreateRowAccessPolicyStatementSegment(BaseSegment):
     """A `CREATE ROW ACCESS POLICY` statement.
 
     https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#create_row_access_policy_statement
     """
 
     type = "create_row_access_policy_statement"
```

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_bigquery_keywords.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_bigquery_keywords.py`

 * *Files 5% similar despite different names*

```diff
@@ -253,14 +253,15 @@
 ROLLBACK
 ROW
 ROUTINE
 SAFE
 SATURDAY
 SCHEMA
 SCHEMAS
+SEARCH
 SECOND
 SEPARATOR
 SERVER
 SEQUENCE
 SESSION_USER
 SHARE
 SNAPSHOT
@@ -294,14 +295,15 @@
 USAGE
 USE
 USE_ANY_ROLE
 USER
 VALUE
 VALUES
 VARYING
+VECTOR
 VERSION
 VIEW
 WAREHOUSE
 WEDNESDAY
 WEEK
 WHILE
 WITHOUT
```

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_clickhouse.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_clickhouse.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,15 +201,15 @@
             type="quoted_literal",
         ),
     ),
     # Drop casefold from ANSI
     NakedIdentifierSegment=SegmentGenerator(
         # Generate the anti template from the set of reserved keywords
         lambda dialect: RegexParser(
-            r"[A-Z0-9_]*[A-Z][A-Z0-9_]*",
+            r"[a-zA-Z_][0-9a-zA-Z_]*",
             IdentifierSegment,
             type="naked_identifier",
             anti_template=r"^(" + r"|".join(dialect.sets("reserved_keywords")) + r")$",
         )
     ),
     SingleIdentifierGrammar=OneOf(
         Ref("NakedIdentifierSegment"),
```

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_clickhouse_keywords.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_clickhouse_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_databricks.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_databricks.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_db2.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_db2.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_db2_keywords.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_db2_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_duckdb.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_duckdb.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_exasol.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_exasol.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_exasol_keywords.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_exasol_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_greenplum.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_greenplum.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_greenplum_keywords.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_greenplum_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_hive.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_hive.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_hive_keywords.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_hive_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_materialize.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_materialize.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_materialize_keywords.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_materialize_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_mysql.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_mysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,22 @@
         "QUARTER",
         "SECOND",
         "MICROSECOND",
         "YEAR",
     ]
 )
 
+mysql_dialect.sets("date_part_function_name").clear()
+mysql_dialect.sets("date_part_function_name").update(
+    [
+        "EXTRACT",
+        "TIMESTAMPADD",
+        "TIMESTAMPDIFF",
+    ]
+)
 
 mysql_dialect.replace(
     QuotedIdentifierSegment=TypedParser(
         "back_quote",
         IdentifierSegment,
         type="quoted_identifier",
         trim_chars=("`",),
@@ -183,14 +191,22 @@
     ).copy(
         insert=[
             Ref("SessionVariableNameSegment"),
             Ref("LocalVariableNameSegment"),
             Ref("VariableAssignmentSegment"),
         ]
     ),
+    ArithmeticBinaryOperatorGrammar=ansi_dialect.get_grammar(
+        "ArithmeticBinaryOperatorGrammar"
+    ).copy(
+        insert=[
+            Ref("DivOperatorSegment"),
+            Ref("ModOperatorSegment"),
+        ],
+    ),
     DateTimeLiteralGrammar=Sequence(
         # MySQL does not require the keyword to be specified:
         # https://dev.mysql.com/doc/refman/8.0/en/date-and-time-literals.html
         OneOf(
             "DATE",
             "TIME",
             "TIMESTAMP",
@@ -279,14 +295,16 @@
         type="at_sign_literal",
     ),
     SystemVariableSegment=RegexParser(
         r"@@(session|global)\.[A-Za-z0-9_]+",
         CodeSegment,
         type="system_variable",
     ),
+    DivOperatorSegment=StringParser("DIV", KeywordSegment, type="binary_operator"),
+    ModOperatorSegment=StringParser("MOD", KeywordSegment, type="binary_operator"),
     DoubleQuotedJSONPath=TypedParser(
         "double_quote",
         CodeSegment,
         type="json_path",
         trim_chars=('"',),
     ),
     SingleQuotedJSONPath=TypedParser(
```

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_mysql_keywords.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_mysql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_oracle.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_oracle.py`

 * *Files 0% similar despite different names*

```diff
@@ -605,14 +605,15 @@
         Sequence(Ref.keyword("NO", optional=True), "FORCE", optional=True),
         OneOf(
             "EDITIONING",
             Sequence("EDITIONABLE", Ref.keyword("EDITIONING", optional=True)),
             "NONEDITIONABLE",
             optional=True,
         ),
+        Ref.keyword("MATERIALIZED", optional=True),
         "VIEW",
         Ref("IfNotExistsGrammar", optional=True),
         Ref("TableReferenceSegment"),
         # Optional list of column names
         Ref("BracketedColumnReferenceListGrammar", optional=True),
         "AS",
         OptionallyBracketed(Ref("SelectableGrammar")),
```

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_postgres.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_postgres.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_postgres_keywords.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_postgres_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_redshift.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_redshift.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_redshift_keywords.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_redshift_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_snowflake.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_snowflake_keywords.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_snowflake_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_soql.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_soql.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_sparksql.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_sparksql.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_sparksql_keywords.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_sparksql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_sqlite.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_sqlite.py`

 * *Files 9% similar despite different names*

```diff
@@ -97,15 +97,19 @@
         # match ANSI's naked identifier casefold, sqlite is case-insensitive.
         casefold=str.upper,
     ),
 )
 
 sqlite_dialect.replace(
     PrimaryKeyGrammar=Sequence(
-        "PRIMARY", "KEY", Sequence("AUTOINCREMENT", optional=True)
+        "PRIMARY",
+        "KEY",
+        OneOf("ASC", "DESC", optional=True),
+        Ref("ConflictClauseSegment", optional=True),
+        Sequence("AUTOINCREMENT", optional=True),
     ),
     TemporaryTransientGrammar=Ref("TemporaryGrammar"),
     DateTimeLiteralGrammar=Sequence(
         OneOf("DATE", "DATETIME"),
         TypedParser("single_quote", LiteralSegment, type="date_constructor_literal"),
     ),
     BaseExpressionElementGrammar=OneOf(
@@ -119,14 +123,30 @@
             Ref("LiteralGrammar"),
         ),
         terminators=[
             Ref("CommaSegment"),
             Ref.keyword("AS"),
         ],
     ),
+    AlterTableOptionsGrammar=OneOf(
+        Sequence("RENAME", "TO", Ref("SingleIdentifierGrammar")),
+        Sequence(
+            "RENAME",
+            Sequence("COLUMN", optional=True),
+            Ref("ColumnReferenceSegment"),
+            "TO",
+            Ref("SingleIdentifierGrammar"),
+        ),
+        Sequence(
+            "ADD", Sequence("COLUMN", optional=True), Ref("ColumnDefinitionSegment")
+        ),
+        Sequence(
+            "DROP", Sequence("COLUMN", optional=True), Ref("ColumnReferenceSegment")
+        ),
+    ),
     AutoIncrementGrammar=Nothing(),
     CommentClauseSegment=Nothing(),
     IntervalExpressionSegment=Nothing(),
     TimeZoneGrammar=Nothing(),
     FetchClauseSegment=Nothing(),
     TrimParametersGrammar=Nothing(),
     LikeGrammar=Sequence("LIKE"),
@@ -248,14 +268,15 @@
     # match ANSI's naked identifier casefold, sqlite is case-insensitive.
     QuotedIdentifierSegment=TypedParser(
         "double_quote", IdentifierSegment, type="quoted_identifier", casefold=str.upper
     ),
     SingleQuotedIdentifierSegment=TypedParser(
         "single_quote", IdentifierSegment, type="quoted_identifier", casefold=str.upper
     ),
+    ColumnConstraintDefaultGrammar=Ref("ExpressionSegment"),
 )
 
 
 class SetOperatorSegment(BaseSegment):
     """A set operator such as Union, Minus, Except or Intersect."""
 
     type = "set_operator"
@@ -361,14 +382,64 @@
                 Ref("ExpressionSegment"),
                 Ref("AliasExpressionSegment", optional=True),
             ),
         ),
     )
 
 
+class ConflictTargetSegment(BaseSegment):
+    """An upsert conflict target.
+
+    https://www.sqlite.org/lang_upsert.html
+    """
+
+    type = "conflict_target"
+    match_grammar = Sequence(
+        Delimited(Ref("IndexColumnDefinitionSegment")),
+        Sequence("WHERE", Ref("ExpressionSegment"), optional=True),
+    )
+
+
+class UpsertClauseSegment(BaseSegment):
+    """An upsert clause.
+
+    https://www.sqlite.org/lang_upsert.html
+    """
+
+    type = "upsert_clause"
+    match_grammar = Sequence(
+        "ON",
+        "CONFLICT",
+        Ref("ConflictTargetSegment", optional=True),
+        "DO",
+        OneOf(
+            "NOTHING",
+            Sequence(
+                "UPDATE",
+                "SET",
+                Delimited(
+                    Sequence(
+                        OneOf(
+                            Ref("SingleIdentifierGrammar"),
+                            Ref("BracketedColumnReferenceListGrammar"),
+                        ),
+                        Ref("EqualsSegment"),
+                        Ref("ExpressionSegment"),
+                    ),
+                ),
+                Sequence(
+                    "WHERE",
+                    Ref("ExpressionSegment"),
+                    optional=True,
+                ),
+            ),
+        ),
+    )
+
+
 class InsertStatementSegment(BaseSegment):
     """An`INSERT` statement.
 
     https://www.sqlite.org/lang_insert.html
     """
 
     type = "insert_statement"
@@ -391,34 +462,95 @@
             # REPLACE is just an alias for INSERT OR REPLACE
             "REPLACE",
         ),
         "INTO",
         Ref("TableReferenceSegment"),
         Ref("BracketedColumnReferenceListGrammar", optional=True),
         OneOf(
-            Ref("ValuesClauseSegment"),
-            OptionallyBracketed(Ref("SelectableGrammar")),
+            Sequence(
+                Ref("ValuesClauseSegment"),
+                Ref("UpsertClauseSegment", optional=True),
+            ),
+            Sequence(
+                OptionallyBracketed(Ref("SelectableGrammar")),
+                Ref("UpsertClauseSegment", optional=True),
+            ),
             Ref("DefaultValuesGrammar"),
         ),
         Ref("ReturningClauseSegment", optional=True),
     )
 
 
+class ConflictClauseSegment(BaseSegment):
+    """A conflict clause.
+
+    https://www.sqlite.org/lang_conflict.html
+    """
+
+    type = "conflict_clause"
+    match_grammar = Sequence(
+        "ON",
+        "CONFLICT",
+        OneOf(
+            "ROLLBACK",
+            "ABORT",
+            "FAIL",
+            "IGNORE",
+            "REPLACE",
+        ),
+    )
+
+
 class ColumnConstraintSegment(ansi.ColumnConstraintSegment):
-    """Overriding ColumnConstraintSegment to allow for additional segment parsing."""
+    """A column option; each CREATE TABLE column can have 0 or more.
 
-    match_grammar = ansi.ColumnConstraintSegment.match_grammar.copy(
-        insert=[
-            OneOf("DEFERRABLE", Sequence("NOT", "DEFERRABLE"), optional=True),
-            OneOf(
-                Sequence("INITIALLY", "DEFERRED"),
-                Sequence("INITIALLY", "IMMEDIATE"),
-                optional=True,
+    Overriding ColumnConstraintSegment to allow for additional segment parsing
+    and to support on conflict clauses.
+    """
+
+    match_grammar: Matchable = Sequence(
+        Sequence(
+            "CONSTRAINT",
+            Ref("ObjectReferenceSegment"),  # Constraint name
+            optional=True,
+        ),
+        OneOf(
+            Sequence(
+                Ref.keyword("NOT", optional=True),
+                "NULL",
+                Ref("ConflictClauseSegment", optional=True),
+            ),  # NOT NULL or NULL
+            Sequence("CHECK", Bracketed(Ref("ExpressionSegment"))),
+            Sequence(  # DEFAULT <value>
+                "DEFAULT",
+                Ref("ColumnConstraintDefaultGrammar"),
             ),
-        ],
+            Ref("PrimaryKeyGrammar"),
+            Sequence(
+                Ref("UniqueKeyGrammar"), Ref("ConflictClauseSegment", optional=True)
+            ),  # UNIQUE
+            Ref("AutoIncrementGrammar"),
+            Ref("ReferenceDefinitionGrammar"),  # REFERENCES reftable [ ( refcolumn) ]x
+            Ref("CommentClauseSegment"),
+            Sequence(
+                "COLLATE", Ref("CollationReferenceSegment")
+            ),  # https://www.sqlite.org/datatype3.html#collation
+            Sequence(
+                Sequence("GENERATED", "ALWAYS", optional=True),
+                "AS",
+                Bracketed(Ref("ExpressionSegment")),
+                OneOf("STORED", "VIRTUAL", optional=True),
+            ),  # https://www.sqlite.org/gencol.html
+        ),
+        OneOf("DEFERRABLE", Sequence("NOT", "DEFERRABLE"), optional=True),
+        OneOf(
+            Sequence("INITIALLY", "DEFERRED"),
+            Sequence("INITIALLY", "IMMEDIATE"),
+            optional=True,
+        ),
     )
 
 
 class TableConstraintSegment(ansi.TableConstraintSegment):
     """Overriding TableConstraintSegment to allow for additional segment parsing."""
 
     match_grammar: Matchable = Sequence(
@@ -434,14 +566,15 @@
                 # Later add support for index_parameters?
             ),
             Sequence(  # PRIMARY KEY ( column_name [, ... ] ) index_parameters
                 Ref("PrimaryKeyGrammar"),
                 # Columns making up PRIMARY KEY constraint
                 Ref("BracketedColumnReferenceListGrammar"),
                 # Later add support for index_parameters?
+                Ref("ConflictClauseSegment", optional=True),
             ),
             Sequence(  # FOREIGN KEY ( column_name [, ... ] )
                 # REFERENCES reftable [ ( refcolumn [, ... ] ) ]
                 Ref("ForeignKeyGrammar"),
                 # Local columns making up FOREIGN KEY constraint
                 Ref("BracketedColumnReferenceListGrammar"),
                 Ref(
```

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_sqlite_keywords.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_sqlite_keywords.py`

 * *Files 8% similar despite different names*

```diff
@@ -200,8 +200,9 @@
     "PASSIVE",
     "RESTART",
     "RESET",
     "STRICT",
     "BINARY",
     "NOCASE",
     "RTRIM",
+    "STORED",  # https://sqlite.org/forum/forumpost/91127ba3db
 ]
```

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_teradata.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_teradata.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_trino.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_trino.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_trino_keywords.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_trino_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_tsql.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_tsql.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_tsql_keywords.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_tsql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_vertica.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_vertica.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/dialects/dialect_vertica_keywords.py` & `sqlfluff-3.0.7/src/sqlfluff/dialects/dialect_vertica_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/diff_quality_plugin.py` & `sqlfluff-3.0.7/src/sqlfluff/diff_quality_plugin.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL01.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/aliasing/AL01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL02.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/aliasing/AL02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL03.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/aliasing/AL03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL04.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/aliasing/AL04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL05.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/aliasing/AL05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL06.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/aliasing/AL06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL07.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/aliasing/AL07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL08.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/aliasing/AL08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/AL09.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/aliasing/AL09.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/aliasing/__init__.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/aliasing/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/ambiguous/AM01.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/ambiguous/AM01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/ambiguous/AM02.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/ambiguous/AM02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/ambiguous/AM03.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/ambiguous/AM03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/ambiguous/AM04.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/ambiguous/AM04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/ambiguous/AM05.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/ambiguous/AM05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/ambiguous/AM06.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/ambiguous/AM06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/ambiguous/AM07.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/ambiguous/AM07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/ambiguous/__init__.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/ambiguous/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/capitalisation/CP01.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/capitalisation/CP01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/capitalisation/CP02.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/capitalisation/CP02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/capitalisation/CP03.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/capitalisation/CP03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/capitalisation/CP04.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/capitalisation/CP04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/capitalisation/CP05.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/capitalisation/CP05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/capitalisation/__init__.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/capitalisation/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV01.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/convention/CV01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV02.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/convention/CV02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV03.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/convention/CV03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV04.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/convention/CV04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV05.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/convention/CV05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV06.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/convention/CV06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV07.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/convention/CV07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV08.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/convention/CV08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV09.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/convention/CV09.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV10.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/convention/CV10.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/convention/CV11.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/convention/CV11.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/convention/__init__.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/convention/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/jinja/JJ01.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/jinja/JJ01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT01.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/layout/LT01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT02.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/layout/LT02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT03.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/layout/LT03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT04.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/layout/LT04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT05.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/layout/LT05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT06.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/layout/LT06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT07.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/layout/LT07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT08.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/layout/LT08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT09.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/layout/LT09.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT10.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/layout/LT10.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT11.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/layout/LT11.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT12.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/layout/LT12.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/layout/LT13.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/layout/LT13.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/layout/__init__.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/references/RF01.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/references/RF01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/references/RF02.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/references/RF02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/references/RF03.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/references/RF03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/references/RF04.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/references/RF04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/references/RF05.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/references/RF05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/references/RF06.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/references/RF06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/references/__init__.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/references/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST01.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/structure/ST01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST02.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/structure/ST02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST03.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/structure/ST03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST04.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/structure/ST04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST05.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/structure/ST05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST06.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/structure/ST06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST07.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/structure/ST07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST08.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/structure/ST08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/structure/ST09.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/structure/ST09.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/structure/__init__.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/structure/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/tsql/TQ01.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/tsql/TQ01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/rules/tsql/__init__.py` & `sqlfluff-3.0.7/src/sqlfluff/rules/tsql/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/utils/analysis/query.py` & `sqlfluff-3.0.7/src/sqlfluff/utils/analysis/query.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/utils/analysis/select.py` & `sqlfluff-3.0.7/src/sqlfluff/utils/analysis/select.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/utils/functional/__init__.py` & `sqlfluff-3.0.7/src/sqlfluff/utils/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/utils/functional/context.py` & `sqlfluff-3.0.7/src/sqlfluff/utils/functional/context.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/utils/functional/raw_file_slice_predicates.py` & `sqlfluff-3.0.7/src/sqlfluff/utils/functional/raw_file_slice_predicates.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/utils/functional/raw_file_slices.py` & `sqlfluff-3.0.7/src/sqlfluff/utils/functional/raw_file_slices.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/utils/functional/segment_predicates.py` & `sqlfluff-3.0.7/src/sqlfluff/utils/functional/segment_predicates.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/utils/functional/segments.py` & `sqlfluff-3.0.7/src/sqlfluff/utils/functional/segments.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,19 @@
 from typing import (
     Any,
     Callable,
     Iterable,
     Iterator,
     List,
     Optional,
+    SupportsIndex,
     Union,
     overload,
 )
 
-from typing_extensions import SupportsIndex  # NOTE: Required for py37
-
 from sqlfluff.core.parser import BaseSegment
 from sqlfluff.core.templaters.base import TemplatedFile
 from sqlfluff.utils.functional.raw_file_slices import RawFileSlices
 
 PredicateType = Callable[[BaseSegment], bool]
```

### Comparing `sqlfluff-3.0.6/src/sqlfluff/utils/functional/templated_file_slice_predicates.py` & `sqlfluff-3.0.7/src/sqlfluff/utils/functional/templated_file_slice_predicates.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/utils/functional/templated_file_slices.py` & `sqlfluff-3.0.7/src/sqlfluff/utils/functional/templated_file_slices.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/utils/identifers.py` & `sqlfluff-3.0.7/src/sqlfluff/utils/identifers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/utils/reflow/config.py` & `sqlfluff-3.0.7/src/sqlfluff/utils/reflow/config.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/utils/reflow/depthmap.py` & `sqlfluff-3.0.7/src/sqlfluff/utils/reflow/depthmap.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/utils/reflow/elements.py` & `sqlfluff-3.0.7/src/sqlfluff/utils/reflow/elements.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/utils/reflow/helpers.py` & `sqlfluff-3.0.7/src/sqlfluff/utils/reflow/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/utils/reflow/rebreak.py` & `sqlfluff-3.0.7/src/sqlfluff/utils/reflow/rebreak.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/utils/reflow/reindent.py` & `sqlfluff-3.0.7/src/sqlfluff/utils/reflow/reindent.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/utils/reflow/respace.py` & `sqlfluff-3.0.7/src/sqlfluff/utils/reflow/respace.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/utils/reflow/sequence.py` & `sqlfluff-3.0.7/src/sqlfluff/utils/reflow/sequence.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/utils/testing/cli.py` & `sqlfluff-3.0.7/src/sqlfluff/utils/testing/cli.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/utils/testing/logging.py` & `sqlfluff-3.0.7/src/sqlfluff/utils/testing/logging.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff/utils/testing/rules.py` & `sqlfluff-3.0.7/src/sqlfluff/utils/testing/rules.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff.egg-info/PKG-INFO` & `sqlfluff-3.0.7/src/sqlfluff.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff
-Version: 3.0.6
+Version: 3.0.7
 Summary: The SQL Linter for Humans
 Author-email: Alan Cruickshank <alan@designingoverload.com>
 License: MIT License
         
         Copyright (c) 2023 Alan Cruickshank
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -65,15 +65,14 @@
 Requires-Dist: pathspec
 Requires-Dist: pytest
 Requires-Dist: pyyaml>=5.1
 Requires-Dist: regex
 Requires-Dist: tblib
 Requires-Dist: toml; python_version < "3.11"
 Requires-Dist: tqdm
-Requires-Dist: typing_extensions
 
 ![SQLFluff](https://raw.githubusercontent.com/sqlfluff/sqlfluff/main/images/sqlfluff-wide.png)
 
 # The SQL Linter for Humans
 
 [![PyPi Version](https://img.shields.io/pypi/v/sqlfluff.svg?style=flat-square&logo=PyPi)](https://pypi.org/project/sqlfluff/)
 [![PyPi License](https://img.shields.io/pypi/l/sqlfluff.svg?style=flat-square)](https://pypi.org/project/sqlfluff/)
@@ -138,15 +137,18 @@
 
 SQL itself does not lend itself well to [modularity](https://docs.getdbt.com/docs/viewpoint#section-modularity),
 so to introduce some flexibility and reusability it is often [templated](https://en.wikipedia.org/wiki/Template_processor)
 as discussed more in [our modularity documentation](https://docs.sqlfluff.com/en/stable/realworld.html#modularity).
 
 **SQLFluff** supports the following templates:
 - [Jinja](https://jinja.palletsprojects.com/) (aka Jinja2)
-- [dbt](https://www.getdbt.com/)
+- SQL placeholders (e.g. SQLAlchemy parameters)
+- [Python format strings](https://docs.python.org/3/library/string.html#format-string-syntax)
+- [dbt](https://www.getdbt.com/) (requires plugin)
+
 
 Again, please raise issues if you wish to support more templating languages/syntaxes.
 
 ## VS Code Extension
 
 We also have a VS Code extension:
```

### Comparing `sqlfluff-3.0.6/src/sqlfluff.egg-info/SOURCES.txt` & `sqlfluff-3.0.7/src/sqlfluff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/src/sqlfluff.egg-info/entry_points.txt` & `sqlfluff-3.0.7/src/sqlfluff.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.6/test/testing_test.py` & `sqlfluff-3.0.7/test/testing_test.py`

 * *Files identical despite different names*

