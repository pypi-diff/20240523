# Comparing `tmp/nextline_rdb-0.6.6.tar.gz` & `tmp/nextline_rdb-0.6.7.tar.gz`

## Comparing `nextline_rdb-0.6.6.tar` & `nextline_rdb-0.6.7.tar`

### file list

```diff
@@ -1,241 +1,247 @@
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/Dockerfile
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/setup.cfg
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/.github/dependabot.yml
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/.github/release.yml
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/.github/workflows/pypi.yml
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/.github/workflows/release.yml
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/.github/workflows/type-check.yml
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/.github/workflows/unit-test.yml
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/.vscode/settings.json
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/.gitignore
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/__about__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/__init__.py
--rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/db.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/default.toml
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/init.py
--rw-r--r--   0        0        0     4763 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/pagination.py
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/py.typed
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/README.md
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/alembic.ini
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/conftest.py
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/env.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/script.py.mako
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/__init__.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_245c4152e8d7/__init__.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_245c4152e8d7/model_hello.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_245c4152e8d7/model_prompt.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_245c4152e8d7/model_run.py
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_245c4152e8d7/model_script.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_245c4152e8d7/model_stdout.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_245c4152e8d7/model_trace.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_245c4152e8d7/base/__init__.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_245c4152e8d7/base/convention.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_245c4152e8d7/base/model_base.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_245c4152e8d7/base/repr_.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/__init__.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/model_hello.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/model_prompt.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/model_run.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/model_stdout.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/model_trace.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/base/__init__.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/base/convention.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/base/model_base.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/base/repr_.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/__init__.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/st_prompt.py
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/st_run.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/st_stdout.py
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/st_trace.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/__init__.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_prompt.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_prompt_list.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_run.py
--rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_run_list.py
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_started_at_ended_at.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_stdout.py
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_stdout_list.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_trace.py
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_trace_list.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/tests/__init__.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/tests/test_model_prompt.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/tests/test_model_run.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/tests/test_model_stdout.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/tests/test_model_trace.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/tests/test_repr_val.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_6e3cf7d9b6bf/__init__.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_6e3cf7d9b6bf/model_hello.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_6e3cf7d9b6bf/model_prompt.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_6e3cf7d9b6bf/model_run.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_6e3cf7d9b6bf/model_script.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_6e3cf7d9b6bf/model_stdout.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_6e3cf7d9b6bf/model_trace.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_6e3cf7d9b6bf/base/__init__.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_6e3cf7d9b6bf/base/convention.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_6e3cf7d9b6bf/base/model_base.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_6e3cf7d9b6bf/base/repr_.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/__init__.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/model_hello.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/model_prompt.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/model_run.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/model_script.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/model_stdout.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/model_trace.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/base/__init__.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/base/convention.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/base/model_base.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/base/repr_.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/__init__.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/st_prompt.py
--rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/st_run.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/st_script.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/st_stdout.py
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/st_trace.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/__init__.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_prompt.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_prompt_list.py
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_run.py
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_run_list.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_script.py
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_started_at_ended_at.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_stdout.py
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_stdout_list.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_trace.py
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_trace_list.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/tests/__init__.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/tests/test_model_prompt.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/tests/test_model_run.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/tests/test_model_stdout.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/tests/test_model_trace.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/tests/test_repr_val.py
--rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/versions/2022-03-14_14:00-de90b787e92f.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/versions/2022-03-16_19:01-5a08750d6760.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/versions/2024-01-29_14:12-2fa41efc56f0.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/versions/2024-01-29_15:11-6e3cf7d9b6bf.py
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/versions/2024-01-29_16:33-cafceacada62.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/versions/2024-01-30_13:48-f9a742bb2297.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/versions/2024-02-02_14:02-c72fa3ee6a1a.py
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/versions/2024-02-02_15:38-245c4152e8d7.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/versions/2024-02-03_14:13-68cb1c590d1f.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/alembic/versions/2024-02-04_09:01-4dc6a93dfed8.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/__init__.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/model_hello.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/model_prompt.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/model_run.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/model_script.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/model_stdout.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/model_trace.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/base/__init__.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/base/convention.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/base/model_base.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/base/repr_.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/__init__.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/st_instance.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/st_prompt.py
--rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/st_run.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/st_script.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/st_stdout.py
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/st_trace.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/tests/__init__.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/tests/test_st_instance_list.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/tests/test_st_prompt.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/tests/test_st_prompt_list.py
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/tests/test_st_run.py
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/tests/test_st_run_list.py
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/tests/test_st_script.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/tests/test_st_script_list.py
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/tests/test_st_started_at_ended_at.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/tests/test_st_stdout.py
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/tests/test_st_stdout_list.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/tests/test_st_trace.py
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/tests/test_st_trace_list.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/tests/__init__.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/tests/test_model_prompt.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/tests/test_model_run.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/tests/test_model_script.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/tests/test_model_stdout.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/tests/test_model_trace.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/models/tests/test_repr_val.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/schema/__init__.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/schema/mutation.py
--rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/schema/query.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/schema/nodes/__init__.py
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/schema/nodes/prompt_node.py
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/schema/nodes/run_node.py
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/schema/nodes/stdout_node.py
--rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/schema/nodes/trace_node.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/schema/pagination/__init__.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/schema/pagination/connection.py
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/schema/pagination/db.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/utils/__init__.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/utils/gen.py
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/utils/sa.py
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/utils/safe.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/utils/url.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/utils/utc.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/utils/strategies/__init__.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/utils/strategies/datetime.py
--rw-r--r--   0        0        0     4410 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/utils/strategies/misc.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/utils/strategies/script.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/write/__init__.py
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/write/write_prompt_table.py
--rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/write/write_run_table.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/write/write_script_table.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/write/write_stdout_table.py
--rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/src/nextline_rdb/write/write_trace_table.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/__init__.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/conftest.py
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/test_init.py
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/test_plugin.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/test_version.py
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/test_write.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/alembic/__init__.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/alembic/conftest.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/alembic/test_up_to_date.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/alembic/migrations/__init__.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/alembic/migrations/conftest.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/alembic/migrations/test_2024-01-30_13:48-f9a742bb2297.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/alembic/migrations/test_2024-02-02_14:02-c72fa3ee6a1a.py
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/alembic/migrations/test_2024-02-04_09:01-4dc6a93dfed8.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/db/__init__.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/db/models.py
--rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/db/test_db.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/db/test_foreign_keys.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/example_script/__init__.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/example_script/script.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/example_script/script_asyncio.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/example_script/script_threading.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/pagination/__init__.py
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/pagination/funcs.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/pagination/models.py
--rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/pagination/test_load_models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/schema/__init__.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/schema/graphql/__init__.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/schema/graphql/mutations/RDBDeleteRuns.gql
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/schema/graphql/queries/RDBConnections.gql
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/schema/graphql/queries/RDBRun.gql
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/schema/graphql/queries/RDBRuns.gql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/schema/mutations/__init__.py
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/schema/mutations/test_delete_runs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/schema/queries/__init__.py
--rw-r--r--   0        0        0     6778 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/schema/queries/test_pagination.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/schema/queries/test_rdb.py
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/schema/queries/test_run.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/utils/__init__.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/utils/test_mark_last.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/utils/test_safe_compare.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/utils/test_safe_min_max.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/utils/strategies/__init__.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/utils/strategies/test_st_datetimes.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/utils/strategies/test_st_ints.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/utils/strategies/test_st_python_scripts.py
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/tests/utils/strategies/test_st_ranges.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/LICENSE.txt
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/README.md
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/pyproject.toml
--rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 nextline_rdb-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/Dockerfile
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/setup.cfg
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/.github/CODEOWNERS
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/.github/dependabot.yml
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/.github/release.yml
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/.github/workflows/docker-test.yml
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/.github/workflows/release.yml
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/.github/workflows/type-check.yml
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/.github/workflows/unit-test-latest.yml
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/.github/workflows/unit-test-min.yml
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/.github/workflows/unit-test.yml
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/.vscode/settings.json
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/ci/latest/requirements.txt
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/ci/minimum/requirements.txt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/.gitignore
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/__about__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/__init__.py
+-rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/db.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/default.toml
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/init.py
+-rw-r--r--   0        0        0     4763 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/pagination.py
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/py.typed
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/README.md
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/alembic.ini
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/conftest.py
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/env.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/script.py.mako
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/__init__.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_245c4152e8d7/__init__.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_245c4152e8d7/model_hello.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_245c4152e8d7/model_prompt.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_245c4152e8d7/model_run.py
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_245c4152e8d7/model_script.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_245c4152e8d7/model_stdout.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_245c4152e8d7/model_trace.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_245c4152e8d7/base/__init__.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_245c4152e8d7/base/convention.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_245c4152e8d7/base/model_base.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_245c4152e8d7/base/repr_.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/__init__.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/model_hello.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/model_prompt.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/model_run.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/model_stdout.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/model_trace.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/base/__init__.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/base/convention.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/base/model_base.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/base/repr_.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/__init__.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/st_prompt.py
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/st_run.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/st_stdout.py
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/st_trace.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/__init__.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_prompt.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_prompt_list.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_run.py
+-rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_run_list.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_started_at_ended_at.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_stdout.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_stdout_list.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_trace.py
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_trace_list.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/tests/__init__.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/tests/test_model_prompt.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/tests/test_model_run.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/tests/test_model_stdout.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/tests/test_model_trace.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/tests/test_repr_val.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_6e3cf7d9b6bf/__init__.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_6e3cf7d9b6bf/model_hello.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_6e3cf7d9b6bf/model_prompt.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_6e3cf7d9b6bf/model_run.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_6e3cf7d9b6bf/model_script.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_6e3cf7d9b6bf/model_stdout.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_6e3cf7d9b6bf/model_trace.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_6e3cf7d9b6bf/base/__init__.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_6e3cf7d9b6bf/base/convention.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_6e3cf7d9b6bf/base/model_base.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_6e3cf7d9b6bf/base/repr_.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/__init__.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/model_hello.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/model_prompt.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/model_run.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/model_script.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/model_stdout.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/model_trace.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/base/__init__.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/base/convention.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/base/model_base.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/base/repr_.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/__init__.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/st_prompt.py
+-rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/st_run.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/st_script.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/st_stdout.py
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/st_trace.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/__init__.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_prompt.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_prompt_list.py
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_run.py
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_run_list.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_script.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_started_at_ended_at.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_stdout.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_stdout_list.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_trace.py
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_trace_list.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/tests/__init__.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/tests/test_model_prompt.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/tests/test_model_run.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/tests/test_model_stdout.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/tests/test_model_trace.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/tests/test_repr_val.py
+-rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/versions/2022-03-14_14:00-de90b787e92f.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/versions/2022-03-16_19:01-5a08750d6760.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/versions/2024-01-29_14:12-2fa41efc56f0.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/versions/2024-01-29_15:11-6e3cf7d9b6bf.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/versions/2024-01-29_16:33-cafceacada62.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/versions/2024-01-30_13:48-f9a742bb2297.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/versions/2024-02-02_14:02-c72fa3ee6a1a.py
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/versions/2024-02-02_15:38-245c4152e8d7.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/versions/2024-02-03_14:13-68cb1c590d1f.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/alembic/versions/2024-02-04_09:01-4dc6a93dfed8.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/__init__.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/model_hello.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/model_prompt.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/model_run.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/model_script.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/model_stdout.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/model_trace.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/base/__init__.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/base/convention.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/base/model_base.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/base/repr_.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/__init__.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/st_instance.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/st_prompt.py
+-rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/st_run.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/st_script.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/st_stdout.py
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/st_trace.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/tests/__init__.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/tests/test_st_instance_list.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/tests/test_st_prompt.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/tests/test_st_prompt_list.py
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/tests/test_st_run.py
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/tests/test_st_run_list.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/tests/test_st_script.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/tests/test_st_script_list.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/tests/test_st_started_at_ended_at.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/tests/test_st_stdout.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/tests/test_st_stdout_list.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/tests/test_st_trace.py
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/tests/test_st_trace_list.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/tests/__init__.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/tests/test_model_prompt.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/tests/test_model_run.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/tests/test_model_script.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/tests/test_model_stdout.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/tests/test_model_trace.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/models/tests/test_repr_val.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/schema/__init__.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/schema/mutation.py
+-rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/schema/query.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/schema/nodes/__init__.py
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/schema/nodes/prompt_node.py
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/schema/nodes/run_node.py
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/schema/nodes/stdout_node.py
+-rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/schema/nodes/trace_node.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/schema/pagination/__init__.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/schema/pagination/connection.py
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/schema/pagination/db.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/utils/__init__.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/utils/gen.py
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/utils/sa.py
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/utils/safe.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/utils/url.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/utils/utc.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/utils/strategies/__init__.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/utils/strategies/datetime.py
+-rw-r--r--   0        0        0     4410 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/utils/strategies/misc.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/utils/strategies/script.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/write/__init__.py
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/write/write_prompt_table.py
+-rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/write/write_run_table.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/write/write_script_table.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/write/write_stdout_table.py
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/src/nextline_rdb/write/write_trace_table.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/__init__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/conftest.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/test_init.py
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/test_plugin.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/test_version.py
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/test_write.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/alembic/__init__.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/alembic/conftest.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/alembic/test_up_to_date.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/alembic/migrations/__init__.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/alembic/migrations/conftest.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/alembic/migrations/test_2024-01-30_13:48-f9a742bb2297.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/alembic/migrations/test_2024-02-02_14:02-c72fa3ee6a1a.py
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/alembic/migrations/test_2024-02-04_09:01-4dc6a93dfed8.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/db/__init__.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/db/models.py
+-rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/db/test_db.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/db/test_foreign_keys.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/example_script/__init__.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/example_script/script.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/example_script/script_asyncio.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/example_script/script_threading.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/pagination/__init__.py
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/pagination/funcs.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/pagination/models.py
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/pagination/test_load_models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/schema/__init__.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/schema/graphql/__init__.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/schema/graphql/mutations/RDBDeleteRuns.gql
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/schema/graphql/queries/RDBConnections.gql
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/schema/graphql/queries/RDBRun.gql
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/schema/graphql/queries/RDBRuns.gql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/schema/mutations/__init__.py
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/schema/mutations/test_delete_runs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/schema/queries/__init__.py
+-rw-r--r--   0        0        0     6778 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/schema/queries/test_pagination.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/schema/queries/test_rdb.py
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/schema/queries/test_run.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/utils/__init__.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/utils/test_mark_last.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/utils/test_safe_compare.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/utils/test_safe_min_max.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/utils/strategies/__init__.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/utils/strategies/test_st_datetimes.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/utils/strategies/test_st_ints.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/utils/strategies/test_st_python_scripts.py
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/tests/utils/strategies/test_st_ranges.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/LICENSE.txt
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/README.md
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 nextline_rdb-0.6.7/PKG-INFO
```

### Comparing `nextline_rdb-0.6.6/.github/workflows/pypi.yml` & `nextline_rdb-0.6.7/.github/workflows/pypi.yml`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 jobs:
   deploy:
     runs-on: ubuntu-latest
     environment: pypi
     permissions:
       id-token: write
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: '3.10'
 
       - name: Install packages
         run: |
           pip install --upgrade pip
           pip install --upgrade hatch
```

### Comparing `nextline_rdb-0.6.6/.github/workflows/release.yml` & `nextline_rdb-0.6.7/.github/workflows/release.yml`

 * *Files 22% similar despite different names*

```diff
@@ -9,17 +9,17 @@
   deploy:
     runs-on: ubuntu-latest
     permissions:
       contents: write
 
     steps:
       - name: Checkout
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
       - name: Install gh CLI
-        uses: actions/setup-node@v3
+        uses: actions/setup-node@v4
         with:
           node-version: "18"
       - name: Create Release
         env:
           GH_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         run: |
           gh release create ${GITHUB_REF#refs/tags/} \
```

### Comparing `nextline_rdb-0.6.6/.github/workflows/type-check.yml` & `nextline_rdb-0.6.7/.github/workflows/type-check.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 name: Check static types
 
 on:
   push:
     branches:
-      - "**"
+      - main
   pull_request:
     branches:
-      - "**"
+      - main
 
 jobs:
   run:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.10"
 
       - name: Install packages
         run: |
           pip install --upgrade pip
           pip install -e '.[tests]'
```

### Comparing `nextline_rdb-0.6.6/.github/workflows/unit-test.yml` & `nextline_rdb-0.6.7/.github/workflows/unit-test.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 name: Run unit tests
 
 on:
   push:
     branches:
-      - "**"
+      - main
   pull_request:
     branches:
-      - "**"
+      - main
 
 concurrency:
   group: unit-test-${{ github.head_ref }}
   cancel-in-progress: true
 
 env:
   PYTHONUNBUFFERED: "1"
@@ -22,29 +22,39 @@
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.10", "3.11", "3.12"]
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install packages
         run: |
           pip install --upgrade pip
           pip install -e '.[tests]'
           pip list
 
       - name: Run tests
         run: pytest -vv --cov --cov-report=xml
 
+      - name: Check Codecov token # e.g., Dependabot doesn't have the CODECOV_TOKEN
+        id: check_codecov_token
+        run: |
+          if [ -n "${{ secrets.CODECOV_TOKEN }}" ]; then
+            echo "exists=true" >> $GITHUB_OUTPUT
+          else
+            echo "exists=false" >> $GITHUB_OUTPUT
+          fi
+
       - name: Upload coverage to Codecov
-        uses: codecov/codecov-action@v1
+        if: steps.check_codecov_token.outputs.exists == 'true'
+        uses: codecov/codecov-action@v4
         with:
           fail_ci_if_error: true
           token: ${{ secrets.CODECOV_TOKEN }}
           verbose: true
```

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/db.py` & `nextline_rdb-0.6.7/src/nextline_rdb/db.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/init.py` & `nextline_rdb-0.6.7/src/nextline_rdb/init.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/pagination.py` & `nextline_rdb-0.6.7/src/nextline_rdb/pagination.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/plugin.py` & `nextline_rdb-0.6.7/src/nextline_rdb/plugin.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/README.md` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/README.md`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/alembic.ini` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/env.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/env.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/script.py.mako` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_245c4152e8d7/model_prompt.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_245c4152e8d7/model_prompt.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_245c4152e8d7/model_run.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_245c4152e8d7/model_run.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_245c4152e8d7/model_script.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_245c4152e8d7/model_script.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_245c4152e8d7/model_stdout.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_245c4152e8d7/model_stdout.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_245c4152e8d7/model_trace.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_245c4152e8d7/model_trace.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_245c4152e8d7/base/convention.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_245c4152e8d7/base/convention.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_245c4152e8d7/base/repr_.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_245c4152e8d7/base/repr_.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/model_prompt.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/model_prompt.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/model_run.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/model_run.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/model_stdout.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/model_stdout.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/model_trace.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/model_trace.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/base/convention.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/base/convention.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/base/repr_.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/base/repr_.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/__init__.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/st_prompt.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/st_prompt.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/st_run.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/st_run.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/st_stdout.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/st_stdout.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/st_trace.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/st_trace.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/utils.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/utils.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_prompt.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_prompt.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_prompt_list.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_prompt_list.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_run.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_run.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_run_list.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_run_list.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_started_at_ended_at.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_started_at_ended_at.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_stdout.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_stdout.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_stdout_list.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_stdout_list.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_trace.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_trace.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_trace_list.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/strategies/tests/test_st_trace_list.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/tests/test_model_prompt.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/tests/test_model_prompt.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/tests/test_model_run.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/tests/test_model_run.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/tests/test_model_stdout.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/tests/test_model_stdout.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/tests/test_model_trace.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/tests/test_model_trace.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_5a08750d6760/tests/test_repr_val.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_5a08750d6760/tests/test_repr_val.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_6e3cf7d9b6bf/model_prompt.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_6e3cf7d9b6bf/model_prompt.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_6e3cf7d9b6bf/model_run.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_6e3cf7d9b6bf/model_run.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_6e3cf7d9b6bf/model_stdout.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_6e3cf7d9b6bf/model_stdout.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_6e3cf7d9b6bf/model_trace.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_6e3cf7d9b6bf/model_trace.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_6e3cf7d9b6bf/base/convention.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_6e3cf7d9b6bf/base/convention.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_6e3cf7d9b6bf/base/repr_.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_6e3cf7d9b6bf/base/repr_.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/model_prompt.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/model_prompt.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/model_run.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/model_run.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/model_stdout.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/model_stdout.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/model_trace.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/model_trace.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/base/convention.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/base/convention.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/base/repr_.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/base/repr_.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/__init__.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/st_prompt.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/st_prompt.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/st_run.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/st_run.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/st_stdout.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/st_stdout.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/st_trace.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/st_trace.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/utils.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/utils.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_prompt.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_prompt.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_prompt_list.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_prompt_list.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_run.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_run.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_run_list.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_run_list.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_script.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_script.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_started_at_ended_at.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_started_at_ended_at.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_stdout.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_stdout.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_stdout_list.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_stdout_list.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_trace.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_trace.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_trace_list.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/strategies/tests/test_st_trace_list.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/tests/test_model_prompt.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/tests/test_model_prompt.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/tests/test_model_run.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/tests/test_model_run.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/tests/test_model_stdout.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/tests/test_model_stdout.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/tests/test_model_trace.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/tests/test_model_trace.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/models/rev_f9a742bb2297/tests/test_repr_val.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/models/rev_f9a742bb2297/tests/test_repr_val.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/versions/2022-03-14_14:00-de90b787e92f.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/versions/2022-03-14_14:00-de90b787e92f.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/versions/2022-03-16_19:01-5a08750d6760.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/versions/2022-03-16_19:01-5a08750d6760.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/versions/2024-01-29_14:12-2fa41efc56f0.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/versions/2024-01-29_14:12-2fa41efc56f0.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/versions/2024-01-29_15:11-6e3cf7d9b6bf.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/versions/2024-01-29_15:11-6e3cf7d9b6bf.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/versions/2024-01-29_16:33-cafceacada62.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/versions/2024-01-29_16:33-cafceacada62.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/versions/2024-01-30_13:48-f9a742bb2297.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/versions/2024-01-30_13:48-f9a742bb2297.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/versions/2024-02-02_14:02-c72fa3ee6a1a.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/versions/2024-02-02_14:02-c72fa3ee6a1a.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/versions/2024-02-02_15:38-245c4152e8d7.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/versions/2024-02-02_15:38-245c4152e8d7.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/versions/2024-02-03_14:13-68cb1c590d1f.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/versions/2024-02-03_14:13-68cb1c590d1f.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/alembic/versions/2024-02-04_09:01-4dc6a93dfed8.py` & `nextline_rdb-0.6.7/src/nextline_rdb/alembic/versions/2024-02-04_09:01-4dc6a93dfed8.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/models/model_prompt.py` & `nextline_rdb-0.6.7/src/nextline_rdb/models/model_prompt.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/models/model_run.py` & `nextline_rdb-0.6.7/src/nextline_rdb/models/model_run.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/models/model_script.py` & `nextline_rdb-0.6.7/src/nextline_rdb/models/model_script.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/models/model_stdout.py` & `nextline_rdb-0.6.7/src/nextline_rdb/models/model_stdout.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/models/model_trace.py` & `nextline_rdb-0.6.7/src/nextline_rdb/models/model_trace.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/models/base/convention.py` & `nextline_rdb-0.6.7/src/nextline_rdb/models/base/convention.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/models/base/repr_.py` & `nextline_rdb-0.6.7/src/nextline_rdb/models/base/repr_.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/__init__.py` & `nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/st_instance.py` & `nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/st_instance.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/st_prompt.py` & `nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/st_prompt.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/st_run.py` & `nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/st_run.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/st_script.py` & `nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/st_script.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/st_stdout.py` & `nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/st_stdout.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/st_trace.py` & `nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/st_trace.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/utils.py` & `nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/utils.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/tests/test_st_instance_list.py` & `nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/tests/test_st_instance_list.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/tests/test_st_prompt.py` & `nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/tests/test_st_prompt.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/tests/test_st_prompt_list.py` & `nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/tests/test_st_prompt_list.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/tests/test_st_run.py` & `nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/tests/test_st_run.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/tests/test_st_run_list.py` & `nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/tests/test_st_run_list.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/tests/test_st_script.py` & `nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/tests/test_st_script.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/tests/test_st_script_list.py` & `nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/tests/test_st_script_list.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/tests/test_st_started_at_ended_at.py` & `nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/tests/test_st_started_at_ended_at.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/tests/test_st_stdout.py` & `nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/tests/test_st_stdout.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/tests/test_st_stdout_list.py` & `nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/tests/test_st_stdout_list.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/tests/test_st_trace.py` & `nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/tests/test_st_trace.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/models/strategies/tests/test_st_trace_list.py` & `nextline_rdb-0.6.7/src/nextline_rdb/models/strategies/tests/test_st_trace_list.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/models/tests/test_model_prompt.py` & `nextline_rdb-0.6.7/src/nextline_rdb/models/tests/test_model_prompt.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/models/tests/test_model_run.py` & `nextline_rdb-0.6.7/src/nextline_rdb/models/tests/test_model_run.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/models/tests/test_model_script.py` & `nextline_rdb-0.6.7/src/nextline_rdb/models/tests/test_model_script.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/models/tests/test_model_stdout.py` & `nextline_rdb-0.6.7/src/nextline_rdb/models/tests/test_model_stdout.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/models/tests/test_model_trace.py` & `nextline_rdb-0.6.7/src/nextline_rdb/models/tests/test_model_trace.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/models/tests/test_repr_val.py` & `nextline_rdb-0.6.7/src/nextline_rdb/models/tests/test_repr_val.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/schema/mutation.py` & `nextline_rdb-0.6.7/src/nextline_rdb/schema/mutation.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/schema/query.py` & `nextline_rdb-0.6.7/src/nextline_rdb/schema/query.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/schema/nodes/prompt_node.py` & `nextline_rdb-0.6.7/src/nextline_rdb/schema/nodes/prompt_node.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/schema/nodes/run_node.py` & `nextline_rdb-0.6.7/src/nextline_rdb/schema/nodes/run_node.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/schema/nodes/stdout_node.py` & `nextline_rdb-0.6.7/src/nextline_rdb/schema/nodes/stdout_node.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/schema/nodes/trace_node.py` & `nextline_rdb-0.6.7/src/nextline_rdb/schema/nodes/trace_node.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/schema/pagination/connection.py` & `nextline_rdb-0.6.7/src/nextline_rdb/schema/pagination/connection.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/schema/pagination/db.py` & `nextline_rdb-0.6.7/src/nextline_rdb/schema/pagination/db.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/utils/__init__.py` & `nextline_rdb-0.6.7/src/nextline_rdb/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/utils/gen.py` & `nextline_rdb-0.6.7/src/nextline_rdb/utils/gen.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/utils/sa.py` & `nextline_rdb-0.6.7/src/nextline_rdb/utils/sa.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/utils/safe.py` & `nextline_rdb-0.6.7/src/nextline_rdb/utils/safe.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/utils/url.py` & `nextline_rdb-0.6.7/src/nextline_rdb/utils/url.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/utils/utc.py` & `nextline_rdb-0.6.7/src/nextline_rdb/utils/utc.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/utils/strategies/datetime.py` & `nextline_rdb-0.6.7/src/nextline_rdb/utils/strategies/datetime.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/utils/strategies/misc.py` & `nextline_rdb-0.6.7/src/nextline_rdb/utils/strategies/misc.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/utils/strategies/script.py` & `nextline_rdb-0.6.7/src/nextline_rdb/utils/strategies/script.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/write/__init__.py` & `nextline_rdb-0.6.7/src/nextline_rdb/write/__init__.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/write/write_prompt_table.py` & `nextline_rdb-0.6.7/src/nextline_rdb/write/write_prompt_table.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/write/write_run_table.py` & `nextline_rdb-0.6.7/src/nextline_rdb/write/write_run_table.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/write/write_script_table.py` & `nextline_rdb-0.6.7/src/nextline_rdb/write/write_script_table.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/write/write_stdout_table.py` & `nextline_rdb-0.6.7/src/nextline_rdb/write/write_stdout_table.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/src/nextline_rdb/write/write_trace_table.py` & `nextline_rdb-0.6.7/src/nextline_rdb/write/write_trace_table.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/tests/test_init.py` & `nextline_rdb-0.6.7/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/tests/test_plugin.py` & `nextline_rdb-0.6.7/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/tests/test_write.py` & `nextline_rdb-0.6.7/tests/test_write.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/tests/alembic/conftest.py` & `nextline_rdb-0.6.7/tests/alembic/conftest.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/tests/alembic/test_up_to_date.py` & `nextline_rdb-0.6.7/tests/alembic/test_up_to_date.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/tests/alembic/migrations/conftest.py` & `nextline_rdb-0.6.7/tests/alembic/migrations/conftest.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/tests/alembic/migrations/test_2024-01-30_13:48-f9a742bb2297.py` & `nextline_rdb-0.6.7/tests/alembic/migrations/test_2024-01-30_13:48-f9a742bb2297.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/tests/alembic/migrations/test_2024-02-02_14:02-c72fa3ee6a1a.py` & `nextline_rdb-0.6.7/tests/alembic/migrations/test_2024-02-02_14:02-c72fa3ee6a1a.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/tests/alembic/migrations/test_2024-02-04_09:01-4dc6a93dfed8.py` & `nextline_rdb-0.6.7/tests/alembic/migrations/test_2024-02-04_09:01-4dc6a93dfed8.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/tests/db/models.py` & `nextline_rdb-0.6.7/tests/db/models.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/tests/db/test_db.py` & `nextline_rdb-0.6.7/tests/db/test_db.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/tests/db/test_foreign_keys.py` & `nextline_rdb-0.6.7/tests/db/test_foreign_keys.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/tests/pagination/funcs.py` & `nextline_rdb-0.6.7/tests/pagination/funcs.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/tests/pagination/test_load_models.py` & `nextline_rdb-0.6.7/tests/pagination/test_load_models.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/tests/schema/graphql/queries/RDBConnections.gql` & `nextline_rdb-0.6.7/tests/schema/graphql/queries/RDBConnections.gql`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/tests/schema/graphql/queries/RDBRun.gql` & `nextline_rdb-0.6.7/tests/schema/graphql/queries/RDBRun.gql`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/tests/schema/mutations/test_delete_runs.py` & `nextline_rdb-0.6.7/tests/schema/mutations/test_delete_runs.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/tests/schema/queries/test_pagination.py` & `nextline_rdb-0.6.7/tests/schema/queries/test_pagination.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/tests/schema/queries/test_rdb.py` & `nextline_rdb-0.6.7/tests/schema/queries/test_rdb.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/tests/schema/queries/test_run.py` & `nextline_rdb-0.6.7/tests/schema/queries/test_run.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/tests/utils/test_safe_compare.py` & `nextline_rdb-0.6.7/tests/utils/test_safe_compare.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/tests/utils/test_safe_min_max.py` & `nextline_rdb-0.6.7/tests/utils/test_safe_min_max.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/tests/utils/strategies/test_st_ints.py` & `nextline_rdb-0.6.7/tests/utils/strategies/test_st_ints.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/tests/utils/strategies/test_st_ranges.py` & `nextline_rdb-0.6.7/tests/utils/strategies/test_st_ranges.py`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/.gitignore` & `nextline_rdb-0.6.7/.gitignore`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/LICENSE.txt` & `nextline_rdb-0.6.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nextline_rdb-0.6.6/README.md` & `nextline_rdb-0.6.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Nextline RDB
+# nextline-rdb
 
 [![PyPI - Version](https://img.shields.io/pypi/v/nextline-rdb.svg)](https://pypi.org/project/nextline-rdb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nextline-rdb.svg)](https://pypi.org/project/nextline-rdb)
 
 [![Test Status](https://github.com/simonsobs/nextline-rdb/actions/workflows/unit-test.yml/badge.svg)](https://github.com/simonsobs/nextline-rdb/actions/workflows/unit-test.yml)
 [![Test Status](https://github.com/simonsobs/nextline-rdb/actions/workflows/type-check.yml/badge.svg)](https://github.com/simonsobs/nextline-rdb/actions/workflows/type-check.yml)
 [![codecov](https://codecov.io/gh/simonsobs/nextline-rdb/branch/main/graph/badge.svg)](https://codecov.io/gh/simonsobs/nextline-rdb)
```

### Comparing `nextline_rdb-0.6.6/pyproject.toml` & `nextline_rdb-0.6.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
   "nextline-graphql>=0.7.8",
   "alembic>=1.9",
   "SQLAlchemy[asyncio]>=2.0",
-  "aiosqlite>=0.10",
+  "aiosqlite>=0.16",
   "hypothesis>=6.88",
   "black>=23.10",
   "tomli>=2.0",
   "tomli-w>=1.0",
 ]
 dynamic = ["version"]
```

### Comparing `nextline_rdb-0.6.6/PKG-INFO` & `nextline_rdb-0.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nextline-rdb
-Version: 0.6.6
+Version: 0.6.7
 Summary: A plugin of nextline-graphql. A relational database for nextline
 Project-URL: Documentation, https://github.com/simonsobs/nextline-rdb#readme
 Project-URL: Issues, https://github.com/simonsobs/nextline-rdb/issues
 Project-URL: Source, https://github.com/simonsobs/nextline-rdb
 Author-email: Simons Observatory <so_software@simonsobservatory.org>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -12,15 +12,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
-Requires-Dist: aiosqlite>=0.10
+Requires-Dist: aiosqlite>=0.16
 Requires-Dist: alembic>=1.9
 Requires-Dist: black>=23.10
 Requires-Dist: hypothesis>=6.88
 Requires-Dist: nextline-graphql>=0.7.8
 Requires-Dist: sqlalchemy[asyncio]>=2.0
 Requires-Dist: tomli-w>=1.0
 Requires-Dist: tomli>=2.0
@@ -28,15 +28,15 @@
 Requires-Dist: async-asgi-testclient>=1.4; extra == 'tests'
 Requires-Dist: pytest-asyncio>=0.18; extra == 'tests'
 Requires-Dist: pytest-cov>=3.0; extra == 'tests'
 Requires-Dist: pytest-timeout>=2.1; extra == 'tests'
 Requires-Dist: pytest>=7.0; extra == 'tests'
 Description-Content-Type: text/markdown
 
-# Nextline RDB
+# nextline-rdb
 
 [![PyPI - Version](https://img.shields.io/pypi/v/nextline-rdb.svg)](https://pypi.org/project/nextline-rdb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nextline-rdb.svg)](https://pypi.org/project/nextline-rdb)
 
 [![Test Status](https://github.com/simonsobs/nextline-rdb/actions/workflows/unit-test.yml/badge.svg)](https://github.com/simonsobs/nextline-rdb/actions/workflows/unit-test.yml)
 [![Test Status](https://github.com/simonsobs/nextline-rdb/actions/workflows/type-check.yml/badge.svg)](https://github.com/simonsobs/nextline-rdb/actions/workflows/type-check.yml)
 [![codecov](https://codecov.io/gh/simonsobs/nextline-rdb/branch/main/graph/badge.svg)](https://codecov.io/gh/simonsobs/nextline-rdb)
```

