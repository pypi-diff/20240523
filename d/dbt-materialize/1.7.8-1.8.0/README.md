# Comparing `tmp/dbt-materialize-1.7.8.tar.gz` & `tmp/dbt-materialize-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-materialize-1.7.8.tar", last modified: Mon May  6 17:47:50 2024, max compression
+gzip compressed data, was "dbt-materialize-1.8.0.tar", last modified: Thu May 23 07:09:06 2024, max compression
```

## Comparing `dbt-materialize-1.7.8.tar` & `dbt-materialize-1.8.0.tar`

### file list

```diff
@@ -1,74 +1,76 @@
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/
--rw-r--r--   0 materialize  (2000) materialize   (993)      424 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/MANIFEST.in
--rw-r--r--   0 materialize  (2000) materialize   (993)     6613 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/PKG-INFO
--rw-r--r--   0 materialize  (2000) materialize   (993)     6292 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/README.md
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/dbt/
--rw-r--r--   0 materialize  (2000) materialize   (993)      729 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/__init__.py
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/dbt/adapters/
--rw-r--r--   0 materialize  (2000) materialize   (993)      729 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/adapters/__init__.py
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/dbt/adapters/materialize/
--rw-r--r--   0 materialize  (2000) materialize   (993)     1125 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/adapters/materialize/__init__.py
--rw-r--r--   0 materialize  (2000) materialize   (993)      801 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/adapters/materialize/__version__.py
--rw-r--r--   0 materialize  (2000) materialize   (993)     5553 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/adapters/materialize/connections.py
--rw-r--r--   0 materialize  (2000) materialize   (993)     1598 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/adapters/materialize/exceptions.py
--rw-r--r--   0 materialize  (2000) materialize   (993)    11918 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/adapters/materialize/impl.py
--rw-r--r--   0 materialize  (2000) materialize   (993)     2284 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/adapters/materialize/relation.py
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/dbt/include/
--rw-r--r--   0 materialize  (2000) materialize   (993)      729 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/__init__.py
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/dbt/include/materialize/
--rw-r--r--   0 materialize  (2000) materialize   (993)      782 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/__init__.py
--rw-r--r--   0 materialize  (2000) materialize   (993)      808 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/dbt_project.yml
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/dbt/include/materialize/macros/
--rw-r--r--   0 materialize  (2000) materialize   (993)     9472 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/adapters.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     2592 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/catalog.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)      979 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/columns.sql
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/dbt/include/materialize/macros/deploy/
--rw-r--r--   0 materialize  (2000) materialize   (993)     1711 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/deploy/deploy_await.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1981 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/deploy/deploy_cleanup.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)    12199 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/deploy/deploy_init.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     6053 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/deploy/deploy_permission_validation.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     5361 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/deploy/deploy_promote.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)      989 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/freshness.sql
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/dbt/include/materialize/macros/materializations/
--rw-r--r--   0 materialize  (2000) materialize   (993)     1911 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/materializations/incremental.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1922 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/materializations/materialized_view.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1224 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/materializations/materializedview.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1970 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/materializations/sink.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1835 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/materializations/source.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1974 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/materializations/table.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     2828 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/materializations/test.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1883 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/materializations/view.sql
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/dbt/include/materialize/macros/tests/
--rw-r--r--   0 materialize  (2000) materialize   (993)     1033 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/tests/helpers.sql
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/dbt/include/materialize/macros/utils/
--rw-r--r--   0 materialize  (2000) materialize   (993)     1151 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/utils/await_cluster_ready.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     3245 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/utils/ci_utils.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1986 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/utils/exists.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)      887 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/utils/generate_cluster_name.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1285 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/utils/generate_schema_name.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     5211 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/utils/is_cluster_ready.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1016 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/macros/utils/listagg.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     1257 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/profile_template.yml
--rw-r--r--   0 materialize  (2000) materialize   (993)     1277 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/materialize/sample_profiles.yml
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/dbt/include/starter_project/
--rw-r--r--   0 materialize  (2000) materialize   (993)      917 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/starter_project/dbt_project.yml
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/dbt/include/starter_project/models/
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/dbt/include/starter_project/models/example/
--rw-r--r--   0 materialize  (2000) materialize   (993)      972 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/starter_project/models/example/fraud_activity.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)      999 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/starter_project/models/example/funds_movement.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)      936 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/starter_project/models/example/my_first_dbt_model.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)      753 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/starter_project/models/example/my_second_dbt_model.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)     2822 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/starter_project/models/example/schema.yml
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/dbt/include/starter_project/models/example/sources/
--rw-r--r--   0 materialize  (2000) materialize   (993)      774 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/starter_project/models/example/sources/auction.sql
--rw-r--r--   0 materialize  (2000) materialize   (993)      866 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/starter_project/models/example/sources/sources.yml
--rw-r--r--   0 materialize  (2000) materialize   (993)     1068 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/dbt/include/starter_project/models/example/winning_bids.sql
-drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/dbt_materialize.egg-info/
--rw-r--r--   0 materialize  (2000) materialize   (993)     6613 2024-05-06 17:47:50.000000 dbt-materialize-1.7.8/dbt_materialize.egg-info/PKG-INFO
--rw-r--r--   0 materialize  (2000) materialize   (993)     2636 2024-05-06 17:47:50.000000 dbt-materialize-1.7.8/dbt_materialize.egg-info/SOURCES.txt
--rw-r--r--   0 materialize  (2000) materialize   (993)        1 2024-05-06 17:47:50.000000 dbt-materialize-1.7.8/dbt_materialize.egg-info/dependency_links.txt
--rw-r--r--   0 materialize  (2000) materialize   (993)       52 2024-05-06 17:47:50.000000 dbt-materialize-1.7.8/dbt_materialize.egg-info/requires.txt
--rw-r--r--   0 materialize  (2000) materialize   (993)        4 2024-05-06 17:47:50.000000 dbt-materialize-1.7.8/dbt_materialize.egg-info/top_level.txt
--rw-r--r--   0 materialize  (2000) materialize   (993)      464 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/pyproject.toml
--rw-r--r--   0 materialize  (2000) materialize   (993)       38 2024-05-06 17:47:50.728657 dbt-materialize-1.7.8/setup.cfg
--rw-r--r--   0 materialize  (2000) materialize   (993)     1814 2024-05-06 17:45:33.000000 dbt-materialize-1.7.8/setup.py
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-23 07:09:06.873289 dbt-materialize-1.8.0/
+-rw-r--r--   0 materialize  (2000) materialize   (993)      424 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/MANIFEST.in
+-rw-r--r--   0 materialize  (2000) materialize   (993)     6613 2024-05-23 07:09:06.873289 dbt-materialize-1.8.0/PKG-INFO
+-rw-r--r--   0 materialize  (2000) materialize   (993)     6292 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/README.md
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-23 07:09:06.863289 dbt-materialize-1.8.0/dbt/
+-rw-r--r--   0 materialize  (2000) materialize   (993)      729 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/__init__.py
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-23 07:09:06.863289 dbt-materialize-1.8.0/dbt/adapters/
+-rw-r--r--   0 materialize  (2000) materialize   (993)      729 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/adapters/__init__.py
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-23 07:09:06.863289 dbt-materialize-1.8.0/dbt/adapters/materialize/
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1125 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/adapters/materialize/__init__.py
+-rw-r--r--   0 materialize  (2000) materialize   (993)      801 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/adapters/materialize/__version__.py
+-rw-r--r--   0 materialize  (2000) materialize   (993)     5550 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/adapters/materialize/connections.py
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1605 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/adapters/materialize/exceptions.py
+-rw-r--r--   0 materialize  (2000) materialize   (993)    11996 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/adapters/materialize/impl.py
+-rw-r--r--   0 materialize  (2000) materialize   (993)     2310 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/adapters/materialize/relation.py
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-23 07:09:06.863289 dbt-materialize-1.8.0/dbt/include/
+-rw-r--r--   0 materialize  (2000) materialize   (993)      729 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/__init__.py
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-23 07:09:06.863289 dbt-materialize-1.8.0/dbt/include/materialize/
+-rw-r--r--   0 materialize  (2000) materialize   (993)      782 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/materialize/__init__.py
+-rw-r--r--   0 materialize  (2000) materialize   (993)      808 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/materialize/dbt_project.yml
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-23 07:09:06.863289 dbt-materialize-1.8.0/dbt/include/materialize/macros/
+-rw-r--r--   0 materialize  (2000) materialize   (993)     9472 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/materialize/macros/adapters.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     2592 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/materialize/macros/catalog.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)      979 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/materialize/macros/columns.sql
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-23 07:09:06.863289 dbt-materialize-1.8.0/dbt/include/materialize/macros/deploy/
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1711 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/materialize/macros/deploy/deploy_await.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1981 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/materialize/macros/deploy/deploy_cleanup.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)    12199 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/materialize/macros/deploy/deploy_init.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     6053 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/materialize/macros/deploy/deploy_permission_validation.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     5361 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/materialize/macros/deploy/deploy_promote.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)      989 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/materialize/macros/freshness.sql
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-23 07:09:06.873289 dbt-materialize-1.8.0/dbt/include/materialize/macros/materializations/
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1911 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/materialize/macros/materializations/incremental.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1922 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/materialize/macros/materializations/materialized_view.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1224 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/materialize/macros/materializations/materializedview.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1970 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/materialize/macros/materializations/sink.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1835 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/materialize/macros/materializations/source.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1974 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/materialize/macros/materializations/table.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     2828 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/materialize/macros/materializations/test.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     2003 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/materialize/macros/materializations/unit.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1883 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/materialize/macros/materializations/view.sql
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-23 07:09:06.873289 dbt-materialize-1.8.0/dbt/include/materialize/macros/tests/
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1399 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/materialize/macros/tests/helpers.sql
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-23 07:09:06.873289 dbt-materialize-1.8.0/dbt/include/materialize/macros/utils/
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1151 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/materialize/macros/utils/await_cluster_ready.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1279 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/materialize/macros/utils/cast.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     3245 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/materialize/macros/utils/ci_utils.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1986 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/materialize/macros/utils/exists.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)      887 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/materialize/macros/utils/generate_cluster_name.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1285 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/materialize/macros/utils/generate_schema_name.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     5211 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/materialize/macros/utils/is_cluster_ready.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1016 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/materialize/macros/utils/listagg.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1257 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/materialize/profile_template.yml
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1277 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/materialize/sample_profiles.yml
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-23 07:09:06.873289 dbt-materialize-1.8.0/dbt/include/starter_project/
+-rw-r--r--   0 materialize  (2000) materialize   (993)      922 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/starter_project/dbt_project.yml
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-23 07:09:06.863289 dbt-materialize-1.8.0/dbt/include/starter_project/models/
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-23 07:09:06.873289 dbt-materialize-1.8.0/dbt/include/starter_project/models/example/
+-rw-r--r--   0 materialize  (2000) materialize   (993)      972 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/starter_project/models/example/fraud_activity.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)      999 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/starter_project/models/example/funds_movement.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)      936 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/starter_project/models/example/my_first_dbt_model.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)      753 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/starter_project/models/example/my_second_dbt_model.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)     2847 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/starter_project/models/example/schema.yml
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-23 07:09:06.873289 dbt-materialize-1.8.0/dbt/include/starter_project/models/example/sources/
+-rw-r--r--   0 materialize  (2000) materialize   (993)      774 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/starter_project/models/example/sources/auction.sql
+-rw-r--r--   0 materialize  (2000) materialize   (993)      866 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/starter_project/models/example/sources/sources.yml
+-rw-r--r--   0 materialize  (2000) materialize   (993)     1068 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/dbt/include/starter_project/models/example/winning_bids.sql
+drwxr-xr-x   0 materialize  (2000) materialize   (993)        0 2024-05-23 07:09:06.873289 dbt-materialize-1.8.0/dbt_materialize.egg-info/
+-rw-r--r--   0 materialize  (2000) materialize   (993)     6613 2024-05-23 07:09:06.000000 dbt-materialize-1.8.0/dbt_materialize.egg-info/PKG-INFO
+-rw-r--r--   0 materialize  (2000) materialize   (993)     2739 2024-05-23 07:09:06.000000 dbt-materialize-1.8.0/dbt_materialize.egg-info/SOURCES.txt
+-rw-r--r--   0 materialize  (2000) materialize   (993)        1 2024-05-23 07:09:06.000000 dbt-materialize-1.8.0/dbt_materialize.egg-info/dependency_links.txt
+-rw-r--r--   0 materialize  (2000) materialize   (993)      216 2024-05-23 07:09:06.000000 dbt-materialize-1.8.0/dbt_materialize.egg-info/requires.txt
+-rw-r--r--   0 materialize  (2000) materialize   (993)        4 2024-05-23 07:09:06.000000 dbt-materialize-1.8.0/dbt_materialize.egg-info/top_level.txt
+-rw-r--r--   0 materialize  (2000) materialize   (993)      464 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/pyproject.toml
+-rw-r--r--   0 materialize  (2000) materialize   (993)       38 2024-05-23 07:09:06.873289 dbt-materialize-1.8.0/setup.cfg
+-rw-r--r--   0 materialize  (2000) materialize   (993)     2159 2024-05-23 07:08:39.000000 dbt-materialize-1.8.0/setup.py
```

### Comparing `dbt-materialize-1.7.8/PKG-INFO` & `dbt-materialize-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-materialize
-Version: 1.7.8
+Version: 1.8.0
 Summary: The Materialize adapter plugin for dbt.
 Home-page: https://github.com/MaterializeInc/materialize/blob/main/misc/dbt-materialize
 Author: Materialize, Inc.
 Author-email: support@materialize.com
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `dbt-materialize-1.7.8/README.md` & `dbt-materialize-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/__init__.py` & `dbt-materialize-1.8.0/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/adapters/__init__.py` & `dbt-materialize-1.8.0/dbt/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/adapters/materialize/__init__.py` & `dbt-materialize-1.8.0/dbt/adapters/materialize/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/adapters/materialize/__version__.py` & `dbt-materialize-1.8.0/dbt/adapters/materialize/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # If you bump this version, bump it in setup.py too.
-version = "1.7.8"
+version = "1.8.0"
```

### Comparing `dbt-materialize-1.7.8/dbt/adapters/materialize/connections.py` & `dbt-materialize-1.8.0/dbt/adapters/materialize/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,21 +13,20 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from dataclasses import dataclass
 from typing import Optional
 
+import dbt_common.exceptions
 import psycopg2
+from dbt_common.semver import versions_compatible
 
-import dbt.adapters.postgres.connections
-import dbt.exceptions
+from dbt.adapters.events.logging import AdapterLogger
 from dbt.adapters.postgres import PostgresConnectionManager, PostgresCredentials
-from dbt.events import AdapterLogger
-from dbt.semver import versions_compatible
 
 # If you bump this version, bump it in README.md too.
 SUPPORTED_MATERIALIZE_VERSIONS = ">=0.68.0"
 
 logger = AdapterLogger("Materialize")
 
 # Override the psycopg2 connect function in order to inject Materialize-specific
@@ -93,15 +92,15 @@
 
         mz_version = connection.handle.info.parameter_status(
             "mz_version"
         )  # e.g. v0.79.0-dev (937dfde5e)
         mz_version = mz_version.split()[0]  # e.g. v0.79.0-dev
         mz_version = mz_version[1:]  # e.g. 0.79.0-dev
         if not versions_compatible(mz_version, SUPPORTED_MATERIALIZE_VERSIONS):
-            raise dbt.exceptions.DbtRuntimeError(
+            raise dbt_common.exceptions.DbtRuntimeError(
                 f"Detected unsupported Materialize version {mz_version}\n"
                 f"  Supported versions: {SUPPORTED_MATERIALIZE_VERSIONS}"
             )
 
         return connection
 
     def cancel(self, connection):
```

### Comparing `dbt-materialize-1.7.8/dbt/adapters/materialize/exceptions.py` & `dbt-materialize-1.8.0/dbt/adapters/materialize/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Any
 
-from dbt.exceptions import CompilationError
+from dbt_common.exceptions import CompilationError
 
 
 class RefreshIntervalConfigNotDictError(CompilationError):
     def __init__(self, raw_refresh_interval: Any):
         self.raw_refresh_interval = raw_refresh_interval
         super().__init__(msg=self.get_message())
```

### Comparing `dbt-materialize-1.7.8/dbt/adapters/materialize/impl.py` & `dbt-materialize-1.8.0/dbt/adapters/materialize/impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,37 +13,38 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import time
 from dataclasses import dataclass
 from typing import Any, Dict, List, Optional
 
-import dbt.exceptions
+import dbt_common.exceptions
+from dbt_common.contracts.constraints import (
+    ColumnLevelConstraint,
+    ConstraintType,
+)
+from dbt_common.dataclass_schema import ValidationError, dbtClassMixin
+
 from dbt.adapters.base.impl import AdapterConfig, ConstraintSupport
 from dbt.adapters.base.meta import available
 from dbt.adapters.capability import (
     Capability,
     CapabilityDict,
     CapabilitySupport,
     Support,
 )
 from dbt.adapters.materialize.connections import MaterializeConnectionManager
 from dbt.adapters.materialize.exceptions import (
     RefreshIntervalConfigError,
     RefreshIntervalConfigNotDictError,
 )
 from dbt.adapters.materialize.relation import MaterializeRelation
-from dbt.adapters.postgres import PostgresAdapter
 from dbt.adapters.postgres.column import PostgresColumn
+from dbt.adapters.postgres.impl import PostgresAdapter
 from dbt.adapters.sql.impl import LIST_RELATIONS_MACRO_NAME
-from dbt.contracts.graph.nodes import (
-    ColumnLevelConstraint,
-    ConstraintType,
-)
-from dbt.dataclass_schema import ValidationError, dbtClassMixin
 
 
 # types in ./misc/dbt-materialize need to import generic types from typing
 @dataclass
 class MaterializeIndexConfig(dbtClassMixin):
     columns: Optional[List[str]] = None
     default: Optional[bool] = False
@@ -54,18 +55,20 @@
     def parse(cls, raw_index) -> Optional["MaterializeIndexConfig"]:
         if raw_index is None:
             return None
         try:
             cls.validate(raw_index)
             return cls.from_dict(raw_index)
         except ValidationError as exc:
-            msg = dbt.exceptions.validator_error_message(exc)
-            dbt.exceptions.CompilationError(f"Could not parse index config: {msg}")
+            msg = dbt_common.exceptions.validator_error_message(exc)
+            dbt_common.exceptions.CompilationError(
+                f"Could not parse index config: {msg}"
+            )
         except TypeError:
-            dbt.exceptions.CompilationError(
+            dbt_common.exceptions.CompilationError(
                 "Invalid index config:\n"
                 f"  Got: {raw_index}\n"
                 '  Expected a dictionary with at minimum a "columns" key'
             )
 
 
 # NOTE(morsapaes): Materialize allows configuring a refresh interval for the
```

### Comparing `dbt-materialize-1.7.8/dbt/adapters/materialize/relation.py` & `dbt-materialize-1.8.0/dbt/adapters/materialize/relation.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from dataclasses import dataclass
 from typing import Optional, Type
 
-from dbt.adapters.postgres import PostgresRelation
-from dbt.dataclass_schema import StrEnum
-from dbt.utils import classproperty
+from dbt_common.dataclass_schema import StrEnum
+
+from dbt.adapters.postgres.relation import PostgresRelation
+from dbt.adapters.utils import classproperty
 
 
 # types in ./misc/dbt-materialize need to import generic types from typing
 class MaterializeRelationType(StrEnum):
     # Built-in materialization types.
     Table = "table"
     View = "view"
```

### Comparing `dbt-materialize-1.7.8/dbt/include/__init__.py` & `dbt-materialize-1.8.0/dbt/include/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/materialize/__init__.py` & `dbt-materialize-1.8.0/dbt/include/materialize/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/materialize/dbt_project.yml` & `dbt-materialize-1.8.0/dbt/include/materialize/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/materialize/macros/adapters.sql` & `dbt-materialize-1.8.0/dbt/include/materialize/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/materialize/macros/catalog.sql` & `dbt-materialize-1.8.0/dbt/include/materialize/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/materialize/macros/columns.sql` & `dbt-materialize-1.8.0/dbt/include/materialize/macros/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/materialize/macros/deploy/deploy_await.sql` & `dbt-materialize-1.8.0/dbt/include/materialize/macros/deploy/deploy_await.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/materialize/macros/deploy/deploy_cleanup.sql` & `dbt-materialize-1.8.0/dbt/include/materialize/macros/deploy/deploy_cleanup.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/materialize/macros/deploy/deploy_init.sql` & `dbt-materialize-1.8.0/dbt/include/materialize/macros/deploy/deploy_init.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/materialize/macros/deploy/deploy_permission_validation.sql` & `dbt-materialize-1.8.0/dbt/include/materialize/macros/deploy/deploy_permission_validation.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/materialize/macros/deploy/deploy_promote.sql` & `dbt-materialize-1.8.0/dbt/include/materialize/macros/deploy/deploy_promote.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/materialize/macros/freshness.sql` & `dbt-materialize-1.8.0/dbt/include/materialize/macros/freshness.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/materialize/macros/materializations/incremental.sql` & `dbt-materialize-1.8.0/dbt/include/materialize/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/materialize/macros/materializations/materialized_view.sql` & `dbt-materialize-1.8.0/dbt/include/materialize/macros/materializations/materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/materialize/macros/materializations/materializedview.sql` & `dbt-materialize-1.8.0/dbt/include/materialize/macros/materializations/materializedview.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/materialize/macros/materializations/sink.sql` & `dbt-materialize-1.8.0/dbt/include/materialize/macros/materializations/sink.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/materialize/macros/materializations/source.sql` & `dbt-materialize-1.8.0/dbt/include/materialize/macros/materializations/source.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/materialize/macros/materializations/table.sql` & `dbt-materialize-1.8.0/dbt/include/materialize/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/materialize/macros/materializations/test.sql` & `dbt-materialize-1.8.0/dbt/include/materialize/macros/materializations/test.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/materialize/macros/materializations/view.sql` & `dbt-materialize-1.8.0/dbt/include/materialize/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/materialize/macros/tests/helpers.sql` & `dbt-materialize-1.8.0/dbt/include/materialize/macros/tests/helpers.sql`

 * *Files 10% similar despite different names*

```diff
@@ -18,7 +18,17 @@
         {% call statement(auto_begin=True) %}
             set cluster = {{ cluster }}
         {% endcall %}
     {% endif %}
 
   {{ adapter.dispatch('get_test_sql', 'dbt')(main_sql, fail_calc, warn_if, error_if, limit) }}
 {%- endmacro %}
+
+{% macro get_unit_test_sql(main_sql, expected_fixture_sql, expected_column_names, cluster) -%}
+    {% if cluster %}
+        {% call statement(auto_begin=True) %}
+            set cluster = {{ cluster }}
+        {% endcall %}
+    {% endif %}
+
+  {{ adapter.dispatch('get_unit_test_sql', 'dbt')(main_sql, expected_fixture_sql, expected_column_names) }}
+{%- endmacro %}
```

### Comparing `dbt-materialize-1.7.8/dbt/include/materialize/macros/utils/await_cluster_ready.sql` & `dbt-materialize-1.8.0/dbt/include/materialize/macros/utils/await_cluster_ready.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/materialize/macros/utils/ci_utils.sql` & `dbt-materialize-1.8.0/dbt/include/materialize/macros/utils/ci_utils.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/materialize/macros/utils/exists.sql` & `dbt-materialize-1.8.0/dbt/include/materialize/macros/utils/exists.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/materialize/macros/utils/generate_cluster_name.sql` & `dbt-materialize-1.8.0/dbt/include/materialize/macros/utils/generate_cluster_name.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/materialize/macros/utils/generate_schema_name.sql` & `dbt-materialize-1.8.0/dbt/include/materialize/macros/utils/generate_schema_name.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/materialize/macros/utils/is_cluster_ready.sql` & `dbt-materialize-1.8.0/dbt/include/materialize/macros/utils/is_cluster_ready.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/materialize/macros/utils/listagg.sql` & `dbt-materialize-1.8.0/dbt/include/materialize/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/materialize/profile_template.yml` & `dbt-materialize-1.8.0/dbt/include/materialize/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/materialize/sample_profiles.yml` & `dbt-materialize-1.8.0/dbt/include/materialize/sample_profiles.yml`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/starter_project/dbt_project.yml` & `dbt-materialize-1.8.0/dbt/include/starter_project/dbt_project.yml`

 * *Files 2% similar despite different names*

```diff
@@ -21,11 +21,11 @@
 
 model-paths: ["models"]
 
 clean-targets:
   - "target"
   - "dbt_packages"
 
-tests:
+data_tests:
   {project_name}:
     +store_failures: true
     +schema: 'etl_failure'
```

### Comparing `dbt-materialize-1.7.8/dbt/include/starter_project/models/example/fraud_activity.sql` & `dbt-materialize-1.8.0/dbt/include/starter_project/models/example/fraud_activity.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/starter_project/models/example/funds_movement.sql` & `dbt-materialize-1.8.0/dbt/include/starter_project/models/example/funds_movement.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/starter_project/models/example/my_first_dbt_model.sql` & `dbt-materialize-1.8.0/dbt/include/starter_project/models/example/my_first_dbt_model.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/starter_project/models/example/my_second_dbt_model.sql` & `dbt-materialize-1.8.0/dbt/include/starter_project/models/example/my_second_dbt_model.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/starter_project/models/example/schema.yml` & `dbt-materialize-1.8.0/dbt/include/starter_project/models/example/schema.yml`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 models:
   - name: fraud_activity
     description: "Detects when a user wins an auction as a bidder, and then is identified as a seller for an item at a higher price."
     columns:
       - name: seller
         description: "The seller for an auction"
-        tests:
+        data_tests:
           - unique
           - not_null
       - name: seller_item
         description: "The name of the seller item"
       - name: seller_amount
         description: "The bid amount of the seller"
       - name: buyer_item
@@ -36,27 +36,27 @@
         description: "The bid amount of the buyer"
 
   - name: funds_movement
     description: "Tracks the credits and debits of all winning bids."
     columns:
       - name: id
         description: "The id of the buyer or seller"
-        tests:
+        data_tests:
           - not_null
       - name: credits
         description: "Credit from an auction"
       - name: debits
         description: "Debit from an auction"
 
   - name: winning_bids
     description: "joins data from `auctions` and `bids` to get the bid with the highest `amount` for each auction at its `end_time`."
     columns:
       - name: id
         description: "The primary key of the auction"
-        tests:
+        data_tests:
           - unique
           - not_null
       - name: buyer
         description: "The id of the buyer"
       - name: auction_id
         description: "The id of the auction"
       - name: amount
@@ -69,19 +69,19 @@
         description: "The id of the seller"
 
   - name: my_first_dbt_model
     description: "A starter dbt model"
     columns:
       - name: id
         description: "The primary key for this table"
-        tests:
+        data_tests:
           - unique
           - not_null
 
   - name: my_second_dbt_model
     description: "A starter dbt model"
     columns:
       - name: id
         description: "The primary key for this table"
-        tests:
+        data_tests:
           - unique
           - not_null
```

### Comparing `dbt-materialize-1.7.8/dbt/include/starter_project/models/example/sources/auction.sql` & `dbt-materialize-1.8.0/dbt/include/starter_project/models/example/sources/auction.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/starter_project/models/example/sources/sources.yml` & `dbt-materialize-1.8.0/dbt/include/starter_project/models/example/sources/sources.yml`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt/include/starter_project/models/example/winning_bids.sql` & `dbt-materialize-1.8.0/dbt/include/starter_project/models/example/winning_bids.sql`

 * *Files identical despite different names*

### Comparing `dbt-materialize-1.7.8/dbt_materialize.egg-info/PKG-INFO` & `dbt-materialize-1.8.0/dbt_materialize.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-materialize
-Version: 1.7.8
+Version: 1.8.0
 Summary: The Materialize adapter plugin for dbt.
 Home-page: https://github.com/MaterializeInc/materialize/blob/main/misc/dbt-materialize
 Author: Materialize, Inc.
 Author-email: support@materialize.com
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `dbt-materialize-1.7.8/dbt_materialize.egg-info/SOURCES.txt` & `dbt-materialize-1.8.0/dbt_materialize.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,17 +27,19 @@
 dbt/include/materialize/macros/materializations/incremental.sql
 dbt/include/materialize/macros/materializations/materialized_view.sql
 dbt/include/materialize/macros/materializations/materializedview.sql
 dbt/include/materialize/macros/materializations/sink.sql
 dbt/include/materialize/macros/materializations/source.sql
 dbt/include/materialize/macros/materializations/table.sql
 dbt/include/materialize/macros/materializations/test.sql
+dbt/include/materialize/macros/materializations/unit.sql
 dbt/include/materialize/macros/materializations/view.sql
 dbt/include/materialize/macros/tests/helpers.sql
 dbt/include/materialize/macros/utils/await_cluster_ready.sql
+dbt/include/materialize/macros/utils/cast.sql
 dbt/include/materialize/macros/utils/ci_utils.sql
 dbt/include/materialize/macros/utils/exists.sql
 dbt/include/materialize/macros/utils/generate_cluster_name.sql
 dbt/include/materialize/macros/utils/generate_schema_name.sql
 dbt/include/materialize/macros/utils/is_cluster_ready.sql
 dbt/include/materialize/macros/utils/listagg.sql
 dbt/include/starter_project/dbt_project.yml
```

