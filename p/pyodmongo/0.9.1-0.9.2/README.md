# Comparing `tmp/pyodmongo-0.9.1.tar.gz` & `tmp/pyodmongo-0.9.2.tar.gz`

## Comparing `pyodmongo-0.9.1.tar` & `pyodmongo-0.9.2.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/code_of_conduct.md
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/coverage.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs_release_notes.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/mkdocs.yml
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyproject.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/requirements.txt
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/.github/workflows/black_formatter.yml
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/.github/workflows/publishing_docs_s3.yml
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/.github/workflows/python_publish.yml
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0    56292 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/assets/images/favicon.png
--rw-r--r--   0        0        0    94192 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/assets/images/insomnia_request.png
--rw-r--r--   0        0        0    57259 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/assets/images/logo.png
--rw-r--r--   0        0        0    70935 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/assets/images/pyodmongo_Logo_BG_Dark.png
--rw-r--r--   0        0        0    72399 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/assets/images/pyodmongo_Logo_BG_White.png
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/en/aggregation.md
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/en/contributing.md
--rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/en/db_model.md
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/en/delete.md
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/en/fastapi.md
--rw-r--r--   0        0        0     7640 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/en/find.md
--rw-r--r--   0        0        0     5642 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/en/getting_started.md
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/en/index.md
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/en/indexes.md
--rw-r--r--   0        0        0     7707 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/en/query.md
--rw-r--r--   0        0        0     4849 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/en/save.md
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/pt-BR/aggregation.md
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/pt-BR/contributing.md
--rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/pt-BR/db_model.md
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/pt-BR/delete.md
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/pt-BR/fastapi.md
--rw-r--r--   0        0        0     7920 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/pt-BR/find.md
--rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/pt-BR/getting_started.md
--rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/pt-BR/index.md
--rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/pt-BR/indexes.md
--rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/pt-BR/query.md
--rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/pt-BR/save.md
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/docs/stylesheets/extras.css
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/__init__.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/version.py
--rw-r--r--   0        0        0    16992 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/async_engine/engine.py
--rw-r--r--   0        0        0    18792 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/engine/engine.py
--rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/engine/utils.py
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/models/db_field_info.py
--rw-r--r--   0        0        0     4948 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/models/db_model.py
--rw-r--r--   0        0        0     9486 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/models/fields.py
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/models/id_model.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/models/paginate.py
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/models/query_operators.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/models/responses.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/models/sort_operators.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/queries/__init__.py
--rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/queries/comparison_operators.py
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/queries/logical_operators.py
--rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/queries/query_string.py
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/queries/sort_operator.py
--rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/services/aggregate_stages.py
--rw-r--r--   0        0        0     9853 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/services/model_init.py
--rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyodmongo/services/query_operators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/__init__.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/conftest.py
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/test_async_aggregate.py
--rw-r--r--   0        0        0    19988 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/test_async_crud_db.py
--rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/test_class.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/test_db_field_info.py
--rw-r--r--   0        0        0     7759 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/test_db_index.py
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/test_dict_empty.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/test_fastapi.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/test_model_init_functions.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/test_object_id.py
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/test_project_pipeline.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/test_pydantic_validators.py
--rw-r--r--   0        0        0    12859 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/test_queries.py
--rw-r--r--   0        0        0     9193 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/test_reference_pipeline.py
--rw-r--r--   0        0        0     8320 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/test_save_dict.py
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/test_sync_aggregate.py
--rw-r--r--   0        0        0    14008 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/test_sync_crud_db.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/tests/test_version.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/LICENSE
--rw-r--r--   0        0        0     4240 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/README.md
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 pyodmongo-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/code_of_conduct.md
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/coverage.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/docs_release_notes.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/mkdocs.yml
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/pyproject.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/requirements.txt
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/.github/workflows/black_formatter.yml
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/.github/workflows/publishing_docs_s3.yml
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/.github/workflows/python_publish.yml
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/.github/workflows/tests.yml
+-rw-r--r--   0        0        0    56292 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/docs/assets/images/favicon.png
+-rw-r--r--   0        0        0    94192 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/docs/assets/images/insomnia_request.png
+-rw-r--r--   0        0        0    57259 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/docs/assets/images/logo.png
+-rw-r--r--   0        0        0    70935 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/docs/assets/images/pyodmongo_Logo_BG_Dark.png
+-rw-r--r--   0        0        0    72399 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/docs/assets/images/pyodmongo_Logo_BG_White.png
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/docs/en/aggregation.md
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/docs/en/contributing.md
+-rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/docs/en/db_model.md
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/docs/en/delete.md
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/docs/en/fastapi.md
+-rw-r--r--   0        0        0     7640 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/docs/en/find.md
+-rw-r--r--   0        0        0     5642 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/docs/en/getting_started.md
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/docs/en/index.md
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/docs/en/indexes.md
+-rw-r--r--   0        0        0     7707 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/docs/en/query.md
+-rw-r--r--   0        0        0     4849 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/docs/en/save.md
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/docs/pt-BR/aggregation.md
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/docs/pt-BR/contributing.md
+-rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/docs/pt-BR/db_model.md
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/docs/pt-BR/delete.md
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/docs/pt-BR/fastapi.md
+-rw-r--r--   0        0        0     7920 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/docs/pt-BR/find.md
+-rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/docs/pt-BR/getting_started.md
+-rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/docs/pt-BR/index.md
+-rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/docs/pt-BR/indexes.md
+-rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/docs/pt-BR/query.md
+-rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/docs/pt-BR/save.md
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/docs/stylesheets/extras.css
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/pyodmongo/__init__.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/pyodmongo/version.py
+-rw-r--r--   0        0        0    16992 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/pyodmongo/async_engine/engine.py
+-rw-r--r--   0        0        0    18792 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/pyodmongo/engine/engine.py
+-rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/pyodmongo/engine/utils.py
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/pyodmongo/models/db_field_info.py
+-rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/pyodmongo/models/db_model.py
+-rw-r--r--   0        0        0     9486 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/pyodmongo/models/fields.py
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/pyodmongo/models/id_model.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/pyodmongo/models/paginate.py
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/pyodmongo/models/query_operators.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/pyodmongo/models/responses.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/pyodmongo/models/sort_operators.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/pyodmongo/queries/__init__.py
+-rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/pyodmongo/queries/comparison_operators.py
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/pyodmongo/queries/logical_operators.py
+-rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/pyodmongo/queries/query_string.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/pyodmongo/queries/sort_operator.py
+-rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/pyodmongo/services/aggregate_stages.py
+-rw-r--r--   0        0        0     9853 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/pyodmongo/services/model_init.py
+-rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/pyodmongo/services/query_operators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/tests/__init__.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/tests/conftest.py
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/tests/test_async_aggregate.py
+-rw-r--r--   0        0        0    19988 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/tests/test_async_crud_db.py
+-rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/tests/test_class.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/tests/test_db_field_info.py
+-rw-r--r--   0        0        0     7759 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/tests/test_db_index.py
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/tests/test_dict_empty.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/tests/test_fastapi.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/tests/test_model_init_functions.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/tests/test_object_id.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/tests/test_project_pipeline.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/tests/test_pydantic_validators.py
+-rw-r--r--   0        0        0    12859 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/tests/test_queries.py
+-rw-r--r--   0        0        0     9193 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/tests/test_reference_pipeline.py
+-rw-r--r--   0        0        0     8320 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/tests/test_save_dict.py
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/tests/test_sync_aggregate.py
+-rw-r--r--   0        0        0    14008 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/tests/test_sync_crud_db.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/tests/test_version.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/LICENSE
+-rw-r--r--   0        0        0     4240 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/README.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 pyodmongo-0.9.2/PKG-INFO
```

### Comparing `pyodmongo-0.9.1/code_of_conduct.md` & `pyodmongo-0.9.2/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/docs_release_notes.py` & `pyodmongo-0.9.2/docs_release_notes.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/mkdocs.yml` & `pyodmongo-0.9.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/pyproject.py` & `pyodmongo-0.9.2/pyproject.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/requirements.txt` & `pyodmongo-0.9.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/.github/ISSUE_TEMPLATE/bug.yml` & `pyodmongo-0.9.2/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/.github/workflows/black_formatter.yml` & `pyodmongo-0.9.2/.github/workflows/black_formatter.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/.github/workflows/publishing_docs_s3.yml` & `pyodmongo-0.9.2/.github/workflows/publishing_docs_s3.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/.github/workflows/python_publish.yml` & `pyodmongo-0.9.2/.github/workflows/python_publish.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/.github/workflows/tests.yml` & `pyodmongo-0.9.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/docs/assets/images/favicon.png` & `pyodmongo-0.9.2/docs/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/docs/assets/images/insomnia_request.png` & `pyodmongo-0.9.2/docs/assets/images/insomnia_request.png`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/docs/assets/images/logo.png` & `pyodmongo-0.9.2/docs/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/docs/assets/images/pyodmongo_Logo_BG_Dark.png` & `pyodmongo-0.9.2/docs/assets/images/pyodmongo_Logo_BG_Dark.png`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/docs/assets/images/pyodmongo_Logo_BG_White.png` & `pyodmongo-0.9.2/docs/assets/images/pyodmongo_Logo_BG_White.png`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/docs/en/aggregation.md` & `pyodmongo-0.9.2/docs/en/aggregation.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/docs/en/contributing.md` & `pyodmongo-0.9.2/docs/en/contributing.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/docs/en/db_model.md` & `pyodmongo-0.9.2/docs/en/db_model.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/docs/en/delete.md` & `pyodmongo-0.9.2/docs/en/delete.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/docs/en/fastapi.md` & `pyodmongo-0.9.2/docs/en/fastapi.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/docs/en/find.md` & `pyodmongo-0.9.2/docs/en/find.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/docs/en/getting_started.md` & `pyodmongo-0.9.2/docs/en/getting_started.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/docs/en/index.md` & `pyodmongo-0.9.2/docs/en/index.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/docs/en/indexes.md` & `pyodmongo-0.9.2/docs/en/indexes.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/docs/en/query.md` & `pyodmongo-0.9.2/docs/en/query.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/docs/en/save.md` & `pyodmongo-0.9.2/docs/en/save.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/docs/pt-BR/aggregation.md` & `pyodmongo-0.9.2/docs/pt-BR/aggregation.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/docs/pt-BR/contributing.md` & `pyodmongo-0.9.2/docs/pt-BR/contributing.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/docs/pt-BR/db_model.md` & `pyodmongo-0.9.2/docs/pt-BR/db_model.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/docs/pt-BR/delete.md` & `pyodmongo-0.9.2/docs/pt-BR/delete.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/docs/pt-BR/fastapi.md` & `pyodmongo-0.9.2/docs/pt-BR/fastapi.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/docs/pt-BR/find.md` & `pyodmongo-0.9.2/docs/pt-BR/find.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/docs/pt-BR/getting_started.md` & `pyodmongo-0.9.2/docs/pt-BR/getting_started.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/docs/pt-BR/index.md` & `pyodmongo-0.9.2/docs/pt-BR/index.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/docs/pt-BR/indexes.md` & `pyodmongo-0.9.2/docs/pt-BR/indexes.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/docs/pt-BR/query.md` & `pyodmongo-0.9.2/docs/pt-BR/query.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/docs/pt-BR/save.md` & `pyodmongo-0.9.2/docs/pt-BR/save.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/pyodmongo/async_engine/engine.py` & `pyodmongo-0.9.2/pyodmongo/async_engine/engine.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/pyodmongo/engine/engine.py` & `pyodmongo-0.9.2/pyodmongo/engine/engine.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/pyodmongo/engine/utils.py` & `pyodmongo-0.9.2/pyodmongo/engine/utils.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/pyodmongo/models/db_field_info.py` & `pyodmongo-0.9.2/pyodmongo/models/db_field_info.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/pyodmongo/models/db_model.py` & `pyodmongo-0.9.2/pyodmongo/models/db_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,19 +100,19 @@
     model_config = ConfigDict(populate_by_name=True)
     _pipeline: ClassVar = []
 
     def __remove_empty_dict(self, dct: dict):
         if dct == {}:
             return None
         for key, value in dct.items():
-            if value == {} or value == []:
+            if value == {}:
                 dct[key] = None
             elif type(value) == dict:
                 dct[key] = self.__remove_empty_dict(dct=value)
-        is_full_empty = all(v == None or v == {} or v == [] for v in dct.values())
+        is_full_empty = all(v == None or v == {} for v in dct.values())
         if is_full_empty:
             return None
         return dct
 
     def __init__(self, **attrs):
         for key, value in attrs.items():
             if type(value) == dict:
```

### Comparing `pyodmongo-0.9.1/pyodmongo/models/fields.py` & `pyodmongo-0.9.2/pyodmongo/models/fields.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/pyodmongo/models/id_model.py` & `pyodmongo-0.9.2/pyodmongo/models/id_model.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/pyodmongo/models/paginate.py` & `pyodmongo-0.9.2/pyodmongo/models/paginate.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/pyodmongo/models/query_operators.py` & `pyodmongo-0.9.2/pyodmongo/models/query_operators.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/pyodmongo/models/responses.py` & `pyodmongo-0.9.2/pyodmongo/models/responses.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/pyodmongo/queries/comparison_operators.py` & `pyodmongo-0.9.2/pyodmongo/queries/comparison_operators.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/pyodmongo/queries/logical_operators.py` & `pyodmongo-0.9.2/pyodmongo/queries/logical_operators.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/pyodmongo/queries/query_string.py` & `pyodmongo-0.9.2/pyodmongo/queries/query_string.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/pyodmongo/queries/sort_operator.py` & `pyodmongo-0.9.2/pyodmongo/queries/sort_operator.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/pyodmongo/services/aggregate_stages.py` & `pyodmongo-0.9.2/pyodmongo/services/aggregate_stages.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/pyodmongo/services/model_init.py` & `pyodmongo-0.9.2/pyodmongo/services/model_init.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/pyodmongo/services/query_operators.py` & `pyodmongo-0.9.2/pyodmongo/services/query_operators.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/tests/test_async_aggregate.py` & `pyodmongo-0.9.2/tests/test_async_aggregate.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/tests/test_async_crud_db.py` & `pyodmongo-0.9.2/tests/test_async_crud_db.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/tests/test_class.py` & `pyodmongo-0.9.2/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/tests/test_db_field_info.py` & `pyodmongo-0.9.2/tests/test_db_field_info.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/tests/test_db_index.py` & `pyodmongo-0.9.2/tests/test_db_index.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/tests/test_dict_empty.py` & `pyodmongo-0.9.2/tests/test_fastapi.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,41 @@
-from pyodmongo import DbModel, Id
+from fastapi import FastAPI
+from fastapi.testclient import TestClient
+from pyodmongo import DbModel
 
+app = FastAPI()
 
-def test_empty_dict():
-    class MyModel1(DbModel):
-        attr1: str | None
-        _collection = "my_model_1"
-
-    class MyModel2(DbModel):
-        attr2: str | None
-        my_model_1: MyModel1 | Id | None
-        _collection = "my_model_2"
-
-    class MyModel3(DbModel):
-        attr3: str | None
-        my_model_2: MyModel2 | Id | None
-        my_model_2_2: MyModel2 | Id | None
-        my_model_2_3: MyModel2 | Id | None
-        _collection = "my_model_3"
-
-    dct = {
-        "attr3": "attr3",
-        "my_model_2": {"attr2": "Escrito", "my_model_1": {"attr1": {}}},
-        "my_model_2_2": {"my_model_1": {}},
-        "my_model_2_3": {},
+
+class Model1(DbModel):
+    attr1: str = None
+    attr2: str
+
+
+class Model2(Model1):
+    attr3: str
+    attr4: str = None
+
+
+@app.post("/", response_model=Model2)
+async def read_main(input_obj: Model2):
+    return input_obj
+
+
+client = TestClient(app)
+
+
+def test_response_model_and_output_obj():
+    json_body = {
+        "attr2": "Value 2",
+        "attr3": "Value 3",
     }
-    obj = MyModel3(**dct)
-    assert obj.model_dump() == {
-        "attr3": "attr3",
-        "my_model_2": {
-            "id": None,
-            "created_at": None,
-            "updated_at": None,
-            "attr2": "Escrito",
-            "my_model_1": None,
-        },
-        "my_model_2_2": None,
-        "my_model_2_3": None,
+    response = client.post(url="/", json=json_body)
+    assert response.status_code == 200
+    assert response.json() == {
         "id": None,
         "created_at": None,
         "updated_at": None,
+        "attr1": None,
+        "attr2": "Value 2",
+        "attr3": "Value 3",
+        "attr4": None,
     }
```

### Comparing `pyodmongo-0.9.1/tests/test_model_init_functions.py` & `pyodmongo-0.9.2/tests/test_model_init_functions.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/tests/test_object_id.py` & `pyodmongo-0.9.2/tests/test_object_id.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/tests/test_project_pipeline.py` & `pyodmongo-0.9.2/tests/test_project_pipeline.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/tests/test_pydantic_validators.py` & `pyodmongo-0.9.2/tests/test_pydantic_validators.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/tests/test_queries.py` & `pyodmongo-0.9.2/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/tests/test_reference_pipeline.py` & `pyodmongo-0.9.2/tests/test_reference_pipeline.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/tests/test_save_dict.py` & `pyodmongo-0.9.2/tests/test_save_dict.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/tests/test_sync_aggregate.py` & `pyodmongo-0.9.2/tests/test_sync_aggregate.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/tests/test_sync_crud_db.py` & `pyodmongo-0.9.2/tests/test_sync_crud_db.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/.gitignore` & `pyodmongo-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/LICENSE` & `pyodmongo-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/README.md` & `pyodmongo-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.9.1/pyproject.toml` & `pyodmongo-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyodmongo"
-version = "0.9.1"
+version = "0.9.2"
 license = "MIT"
 authors = [
   { name="Mauro André", email="eng.mauroandre@gmail.com" },
 ]
 description = "A syncrounous and asyncrounous Python ODM for MongoDB based on Pydantic"
 readme = "README.md"
 requires-python = ">=3.11"
```

### Comparing `pyodmongo-0.9.1/PKG-INFO` & `pyodmongo-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyodmongo
-Version: 0.9.1
+Version: 0.9.2
 Summary: A syncrounous and asyncrounous Python ODM for MongoDB based on Pydantic
 Project-URL: Homepage, https://github.com/mauro-andre/pyodmongo
 Project-URL: Documentation, https://pyodmongo.dev
 Author-email: Mauro André <eng.mauroandre@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

