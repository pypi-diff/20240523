# Comparing `tmp/astronomer_cosmos-1.4.1rc1.tar.gz` & `tmp/astronomer_cosmos-1.5.0a1.tar.gz`

## Comparing `astronomer_cosmos-1.4.1rc1.tar` & `astronomer_cosmos-1.5.0a1.tar`

### file list

```diff
@@ -1,74 +1,75 @@
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/__init__.py
--rw-r--r--   0        0        0     7542 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/cache.py
--rw-r--r--   0        0        0    15300 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/config.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/constants.py
--rw-r--r--   0        0        0    12060 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/converter.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/exceptions.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/log.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/airflow/__init__.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/airflow/dag.py
--rw-r--r--   0        0        0    13398 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/airflow/graph.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/airflow/task_group.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/core/__init__.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/core/airflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/core/graph/__init__.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/core/graph/entities.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/dbt/__init__.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/dbt/executable.py
--rw-r--r--   0        0        0    18591 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/dbt/graph.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/dbt/project.py
--rw-r--r--   0        0        0    17017 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/dbt/selector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/dbt/parser/__init__.py
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/dbt/parser/output.py
--rw-r--r--   0        0        0    16190 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/dbt/parser/project.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/hooks/__init__.py
--rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/hooks/subprocess.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/operators/__init__.py
--rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/operators/azure_container_instance.py
--rw-r--r--   0        0        0    15068 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/operators/base.py
--rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/operators/docker.py
--rw-r--r--   0        0        0     9459 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/operators/kubernetes.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/operators/lazy_load.py
--rw-r--r--   0        0        0    33776 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/operators/local.py
--rw-r--r--   0        0        0     6282 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/operators/virtualenv.py
--rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/plugin/__init__.py
--rw-r--r--   0        0        0    13431 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/plugin/static/iframeResizer.contentWindow.min.js
--rw-r--r--   0        0        0    14167 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/plugin/static/iframeResizer.min.js
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/plugin/templates/dbt_docs.html
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/plugin/templates/dbt_docs_not_set_up.html
--rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/__init__.py
--rwxr-xr-x   0        0        0    11466 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/base.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/athena/__init__.py
--rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/athena/access_key.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/bigquery/__init__.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/bigquery/oauth.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/bigquery/service_account_file.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/bigquery/service_account_keyfile_dict.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/databricks/__init__.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/databricks/token.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/exasol/__init__.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/exasol/user_pass.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/postgres/__init__.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/postgres/user_pass.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/redshift/__init__.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/redshift/user_pass.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/snowflake/__init__.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/snowflake/user_encrypted_privatekey_env_variable.py
--rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/snowflake/user_encrypted_privatekey_file.py
--rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/snowflake/user_pass.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/snowflake/user_privatekey.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/spark/__init__.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/spark/thrift.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/trino/__init__.py
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/trino/base.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/trino/certificate.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/trino/jwt.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/trino/ldap.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/vertica/__init__.py
--rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/cosmos/profiles/vertica/user_pass.py
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/LICENSE
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/README.rst
--rw-r--r--   0        0        0     5945 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/pyproject.toml
--rw-r--r--   0        0        0     7748 2020-02-02 00:00:00.000000 astronomer_cosmos-1.4.1rc1/PKG-INFO
+-rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/__init__.py
+-rw-r--r--   0        0        0    10981 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/cache.py
+-rw-r--r--   0        0        0    15300 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/config.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/constants.py
+-rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/converter.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/exceptions.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/log.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/airflow/__init__.py
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/airflow/dag.py
+-rw-r--r--   0        0        0    13398 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/airflow/graph.py
+-rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/airflow/task_group.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/core/__init__.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/core/airflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/core/graph/__init__.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/core/graph/entities.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/dbt/__init__.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/dbt/executable.py
+-rw-r--r--   0        0        0    18591 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/dbt/graph.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/dbt/project.py
+-rw-r--r--   0        0        0    17017 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/dbt/selector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/dbt/parser/__init__.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/dbt/parser/output.py
+-rw-r--r--   0        0        0    16190 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/dbt/parser/project.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/hooks/__init__.py
+-rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/hooks/subprocess.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/operators/__init__.py
+-rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/operators/aws_eks.py
+-rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/operators/azure_container_instance.py
+-rw-r--r--   0        0        0    15005 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/operators/base.py
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/operators/docker.py
+-rw-r--r--   0        0        0     9450 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/operators/kubernetes.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/operators/lazy_load.py
+-rw-r--r--   0        0        0    33470 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/operators/local.py
+-rw-r--r--   0        0        0     6282 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/operators/virtualenv.py
+-rw-r--r--   0        0        0     6843 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/plugin/__init__.py
+-rw-r--r--   0        0        0    13431 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/plugin/static/iframeResizer.contentWindow.min.js
+-rw-r--r--   0        0        0    14167 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/plugin/static/iframeResizer.min.js
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/plugin/templates/dbt_docs.html
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/plugin/templates/dbt_docs_not_set_up.html
+-rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/profiles/__init__.py
+-rwxr-xr-x   0        0        0    11466 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/profiles/base.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/profiles/athena/__init__.py
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/profiles/athena/access_key.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/profiles/bigquery/__init__.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/profiles/bigquery/oauth.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/profiles/bigquery/service_account_file.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/profiles/bigquery/service_account_keyfile_dict.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/profiles/databricks/__init__.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/profiles/databricks/token.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/profiles/exasol/__init__.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/profiles/exasol/user_pass.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/profiles/postgres/__init__.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/profiles/postgres/user_pass.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/profiles/redshift/__init__.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/profiles/redshift/user_pass.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/profiles/snowflake/__init__.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/profiles/snowflake/user_encrypted_privatekey_env_variable.py
+-rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/profiles/snowflake/user_encrypted_privatekey_file.py
+-rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/profiles/snowflake/user_pass.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/profiles/snowflake/user_privatekey.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/profiles/spark/__init__.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/profiles/spark/thrift.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/profiles/trino/__init__.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/profiles/trino/base.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/profiles/trino/certificate.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/profiles/trino/jwt.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/profiles/trino/ldap.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/profiles/vertica/__init__.py
+-rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/cosmos/profiles/vertica/user_pass.py
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/LICENSE
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/README.rst
+-rw-r--r--   0        0        0     6180 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/pyproject.toml
+-rw-r--r--   0        0        0     7853 2020-02-02 00:00:00.000000 astronomer_cosmos-1.5.0a1/PKG-INFO
```

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/__init__.py` & `astronomer_cosmos-1.5.0a1/cosmos/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # type: ignore # ignores "Cannot assign to a type" MyPy error
 
 """
 Astronomer Cosmos is a library for rendering dbt workflows in Airflow.
 
 Contains dags, task groups, and operators.
 """
-__version__ = "1.4.1rc1"
+__version__ = "1.5.0a1"
 
 
 from cosmos.airflow.dag import DbtDag
 from cosmos.airflow.task_group import DbtTaskGroup
 from cosmos.config import (
     ExecutionConfig,
     ProfileConfig,
```

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/cache.py` & `astronomer_cosmos-1.5.0a1/cosmos/cache.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from __future__ import annotations
 
+import functools
 import shutil
+import time
 from pathlib import Path
 
 import msgpack
 from airflow.models.dag import DAG
 from airflow.utils.task_group import TaskGroup
 
 from cosmos import settings
@@ -167,7 +169,88 @@
     target_manifest_filepath = target_partial_parse_file.parent / DBT_MANIFEST_FILE_NAME
     shutil.copy(str(partial_parse_filepath), str(target_partial_parse_file))
 
     patch_partial_parse_content(target_partial_parse_file, project_path)
 
     if source_manifest_filepath.exists():
         shutil.copy(str(source_manifest_filepath), str(target_manifest_filepath))
+
+
+# The following methods are being used to cache DbtDag / DbtTaskGroup
+
+
+# It was considered to create a cache identifier based on the dbt project path, as opposed
+# to where it is used in Airflow. However, we could have concurrency issues if the same
+# dbt cached directory was being used by different dbt task groups or DAGs within the same
+# node. For this reason, as a starting point, the cache is identified by where it is used.
+# This can be reviewed in the future.
+def create_cache_identifier_v2(dag_id: str | None, task_group_id: str | None) -> str:
+    # FIXME: To be refactored and merged with _create_cache_identifier
+    # Missing support to: task_group.group_id
+    """
+    Given a DAG name and a (optional) task_group_name, create the identifier for caching.
+
+    :param dag_name: Name of the Cosmos DbtDag being cached
+    :param task_group_name: (optional) Name of the Cosmos DbtTaskGroup being cached
+    :return: Unique identifier representing the cache
+    """
+    cache_identifiers_list = []
+    if task_group_id:
+        if dag_id is not None:
+            cache_identifiers_list.append(dag_id)
+        if task_group_id is not None:
+            cache_identifiers_list.append(task_group_id)
+        cache_identifier = "__".join(cache_identifiers_list)
+    else:
+        cache_identifier = str(dag_id)
+
+    return cache_identifier
+
+
+@functools.lru_cache
+def get_cache_filepath(cache_identifier: str) -> Path:
+    cache_dir_path = _obtain_cache_dir_path(cache_identifier)
+    return cache_dir_path / f"{cache_identifier}.pkl"
+
+
+@functools.lru_cache
+def get_cache_version_filepath(cache_identifier: str) -> Path:
+    return Path(str(get_cache_filepath(cache_identifier)) + ".version")
+
+
+@functools.lru_cache
+def should_use_cache() -> bool:
+    return settings.enable_cache and settings.experimental_cache
+
+
+@functools.lru_cache
+def calculate_current_version(dag_id: str, project_dir: Path) -> str:
+    start_time = time.process_time()
+
+    # When DAG file was last changed - this is very slow (e.g. 0.6s)
+    # caller_dag_frame = inspect.stack()[1]
+    # caller_dag_filepath = Path(caller_dag_frame.filename)
+    # logger.info("The %s DAG is located in: %s" % (dag_id, caller_dag_filepath))
+    # dag_last_modified = caller_dag_filepath.stat().st_mtime
+    # mid_time = time.process_time() - start_time
+    # logger.info(f"It took {mid_time:.3}s to calculate the first part of the version")
+    # dag_last_modified = None
+
+    # Combined value for when the dbt project directory files were last modified
+    # This is fast (e.g. 0.01s for jaffle shop, 0.135s for a 5k models dbt folder)
+    dbt_combined_last_modified = sum([path.stat().st_mtime for path in project_dir.glob("**/*")])
+
+    elapsed_time = time.process_time() - start_time
+    logger.info(f"It took {elapsed_time:.3}s to calculate the cache version for the {dag_id}")
+    # return f"{dag_last_modified} {dbt_combined_last_modified}"
+    return f"{dbt_combined_last_modified}"
+
+
+@functools.lru_cache
+def is_project_unmodified(dag_id: str, current_version: str) -> Path | None:
+    cache_filepath = get_cache_filepath(dag_id)
+    cache_version_filepath = get_cache_version_filepath(dag_id)
+    if cache_version_filepath.exists() and cache_filepath.exists():
+        previous_cache_version = cache_version_filepath.read_text()
+        if previous_cache_version == current_version:
+            return cache_filepath
+    return None
```

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/config.py` & `astronomer_cosmos-1.5.0a1/cosmos/config.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/constants.py` & `astronomer_cosmos-1.5.0a1/cosmos/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     """
     Where the Cosmos tasks should be executed.
     """
 
     LOCAL = "local"
     DOCKER = "docker"
     KUBERNETES = "kubernetes"
+    AWS_EKS = "aws_eks"
     VIRTUALENV = "virtualenv"
     AZURE_CONTAINER_INSTANCE = "azure_container_instance"
 
 
 class InvocationMode(Enum):
     """
     How the dbt command should be invoked.
```

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/converter.py` & `astronomer_cosmos-1.5.0a1/cosmos/converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,14 +111,15 @@
     :param profile_config: Configuration related to dbt database configuration (profile)
     :param project_config: Configuration related to the overall dbt project
     :param render_config: Configuration related to how to convert the dbt workflow into an Airflow DAG
     :param operator_args: Arguments to pass to the underlying operators.
     """
     if profile_config is None and execution_config.execution_mode not in (
         ExecutionMode.KUBERNETES,
+        ExecutionMode.AWS_EKS,
         ExecutionMode.DOCKER,
     ):
         raise CosmosValueError(f"The profile_config is mandatory when using {execution_config.execution_mode}")
 
     # Since we now support both project_config.dbt_project_path, render_config.project_path and execution_config.project_path
     # We need to ensure that only one interface is being used.
     if project_config.dbt_project_path and (render_config.project_path or execution_config.project_path):
```

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/log.py` & `astronomer_cosmos-1.5.0a1/cosmos/log.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import logging
 
-from airflow.configuration import conf
 from airflow.utils.log.colored_log import CustomTTYColoredFormatter
 
+from cosmos.settings import propagate_logs
+
 LOG_FORMAT: str = (
     "[%(blue)s%(asctime)s%(reset)s] "
     "{%(blue)s%(filename)s:%(reset)s%(lineno)d} "
     "%(log_color)s%(levelname)s%(reset)s - "
     "%(purple)s(astronomer-cosmos)%(reset)s - "
     "%(log_color)s%(message)s%(reset)s"
 )
@@ -20,17 +21,14 @@
 
     Airflow logs usually look like:
     [2023-08-09T14:20:55.532+0100] {subprocess.py:94} INFO - 13:20:55  Completed successfully
 
     By using this logger, we introduce a (yellow) astronomer-cosmos string into the project's log messages:
     [2023-08-09T14:20:55.532+0100] {subprocess.py:94} INFO - (astronomer-cosmos) - 13:20:55  Completed successfully
     """
-    propagateLogs: bool = True
-    if conf.has_option("cosmos", "propagate_logs"):
-        propagateLogs = conf.getboolean("cosmos", "propagate_logs")
     logger = logging.getLogger(name)
     formatter: logging.Formatter = CustomTTYColoredFormatter(fmt=LOG_FORMAT)  # type: ignore
     handler = logging.StreamHandler()
     handler.setFormatter(formatter)
     logger.addHandler(handler)
-    logger.propagate = propagateLogs
+    logger.propagate = propagate_logs
     return logger
```

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/airflow/graph.py` & `astronomer_cosmos-1.5.0a1/cosmos/airflow/graph.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/core/airflow.py` & `astronomer_cosmos-1.5.0a1/cosmos/core/airflow.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/core/graph/entities.py` & `astronomer_cosmos-1.5.0a1/cosmos/core/graph/entities.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/dbt/graph.py` & `astronomer_cosmos-1.5.0a1/cosmos/dbt/graph.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/dbt/project.py` & `astronomer_cosmos-1.5.0a1/cosmos/dbt/project.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 import os
-import shutil
 from contextlib import contextmanager
 from pathlib import Path
 from typing import Generator
 
 from cosmos.constants import DBT_LOG_DIR_NAME, DBT_PARTIAL_PARSE_FILE_NAME, DBT_TARGET_DIR_NAME
```

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/dbt/selector.py` & `astronomer_cosmos-1.5.0a1/cosmos/dbt/selector.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/dbt/parser/output.py` & `astronomer_cosmos-1.5.0a1/cosmos/dbt/parser/output.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/dbt/parser/project.py` & `astronomer_cosmos-1.5.0a1/cosmos/dbt/parser/project.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/hooks/subprocess.py` & `astronomer_cosmos-1.5.0a1/cosmos/hooks/subprocess.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/operators/__init__.py` & `astronomer_cosmos-1.5.0a1/cosmos/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/operators/azure_container_instance.py` & `astronomer_cosmos-1.5.0a1/cosmos/operators/azure_container_instance.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/operators/base.py` & `astronomer_cosmos-1.5.0a1/cosmos/operators/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from __future__ import annotations
 
 import os
 from abc import ABCMeta, abstractmethod
-from functools import cached_property
 from pathlib import Path
 from typing import Any, Sequence, Tuple
 
 import yaml
 from airflow.models.baseoperator import BaseOperator
 from airflow.utils.context import Context
 from airflow.utils.operator_helpers import context_to_airflow_vars
 from airflow.utils.strings import to_boolean
 
-from cosmos import cache
 from cosmos.dbt.executable import get_system_dbt
 from cosmos.log import get_logger
 
 logger = get_logger(__name__)
 
 
 class AbstractDbtBaseOperator(BaseOperator, metaclass=ABCMeta):
```

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/operators/docker.py` & `astronomer_cosmos-1.5.0a1/cosmos/operators/docker.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/operators/kubernetes.py` & `astronomer_cosmos-1.5.0a1/cosmos/operators/kubernetes.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     )
     from airflow.providers.cncf.kubernetes.operators.pod import KubernetesPodOperator
     from airflow.providers.cncf.kubernetes.utils.pod_manager import OnFinishAction
 except ImportError:
     try:
         # apache-airflow-providers-cncf-kubernetes < 7.4.0
         from airflow.providers.cncf.kubernetes.operators.kubernetes_pod import KubernetesPodOperator
-    except ImportError as error:
+    except ImportError:
         raise ImportError(
             "Could not import KubernetesPodOperator. Ensure you've installed the Kubernetes provider "
             "separately or with with `pip install astronomer-cosmos[...,kubernetes]`."
         )
 
 
 class DbtKubernetesBaseOperator(AbstractDbtBaseOperator, KubernetesPodOperator):  # type: ignore
```

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/operators/local.py` & `astronomer_cosmos-1.5.0a1/cosmos/operators/local.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,28 +4,27 @@
 import tempfile
 import warnings
 from abc import ABC, abstractmethod
 from functools import cached_property
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Callable, Literal, Sequence
 
-import airflow
 import jinja2
 from airflow import DAG
-from airflow.configuration import conf
 from airflow.exceptions import AirflowException, AirflowSkipException
 from airflow.models.taskinstance import TaskInstance
 from airflow.utils.context import Context
 from airflow.utils.session import NEW_SESSION, create_session, provide_session
 from attr import define
 
 from cosmos import cache
 from cosmos.constants import InvocationMode
 from cosmos.dbt.project import get_partial_parse_path
 from cosmos.exceptions import AirflowCompatibilityError
+from cosmos.settings import LINEAGE_NAMESPACE
 
 try:
     from airflow.datasets import Dataset
     from openlineage.common.provider.dbt.local import DbtLocalArtifactProcessor
 except ModuleNotFoundError:
     is_openlineage_available = False
     DbtLocalArtifactProcessor = None
@@ -37,17 +36,14 @@
     from dbt.cli.main import dbtRunner, dbtRunnerResult
     from openlineage.client.run import RunEvent
 
 from sqlalchemy.orm import Session
 
 from cosmos.config import ProfileConfig
 from cosmos.constants import (
-    DBT_PARTIAL_PARSE_FILE_NAME,
-    DBT_TARGET_DIR_NAME,
-    DEFAULT_OPENLINEAGE_NAMESPACE,
     OPENLINEAGE_PRODUCER,
 )
 from cosmos.dbt.parser.output import (
     extract_dbt_runner_issues,
     extract_log_issues,
     parse_number_of_warnings_dbt_runner,
     parse_number_of_warnings_subprocess,
@@ -90,20 +86,14 @@
         class OperatorLineage:  # type: ignore
             inputs: list[str] = list()
             outputs: list[str] = list()
             run_facets: dict[str, str] = dict()
             job_facets: dict[str, str] = dict()
 
 
-try:
-    LINEAGE_NAMESPACE = conf.get("openlineage", "namespace")
-except airflow.exceptions.AirflowConfigException:
-    LINEAGE_NAMESPACE = os.getenv("OPENLINEAGE_NAMESPACE", DEFAULT_OPENLINEAGE_NAMESPACE)
-
-
 class DbtLocalBaseOperator(AbstractDbtBaseOperator):
     """
     Executes a dbt core cli command locally.
 
     :param profile_args: Arguments to pass to the profile. See
         :py:class:`cosmos.providers.dbt.core.profiles.BaseProfileMapping`.
     :param profile_name: A name to use for the dbt profile. If not provided, and no profile target is found
@@ -172,15 +162,15 @@
 
     def _discover_invocation_mode(self) -> None:
         """Discovers the invocation mode based on the availability of dbtRunner for import. If dbtRunner is available, it will
         be used since it is faster than subprocess. If dbtRunner is not available, it will fall back to subprocess.
         This method is called at runtime to work in the environment where the operator is running.
         """
         try:
-            from dbt.cli.main import dbtRunner
+            from dbt.cli.main import dbtRunner  # noqa
         except ImportError:
             self.invocation_mode = InvocationMode.SUBPROCESS
             logger.info("Could not import dbtRunner. Falling back to subprocess for invoking dbt.")
         else:
             self.invocation_mode = InvocationMode.DBT_RUNNER
             logger.info("dbtRunner is available. Using dbtRunner for invoking dbt.")
         self._set_invocation_methods()
@@ -422,15 +412,15 @@
                 dataset_uri = output.namespace + "/" + output.name
                 uris.append(dataset_uri)
         logger.debug("URIs to be converted to Dataset: %s", uris)
 
         datasets = []
         try:
             datasets = [Dataset(uri) for uri in uris]
-        except ValueError as e:
+        except ValueError:
             raise AirflowCompatibilityError(
                 """
                 Apache Airflow 2.9.0 & 2.9.1 introduced a breaking change in Dataset URIs, to be fixed in newer versions:
                 https://github.com/apache/airflow/issues/39486
 
                 If you want to use Cosmos with one of these Airflow versions, you will have to disable emission of Datasets:
                 By setting ``emit_datasets=False`` in ``RenderConfig``. For more information, see https://astronomer.github.io/astronomer-cosmos/configuration/render-config.html.
```

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/operators/virtualenv.py` & `astronomer_cosmos-1.5.0a1/cosmos/operators/virtualenv.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/plugin/__init__.py` & `astronomer_cosmos-1.5.0a1/cosmos/plugin/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import os.path as op
 from typing import Any, Dict, Optional, Tuple
 from urllib.parse import urlsplit
 
-from airflow.configuration import conf
 from airflow.plugins_manager import AirflowPlugin
 from airflow.security import permissions
 from airflow.www.auth import has_access
 from airflow.www.views import AirflowBaseView
 from flask import abort, url_for
 from flask_appbuilder import AppBuilder, expose
 
+from cosmos.settings import dbt_docs_conn_id, dbt_docs_dir
+
 
 def bucket_and_key(path: str) -> Tuple[str, str]:
     parsed_url = urlsplit(path)
     bucket = parsed_url.netloc
     key = parsed_url.path.lstrip("/")
     return bucket, key
 
@@ -65,24 +66,22 @@
     res = hook.run(endpoint=path)
     hook.check_response(res)
     return res.text  # type: ignore[no-any-return]
 
 
 def open_file(path: str) -> str:
     """Retrieve a file from http, https, gs, s3, or wasb."""
-    conn_id: Optional[str] = conf.get("cosmos", "dbt_docs_conn_id", fallback=None)
-
     if path.strip().startswith("s3://"):
-        return open_s3_file(conn_id=conn_id, path=path)
+        return open_s3_file(conn_id=dbt_docs_conn_id, path=path)
     elif path.strip().startswith("gs://"):
-        return open_gcs_file(conn_id=conn_id, path=path)
+        return open_gcs_file(conn_id=dbt_docs_conn_id, path=path)
     elif path.strip().startswith("wasb://"):
-        return open_azure_file(conn_id=conn_id, path=path)
+        return open_azure_file(conn_id=dbt_docs_conn_id, path=path)
     elif path.strip().startswith("http://") or path.strip().startswith("https://"):
-        return open_http_file(conn_id=conn_id, path=path)
+        return open_http_file(conn_id=dbt_docs_conn_id, path=path)
     else:
         with open(path) as f:
             content = f.read()
         return content  # type: ignore[no-any-return]
 
 
 iframe_script = """
@@ -155,46 +154,43 @@
     ) -> None:
         # Make sure the static folder is not overwritten, as we want to use it.
         return super().create_blueprint(appbuilder, endpoint=endpoint, static_folder=self.static_folder)  # type: ignore[no-any-return]
 
     @expose("/dbt_docs")  # type: ignore[misc]
     @has_access([(permissions.ACTION_CAN_READ, permissions.RESOURCE_WEBSITE)])
     def dbt_docs(self) -> str:
-        if conf.get("cosmos", "dbt_docs_dir", fallback=None) is None:
+        if dbt_docs_dir is None:
             return self.render_template("dbt_docs_not_set_up.html")  # type: ignore[no-any-return,no-untyped-call]
         return self.render_template("dbt_docs.html")  # type: ignore[no-any-return,no-untyped-call]
 
     @expose("/dbt_docs_index.html")  # type: ignore[misc]
     @has_access([(permissions.ACTION_CAN_READ, permissions.RESOURCE_WEBSITE)])
     def dbt_docs_index(self) -> str:
-        docs_dir = conf.get("cosmos", "dbt_docs_dir", fallback=None)
-        if docs_dir is None:
+        if dbt_docs_dir is None:
             abort(404)
-        html = open_file(op.join(docs_dir, "index.html"))
+        html = open_file(op.join(dbt_docs_dir, "index.html"))
         # Hack the dbt docs to render properly in an iframe
         iframe_resizer_url = url_for(".static", filename="iframeResizer.contentWindow.min.js")
         html = html.replace("</head>", f'{iframe_script}<script src="{iframe_resizer_url}"></script></head>', 1)
         return html
 
     @expose("/catalog.json")  # type: ignore[misc]
     @has_access([(permissions.ACTION_CAN_READ, permissions.RESOURCE_WEBSITE)])
     def catalog(self) -> Tuple[str, int, Dict[str, Any]]:
-        docs_dir = conf.get("cosmos", "dbt_docs_dir", fallback=None)
-        if docs_dir is None:
+        if dbt_docs_dir is None:
             abort(404)
-        data = open_file(op.join(docs_dir, "catalog.json"))
+        data = open_file(op.join(dbt_docs_dir, "catalog.json"))
         return data, 200, {"Content-Type": "application/json"}
 
     @expose("/manifest.json")  # type: ignore[misc]
     @has_access([(permissions.ACTION_CAN_READ, permissions.RESOURCE_WEBSITE)])
     def manifest(self) -> Tuple[str, int, Dict[str, Any]]:
-        docs_dir = conf.get("cosmos", "dbt_docs_dir", fallback=None)
-        if docs_dir is None:
+        if dbt_docs_dir is None:
             abort(404)
-        data = open_file(op.join(docs_dir, "manifest.json"))
+        data = open_file(op.join(dbt_docs_dir, "manifest.json"))
         return data, 200, {"Content-Type": "application/json"}
 
 
 dbt_docs_view = DbtDocsView()
 
 
 class CosmosPlugin(AirflowPlugin):
```

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/plugin/static/iframeResizer.contentWindow.min.js` & `astronomer_cosmos-1.5.0a1/cosmos/plugin/static/iframeResizer.contentWindow.min.js`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/plugin/static/iframeResizer.min.js` & `astronomer_cosmos-1.5.0a1/cosmos/plugin/static/iframeResizer.min.js`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/profiles/__init__.py` & `astronomer_cosmos-1.5.0a1/cosmos/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/profiles/base.py` & `astronomer_cosmos-1.5.0a1/cosmos/profiles/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/profiles/athena/access_key.py` & `astronomer_cosmos-1.5.0a1/cosmos/profiles/athena/access_key.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/profiles/bigquery/oauth.py` & `astronomer_cosmos-1.5.0a1/cosmos/profiles/bigquery/oauth.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/profiles/bigquery/service_account_file.py` & `astronomer_cosmos-1.5.0a1/cosmos/profiles/bigquery/service_account_file.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/profiles/bigquery/service_account_keyfile_dict.py` & `astronomer_cosmos-1.5.0a1/cosmos/profiles/bigquery/service_account_keyfile_dict.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/profiles/databricks/token.py` & `astronomer_cosmos-1.5.0a1/cosmos/profiles/databricks/token.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/profiles/exasol/user_pass.py` & `astronomer_cosmos-1.5.0a1/cosmos/profiles/exasol/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/profiles/postgres/user_pass.py` & `astronomer_cosmos-1.5.0a1/cosmos/profiles/postgres/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/profiles/redshift/user_pass.py` & `astronomer_cosmos-1.5.0a1/cosmos/profiles/redshift/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/profiles/snowflake/__init__.py` & `astronomer_cosmos-1.5.0a1/cosmos/profiles/snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/profiles/snowflake/user_encrypted_privatekey_env_variable.py` & `astronomer_cosmos-1.5.0a1/cosmos/profiles/snowflake/user_encrypted_privatekey_env_variable.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/profiles/snowflake/user_encrypted_privatekey_file.py` & `astronomer_cosmos-1.5.0a1/cosmos/profiles/snowflake/user_encrypted_privatekey_file.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/profiles/snowflake/user_pass.py` & `astronomer_cosmos-1.5.0a1/cosmos/profiles/snowflake/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/profiles/snowflake/user_privatekey.py` & `astronomer_cosmos-1.5.0a1/cosmos/profiles/snowflake/user_privatekey.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/profiles/spark/thrift.py` & `astronomer_cosmos-1.5.0a1/cosmos/profiles/spark/thrift.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/profiles/trino/base.py` & `astronomer_cosmos-1.5.0a1/cosmos/profiles/trino/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/profiles/trino/certificate.py` & `astronomer_cosmos-1.5.0a1/cosmos/profiles/trino/certificate.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/profiles/trino/jwt.py` & `astronomer_cosmos-1.5.0a1/cosmos/profiles/trino/jwt.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/profiles/trino/ldap.py` & `astronomer_cosmos-1.5.0a1/cosmos/profiles/trino/ldap.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/cosmos/profiles/vertica/user_pass.py` & `astronomer_cosmos-1.5.0a1/cosmos/profiles/vertica/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/.gitignore` & `astronomer_cosmos-1.5.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/LICENSE` & `astronomer_cosmos-1.5.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/README.rst` & `astronomer_cosmos-1.5.0a1/README.rst`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.4.1rc1/pyproject.toml` & `astronomer_cosmos-1.5.0a1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "aenum",
     "attrs",
-    "apache-airflow>=2.3.0",
+    "apache-airflow>=2.4.0",
     "importlib-metadata; python_version < '3.8'",
     "Jinja2>=3.0.0",
     "msgpack",
     "pydantic>=1.10.0",
     "typing-extensions; python_version < '3.8'",
     "virtualenv",
 ]
@@ -83,14 +83,17 @@
 ]
 docker = [
     "apache-airflow-providers-docker>=3.5.0",
 ]
 kubernetes = [
     "apache-airflow-providers-cncf-kubernetes>=5.1.1",
 ]
+aws_eks = [
+    "apache-airflow-providers-amazon>=8.0.0,<8.20.0", # https://github.com/apache/airflow/issues/39103
+]
 azure-container-instance = [
     "apache-airflow-providers-microsoft-azure>=8.4.0",
 ]
 
 [project.entry-points.cosmos]
 provider_info = "cosmos:get_provider_info"
 
@@ -116,32 +119,33 @@
 ######################################
 
 [tool.hatch.envs.tests]
 dependencies = [
     "astronomer-cosmos[tests]",
     "apache-airflow-providers-postgres",
     "apache-airflow-providers-cncf-kubernetes>=5.1.1",
+    "apache-airflow-providers-amazon>=3.0.0,<8.20.0", # https://github.com/apache/airflow/issues/39103
     "apache-airflow-providers-docker>=3.5.0",
     "apache-airflow-providers-microsoft-azure",
     "types-PyYAML",
     "types-attrs",
     "types-requests",
     "types-python-dateutil",
     "Werkzeug<3.0.0",
     "apache-airflow=={matrix:airflow}.0",
 ]
 pre-install-commands = ["sh scripts/test/pre-install-airflow.sh {matrix:airflow} {matrix:python}"]
 
 [[tool.hatch.envs.tests.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11"]
-airflow = ["2.3", "2.4", "2.5", "2.6", "2.7", "2.8", "2.9"]
+airflow = ["2.4", "2.5", "2.6", "2.7", "2.8", "2.9"]
 
 [tool.hatch.envs.tests.overrides]
 matrix.airflow.dependencies = [
-    { value = "typing_extensions<4.6", if = ["2.6"] },
+    { value = "typing_extensions<4.6", if = ["2.6"] }
 ]
 
 [tool.hatch.envs.tests.scripts]
 freeze = "pip freeze"
 test = 'sh scripts/test/unit.sh'
 test-cov = 'sh scripts/test/unit-cov.sh'
 test-integration = 'sh scripts/test/integration.sh'
@@ -195,13 +199,14 @@
 strict = true
 ignore_missing_imports = true
 no_warn_unused_ignores = true
 
 [tool.ruff]
 line-length = 120
 [tool.ruff.lint]
-select = ["C901", "I"]
+select = ["C901", "I", "F"]
+ignore = ["F541"]
 [tool.ruff.lint.mccabe]
 max-complexity = 10
 
 [tool.distutils.bdist_wheel]
 universal = true
```

### Comparing `astronomer_cosmos-1.4.1rc1/PKG-INFO` & `astronomer_cosmos-1.5.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: astronomer-cosmos
-Version: 1.4.1rc1
+Version: 1.5.0a1
 Summary: Orchestrate your dbt projects in Airflow
 Project-URL: Homepage, https://github.com/astronomer/astronomer-cosmos
 Project-URL: Documentation, https://astronomer.github.io/astronomer-cosmos
 Project-URL: Source code, https://github.com/astronomer/astronomer-cosmos
 Author-email: Astronomer <humans@astronomer.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Requires-Dist: aenum
-Requires-Dist: apache-airflow>=2.3.0
+Requires-Dist: apache-airflow>=2.4.0
 Requires-Dist: attrs
 Requires-Dist: importlib-metadata; python_version < '3.8'
 Requires-Dist: jinja2>=3.0.0
 Requires-Dist: msgpack
 Requires-Dist: pydantic>=1.10.0
 Requires-Dist: typing-extensions; python_version < '3.8'
 Requires-Dist: virtualenv
@@ -40,14 +40,16 @@
 Requires-Dist: dbt-postgres; extra == 'all'
 Requires-Dist: dbt-redshift; extra == 'all'
 Requires-Dist: dbt-snowflake; extra == 'all'
 Requires-Dist: dbt-spark; extra == 'all'
 Requires-Dist: dbt-vertica; extra == 'all'
 Requires-Dist: openlineage-airflow; extra == 'all'
 Requires-Dist: openlineage-integration-common; extra == 'all'
+Provides-Extra: aws-eks
+Requires-Dist: apache-airflow-providers-amazon<8.20.0,>=8.0.0; extra == 'aws-eks'
 Provides-Extra: azure-container-instance
 Requires-Dist: apache-airflow-providers-microsoft-azure>=8.4.0; extra == 'azure-container-instance'
 Provides-Extra: dbt-all
 Requires-Dist: dbt-athena; extra == 'dbt-all'
 Requires-Dist: dbt-bigquery; extra == 'dbt-all'
 Requires-Dist: dbt-databricks; extra == 'dbt-all'
 Requires-Dist: dbt-exasol; extra == 'dbt-all'
```

