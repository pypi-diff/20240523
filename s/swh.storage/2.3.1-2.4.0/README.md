# Comparing `tmp/swh_storage-2.3.1.tar.gz` & `tmp/swh_storage-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swh_storage-2.3.1.tar", last modified: Tue May 14 12:45:02 2024, max compression
+gzip compressed data, was "swh_storage-2.4.0.tar", last modified: Thu May 23 13:05:40 2024, max compression
```

## Comparing `swh_storage-2.3.1.tar` & `swh_storage-2.4.0.tar`

### file list

```diff
@@ -1,386 +1,402 @@
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:45:02.740685 swh_storage-2.3.1/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      352 2024-05-14 12:44:56.000000 swh_storage-2.3.1/.copier-answers.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      158 2024-05-14 12:44:56.000000 swh_storage-2.3.1/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-05-14 12:44:56.000000 swh_storage-2.3.1/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1453 2024-05-14 12:44:56.000000 swh_storage-2.3.1/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-05-14 12:44:56.000000 swh_storage-2.3.1/AUTHORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-05-14 12:44:56.000000 swh_storage-2.3.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) jenkins    (120)       61 2024-05-14 12:44:56.000000 swh_storage-2.3.1/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-05-14 12:44:56.000000 swh_storage-2.3.1/LICENSE
--rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-05-14 12:44:56.000000 swh_storage-2.3.1/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)       72 2024-05-14 12:44:56.000000 swh_storage-2.3.1/Makefile.local
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8493 2024-05-14 12:45:02.740685 swh_storage-2.3.1/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6270 2024-05-14 12:44:56.000000 swh_storage-2.3.1/README.rst
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:45:02.652686 swh_storage-2.3.1/bin/
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)     1240 2024-05-14 12:44:56.000000 swh_storage-2.3.1/bin/swh-storage-add-dir
--rw-r--r--   0 jenkins    (115) jenkins    (120)      294 2024-05-14 12:44:56.000000 swh_storage-2.3.1/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:45:02.652686 swh_storage-2.3.1/docs/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-14 12:44:56.000000 swh_storage-2.3.1/docs/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)       48 2024-05-14 12:44:56.000000 swh_storage-2.3.1/docs/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)      530 2024-05-14 12:44:56.000000 swh_storage-2.3.1/docs/Makefile.local
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:45:02.652686 swh_storage-2.3.1/docs/_static/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:44:56.000000 swh_storage-2.3.1/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:45:02.652686 swh_storage-2.3.1/docs/_templates/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:44:56.000000 swh_storage-2.3.1/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2206 2024-05-14 12:44:56.000000 swh_storage-2.3.1/docs/archive-copies.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      143 2024-05-14 12:44:56.000000 swh_storage-2.3.1/docs/cli.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-05-14 12:44:56.000000 swh_storage-2.3.1/docs/conf.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12947 2024-05-14 12:44:56.000000 swh_storage-2.3.1/docs/extrinsic-metadata-specification.rst
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:45:02.656686 swh_storage-2.3.1/docs/images/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       12 2024-05-14 12:44:56.000000 swh_storage-2.3.1/docs/images/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)      335 2024-05-14 12:44:56.000000 swh_storage-2.3.1/docs/images/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3031 2024-05-14 12:44:56.000000 swh_storage-2.3.1/docs/images/swh-archive-copies.dia
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2843 2024-05-14 12:44:56.000000 swh_storage-2.3.1/docs/index.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3772 2024-05-14 12:44:56.000000 swh_storage-2.3.1/docs/object-masking.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      268 2024-05-14 12:44:56.000000 swh_storage-2.3.1/docs/sql-storage.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1097 2024-05-14 12:44:56.000000 swh_storage-2.3.1/mypy.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2719 2024-05-14 12:44:56.000000 swh_storage-2.3.1/pyproject.toml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      458 2024-05-14 12:44:56.000000 swh_storage-2.3.1/pytest.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)       19 2024-05-14 12:44:56.000000 swh_storage-2.3.1/requirements-swh-journal.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       94 2024-05-14 12:44:56.000000 swh_storage-2.3.1/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      406 2024-05-14 12:44:56.000000 swh_storage-2.3.1/requirements-test.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      189 2024-05-14 12:44:56.000000 swh_storage-2.3.1/requirements.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      120 2024-05-14 12:45:02.740685 swh_storage-2.3.1/setup.cfg
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:45:02.656686 swh_storage-2.3.1/sql/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       26 2024-05-14 12:44:56.000000 swh_storage-2.3.1/sql/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1565 2024-05-14 12:44:56.000000 swh_storage-2.3.1/sql/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1094 2024-05-14 12:44:56.000000 swh_storage-2.3.1/sql/TODO
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:45:02.656686 swh_storage-2.3.1/sql/bin/
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)     1701 2024-05-14 12:44:56.000000 swh_storage-2.3.1/sql/bin/db-upgrade
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)      538 2024-05-14 12:44:56.000000 swh_storage-2.3.1/sql/bin/dot_add_content
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2023 2024-05-14 12:44:56.000000 swh_storage-2.3.1/sql/clusters.dot
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:45:02.640686 swh_storage-2.3.1/sql/doc/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:45:02.660686 swh_storage-2.3.1/sql/json/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        8 2024-05-14 12:44:56.000000 swh_storage-2.3.1/sql/json/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)      283 2024-05-14 12:44:56.000000 swh_storage-2.3.1/sql/json/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)      223 2024-05-14 12:44:56.000000 swh_storage-2.3.1/sql/json/entity.lister_metadata.schema.json
--rw-r--r--   0 jenkins    (115) jenkins    (120)      129 2024-05-14 12:44:56.000000 swh_storage-2.3.1/sql/json/entity.metadata.schema.json
--rw-r--r--   0 jenkins    (115) jenkins    (120)      223 2024-05-14 12:44:56.000000 swh_storage-2.3.1/sql/json/entity_history.lister_metadata.schema.json
--rw-r--r--   0 jenkins    (115) jenkins    (120)      137 2024-05-14 12:44:56.000000 swh_storage-2.3.1/sql/json/entity_history.metadata.schema.json
--rw-r--r--   0 jenkins    (115) jenkins    (120)      631 2024-05-14 12:44:56.000000 swh_storage-2.3.1/sql/json/fetch_history.result.schema.json
--rw-r--r--   0 jenkins    (115) jenkins    (120)      133 2024-05-14 12:44:56.000000 swh_storage-2.3.1/sql/json/list_history.result.schema.json
--rw-r--r--   0 jenkins    (115) jenkins    (120)      141 2024-05-14 12:44:56.000000 swh_storage-2.3.1/sql/json/listable_entity.list_params.schema.json
--rw-r--r--   0 jenkins    (115) jenkins    (120)      632 2024-05-14 12:44:56.000000 swh_storage-2.3.1/sql/json/origin_visit.metadata.json
--rw-r--r--   0 jenkins    (115) jenkins    (120)      252 2024-05-14 12:44:56.000000 swh_storage-2.3.1/sql/json/tool.tool_configuration.schema.json
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:45:02.640686 swh_storage-2.3.1/swh/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:45:02.664686 swh_storage-2.3.1/swh/storage/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3478 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:45:02.668686 swh_storage-2.3.1/swh/storage/algos/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/algos/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    16246 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/algos/diff.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12947 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/algos/dir_iterators.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3468 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/algos/directory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1487 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/algos/discovery.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3280 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/algos/origin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    19935 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/algos/revisions_walker.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6525 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/algos/snapshot.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:45:02.668686 swh_storage-2.3.1/swh/storage/api/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/api/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2110 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/api/client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4512 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/api/serializers.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5403 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/api/server.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    20570 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/backfill.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:45:02.668686 swh_storage-2.3.1/swh/storage/cassandra/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      375 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/cassandra/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      516 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/cassandra/common.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5919 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/cassandra/converters.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    62367 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/cassandra/cql.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10766 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/cassandra/model.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     9301 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/cassandra/schema.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    86739 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/cassandra/storage.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    14670 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      496 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/common.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3325 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/exc.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2010 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/fixer.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    31355 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/in_memory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    58274 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/interface.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5033 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/metrics.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    48089 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/migrate_extrinsic_metadata.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4245 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/objstorage.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:45:02.672686 swh_storage-2.3.1/swh/storage/postgresql/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/postgresql/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12515 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/postgresql/converters.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    65514 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/postgresql/db.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    69889 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/postgresql/storage.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:45:02.672686 swh_storage-2.3.1/swh/storage/proxies/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/proxies/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12690 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/proxies/buffer.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2033 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/proxies/counter.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5120 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/proxies/filter.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:45:02.672686 swh_storage-2.3.1/swh/storage/proxies/masking/
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18643 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/proxies/masking/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    13661 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/proxies/masking/cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    14347 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/proxies/masking/db.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:45:02.676686 swh_storage-2.3.1/swh/storage/proxies/masking/sql/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       66 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/proxies/masking/sql/10-superuser-init.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      220 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/proxies/masking/sql/20-types.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1989 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/proxies/masking/sql/30-schema.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      334 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/proxies/masking/sql/60-indexes.sql
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:45:02.676686 swh_storage-2.3.1/swh/storage/proxies/masking/sql/upgrades/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      336 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/proxies/masking/sql/upgrades/193.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4255 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/proxies/record_references.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3229 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/proxies/retry.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7058 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/proxies/tenacious.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2586 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/proxies/validate.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/py.typed
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10170 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/pytest_plugin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10285 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/replay.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:45:02.676686 swh_storage-2.3.1/swh/storage/sql/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      758 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/10-superuser-init.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      984 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/15-flavor.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1080 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/20-enums.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)    24592 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/30-schema.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)    34836 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/40-funcs.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)    13835 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/60-indexes.sql
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:45:02.676686 swh_storage-2.3.1/swh/storage/sql/logical_replication/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1380 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/logical_replication/replication_source.sql
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:45:02.720685 swh_storage-2.3.1/swh/storage/sql/upgrades/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6750 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/015.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      854 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/016.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6452 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/017.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2845 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/018.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      999 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/019.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1416 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/020.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1464 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/021.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1607 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/022.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1561 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/023.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6282 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/024.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3272 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/025.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      658 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/026.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     9090 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/027.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1446 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/028.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2788 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/029.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1706 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/030.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4156 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/032.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1131 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/033.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2599 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/034.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1535 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/035.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2256 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/036.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      654 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/037.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4588 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/038.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1659 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/039.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      553 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/040.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      542 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/041.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      702 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/042.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2902 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/043.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2130 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/044.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      465 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/045.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7305 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/046.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2649 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/047.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1795 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/048.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     9599 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/049.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1688 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/050.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4279 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/051.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6016 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/052.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      905 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/053.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3187 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/054.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2309 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/055.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2350 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/056.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      729 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/057.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1428 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/058.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1528 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/059.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1428 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/060.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      724 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/061.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1427 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/062.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2594 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/063.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      604 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/064.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1664 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/065.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      281 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/066.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1257 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/067.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8795 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/068.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      618 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/069.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      352 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/070.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      687 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/071.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3843 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/072.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1940 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/073.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2662 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/074.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3067 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/075.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      551 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/076.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1567 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/077.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3642 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/078.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      997 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/079.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      631 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/080.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      608 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/081.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3043 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/082.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1834 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/083.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2392 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/084.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2388 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/085.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1249 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/086.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8777 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/087.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3567 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/088.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3788 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/089.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)    21174 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/090.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      959 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/091.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      925 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/092.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1795 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/093.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      735 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/094.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      726 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/095.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1137 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/096.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18174 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/097.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      280 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/098.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      875 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/099.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2055 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/100.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1037 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/101.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6608 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/102.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2399 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/103.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5055 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/104.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1078 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/105.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)    13015 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/106.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1755 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/107.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1427 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/108.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      816 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/109.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)    13273 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/110.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      784 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/111.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1620 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/112.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1142 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/113.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2334 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/114.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5180 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/115.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      276 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/116.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1742 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/117.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2768 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/118.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      850 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/119.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1062 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/120.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      274 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/121.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      366 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/122.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2107 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/123.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1371 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/124.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1302 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/125.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      329 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/126.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1039 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/127.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      609 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/128.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      832 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/129.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1572 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/130.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      401 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/131.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      386 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/132.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      425 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/133.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1626 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/134.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      421 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/135.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1036 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/136.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10048 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/137.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      926 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/138.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      845 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/139.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      456 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/140.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      230 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/141.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      239 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/142.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2897 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/143.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      283 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/144.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      275 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/145.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3340 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/146.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2676 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/147.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2168 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/148.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3849 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/149.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      624 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/150.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      373 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/151.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      302 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/152.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      462 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/153.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1546 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/154.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1044 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/155.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      875 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/156.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2606 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/157.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3118 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/158.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      727 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/159.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1353 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/160.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      548 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/161.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2099 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/162.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1202 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/163.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      304 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/164.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      430 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/165.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      306 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/166.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      591 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/167.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1403 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/168.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1812 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/169.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      614 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/170.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      758 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/171.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      873 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/172.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      561 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/173.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      324 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/174.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1294 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/175.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      886 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/176.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      256 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/177.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      256 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/178.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6715 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/179.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3159 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/180.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      661 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/181.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2782 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/182.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1715 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/183.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      910 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/184.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1091 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/185.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/186.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1601 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/187.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1045 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/188.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      616 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/189.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1105 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/190.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1751 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/191.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      162 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/192.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1731 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/sql/upgrades/193.sql
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:45:02.728685 swh_storage-2.3.1/swh/storage/tests/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:45:02.732685 swh_storage-2.3.1/swh/storage/tests/algos/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/algos/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12969 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/algos/test_diff.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5545 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/algos/test_dir_iterator.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7293 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/algos/test_directory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2284 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/algos/test_discovery.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    11595 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/algos/test_origin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18297 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/algos/test_revisions_walker.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    13842 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/algos/test_snapshot.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2790 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:45:02.732685 swh_storage-2.3.1/swh/storage/tests/data/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      189 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/data/storage.yml
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:45:02.732685 swh_storage-2.3.1/swh/storage/tests/masking/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/masking/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1076 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/masking/conftest.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    19842 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/masking/test_cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10967 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/masking/test_db.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    30504 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/masking/test_proxy.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5872 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/masking/test_proxy_masking.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      960 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/masking/test_proxy_no_masking.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:45:02.736685 swh_storage-2.3.1/swh/storage/tests/migrate_extrinsic_metadata/
--rw-r--r--   0 jenkins    (115) jenkins    (120)    11035 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/migrate_extrinsic_metadata/test_cran.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    20296 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/migrate_extrinsic_metadata/test_debian.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    52095 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/migrate_extrinsic_metadata/test_deposit.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3702 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/migrate_extrinsic_metadata/test_gnu.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4246 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/migrate_extrinsic_metadata/test_nixguix.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    15543 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/migrate_extrinsic_metadata/test_npm.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    25029 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/migrate_extrinsic_metadata/test_pypi.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    27669 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/storage_data.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)   235228 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/storage_tests.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6103 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/test_api_client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    14820 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/test_backfill.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    24799 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/test_buffer.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    29473 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/test_cassandra.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5495 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/test_cassandra_converters.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12438 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/test_cassandra_migration.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    13302 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/test_cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1887 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/test_counter.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2360 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/test_exception.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5260 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/test_filter.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4188 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/test_in_memory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8745 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/test_init.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4944 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/test_kafka_writer.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4698 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/test_metrics.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    20071 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/test_postgresql.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12253 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/test_postgresql_converters.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1399 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/test_postgresql_flavor_mirror.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1423 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/test_postgresql_flavor_readreplica.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      669 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/test_pytest_plugin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8582 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/test_record_references.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    23199 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/test_replay.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8212 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/test_retry.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1589 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/test_revision_bw_compat.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1346 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/test_serializers.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3323 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/test_server.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1186 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/test_storage_data.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    14141 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/test_tenacious.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4755 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/test_utils.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4515 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/tests/test_validate.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3700 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/utils.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4041 2024-05-14 12:44:56.000000 swh_storage-2.3.1/swh/storage/writer.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-14 12:45:02.736685 swh_storage-2.3.1/swh.storage.egg-info/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8493 2024-05-14 12:45:02.000000 swh_storage-2.3.1/swh.storage.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)    11563 2024-05-14 12:45:02.000000 swh_storage-2.3.1/swh.storage.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-05-14 12:45:02.000000 swh_storage-2.3.1/swh.storage.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      882 2024-05-14 12:45:02.000000 swh_storage-2.3.1/swh.storage.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      488 2024-05-14 12:45:02.000000 swh_storage-2.3.1/swh.storage.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-05-14 12:45:02.000000 swh_storage-2.3.1/swh.storage.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1264 2024-05-14 12:44:56.000000 swh_storage-2.3.1/tox.ini
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.973009 swh_storage-2.4.0/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      352 2024-05-23 13:05:35.000000 swh_storage-2.4.0/.copier-answers.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      158 2024-05-23 13:05:35.000000 swh_storage-2.4.0/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-05-23 13:05:35.000000 swh_storage-2.4.0/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1453 2024-05-23 13:05:35.000000 swh_storage-2.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-05-23 13:05:35.000000 swh_storage-2.4.0/AUTHORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-05-23 13:05:35.000000 swh_storage-2.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       61 2024-05-23 13:05:35.000000 swh_storage-2.4.0/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-05-23 13:05:35.000000 swh_storage-2.4.0/LICENSE
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-05-23 13:05:35.000000 swh_storage-2.4.0/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       72 2024-05-23 13:05:35.000000 swh_storage-2.4.0/Makefile.local
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8493 2024-05-23 13:05:40.973009 swh_storage-2.4.0/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6270 2024-05-23 13:05:35.000000 swh_storage-2.4.0/README.rst
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.897010 swh_storage-2.4.0/bin/
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)     1240 2024-05-23 13:05:35.000000 swh_storage-2.4.0/bin/swh-storage-add-dir
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      294 2024-05-23 13:05:35.000000 swh_storage-2.4.0/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.897010 swh_storage-2.4.0/docs/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-23 13:05:35.000000 swh_storage-2.4.0/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       48 2024-05-23 13:05:35.000000 swh_storage-2.4.0/docs/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      530 2024-05-23 13:05:35.000000 swh_storage-2.4.0/docs/Makefile.local
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.901010 swh_storage-2.4.0/docs/_static/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:35.000000 swh_storage-2.4.0/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.901010 swh_storage-2.4.0/docs/_templates/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:35.000000 swh_storage-2.4.0/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2206 2024-05-23 13:05:35.000000 swh_storage-2.4.0/docs/archive-copies.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      143 2024-05-23 13:05:35.000000 swh_storage-2.4.0/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-05-23 13:05:35.000000 swh_storage-2.4.0/docs/conf.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12947 2024-05-23 13:05:35.000000 swh_storage-2.4.0/docs/extrinsic-metadata-specification.rst
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.901010 swh_storage-2.4.0/docs/images/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       12 2024-05-23 13:05:35.000000 swh_storage-2.4.0/docs/images/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      335 2024-05-23 13:05:35.000000 swh_storage-2.4.0/docs/images/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3031 2024-05-23 13:05:35.000000 swh_storage-2.4.0/docs/images/swh-archive-copies.dia
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2843 2024-05-23 13:05:35.000000 swh_storage-2.4.0/docs/index.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3772 2024-05-23 13:05:35.000000 swh_storage-2.4.0/docs/object-masking.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      268 2024-05-23 13:05:35.000000 swh_storage-2.4.0/docs/sql-storage.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1097 2024-05-23 13:05:35.000000 swh_storage-2.4.0/mypy.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2852 2024-05-23 13:05:35.000000 swh_storage-2.4.0/pyproject.toml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      458 2024-05-23 13:05:35.000000 swh_storage-2.4.0/pytest.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       19 2024-05-23 13:05:35.000000 swh_storage-2.4.0/requirements-swh-journal.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       94 2024-05-23 13:05:35.000000 swh_storage-2.4.0/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      406 2024-05-23 13:05:35.000000 swh_storage-2.4.0/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      189 2024-05-23 13:05:35.000000 swh_storage-2.4.0/requirements.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      120 2024-05-23 13:05:40.973009 swh_storage-2.4.0/setup.cfg
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.901010 swh_storage-2.4.0/sql/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       26 2024-05-23 13:05:35.000000 swh_storage-2.4.0/sql/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1565 2024-05-23 13:05:35.000000 swh_storage-2.4.0/sql/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1094 2024-05-23 13:05:35.000000 swh_storage-2.4.0/sql/TODO
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.901010 swh_storage-2.4.0/sql/bin/
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)     1701 2024-05-23 13:05:35.000000 swh_storage-2.4.0/sql/bin/db-upgrade
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)      538 2024-05-23 13:05:35.000000 swh_storage-2.4.0/sql/bin/dot_add_content
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2023 2024-05-23 13:05:35.000000 swh_storage-2.4.0/sql/clusters.dot
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.889010 swh_storage-2.4.0/sql/doc/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.905010 swh_storage-2.4.0/sql/json/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        8 2024-05-23 13:05:35.000000 swh_storage-2.4.0/sql/json/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      283 2024-05-23 13:05:35.000000 swh_storage-2.4.0/sql/json/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      223 2024-05-23 13:05:35.000000 swh_storage-2.4.0/sql/json/entity.lister_metadata.schema.json
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      129 2024-05-23 13:05:35.000000 swh_storage-2.4.0/sql/json/entity.metadata.schema.json
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      223 2024-05-23 13:05:35.000000 swh_storage-2.4.0/sql/json/entity_history.lister_metadata.schema.json
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      137 2024-05-23 13:05:35.000000 swh_storage-2.4.0/sql/json/entity_history.metadata.schema.json
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      631 2024-05-23 13:05:35.000000 swh_storage-2.4.0/sql/json/fetch_history.result.schema.json
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      133 2024-05-23 13:05:35.000000 swh_storage-2.4.0/sql/json/list_history.result.schema.json
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      141 2024-05-23 13:05:35.000000 swh_storage-2.4.0/sql/json/listable_entity.list_params.schema.json
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      632 2024-05-23 13:05:35.000000 swh_storage-2.4.0/sql/json/origin_visit.metadata.json
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      252 2024-05-23 13:05:35.000000 swh_storage-2.4.0/sql/json/tool.tool_configuration.schema.json
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.889010 swh_storage-2.4.0/swh/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.909010 swh_storage-2.4.0/swh/storage/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3478 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.909010 swh_storage-2.4.0/swh/storage/algos/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/algos/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    16246 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/algos/diff.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12947 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/algos/dir_iterators.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3468 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/algos/directory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1487 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/algos/discovery.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3280 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/algos/origin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    19935 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/algos/revisions_walker.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6541 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/algos/snapshot.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.909010 swh_storage-2.4.0/swh/storage/api/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/api/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2051 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/api/client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4512 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/api/serializers.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5403 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/api/server.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    20586 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/backfill.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.913010 swh_storage-2.4.0/swh/storage/cassandra/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      375 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/cassandra/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      516 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/cassandra/common.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5919 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/cassandra/converters.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    62367 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/cassandra/cql.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10766 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/cassandra/model.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     9301 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/cassandra/schema.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    86844 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/cassandra/storage.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    14670 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      496 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/common.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4056 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/exc.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2010 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/fixer.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    31355 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/in_memory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    58274 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/interface.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5033 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/metrics.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    48089 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/migrate_extrinsic_metadata.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4245 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/objstorage.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.913010 swh_storage-2.4.0/swh/storage/postgresql/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/postgresql/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12515 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/postgresql/converters.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    65514 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/postgresql/db.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    69921 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/postgresql/storage.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.913010 swh_storage-2.4.0/swh/storage/proxies/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.913010 swh_storage-2.4.0/swh/storage/proxies/blocking/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4324 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/blocking/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    11863 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/blocking/cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    16395 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/blocking/db.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.913010 swh_storage-2.4.0/swh/storage/proxies/blocking/sql/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       66 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/blocking/sql/10-superuser-init.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2665 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/blocking/sql/30-schema.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      324 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/blocking/sql/60-indexes.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12690 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/buffer.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2033 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/counter.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5120 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/filter.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.917009 swh_storage-2.4.0/swh/storage/proxies/masking/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    18649 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/masking/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    13661 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/masking/cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    14347 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/masking/db.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.917009 swh_storage-2.4.0/swh/storage/proxies/masking/sql/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       66 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/masking/sql/10-superuser-init.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      220 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/masking/sql/20-types.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1989 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/masking/sql/30-schema.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      334 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/masking/sql/60-indexes.sql
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.917009 swh_storage-2.4.0/swh/storage/proxies/masking/sql/upgrades/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      336 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/masking/sql/upgrades/193.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4255 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/record_references.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3229 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/retry.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7058 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/tenacious.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2586 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/proxies/validate.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/py.typed
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10170 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10225 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/replay.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.917009 swh_storage-2.4.0/swh/storage/sql/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      758 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/10-superuser-init.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      984 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/15-flavor.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1080 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/20-enums.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    24592 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/30-schema.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    34836 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/40-funcs.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    13835 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/60-indexes.sql
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.917009 swh_storage-2.4.0/swh/storage/sql/logical_replication/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1380 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/logical_replication/replication_source.sql
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.957009 swh_storage-2.4.0/swh/storage/sql/upgrades/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6750 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/015.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      854 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/016.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6452 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/017.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2845 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/018.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      999 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/019.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1416 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/020.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1464 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/021.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1607 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/022.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1561 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/023.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6282 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/024.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3272 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/025.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      658 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/026.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     9090 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/027.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1446 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/028.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2788 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/029.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1706 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/030.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4156 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/032.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1131 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/033.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2599 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/034.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1535 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/035.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2256 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/036.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      654 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/037.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4588 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/038.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1659 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/039.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      553 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/040.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      542 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/041.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      702 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/042.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2902 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/043.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2130 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/044.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      465 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/045.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7305 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/046.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2649 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/047.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1795 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/048.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     9599 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/049.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1688 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/050.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4279 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/051.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6016 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/052.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      905 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/053.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3187 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/054.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2309 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/055.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2350 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/056.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      729 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/057.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1428 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/058.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1528 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/059.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1428 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/060.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      724 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/061.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1427 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/062.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2594 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/063.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      604 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/064.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1664 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/065.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      281 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/066.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1257 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/067.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8795 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/068.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      618 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/069.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      352 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/070.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      687 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/071.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3843 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/072.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1940 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/073.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2662 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/074.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3067 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/075.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      551 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/076.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1567 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/077.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3642 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/078.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      997 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/079.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      631 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/080.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      608 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/081.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3043 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/082.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1834 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/083.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2392 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/084.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2388 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/085.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1249 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/086.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8777 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/087.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3567 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/088.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3788 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/089.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    21174 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/090.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      959 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/091.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      925 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/092.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1795 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/093.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      735 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/094.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      726 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/095.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1137 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/096.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    18174 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/097.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      280 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/098.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      875 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/099.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2055 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/100.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1037 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/101.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6608 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/102.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2399 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/103.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5055 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/104.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1078 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/105.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    13015 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/106.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1755 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/107.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1427 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/108.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      816 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/109.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    13273 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/110.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      784 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/111.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1620 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/112.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1142 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/113.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2334 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/114.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5180 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/115.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      276 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/116.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1742 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/117.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2768 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/118.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      850 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/119.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1062 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/120.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      274 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/121.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      366 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/122.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2107 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/123.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1371 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/124.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1302 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/125.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      329 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/126.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1039 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/127.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      609 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/128.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      832 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/129.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1572 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/130.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      401 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/131.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      386 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/132.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      425 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/133.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1626 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/134.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      421 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/135.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1036 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/136.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10048 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/137.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      926 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/138.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      845 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/139.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      456 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/140.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      230 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/141.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      239 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/142.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2897 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/143.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      283 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/144.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      275 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/145.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3340 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/146.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2676 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/147.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2168 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/148.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3849 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/149.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      624 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/150.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      373 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/151.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      302 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/152.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      462 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/153.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1546 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/154.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1044 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/155.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      875 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/156.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2606 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/157.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3118 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/158.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      727 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/159.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1353 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/160.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      548 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/161.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2099 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/162.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1202 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/163.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      304 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/164.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      430 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/165.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      306 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/166.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      591 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/167.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1403 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/168.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1812 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/169.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      614 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/170.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      758 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/171.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      873 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/172.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      561 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/173.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      324 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/174.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1294 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/175.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      886 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/176.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      256 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/177.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      256 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/178.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6715 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/179.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3159 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/180.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      661 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/181.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2782 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/182.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1715 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/183.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      910 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/184.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1091 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/185.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/186.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1601 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/187.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1045 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/188.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      616 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/189.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1105 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/190.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1751 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/191.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      162 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/192.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1731 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/sql/upgrades/193.sql
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.965009 swh_storage-2.4.0/swh/storage/tests/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.965009 swh_storage-2.4.0/swh/storage/tests/algos/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/algos/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12969 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/algos/test_diff.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5545 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/algos/test_dir_iterator.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7293 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/algos/test_directory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2284 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/algos/test_discovery.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    11595 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/algos/test_origin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    18297 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/algos/test_revisions_walker.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    13956 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/algos/test_snapshot.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.965009 swh_storage-2.4.0/swh/storage/tests/blocking/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/blocking/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1094 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/blocking/conftest.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    18586 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/blocking/test_cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     9375 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/blocking/test_db.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    21189 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/blocking/test_proxy.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2801 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/blocking/test_proxy_blocking.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1074 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/blocking/test_proxy_no_blocking.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2790 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.965009 swh_storage-2.4.0/swh/storage/tests/data/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      189 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/data/storage.yml
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.969009 swh_storage-2.4.0/swh/storage/tests/masking/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/masking/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1076 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/masking/conftest.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    19842 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/masking/test_cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10967 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/masking/test_db.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    30500 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/masking/test_proxy.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5872 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/masking/test_proxy_masking.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      960 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/masking/test_proxy_no_masking.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.969009 swh_storage-2.4.0/swh/storage/tests/migrate_extrinsic_metadata/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    11035 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/migrate_extrinsic_metadata/test_cran.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    20328 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/migrate_extrinsic_metadata/test_debian.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    52095 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/migrate_extrinsic_metadata/test_deposit.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3702 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/migrate_extrinsic_metadata/test_gnu.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4246 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/migrate_extrinsic_metadata/test_nixguix.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    15543 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/migrate_extrinsic_metadata/test_npm.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    25053 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/migrate_extrinsic_metadata/test_pypi.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    27741 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/storage_data.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)   235382 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/storage_tests.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6103 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_api_client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    14820 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_backfill.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    24799 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_buffer.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    29473 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_cassandra.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5495 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_cassandra_converters.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12438 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_cassandra_migration.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    13326 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1887 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_counter.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2360 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_exception.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5260 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_filter.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4188 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_in_memory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8745 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_init.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4944 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_kafka_writer.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4698 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_metrics.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    20071 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_postgresql.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12253 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_postgresql_converters.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1399 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_postgresql_flavor_mirror.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1423 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_postgresql_flavor_readreplica.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      669 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8582 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_record_references.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    23199 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_replay.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8212 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_retry.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1589 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_revision_bw_compat.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1346 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_serializers.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3323 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_server.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1186 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_storage_data.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    14141 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_tenacious.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4755 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_utils.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4515 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/tests/test_validate.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3700 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/utils.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4030 2024-05-23 13:05:35.000000 swh_storage-2.4.0/swh/storage/writer.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-23 13:05:40.969009 swh_storage-2.4.0/swh.storage.egg-info/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8493 2024-05-23 13:05:40.000000 swh_storage-2.4.0/swh.storage.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12124 2024-05-23 13:05:40.000000 swh_storage-2.4.0/swh.storage.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-05-23 13:05:40.000000 swh_storage-2.4.0/swh.storage.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1007 2024-05-23 13:05:40.000000 swh_storage-2.4.0/swh.storage.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      488 2024-05-23 13:05:40.000000 swh_storage-2.4.0/swh.storage.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-05-23 13:05:40.000000 swh_storage-2.4.0/swh.storage.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1264 2024-05-23 13:05:35.000000 swh_storage-2.4.0/tox.ini
```

### Comparing `swh_storage-2.3.1/.pre-commit-config.yaml` & `swh_storage-2.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/CODE_OF_CONDUCT.md` & `swh_storage-2.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/LICENSE` & `swh_storage-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/PKG-INFO` & `swh_storage-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.storage
-Version: 2.3.1
+Version: 2.4.0
 Summary: Software Heritage storage manager
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-storage
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-storage/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-storage/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-storage.git
@@ -25,22 +25,22 @@
 Requires-Dist: mypy_extensions
 Requires-Dist: psycopg2
 Requires-Dist: redis
 Requires-Dist: tenacity!=8.2.0,>=6.2
 Requires-Dist: typing-extensions
 Requires-Dist: swh.core[db,http]>=3.0.0
 Requires-Dist: swh.counters>=v0.8.0
-Requires-Dist: swh.model>=6.11.0
+Requires-Dist: swh.model>=6.13.0
 Requires-Dist: swh.objstorage>=2.2.0
 Provides-Extra: testing
 Requires-Dist: hypothesis>=3.11.0; extra == "testing"
 Requires-Dist: pytest>=8.1; extra == "testing"
 Requires-Dist: pytest-mock; extra == "testing"
 Requires-Dist: swh.core[testing]>=3.0.0; extra == "testing"
-Requires-Dist: swh.model[testing]>=0.0.50; extra == "testing"
+Requires-Dist: swh.model[testing]>=6.13.0; extra == "testing"
 Requires-Dist: pytz; extra == "testing"
 Requires-Dist: pytest-redis; extra == "testing"
 Requires-Dist: pytest-xdist; extra == "testing"
 Requires-Dist: types-python-dateutil; extra == "testing"
 Requires-Dist: types-pytz; extra == "testing"
 Requires-Dist: types-pyyaml; extra == "testing"
 Requires-Dist: types-redis; extra == "testing"
```

### Comparing `swh_storage-2.3.1/README.rst` & `swh_storage-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/bin/swh-storage-add-dir` & `swh_storage-2.4.0/bin/swh-storage-add-dir`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/docs/Makefile.local` & `swh_storage-2.4.0/docs/Makefile.local`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/docs/archive-copies.rst` & `swh_storage-2.4.0/docs/archive-copies.rst`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/docs/extrinsic-metadata-specification.rst` & `swh_storage-2.4.0/docs/extrinsic-metadata-specification.rst`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/docs/images/swh-archive-copies.dia` & `swh_storage-2.4.0/docs/images/swh-archive-copies.dia`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/docs/index.rst` & `swh_storage-2.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/docs/object-masking.rst` & `swh_storage-2.4.0/docs/object-masking.rst`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/mypy.ini` & `swh_storage-2.4.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/pyproject.toml` & `swh_storage-2.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -38,18 +38,20 @@
 "counter" = "swh.storage.proxies.counter:CountingProxyStorage"
 "filter" = "swh.storage.proxies.filter:FilteringProxyStorage"
 "retry" = "swh.storage.proxies.retry:RetryingProxyStorage"
 "tenacious" = "swh.storage.proxies.tenacious:TenaciousProxyStorage"
 "validate" = "swh.storage.proxies.validate:ValidatingProxyStorage"
 "record_references" = "swh.storage.proxies.record_references:RecordReferencesProxyStorage"
 "masking" = "swh.storage.proxies.masking:MaskingProxyStorage"
+"blocking" = "swh.storage.proxies.blocking:BlockingProxyStorage"
 
 [project.entry-points."swh.cli.subcommands"]
 "swh.storage" = "swh.storage.cli"
 "swh.storage.proxies.masking" = "swh.storage.proxies.masking.cli"
+"swh.storage.proxies.blocking" = "swh.storage.proxies.blocking.cli"
 
 [project.urls]
 "Homepage" = "https://gitlab.softwareheritage.org/swh/devel/swh-storage"
 "Bug Reports" = "https://gitlab.softwareheritage.org/swh/devel/swh-storage/-/issues"
 "Funding" = "https://www.softwareheritage.org/donate"
 "Documentation" = "https://docs.softwareheritage.org/devel/swh-storage/"
 "Source" = "https://gitlab.softwareheritage.org/swh/devel/swh-storage.git"
```

### Comparing `swh_storage-2.3.1/sql/Makefile` & `swh_storage-2.4.0/sql/Makefile`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/sql/TODO` & `swh_storage-2.4.0/sql/TODO`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/sql/bin/db-upgrade` & `swh_storage-2.4.0/sql/bin/db-upgrade`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/sql/bin/dot_add_content` & `swh_storage-2.4.0/sql/bin/dot_add_content`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/sql/clusters.dot` & `swh_storage-2.4.0/sql/clusters.dot`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/sql/json/fetch_history.result.schema.json` & `swh_storage-2.4.0/sql/json/fetch_history.result.schema.json`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/sql/json/origin_visit.metadata.json` & `swh_storage-2.4.0/sql/json/origin_visit.metadata.json`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/__init__.py` & `swh_storage-2.4.0/swh/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/algos/diff.py` & `swh_storage-2.4.0/swh/storage/algos/diff.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/algos/dir_iterators.py` & `swh_storage-2.4.0/swh/storage/algos/dir_iterators.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/algos/directory.py` & `swh_storage-2.4.0/swh/storage/algos/directory.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/algos/discovery.py` & `swh_storage-2.4.0/swh/storage/algos/discovery.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/algos/origin.py` & `swh_storage-2.4.0/swh/storage/algos/origin.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/algos/revisions_walker.py` & `swh_storage-2.4.0/swh/storage/algos/revisions_walker.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/algos/snapshot.py` & `swh_storage-2.4.0/swh/storage/algos/snapshot.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from swh.model.hashutil import hash_to_hex
 from swh.model.model import (
     OriginVisit,
     OriginVisitStatus,
     Sha1Git,
     Snapshot,
     SnapshotBranch,
-    TargetType,
+    SnapshotTargetType,
 )
 from swh.storage.algos.origin import (
     iter_origin_visit_statuses,
     iter_origin_visits,
     origin_get_latest_visit_status,
 )
 from swh.storage.interface import ListOrder, StorageInterface
@@ -156,15 +156,15 @@
 
             snapshot = snapshot_get_all_branches(storage, snapshot_id)
             if not snapshot:
                 continue
             for branch_name, branch in snapshot.branches.items():
                 if (
                     branch is not None
-                    and branch.target_type == TargetType.REVISION
+                    and branch.target_type == SnapshotTargetType.REVISION
                     and branch.target == revision_id
                 ):  # snapshot found
                     yield (visit, visit_status, snapshot)
 
 
 def snapshot_resolve_alias(
     storage: StorageInterface, snapshot_id: Sha1Git, alias_name: bytes
```

### Comparing `swh_storage-2.3.1/swh/storage/api/client.py` & `swh_storage-2.4.0/swh/storage/api/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -51,16 +51,15 @@
                 # XXX: workaround until we fix these HashCollisions happening
                 # when they shouldn't
                 raise HashCollision(*e.args[0]["args"])
             else:
                 raise
 
     def content_add(self, content: List[Content]) -> Dict[str, int]:
-        content = [c.with_data() if isinstance(c, Content) else c for c in content]
-        return self._post("content/add", {"content": content})
+        return self._post("content/add", {"content": [c.with_data() for c in content]})
 
     def reset(self):
         return self._post("reset", {})
 
     def stat_counters(self):
         return self.get("stat/counters")
```

### Comparing `swh_storage-2.3.1/swh/storage/api/serializers.py` & `swh_storage-2.4.0/swh/storage/api/serializers.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/api/server.py` & `swh_storage-2.4.0/swh/storage/api/server.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/backfill.py` & `swh_storage-2.4.0/swh/storage/backfill.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     DirectoryEntry,
     ExtID,
     RawExtrinsicMetadata,
     Release,
     Revision,
     Snapshot,
     SnapshotBranch,
-    TargetType,
+    SnapshotTargetType,
 )
 from swh.model.swhids import ExtendedObjectType
 from swh.storage.postgresql.converters import (
     db_to_extid,
     db_to_raw_extrinsic_metadata,
     db_to_release,
     db_to_revision,
@@ -284,15 +284,15 @@
         cur.execute(query, (snapshot_d["object_id"],))
         branches = {}
         for name, *row in cur:
             branch_d = dict(zip(columns[1:], row))
             if branch_d["target"] is not None and branch_d["target_type"] is not None:
                 branch: Optional[SnapshotBranch] = SnapshotBranch(
                     target=branch_d["target"],
-                    target_type=TargetType(branch_d["target_type"]),
+                    target_type=SnapshotTargetType(branch_d["target_type"]),
                 )
             else:
                 branch = None
             branches[name] = branch
 
     return Snapshot(
         id=snapshot_d["id"],
```

### Comparing `swh_storage-2.3.1/swh/storage/cassandra/common.py` & `swh_storage-2.4.0/swh/storage/cassandra/common.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/cassandra/converters.py` & `swh_storage-2.4.0/swh/storage/cassandra/converters.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/cassandra/cql.py` & `swh_storage-2.4.0/swh/storage/cassandra/cql.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/cassandra/model.py` & `swh_storage-2.4.0/swh/storage/cassandra/model.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/cassandra/schema.py` & `swh_storage-2.4.0/swh/storage/cassandra/schema.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/cassandra/storage.py` & `swh_storage-2.4.0/swh/storage/cassandra/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     RawExtrinsicMetadata,
     Release,
     Revision,
     Sha1Git,
     SkippedContent,
     Snapshot,
     SnapshotBranch,
-    TargetType,
+    SnapshotTargetType,
 )
 from swh.model.swhids import CoreSWHID, ExtendedObjectType, ExtendedSWHID
 from swh.model.swhids import ObjectType as SwhidObjectType
 from swh.storage.interface import (
     VISIT_STATUSES,
     HashDict,
     ListOrder,
@@ -1168,15 +1168,16 @@
         return PartialBranches(
             id=snapshot_id,
             branches={
                 branch.name: (
                     None
                     if branch.target is None
                     else SnapshotBranch(
-                        target=branch.target, target_type=TargetType(branch.target_type)
+                        target=branch.target,
+                        target_type=SnapshotTargetType(branch.target_type),
                     )
                 )
                 for branch in branches
             },
             next_branch=last_branch,
         )
 
@@ -1204,20 +1205,23 @@
             )
             if len(branches) != 1 or branches[0].name != branch_name:
                 # target branch is None, there could be items in aliases_followed
                 target = None
                 break
             branch = branches[0]
             resolve_chain.append(branch_name)
-            if branch.target_type != TargetType.ALIAS.value or not follow_alias_chain:
+            if (
+                branch.target_type != SnapshotTargetType.ALIAS.value
+                or not follow_alias_chain
+            ):
                 # first non alias branch or the first branch when follow_alias_chain is False
                 target = (
                     SnapshotBranch(
                         target=branch.target,
-                        target_type=TargetType(branch.target_type),
+                        target_type=SnapshotTargetType(branch.target_type),
                     )
                     if branch.target
                     else None
                 )
                 break
             elif (
                 # Circular reference
```

### Comparing `swh_storage-2.3.1/swh/storage/cli.py` & `swh_storage-2.4.0/swh/storage/cli.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/exc.py` & `swh_storage-2.4.0/swh/storage/proxies/validate.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,105 +1,71 @@
-# Copyright (C) 2015-2020  The Software Heritage developers
+# Copyright (C) 2020 The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
-from typing import TYPE_CHECKING, Dict, List
 
-from swh.model.hashutil import hash_to_hex
-from swh.storage.utils import content_bytes_hashes, content_hex_hashes
+from typing import Dict, Iterable, List
 
-if TYPE_CHECKING:
-    from swh.model.swhids import ExtendedSWHID
-    from swh.storage.proxies.masking.db import MaskedStatus
-
-
-class StorageDBError(Exception):
-    """Specific storage db error (connection, erroneous queries, etc...)"""
-
-    def __str__(self):
-        return "An unexpected error occurred in the backend: %s" % (self.args,)
-
-
-class StorageAPIError(Exception):
-    """Specific internal storage api (mainly connection)"""
-
-    def __str__(self):
-        args = self.args
-        return "An unexpected error occurred in the api backend: %s" % (args,)
-
-
-class NonRetryableException(Exception):
-    """Persistent storage exceptions for which clients should not issue automatic
-    retries"""
-
-    pass
-
-
-class StorageArgumentException(NonRetryableException):
-    """Argument passed to a Storage endpoint is invalid."""
-
-    pass
-
-
-class QueryTimeout(StorageAPIError):
-    """Raised when a query to the backend (Cassandra or PostgreSQL) took too long."""
-
-    pass
-
-
-class UnknownMetadataAuthority(StorageArgumentException):
-    """Raised when ``raw_extrinsic_metadata_add`` is called with a non-existing
-    metadata authority as argument."""
-
-    pass
-
-
-class UnknownMetadataFetcher(StorageArgumentException):
-    """Raised when ``raw_extrinsic_metadata_add`` is called with a non-existing
-    metadata fetcher as argument."""
-
-    pass
-
-
-class MaskedObjectException(NonRetryableException):
-    """Raised when the masking proxy attempts to return a masked object"""
-
-    def __init__(self, masked: "Dict[ExtendedSWHID, List[MaskedStatus]]"):
-        if not masked:
-            raise ValueError(
-                "Can't raise a MaskedObjectException if no objects are masked"
-            )
-        for swhid, statuses in masked.items():
-            if not statuses:
-                raise ValueError(f"MaskedObjectException has no statuses for {swhid}")
-
-        self.masked = masked
-
-        super().__init__(masked)
-
-    @staticmethod
-    def _str_one_masked(obj, statuses):
-        status = statuses[0]
-        return f"{obj} by request {status.request} ({status.state.name})" + (
-            " and others" if len(statuses) > 1 else ""
-        )
-
-    def __str__(self):
-        return "Some objects are masked: %s" % ", ".join(
-            self._str_one_masked(obj, statuses)
-            for obj, statuses in self.masked.items()
-            if statuses
-        )
-
-
-class HashCollision(Exception):
-    """Exception raised when a content collides in a storage backend"""
-
-    def __init__(self, algo, hash_id, colliding_contents):
-        self.algo = algo
-        self.hash_id = hash_to_hex(hash_id)
-        self.colliding_contents = [content_hex_hashes(c) for c in colliding_contents]
-        super().__init__(self.algo, self.hash_id, self.colliding_contents)
-
-    def colliding_content_hashes(self) -> List[Dict[str, bytes]]:
-        return [content_bytes_hashes(c) for c in self.colliding_contents]
+from swh.model.hashutil import MultiHash, hash_to_bytes, hash_to_hex
+from swh.model.model import Content, Directory, Release, Revision, Snapshot
+from swh.storage import get_storage
+from swh.storage.exc import StorageArgumentException
+from swh.storage.interface import StorageInterface
+
+
+class ValidatingProxyStorage:
+    """Proxy for storage classes, which checks inserted objects have a correct hash.
+
+    Sample configuration use case for filtering storage:
+
+    .. code-block: yaml
+
+        storage:
+          cls: validate
+          storage:
+            cls: remote
+            url: http://storage.internal.staging.swh.network:5002/
+
+    """
+
+    def __init__(self, storage):
+        self.storage: StorageInterface = get_storage(**storage)
+
+    def __getattr__(self, key):
+        if key == "storage":
+            raise AttributeError(key)
+        return getattr(self.storage, key)
+
+    def _check_hashes(self, objects: Iterable):
+        for obj in objects:
+            id_ = hash_to_bytes(obj.compute_hash())
+            if id_ != obj.id:
+                raise StorageArgumentException(
+                    f"Object has id {hash_to_hex(obj.id)}, "
+                    f"but it should be {hash_to_hex(id_)}: {obj}"
+                )
+
+    def content_add(self, content: List[Content]) -> Dict[str, int]:
+        for cont in content:
+            hashes = MultiHash.from_data(cont.data).digest()
+            if hashes != cont.hashes():
+                raise StorageArgumentException(
+                    f"Object has hashes {cont.hashes()}, but they should be {hashes}"
+                )
+        return self.storage.content_add(content)
+
+    def directory_add(self, directories: List[Directory]) -> Dict[str, int]:
+        self._check_hashes(directories)
+        return self.storage.directory_add(directories)
+
+    def revision_add(self, revisions: List[Revision]) -> Dict[str, int]:
+        self._check_hashes(revisions)
+        return self.storage.revision_add(revisions)
+
+    def release_add(self, releases: List[Release]) -> Dict[str, int]:
+        self._check_hashes(releases)
+        return self.storage.release_add(releases)
+
+    def snapshot_add(self, snapshots: List[Snapshot]) -> Dict[str, int]:
+        self._check_hashes(snapshots)
+        return self.storage.snapshot_add(snapshots)
```

### Comparing `swh_storage-2.3.1/swh/storage/fixer.py` & `swh_storage-2.4.0/swh/storage/fixer.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/in_memory.py` & `swh_storage-2.4.0/swh/storage/in_memory.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/interface.py` & `swh_storage-2.4.0/swh/storage/interface.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/metrics.py` & `swh_storage-2.4.0/swh/storage/metrics.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/migrate_extrinsic_metadata.py` & `swh_storage-2.4.0/swh/storage/migrate_extrinsic_metadata.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/objstorage.py` & `swh_storage-2.4.0/swh/storage/objstorage.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/postgresql/converters.py` & `swh_storage-2.4.0/swh/storage/postgresql/converters.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/postgresql/db.py` & `swh_storage-2.4.0/swh/storage/postgresql/db.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/postgresql/storage.py` & `swh_storage-2.4.0/swh/storage/postgresql/storage.py`

 * *Files identical despite different names*

```diff
@@ -81,4289 +81,4291 @@
 00000500: 7369 634d 6574 6164 6174 612c 0a20 2020  sicMetadata,.   
 00000510: 2052 656c 6561 7365 2c0a 2020 2020 5265   Release,.    Re
 00000520: 7669 7369 6f6e 2c0a 2020 2020 5368 6131  vision,.    Sha1
 00000530: 2c0a 2020 2020 5368 6131 4769 742c 0a20  ,.    Sha1Git,. 
 00000540: 2020 2053 6b69 7070 6564 436f 6e74 656e     SkippedConten
 00000550: 742c 0a20 2020 2053 6e61 7073 686f 742c  t,.    Snapshot,
 00000560: 0a20 2020 2053 6e61 7073 686f 7442 7261  .    SnapshotBra
-00000570: 6e63 682c 0a20 2020 2054 6172 6765 7454  nch,.    TargetT
-00000580: 7970 652c 0a29 0a66 726f 6d20 7377 682e  ype,.).from swh.
-00000590: 6d6f 6465 6c2e 7377 6869 6473 2069 6d70  model.swhids imp
-000005a0: 6f72 7420 4578 7465 6e64 6564 4f62 6a65  ort ExtendedObje
-000005b0: 6374 5479 7065 2c20 4578 7465 6e64 6564  ctType, Extended
-000005c0: 5357 4849 442c 204f 626a 6563 7454 7970  SWHID, ObjectTyp
-000005d0: 650a 6672 6f6d 2073 7768 2e73 746f 7261  e.from swh.stora
-000005e0: 6765 2e65 7863 2069 6d70 6f72 7420 280a  ge.exc import (.
-000005f0: 2020 2020 4861 7368 436f 6c6c 6973 696f      HashCollisio
-00000600: 6e2c 0a20 2020 2051 7565 7279 5469 6d65  n,.    QueryTime
-00000610: 6f75 742c 0a20 2020 2053 746f 7261 6765  out,.    Storage
-00000620: 4172 6775 6d65 6e74 4578 6365 7074 696f  ArgumentExceptio
-00000630: 6e2c 0a20 2020 2053 746f 7261 6765 4442  n,.    StorageDB
-00000640: 4572 726f 722c 0a20 2020 2055 6e6b 6e6f  Error,.    Unkno
-00000650: 776e 4d65 7461 6461 7461 4175 7468 6f72  wnMetadataAuthor
-00000660: 6974 792c 0a20 2020 2055 6e6b 6e6f 776e  ity,.    Unknown
-00000670: 4d65 7461 6461 7461 4665 7463 6865 722c  MetadataFetcher,
-00000680: 0a29 0a66 726f 6d20 7377 682e 7374 6f72  .).from swh.stor
-00000690: 6167 652e 696e 7465 7266 6163 6520 696d  age.interface im
-000006a0: 706f 7274 2028 0a20 2020 2056 4953 4954  port (.    VISIT
-000006b0: 5f53 5441 5455 5345 532c 0a20 2020 2048  _STATUSES,.    H
-000006c0: 6173 6844 6963 742c 0a20 2020 204c 6973  ashDict,.    Lis
-000006d0: 744f 7264 6572 2c0a 2020 2020 4f62 6a65  tOrder,.    Obje
-000006e0: 6374 5265 6665 7265 6e63 652c 0a20 2020  ctReference,.   
-000006f0: 204f 7269 6769 6e56 6973 6974 5769 7468   OriginVisitWith
-00000700: 5374 6174 7573 6573 2c0a 2020 2020 5061  Statuses,.    Pa
-00000710: 6765 6452 6573 756c 742c 0a20 2020 2050  gedResult,.    P
-00000720: 6172 7469 616c 4272 616e 6368 6573 2c0a  artialBranches,.
-00000730: 2020 2020 536e 6170 7368 6f74 4272 616e      SnapshotBran
-00000740: 6368 4279 4e61 6d65 5265 7370 6f6e 7365  chByNameResponse
-00000750: 2c0a 290a 6672 6f6d 2073 7768 2e73 746f  ,.).from swh.sto
-00000760: 7261 6765 2e6f 626a 7374 6f72 6167 6520  rage.objstorage 
-00000770: 696d 706f 7274 204f 626a 5374 6f72 6167  import ObjStorag
-00000780: 650a 6672 6f6d 2073 7768 2e73 746f 7261  e.from swh.stora
-00000790: 6765 2e75 7469 6c73 2069 6d70 6f72 7420  ge.utils import 
-000007a0: 280a 2020 2020 6578 7472 6163 745f 636f  (.    extract_co
-000007b0: 6c6c 6973 696f 6e5f 6861 7368 2c0a 2020  llision_hash,.  
-000007c0: 2020 6765 745f 7061 7274 6974 696f 6e5f    get_partition_
-000007d0: 626f 756e 6473 5f62 7974 6573 2c0a 2020  bounds_bytes,.  
-000007e0: 2020 6d61 705f 6f70 7469 6f6e 616c 2c0a    map_optional,.
-000007f0: 2020 2020 6e6f 772c 0a29 0a66 726f 6d20      now,.).from 
-00000800: 7377 682e 7374 6f72 6167 652e 7772 6974  swh.storage.writ
-00000810: 6572 2069 6d70 6f72 7420 4a6f 7572 6e61  er import Journa
-00000820: 6c57 7269 7465 720a 0a66 726f 6d20 2e20  lWriter..from . 
-00000830: 696d 706f 7274 2063 6f6e 7665 7274 6572  import converter
-00000840: 730a 6672 6f6d 202e 6462 2069 6d70 6f72  s.from .db impor
-00000850: 7420 4462 0a0a 6c6f 6767 6572 203d 206c  t Db..logger = l
-00000860: 6f67 6769 6e67 2e67 6574 4c6f 6767 6572  ogging.getLogger
-00000870: 285f 5f6e 616d 655f 5f29 0a0a 2320 4d61  (__name__)..# Ma
-00000880: 7820 626c 6f63 6b20 7369 7a65 206f 6620  x block size of 
-00000890: 636f 6e74 656e 7473 2074 6f20 7265 7475  contents to retu
-000008a0: 726e 0a42 554c 4b5f 424c 4f43 4b5f 434f  rn.BULK_BLOCK_CO
-000008b0: 4e54 454e 545f 4c45 4e5f 4d41 5820 3d20  NTENT_LEN_MAX = 
-000008c0: 3130 3030 300a 0a45 4d50 5459 5f53 4e41  10000..EMPTY_SNA
-000008d0: 5053 484f 545f 4944 203d 2068 6173 685f  PSHOT_ID = hash_
-000008e0: 746f 5f62 7974 6573 2822 3161 3838 3933  to_bytes("1a8893
-000008f0: 6536 6138 3666 3434 3465 3862 6538 6537  e6a86f444e8be8e7
-00000900: 6264 6136 6362 3334 6662 3137 3335 6130  bda6cb34fb1735a0
-00000910: 3065 2229 0a22 2222 4964 656e 7469 6669  0e")."""Identifi
-00000920: 6572 2066 6f72 2074 6865 2065 6d70 7479  er for the empty
-00000930: 2073 6e61 7073 686f 7422 2222 0a0a 0a56   snapshot"""...V
-00000940: 414c 4944 4154 494f 4e5f 4558 4345 5054  ALIDATION_EXCEPT
-00000950: 494f 4e53 203d 2028 0a20 2020 204b 6579  IONS = (.    Key
-00000960: 4572 726f 722c 0a20 2020 2054 7970 6545  Error,.    TypeE
-00000970: 7272 6f72 2c0a 2020 2020 5661 6c75 6545  rror,.    ValueE
-00000980: 7272 6f72 2c0a 2020 2020 7073 7963 6f70  rror,.    psycop
-00000990: 6732 2e65 7272 6f72 732e 4368 6563 6b56  g2.errors.CheckV
-000009a0: 696f 6c61 7469 6f6e 2c0a 2020 2020 7073  iolation,.    ps
-000009b0: 7963 6f70 6732 2e65 7272 6f72 732e 496e  ycopg2.errors.In
-000009c0: 7465 6772 6974 7945 7272 6f72 2c0a 2020  tegrityError,.  
-000009d0: 2020 7073 7963 6f70 6732 2e65 7272 6f72    psycopg2.error
-000009e0: 732e 496e 7661 6c69 6454 6578 7452 6570  s.InvalidTextRep
-000009f0: 7265 7365 6e74 6174 696f 6e2c 0a20 2020  resentation,.   
-00000a00: 2070 7379 636f 7067 322e 6572 726f 7273   psycopg2.errors
-00000a10: 2e4e 6f74 4e75 6c6c 5669 6f6c 6174 696f  .NotNullViolatio
-00000a20: 6e2c 0a20 2020 2070 7379 636f 7067 322e  n,.    psycopg2.
-00000a30: 6572 726f 7273 2e4e 756d 6572 6963 5661  errors.NumericVa
-00000a40: 6c75 654f 7574 4f66 5261 6e67 652c 0a20  lueOutOfRange,. 
-00000a50: 2020 2070 7379 636f 7067 322e 6572 726f     psycopg2.erro
-00000a60: 7273 2e55 6e64 6566 696e 6564 4675 6e63  rs.UndefinedFunc
-00000a70: 7469 6f6e 2c20 2023 2028 7261 6973 6564  tion,  # (raised
-00000a80: 206f 6e20 7772 6f6e 6720 6172 6775 6d65   on wrong argume
-00000a90: 6e74 2074 7970 7329 0a20 2020 2070 7379  nt typs).    psy
-00000aa0: 636f 7067 322e 6572 726f 7273 2e50 726f  copg2.errors.Pro
-00000ab0: 6772 616d 4c69 6d69 7445 7863 6565 6465  gramLimitExceede
-00000ac0: 642c 2020 2320 7479 7069 6361 6c6c 7920  d,  # typically 
-00000ad0: 7065 7273 6f6e 5f6e 616d 655f 6964 780a  person_name_idx.
-00000ae0: 290a 2222 2245 7863 6570 7469 6f6e 7320  )."""Exceptions 
-00000af0: 7261 6973 6564 2062 7920 706f 7374 6772  raised by postgr
-00000b00: 6573 716c 2077 6865 6e20 7661 6c69 6461  esql when valida
-00000b10: 7469 6f6e 206f 6620 7468 6520 6172 6775  tion of the argu
-00000b20: 6d65 6e74 730a 6661 696c 6564 2e22 2222  ments.failed."""
-00000b30: 0a0a 0a40 636f 6e74 6578 746c 6962 2e63  ...@contextlib.c
-00000b40: 6f6e 7465 7874 6d61 6e61 6765 720a 6465  ontextmanager.de
-00000b50: 6620 636f 6e76 6572 745f 7661 6c69 6461  f convert_valida
-00000b60: 7469 6f6e 5f65 7863 6570 7469 6f6e 7328  tion_exceptions(
-00000b70: 293a 0a20 2020 2022 2222 4361 7463 6865  ):.    """Catche
-00000b80: 7320 706f 7374 6772 6573 716c 2065 7272  s postgresql err
-00000b90: 6f72 7320 7265 6c61 7465 6420 746f 2069  ors related to i
-00000ba0: 6e76 616c 6964 2061 7267 756d 656e 7473  nvalid arguments
-00000bb0: 2c20 616e 640a 2020 2020 7265 2d72 6169  , and.    re-rai
-00000bc0: 7365 7320 6120 5374 6f72 6167 6541 7267  ses a StorageArg
-00000bd0: 756d 656e 7445 7863 6570 7469 6f6e 2e22  umentException."
-00000be0: 2222 0a20 2020 2074 7279 3a0a 2020 2020  "".    try:.    
-00000bf0: 2020 2020 7969 656c 640a 2020 2020 6578      yield.    ex
-00000c00: 6365 7074 2070 7379 636f 7067 322e 6572  cept psycopg2.er
-00000c10: 726f 7273 2e55 6e69 7175 6556 696f 6c61  rors.UniqueViola
-00000c20: 7469 6f6e 3a0a 2020 2020 2020 2020 2320  tion:.        # 
-00000c30: 5468 6973 206f 6e6c 7920 6861 7070 656e  This only happen
-00000c40: 7320 6265 6361 7573 6520 6f66 2063 6f6e  s because of con
-00000c50: 6375 7272 656e 7420 696e 7365 7274 696f  current insertio
-00000c60: 6e73 2c20 6275 7420 6974 2069 730a 2020  ns, but it is.  
-00000c70: 2020 2020 2020 2320 6120 7375 6263 6c61        # a subcla
-00000c80: 7373 206f 6620 496e 7465 6772 6974 7945  ss of IntegrityE
-00000c90: 7272 6f72 3b20 736f 2077 6520 6e65 6564  rror; so we need
-00000ca0: 2074 6f20 6361 7463 6820 616e 6420 7265   to catch and re
-00000cb0: 7261 6973 6520 6974 0a20 2020 2020 2020  raise it.       
-00000cc0: 2023 2062 6566 6f72 6520 7468 6520 6e65   # before the ne
-00000cd0: 7874 2063 6c61 7573 6520 636f 6e76 6572  xt clause conver
-00000ce0: 7473 2069 7420 746f 2053 746f 7261 6765  ts it to Storage
-00000cf0: 4172 6775 6d65 6e74 4578 6365 7074 696f  ArgumentExceptio
-00000d00: 6e2e 0a20 2020 2020 2020 2072 6169 7365  n..        raise
-00000d10: 0a20 2020 2065 7863 6570 7420 5641 4c49  .    except VALI
-00000d20: 4441 5449 4f4e 5f45 5843 4550 5449 4f4e  DATION_EXCEPTION
-00000d30: 5320 6173 2065 3a0a 2020 2020 2020 2020  S as e:.        
-00000d40: 7261 6973 6520 5374 6f72 6167 6541 7267  raise StorageArg
-00000d50: 756d 656e 7445 7863 6570 7469 6f6e 2873  umentException(s
-00000d60: 7472 2865 2929 0a0a 0a64 6566 2064 625f  tr(e))...def db_
-00000d70: 7472 616e 7361 6374 696f 6e5f 6765 6e65  transaction_gene
-00000d80: 7261 746f 7228 2a61 7267 732c 202a 2a6b  rator(*args, **k
-00000d90: 7761 7267 7329 3a0a 2020 2020 6465 6620  wargs):.    def 
-00000da0: 6465 636f 7261 746f 7228 6d65 7468 293a  decorator(meth):
-00000db0: 0a20 2020 2020 2020 206d 6574 6820 3d20  .        meth = 
-00000dc0: 5f64 625f 7472 616e 7361 6374 696f 6e5f  _db_transaction_
-00000dd0: 6765 6e65 7261 746f 7228 2a61 7267 732c  generator(*args,
-00000de0: 202a 2a6b 7761 7267 7329 286d 6574 6829   **kwargs)(meth)
-00000df0: 0a0a 2020 2020 2020 2020 4066 756e 6374  ..        @funct
-00000e00: 6f6f 6c73 2e77 7261 7073 286d 6574 6829  ools.wraps(meth)
-00000e10: 0a20 2020 2020 2020 2064 6566 205f 6d65  .        def _me
-00000e20: 7468 2873 656c 662c 202a 6172 6773 2c20  th(self, *args, 
-00000e30: 2a2a 6b77 6172 6773 293a 0a20 2020 2020  **kwargs):.     
-00000e40: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-00000e50: 2020 2020 2020 2020 2020 2020 7969 656c              yiel
-00000e60: 6420 6672 6f6d 206d 6574 6828 7365 6c66  d from meth(self
-00000e70: 2c20 2a61 7267 732c 202a 2a6b 7761 7267  , *args, **kwarg
-00000e80: 7329 0a20 2020 2020 2020 2020 2020 2065  s).            e
-00000e90: 7863 6570 7420 7073 7963 6f70 6732 2e65  xcept psycopg2.e
-00000ea0: 7272 6f72 732e 5175 6572 7943 616e 6365  rrors.QueryCance
-00000eb0: 6c65 6420 6173 2065 3a0a 2020 2020 2020  led as e:.      
-00000ec0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00000ed0: 5175 6572 7954 696d 656f 7574 282a 652e  QueryTimeout(*e.
-00000ee0: 6172 6773 290a 0a20 2020 2020 2020 2072  args)..        r
-00000ef0: 6574 7572 6e20 5f6d 6574 680a 0a20 2020  eturn _meth..   
-00000f00: 2072 6574 7572 6e20 6465 636f 7261 746f   return decorato
-00000f10: 720a 0a0a 6465 6620 6462 5f74 7261 6e73  r...def db_trans
-00000f20: 6163 7469 6f6e 282a 6172 6773 2c20 2a2a  action(*args, **
-00000f30: 6b77 6172 6773 293a 0a20 2020 2064 6566  kwargs):.    def
-00000f40: 2064 6563 6f72 6174 6f72 286d 6574 6829   decorator(meth)
-00000f50: 3a0a 2020 2020 2020 2020 6d65 7468 203d  :.        meth =
-00000f60: 205f 6462 5f74 7261 6e73 6163 7469 6f6e   _db_transaction
-00000f70: 282a 6172 6773 2c20 2a2a 6b77 6172 6773  (*args, **kwargs
-00000f80: 2928 6d65 7468 290a 0a20 2020 2020 2020  )(meth)..       
-00000f90: 2040 6675 6e63 746f 6f6c 732e 7772 6170   @functools.wrap
-00000fa0: 7328 6d65 7468 290a 2020 2020 2020 2020  s(meth).        
-00000fb0: 6465 6620 5f6d 6574 6828 7365 6c66 2c20  def _meth(self, 
-00000fc0: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
-00000fd0: 3a0a 2020 2020 2020 2020 2020 2020 7472  :.            tr
-00000fe0: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-00000ff0: 2020 2072 6574 7572 6e20 6d65 7468 2873     return meth(s
-00001000: 656c 662c 202a 6172 6773 2c20 2a2a 6b77  elf, *args, **kw
-00001010: 6172 6773 290a 2020 2020 2020 2020 2020  args).          
-00001020: 2020 6578 6365 7074 2070 7379 636f 7067    except psycopg
-00001030: 322e 6572 726f 7273 2e51 7565 7279 4361  2.errors.QueryCa
-00001040: 6e63 656c 6564 2061 7320 653a 0a20 2020  nceled as e:.   
-00001050: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-00001060: 7365 2051 7565 7279 5469 6d65 6f75 7428  se QueryTimeout(
-00001070: 2a65 2e61 7267 7329 0a0a 2020 2020 2020  *e.args)..      
-00001080: 2020 7265 7475 726e 205f 6d65 7468 0a0a    return _meth..
-00001090: 2020 2020 7265 7475 726e 2064 6563 6f72      return decor
-000010a0: 6174 6f72 0a0a 0a54 526f 7720 3d20 5479  ator...TRow = Ty
-000010b0: 7065 5661 7228 2254 526f 7722 2c20 626f  peVar("TRow", bo
-000010c0: 756e 643d 5475 706c 6529 0a54 5265 7375  und=Tuple).TResu
-000010d0: 6c74 203d 2054 7970 6556 6172 2822 5452  lt = TypeVar("TR
-000010e0: 6573 756c 7422 290a 0a0a 6465 6620 5f67  esult")...def _g
-000010f0: 6574 5f70 6167 696e 6174 6564 5f73 6861  et_paginated_sha
-00001100: 315f 7061 7274 6974 696f 6e28 0a20 2020  1_partition(.   
-00001110: 2063 7572 2c0a 2020 2020 7061 7274 6974   cur,.    partit
-00001120: 696f 6e5f 6964 3a20 696e 742c 0a20 2020  ion_id: int,.   
-00001130: 206e 625f 7061 7274 6974 696f 6e73 3a20   nb_partitions: 
-00001140: 696e 742c 0a20 2020 2070 6167 655f 746f  int,.    page_to
-00001150: 6b65 6e3a 204f 7074 696f 6e61 6c5b 7374  ken: Optional[st
-00001160: 725d 2c0a 2020 2020 6c69 6d69 743a 2069  r],.    limit: i
-00001170: 6e74 2c0a 2020 2020 6765 745f 7261 6e67  nt,.    get_rang
-00001180: 653a 2043 616c 6c61 626c 655b 5b62 7974  e: Callable[[byt
-00001190: 6573 2c20 6279 7465 732c 2069 6e74 2c20  es, bytes, int, 
-000011a0: 416e 795d 2c20 4974 6572 6174 6f72 5b54  Any], Iterator[T
-000011b0: 526f 775d 5d2c 0a20 2020 2063 6f6e 7665  Row]],.    conve
-000011c0: 7274 3a20 4361 6c6c 6162 6c65 5b5b 5452  rt: Callable[[TR
-000011d0: 6f77 5d2c 2054 5265 7375 6c74 5d2c 0a20  ow], TResult],. 
-000011e0: 2020 2067 6574 5f69 643a 204f 7074 696f     get_id: Optio
-000011f0: 6e61 6c5b 4361 6c6c 6162 6c65 5b5b 5452  nal[Callable[[TR
-00001200: 6573 756c 745d 2c20 416e 795d 5d20 3d20  esult], Any]] = 
-00001210: 4e6f 6e65 2c0a 2920 2d3e 2050 6167 6564  None,.) -> Paged
-00001220: 5265 7375 6c74 5b54 5265 7375 6c74 5d3a  Result[TResult]:
-00001230: 0a20 2020 2022 2222 496d 706c 656d 656e  .    """Implemen
-00001240: 7473 2074 6865 2062 756c 6b20 6f66 2060  ts the bulk of `
-00001250: 6063 6f6e 7465 6e74 5f67 6574 5f70 6172  `content_get_par
-00001260: 7469 7469 6f6e 6060 2c20 6060 6469 7265  tition``, ``dire
-00001270: 6374 6f72 795f 6765 745f 7061 7274 6974  ctory_get_partit
-00001280: 696f 6e60 602c 0a20 2020 202e 2e2e 3a0a  ion``,.    ...:.
-00001290: 0a20 2020 2031 2e20 636f 6d70 7574 6573  .    1. computes
-000012a0: 2072 616e 6765 2062 6f75 6e64 730a 2020   range bounds.  
-000012b0: 2020 322e 2061 7070 6c69 6573 2070 6167    2. applies pag
-000012c0: 696e 6174 696f 6e20 746f 6b65 6e0a 2020  ination token.  
-000012d0: 2020 332e 2063 6f6e 7665 7274 7320 746f    3. converts to
-000012e0: 2066 696e 616c 206f 626a 6563 7473 0a20   final objects. 
-000012f0: 2020 2034 2e20 6578 7472 6163 7473 206e     4. extracts n
-00001300: 6578 7420 7061 6769 6e61 7469 6f6e 2074  ext pagination t
-00001310: 6f6b 656e 0a20 2020 2022 2222 0a20 2020  oken.    """.   
-00001320: 2069 6620 6c69 6d69 7420 6973 204e 6f6e   if limit is Non
-00001330: 653a 0a20 2020 2020 2020 2072 6169 7365  e:.        raise
-00001340: 2053 746f 7261 6765 4172 6775 6d65 6e74   StorageArgument
-00001350: 4578 6365 7074 696f 6e28 226c 696d 6974  Exception("limit
-00001360: 2073 686f 756c 6420 6e6f 7420 6265 204e   should not be N
-00001370: 6f6e 6522 290a 2020 2020 6966 2067 6574  one").    if get
-00001380: 5f69 6420 6973 204e 6f6e 653a 0a0a 2020  _id is None:..  
-00001390: 2020 2020 2020 6465 6620 6765 745f 6964        def get_id
-000013a0: 286f 626a 3a20 5452 6573 756c 7429 3a0a  (obj: TResult):.
-000013b0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000013c0: 726e 206f 626a 2e69 6420 2023 2074 7970  rn obj.id  # typ
-000013d0: 653a 2069 676e 6f72 655b 6174 7472 2d64  e: ignore[attr-d
-000013e0: 6566 696e 6564 5d0a 0a20 2020 2061 7373  efined]..    ass
-000013f0: 6572 7420 6765 745f 6964 2069 7320 6e6f  ert get_id is no
-00001400: 7420 4e6f 6e65 2020 2320 746f 2070 6c65  t None  # to ple
-00001410: 6173 6520 6d79 7079 0a0a 2020 2020 2873  ase mypy..    (s
-00001420: 7461 7274 2c20 656e 6429 203d 2067 6574  tart, end) = get
-00001430: 5f70 6172 7469 7469 6f6e 5f62 6f75 6e64  _partition_bound
-00001440: 735f 6279 7465 7328 7061 7274 6974 696f  s_bytes(partitio
-00001450: 6e5f 6964 2c20 6e62 5f70 6172 7469 7469  n_id, nb_partiti
-00001460: 6f6e 732c 2053 4841 315f 5349 5a45 290a  ons, SHA1_SIZE).
-00001470: 2020 2020 6966 2070 6167 655f 746f 6b65      if page_toke
-00001480: 6e3a 0a20 2020 2020 2020 2073 7461 7274  n:.        start
-00001490: 203d 2068 6173 685f 746f 5f62 7974 6573   = hash_to_bytes
-000014a0: 2870 6167 655f 746f 6b65 6e29 0a20 2020  (page_token).   
-000014b0: 2069 6620 656e 6420 6973 204e 6f6e 653a   if end is None:
-000014c0: 0a20 2020 2020 2020 2065 6e64 203d 2062  .        end = b
-000014d0: 225c 7866 6622 202a 2053 4841 315f 5349  "\xff" * SHA1_SI
-000014e0: 5a45 0a0a 2020 2020 6e65 7874 5f70 6167  ZE..    next_pag
-000014f0: 655f 746f 6b65 6e3a 204f 7074 696f 6e61  e_token: Optiona
-00001500: 6c5b 7374 725d 203d 204e 6f6e 650a 2020  l[str] = None.  
-00001510: 2020 7265 7375 6c74 7320 3d20 5b5d 0a20    results = []. 
-00001520: 2020 2066 6f72 2063 6f75 6e74 6572 2c20     for counter, 
-00001530: 726f 7720 696e 2065 6e75 6d65 7261 7465  row in enumerate
-00001540: 2867 6574 5f72 616e 6765 2873 7461 7274  (get_range(start
-00001550: 2c20 656e 642c 206c 696d 6974 202b 2031  , end, limit + 1
-00001560: 2c20 6375 7229 293a 0a20 2020 2020 2020  , cur)):.       
-00001570: 2072 6573 756c 7420 3d20 636f 6e76 6572   result = conver
-00001580: 7428 726f 7729 0a20 2020 2020 2020 2069  t(row).        i
-00001590: 6620 636f 756e 7465 7220 3e3d 206c 696d  f counter >= lim
-000015a0: 6974 3a0a 2020 2020 2020 2020 2020 2020  it:.            
-000015b0: 2320 7461 6b65 2074 6865 206c 6173 7420  # take the last 
-000015c0: 636f 6e74 656e 7420 666f 7220 7468 6520  content for the 
-000015d0: 6e65 7874 2070 6167 6520 7374 6172 7469  next page starti
-000015e0: 6e67 2066 726f 6d20 7468 6973 0a20 2020  ng from this.   
-000015f0: 2020 2020 2020 2020 206e 6578 745f 7061           next_pa
-00001600: 6765 5f74 6f6b 656e 203d 2068 6173 685f  ge_token = hash_
-00001610: 746f 5f68 6578 2867 6574 5f69 6428 7265  to_hex(get_id(re
-00001620: 7375 6c74 2929 0a20 2020 2020 2020 2020  sult)).         
-00001630: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
-00001640: 2072 6573 756c 7473 2e61 7070 656e 6428   results.append(
-00001650: 7265 7375 6c74 290a 0a20 2020 2061 7373  result)..    ass
-00001660: 6572 7420 6c65 6e28 7265 7375 6c74 7329  ert len(results)
-00001670: 203c 3d20 6c69 6d69 740a 2020 2020 7265   <= limit.    re
-00001680: 7475 726e 2050 6167 6564 5265 7375 6c74  turn PagedResult
-00001690: 2872 6573 756c 7473 3d72 6573 756c 7473  (results=results
-000016a0: 2c20 6e65 7874 5f70 6167 655f 746f 6b65  , next_page_toke
-000016b0: 6e3d 6e65 7874 5f70 6167 655f 746f 6b65  n=next_page_toke
-000016c0: 6e29 0a0a 0a63 6c61 7373 2053 746f 7261  n)...class Stora
-000016d0: 6765 3a0a 2020 2020 2222 2253 5748 2073  ge:.    """SWH s
-000016e0: 746f 7261 6765 2064 6174 6173 746f 7265  torage datastore
-000016f0: 2070 726f 7879 2c20 656e 636f 6d70 6173   proxy, encompas
-00001700: 7369 6e67 2044 4220 616e 6420 6f62 6a65  sing DB and obje
-00001710: 6374 2073 746f 7261 6765 2222 220a 0a20  ct storage""".. 
-00001720: 2020 2063 7572 7265 6e74 5f76 6572 7369     current_versi
-00001730: 6f6e 3a20 696e 7420 3d20 3139 330a 0a20  on: int = 193.. 
-00001740: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00001750: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00001760: 2020 2020 2020 2064 622c 0a20 2020 2020         db,.     
-00001770: 2020 206f 626a 7374 6f72 6167 653d 4e6f     objstorage=No
-00001780: 6e65 2c0a 2020 2020 2020 2020 6d69 6e5f  ne,.        min_
-00001790: 706f 6f6c 5f63 6f6e 6e73 3d31 2c0a 2020  pool_conns=1,.  
-000017a0: 2020 2020 2020 6d61 785f 706f 6f6c 5f63        max_pool_c
-000017b0: 6f6e 6e73 3d31 302c 0a20 2020 2020 2020  onns=10,.       
-000017c0: 206a 6f75 726e 616c 5f77 7269 7465 723d   journal_writer=
-000017d0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7175  None,.        qu
-000017e0: 6572 795f 6f70 7469 6f6e 733d 4e6f 6e65  ery_options=None
-000017f0: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
-00001800: 2022 2222 496e 7374 616e 7469 6174 6520   """Instantiate 
-00001810: 6120 7374 6f72 6167 6520 696e 7374 616e  a storage instan
-00001820: 6365 2062 6163 6b65 6420 6279 2061 2050  ce backed by a P
-00001830: 6f73 7467 7265 5351 4c20 6461 7461 6261  ostgreSQL databa
-00001840: 7365 2061 6e64 2061 6e0a 2020 2020 2020  se and an.      
-00001850: 2020 6f62 6a73 746f 7261 6765 2e0a 0a20    objstorage... 
-00001860: 2020 2020 2020 2057 6865 6e20 6060 6462         When ``db
-00001870: 6060 2069 7320 7061 7373 6564 2061 7320  `` is passed as 
-00001880: 6120 636f 6e6e 6563 7469 6f6e 2073 7472  a connection str
-00001890: 696e 672c 2074 6865 6e20 7468 6973 206d  ing, then this m
-000018a0: 6f64 756c 6520 6175 746f 6d61 7469 6361  odule automatica
-000018b0: 6c6c 790a 2020 2020 2020 2020 6d61 6e61  lly.        mana
-000018c0: 6765 7320 6120 636f 6e6e 6563 7469 6f6e  ges a connection
-000018d0: 2070 6f6f 6c20 6265 7477 6565 6e20 6060   pool between ``
-000018e0: 6d69 6e5f 706f 6f6c 5f63 6f6e 6e73 6060  min_pool_conns``
-000018f0: 2061 6e64 2060 606d 6178 5f70 6f6f 6c5f   and ``max_pool_
-00001900: 636f 6e6e 7360 602e 0a20 2020 2020 2020  conns``..       
-00001910: 2057 6865 6e20 6060 6462 6060 2069 7320   When ``db`` is 
-00001920: 616e 2065 7870 6c69 6369 7420 7073 7963  an explicit psyc
-00001930: 6f70 6732 2063 6f6e 6e65 6374 696f 6e2c  opg2 connection,
-00001940: 2074 6865 6e20 6060 6d69 6e5f 706f 6f6c   then ``min_pool
-00001950: 5f63 6f6e 6e73 6060 2061 6e64 0a20 2020  _conns`` and.   
-00001960: 2020 2020 2060 606d 6178 5f70 6f6f 6c5f       ``max_pool_
-00001970: 636f 6e6e 7360 6020 6172 6520 6967 6e6f  conns`` are igno
-00001980: 7265 6420 616e 6420 7468 6520 636f 6e6e  red and the conn
-00001990: 6563 7469 6f6e 2069 7320 7573 6564 2064  ection is used d
-000019a0: 6972 6563 746c 792e 0a0a 2020 2020 2020  irectly...      
-000019b0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-000019c0: 2020 2020 6462 3a20 6569 7468 6572 2061      db: either a
-000019d0: 206c 6962 7071 2063 6f6e 6e65 6374 696f   libpq connectio
-000019e0: 6e20 7374 7269 6e67 2c20 6f72 2061 2070  n string, or a p
-000019f0: 7379 636f 7067 3220 636f 6e6e 6563 7469  sycopg2 connecti
-00001a00: 6f6e 0a20 2020 2020 2020 2020 2020 206f  on.            o
-00001a10: 626a 7374 6f72 6167 653a 2063 6f6e 6669  bjstorage: confi
-00001a20: 6775 7261 7469 6f6e 2066 6f72 2074 6865  guration for the
-00001a30: 2062 6163 6b65 6e64 203a 636c 6173 733a   backend :class:
-00001a40: 604f 626a 5374 6f72 6167 6560 3b20 6966  `ObjStorage`; if
-00001a50: 2075 6e73 6574 2c0a 2020 2020 2020 2020   unset,.        
-00001a60: 2020 2020 2020 2075 7365 2061 204e 6f6f         use a Noo
-00001a70: 704f 626a 5374 6f72 6167 650a 2020 2020  pObjStorage.    
-00001a80: 2020 2020 2020 2020 6d69 6e5f 706f 6f6c          min_pool
-00001a90: 5f63 6f6e 6e73 3a20 6d69 6e20 6e75 6d62  _conns: min numb
-00001aa0: 6572 206f 6620 636f 6e6e 6563 7469 6f6e  er of connection
-00001ab0: 7320 696e 2074 6865 2070 7379 636f 7067  s in the psycopg
-00001ac0: 3220 706f 6f6c 0a20 2020 2020 2020 2020  2 pool.         
-00001ad0: 2020 206d 6178 5f70 6f6f 6c5f 636f 6e6e     max_pool_conn
-00001ae0: 733a 206d 6178 206e 756d 6265 7220 6f66  s: max number of
-00001af0: 2063 6f6e 6e65 6374 696f 6e73 2069 6e20   connections in 
-00001b00: 7468 6520 7073 7963 6f70 6732 2070 6f6f  the psycopg2 poo
-00001b10: 6c0a 2020 2020 2020 2020 2020 2020 6a6f  l.            jo
-00001b20: 7572 6e61 6c5f 7772 6974 6572 3a20 636f  urnal_writer: co
-00001b30: 6e66 6967 7572 6174 696f 6e20 666f 7220  nfiguration for 
-00001b40: 7468 6520 3a63 6c61 7373 3a60 4a6f 7572  the :class:`Jour
-00001b50: 6e61 6c57 7269 7465 7260 0a20 2020 2020  nalWriter`.     
-00001b60: 2020 2020 2020 2071 7565 7279 5f6f 7074         query_opt
-00001b70: 696f 6e73 3a20 636f 6e66 6967 7572 6174  ions: configurat
-00001b80: 696f 6e20 666f 7220 7468 6520 7371 6c20  ion for the sql 
-00001b90: 636f 6e6e 6563 7469 6f6e 733b 206b 6579  connections; key
-00001ba0: 7320 6f66 2074 6865 2064 6963 7420 6172  s of the dict ar
-00001bb0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00001bc0: 2074 6865 206d 6574 686f 6420 6e61 6d65   the method name
-00001bd0: 7320 6465 636f 7261 7465 6420 7769 7468  s decorated with
-00001be0: 203a 6675 6e63 3a60 6462 5f74 7261 6e73   :func:`db_trans
-00001bf0: 6163 7469 6f6e 6020 6f72 0a20 2020 2020  action` or.     
-00001c00: 2020 2020 2020 2020 2020 3a66 756e 633a            :func:
-00001c10: 6064 625f 7472 616e 7361 6374 696f 6e5f  `db_transaction_
-00001c20: 6765 6e65 7261 746f 7260 2028 6567 2e20  generator` (eg. 
-00001c30: 3a66 756e 633a 6063 6f6e 7465 6e74 5f66  :func:`content_f
-00001c40: 696e 6460 292c 2061 6e64 2076 616c 7565  ind`), and value
-00001c50: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00001c60: 2061 7265 2064 6963 7473 2028 636f 6e66   are dicts (conf
-00001c70: 6967 5f6e 616d 652c 2063 6f6e 6669 675f  ig_name, config_
-00001c80: 7661 6c75 6529 2075 7365 6420 746f 2063  value) used to c
-00001c90: 6f6e 6669 6775 7265 2074 6865 2073 716c  onfigure the sql
-00001ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001cb0: 636f 6e6e 6563 7469 6f6e 2066 6f72 2074  connection for t
-00001cc0: 6865 206d 6574 686f 645f 6e61 6d65 2e20  he method_name. 
-00001cd0: 466f 7220 6578 616d 706c 652c 2075 7369  For example, usi
-00001ce0: 6e67 3a3a 0a0a 2020 2020 2020 2020 2020  ng::..          
-00001cf0: 2020 2020 2020 2020 7b22 636f 6e74 656e          {"conten
-00001d00: 745f 6765 7422 3a20 7b22 7374 6174 656d  t_get": {"statem
-00001d10: 656e 745f 7469 6d65 6f75 7422 3a20 3530  ent_timeout": 50
-00001d20: 3030 7d7d 0a0a 2020 2020 2020 2020 2020  00}}..          
-00001d30: 2020 2020 2077 696c 6c20 6f76 6572 7269       will overri
-00001d40: 6465 2074 6865 2064 6566 6175 6c74 2073  de the default s
-00001d50: 7461 7465 6d65 6e74 2074 696d 656f 7574  tatement timeout
-00001d60: 2066 6f72 2074 6865 203a 6675 6e63 3a60   for the :func:`
-00001d70: 636f 6e74 656e 745f 6765 7460 0a20 2020  content_get`.   
-00001d80: 2020 2020 2020 2020 2020 2020 656e 6470              endp
-00001d90: 6f69 6e74 2066 726f 6d20 3530 306d 7320  oint from 500ms 
-00001da0: 746f 2035 3030 306d 732e 0a0a 2020 2020  to 5000ms...    
-00001db0: 2020 2020 2020 2020 2020 2053 6565 203a             See :
-00001dc0: 6d6f 643a 6073 7768 2e63 6f72 652e 6462  mod:`swh.core.db
-00001dd0: 2e63 6f6d 6d6f 6e60 2066 6f72 206d 6f72  .common` for mor
-00001de0: 6520 6465 7461 696c 732e 0a0a 2020 2020  e details...    
-00001df0: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-00001e00: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00001e10: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00001e20: 6462 2c20 7073 7963 6f70 6732 2e65 7874  db, psycopg2.ext
-00001e30: 656e 7369 6f6e 732e 636f 6e6e 6563 7469  ensions.connecti
-00001e40: 6f6e 293a 0a20 2020 2020 2020 2020 2020  on):.           
-00001e50: 2020 2020 2073 656c 662e 5f70 6f6f 6c20       self._pool 
-00001e60: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
-00001e70: 2020 2020 2020 2073 656c 662e 5f64 6220         self._db 
-00001e80: 3d20 4462 2864 6229 0a0a 2020 2020 2020  = Db(db)..      
-00001e90: 2020 2020 2020 2020 2020 2320 5365 6520            # See 
-00001ea0: 636f 6d6d 656e 7420 6265 6c6f 770a 2020  comment below.  
-00001eb0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00001ec0: 6c66 2e5f 6462 2e63 7572 736f 7228 292e  lf._db.cursor().
-00001ed0: 6578 6563 7574 6528 2253 4554 2054 494d  execute("SET TIM
-00001ee0: 4520 5a4f 4e45 2027 5554 4327 2229 0a20  E ZONE 'UTC'"). 
-00001ef0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00001f00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001f10: 2073 656c 662e 5f70 6f6f 6c20 3d20 7073   self._pool = ps
-00001f20: 7963 6f70 6732 2e70 6f6f 6c2e 5468 7265  ycopg2.pool.Thre
-00001f30: 6164 6564 436f 6e6e 6563 7469 6f6e 506f  adedConnectionPo
-00001f40: 6f6c 280a 2020 2020 2020 2020 2020 2020  ol(.            
-00001f50: 2020 2020 2020 2020 6d69 6e5f 706f 6f6c          min_pool
-00001f60: 5f63 6f6e 6e73 2c20 6d61 785f 706f 6f6c  _conns, max_pool
-00001f70: 5f63 6f6e 6e73 2c20 6462 0a20 2020 2020  _conns, db.     
-00001f80: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00001f90: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00001fa0: 662e 5f64 6220 3d20 4e6f 6e65 0a20 2020  f._db = None.   
-00001fb0: 2020 2020 2065 7863 6570 7420 7073 7963       except psyc
-00001fc0: 6f70 6732 2e4f 7065 7261 7469 6f6e 616c  opg2.Operational
-00001fd0: 4572 726f 7220 6173 2065 3a0a 2020 2020  Error as e:.    
-00001fe0: 2020 2020 2020 2020 7261 6973 6520 5374          raise St
-00001ff0: 6f72 6167 6544 4245 7272 6f72 2865 290a  orageDBError(e).
-00002000: 2020 2020 2020 2020 7365 6c66 2e6a 6f75          self.jou
-00002010: 726e 616c 5f77 7269 7465 7220 3d20 4a6f  rnal_writer = Jo
-00002020: 7572 6e61 6c57 7269 7465 7228 6a6f 7572  urnalWriter(jour
-00002030: 6e61 6c5f 7772 6974 6572 290a 2020 2020  nal_writer).    
-00002040: 2020 2020 7365 6c66 2e6f 626a 7374 6f72      self.objstor
-00002050: 6167 6520 3d20 4f62 6a53 746f 7261 6765  age = ObjStorage
-00002060: 2873 656c 662c 206f 626a 7374 6f72 6167  (self, objstorag
-00002070: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
-00002080: 7175 6572 795f 6f70 7469 6f6e 7320 3d20  query_options = 
-00002090: 7175 6572 795f 6f70 7469 6f6e 730a 2020  query_options.  
-000020a0: 2020 2020 2020 7365 6c66 2e5f 666c 6176        self._flav
-000020b0: 6f72 3a20 4f70 7469 6f6e 616c 5b73 7472  or: Optional[str
-000020c0: 5d20 3d20 4e6f 6e65 0a0a 2020 2020 2323  ] = None..    ##
-000020d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000020e0: 2323 2323 2323 2323 0a20 2020 2023 2055  ########.    # U
-000020f0: 7469 6c69 7469 6573 0a20 2020 2023 2323  tilities.    ###
-00002100: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002110: 2323 2323 2323 230a 0a20 2020 2064 6566  #######..    def
-00002120: 2067 6574 5f64 6228 7365 6c66 293a 0a20   get_db(self):. 
-00002130: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
-00002140: 6462 3a0a 2020 2020 2020 2020 2020 2020  db:.            
-00002150: 7265 7475 726e 2073 656c 662e 5f64 620a  return self._db.
-00002160: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00002170: 2020 2020 2020 2020 2020 6462 203d 2044            db = D
-00002180: 622e 6672 6f6d 5f70 6f6f 6c28 7365 6c66  b.from_pool(self
-00002190: 2e5f 706f 6f6c 290a 0a20 2020 2020 2020  ._pool)..       
-000021a0: 2020 2020 2023 2057 6f72 6b61 726f 756e       # Workaroun
-000021b0: 6420 666f 7220 7073 7963 6f70 6732 203c  d for psycopg2 <
-000021c0: 2032 2e39 2e30 206e 6f74 2068 616e 646c   2.9.0 not handl
-000021d0: 696e 6720 6672 6163 7469 6f6e 616c 2074  ing fractional t
-000021e0: 696d 657a 6f6e 6573 2c0a 2020 2020 2020  imezones,.      
-000021f0: 2020 2020 2020 2320 7768 6963 6820 6d61        # which ma
-00002200: 7920 6861 7070 656e 206f 6e20 6f6c 6420  y happen on old 
-00002210: 7265 7669 7369 6f6e 2f72 656c 6561 7365  revision/release
-00002220: 2064 6174 6573 206f 6e20 7379 7374 656d   dates on system
-00002230: 7320 636f 6e66 6967 7572 6564 0a20 2020  s configured.   
-00002240: 2020 2020 2020 2020 2023 2077 6974 6820           # with 
-00002250: 6e6f 6e2d 5554 4320 7469 6d65 7a6f 6e65  non-UTC timezone
-00002260: 732e 0a20 2020 2020 2020 2020 2020 2023  s..            #
-00002270: 2068 7474 7073 3a2f 2f77 7777 2e70 7379   https://www.psy
-00002280: 636f 7067 2e6f 7267 2f64 6f63 732f 7573  copg.org/docs/us
-00002290: 6167 652e 6874 6d6c 2374 696d 652d 7a6f  age.html#time-zo
-000022a0: 6e65 732d 6861 6e64 6c69 6e67 0a20 2020  nes-handling.   
-000022b0: 2020 2020 2020 2020 2064 622e 6375 7273           db.curs
-000022c0: 6f72 2829 2e65 7865 6375 7465 2822 5345  or().execute("SE
-000022d0: 5420 5449 4d45 205a 4f4e 4520 2755 5443  T TIME ZONE 'UTC
-000022e0: 2722 290a 0a20 2020 2020 2020 2020 2020  '")..           
-000022f0: 2072 6574 7572 6e20 6462 0a0a 2020 2020   return db..    
-00002300: 6465 6620 7075 745f 6462 2873 656c 662c  def put_db(self,
-00002310: 2064 6229 3a0a 2020 2020 2020 2020 6966   db):.        if
-00002320: 2064 6220 6973 206e 6f74 2073 656c 662e   db is not self.
-00002330: 5f64 623a 0a20 2020 2020 2020 2020 2020  _db:.           
-00002340: 2064 622e 7075 745f 636f 6e6e 2829 0a0a   db.put_conn()..
-00002350: 2020 2020 4063 6f6e 7465 7874 6d61 6e61      @contextmana
-00002360: 6765 720a 2020 2020 6465 6620 6462 2873  ger.    def db(s
-00002370: 656c 6629 3a0a 2020 2020 2020 2020 6462  elf):.        db
-00002380: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-00002390: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-000023a0: 2064 6220 3d20 7365 6c66 2e67 6574 5f64   db = self.get_d
-000023b0: 6228 290a 2020 2020 2020 2020 2020 2020  b().            
-000023c0: 7969 656c 6420 6462 0a20 2020 2020 2020  yield db.       
-000023d0: 2066 696e 616c 6c79 3a0a 2020 2020 2020   finally:.      
-000023e0: 2020 2020 2020 6966 2064 623a 0a20 2020        if db:.   
-000023f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00002400: 662e 7075 745f 6462 2864 6229 0a0a 2020  f.put_db(db)..  
-00002410: 2020 4064 625f 7472 616e 7361 6374 696f    @db_transactio
-00002420: 6e28 290a 2020 2020 6465 6620 6765 745f  n().    def get_
-00002430: 666c 6176 6f72 2873 656c 662c 202a 2c20  flavor(self, *, 
-00002440: 6462 3a20 4462 2c20 6375 723d 4e6f 6e65  db: Db, cur=None
-00002450: 2920 2d3e 2073 7472 3a0a 2020 2020 2020  ) -> str:.      
-00002460: 2020 666c 6176 6f72 203d 2073 7768 5f64    flavor = swh_d
-00002470: 625f 666c 6176 6f72 2864 622e 636f 6e6e  b_flavor(db.conn
-00002480: 2e64 736e 290a 2020 2020 2020 2020 6173  .dsn).        as
-00002490: 7365 7274 2066 6c61 766f 7220 6973 206e  sert flavor is n
-000024a0: 6f74 204e 6f6e 650a 2020 2020 2020 2020  ot None.        
-000024b0: 7265 7475 726e 2066 6c61 766f 720a 0a20  return flavor.. 
-000024c0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-000024d0: 2064 6566 2066 6c61 766f 7228 7365 6c66   def flavor(self
-000024e0: 2920 2d3e 2073 7472 3a0a 2020 2020 2020  ) -> str:.      
-000024f0: 2020 6966 2073 656c 662e 5f66 6c61 766f    if self._flavo
-00002500: 7220 6973 204e 6f6e 653a 0a20 2020 2020  r is None:.     
-00002510: 2020 2020 2020 2073 656c 662e 5f66 6c61         self._fla
-00002520: 766f 7220 3d20 7365 6c66 2e67 6574 5f66  vor = self.get_f
-00002530: 6c61 766f 7228 290a 2020 2020 2020 2020  lavor().        
-00002540: 6173 7365 7274 2073 656c 662e 5f66 6c61  assert self._fla
-00002550: 766f 7220 6973 206e 6f74 204e 6f6e 650a  vor is not None.
-00002560: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00002570: 656c 662e 5f66 6c61 766f 720a 0a20 2020  elf._flavor..   
-00002580: 2040 6462 5f74 7261 6e73 6163 7469 6f6e   @db_transaction
-00002590: 2829 0a20 2020 2064 6566 2063 6865 636b  ().    def check
-000025a0: 5f63 6f6e 6669 6728 7365 6c66 2c20 2a2c  _config(self, *,
-000025b0: 2063 6865 636b 5f77 7269 7465 3a20 626f   check_write: bo
-000025c0: 6f6c 2c20 6462 3a20 4462 2c20 6375 723d  ol, db: Db, cur=
-000025d0: 4e6f 6e65 2920 2d3e 2062 6f6f 6c3a 0a20  None) -> bool:. 
-000025e0: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-000025f0: 6c66 2e6f 626a 7374 6f72 6167 652e 6368  lf.objstorage.ch
-00002600: 6563 6b5f 636f 6e66 6967 2863 6865 636b  eck_config(check
-00002610: 5f77 7269 7465 3d63 6865 636b 5f77 7269  _write=check_wri
-00002620: 7465 293a 0a20 2020 2020 2020 2020 2020  te):.           
-00002630: 2072 6574 7572 6e20 4661 6c73 650a 0a20   return False.. 
-00002640: 2020 2020 2020 2064 6276 6572 7369 6f6e         dbversion
-00002650: 203d 2073 7768 5f64 625f 7665 7273 696f   = swh_db_versio
-00002660: 6e28 6462 2e63 6f6e 6e2e 6473 6e29 0a20  n(db.conn.dsn). 
-00002670: 2020 2020 2020 2069 6620 6462 7665 7273         if dbvers
-00002680: 696f 6e20 213d 2073 656c 662e 6375 7272  ion != self.curr
-00002690: 656e 745f 7665 7273 696f 6e3a 0a20 2020  ent_version:.   
-000026a0: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-000026b0: 7761 726e 696e 6728 0a20 2020 2020 2020  warning(.       
-000026c0: 2020 2020 2020 2020 2022 6461 7461 6261           "databa
-000026d0: 7365 2064 6276 6572 7369 6f6e 2028 2573  se dbversion (%s
-000026e0: 2920 213d 2025 7320 6375 7272 656e 745f  ) != %s current_
-000026f0: 7665 7273 696f 6e20 2825 7329 222c 0a20  version (%s)",. 
-00002700: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00002710: 6276 6572 7369 6f6e 2c0a 2020 2020 2020  bversion,.      
-00002720: 2020 2020 2020 2020 2020 5f5f 6e61 6d65            __name
-00002730: 5f5f 2c0a 2020 2020 2020 2020 2020 2020  __,.            
-00002740: 2020 2020 7365 6c66 2e63 7572 7265 6e74      self.current
-00002750: 5f76 6572 7369 6f6e 2c0a 2020 2020 2020  _version,.      
-00002760: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00002770: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-00002780: 0a0a 2020 2020 2020 2020 2320 4368 6563  ..        # Chec
-00002790: 6b20 7065 726d 6973 7369 6f6e 7320 6f6e  k permissions on
-000027a0: 206f 6e65 206f 6620 7468 6520 7461 626c   one of the tabl
-000027b0: 6573 0a20 2020 2020 2020 2063 6865 636b  es.        check
-000027c0: 203d 2022 494e 5345 5254 2220 6966 2063   = "INSERT" if c
-000027d0: 6865 636b 5f77 7269 7465 2065 6c73 6520  heck_write else 
-000027e0: 2253 454c 4543 5422 0a0a 2020 2020 2020  "SELECT"..      
-000027f0: 2020 6375 722e 6578 6563 7574 6528 2273    cur.execute("s
-00002800: 656c 6563 7420 6861 735f 7461 626c 655f  elect has_table_
-00002810: 7072 6976 696c 6567 6528 6375 7272 656e  privilege(curren
-00002820: 745f 7573 6572 2c20 2763 6f6e 7465 6e74  t_user, 'content
-00002830: 272c 2025 7329 222c 2028 6368 6563 6b2c  ', %s)", (check,
-00002840: 2929 0a20 2020 2020 2020 2072 6574 7572  )).        retur
-00002850: 6e20 6375 722e 6665 7463 686f 6e65 2829  n cur.fetchone()
-00002860: 5b30 5d0a 0a20 2020 2023 2323 2323 2323  [0]..    #######
-00002870: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002880: 2323 230a 2020 2020 2320 436f 6e74 656e  ###.    # Conten
-00002890: 740a 2020 2020 2323 2323 2323 2323 2323  t.    ##########
+00000570: 6e63 682c 0a20 2020 2053 6e61 7073 686f  nch,.    Snapsho
+00000580: 7454 6172 6765 7454 7970 652c 0a29 0a66  tTargetType,.).f
+00000590: 726f 6d20 7377 682e 6d6f 6465 6c2e 7377  rom swh.model.sw
+000005a0: 6869 6473 2069 6d70 6f72 7420 4578 7465  hids import Exte
+000005b0: 6e64 6564 4f62 6a65 6374 5479 7065 2c20  ndedObjectType, 
+000005c0: 4578 7465 6e64 6564 5357 4849 442c 204f  ExtendedSWHID, O
+000005d0: 626a 6563 7454 7970 650a 6672 6f6d 2073  bjectType.from s
+000005e0: 7768 2e73 746f 7261 6765 2e65 7863 2069  wh.storage.exc i
+000005f0: 6d70 6f72 7420 280a 2020 2020 4861 7368  mport (.    Hash
+00000600: 436f 6c6c 6973 696f 6e2c 0a20 2020 2051  Collision,.    Q
+00000610: 7565 7279 5469 6d65 6f75 742c 0a20 2020  ueryTimeout,.   
+00000620: 2053 746f 7261 6765 4172 6775 6d65 6e74   StorageArgument
+00000630: 4578 6365 7074 696f 6e2c 0a20 2020 2053  Exception,.    S
+00000640: 746f 7261 6765 4442 4572 726f 722c 0a20  torageDBError,. 
+00000650: 2020 2055 6e6b 6e6f 776e 4d65 7461 6461     UnknownMetada
+00000660: 7461 4175 7468 6f72 6974 792c 0a20 2020  taAuthority,.   
+00000670: 2055 6e6b 6e6f 776e 4d65 7461 6461 7461   UnknownMetadata
+00000680: 4665 7463 6865 722c 0a29 0a66 726f 6d20  Fetcher,.).from 
+00000690: 7377 682e 7374 6f72 6167 652e 696e 7465  swh.storage.inte
+000006a0: 7266 6163 6520 696d 706f 7274 2028 0a20  rface import (. 
+000006b0: 2020 2056 4953 4954 5f53 5441 5455 5345     VISIT_STATUSE
+000006c0: 532c 0a20 2020 2048 6173 6844 6963 742c  S,.    HashDict,
+000006d0: 0a20 2020 204c 6973 744f 7264 6572 2c0a  .    ListOrder,.
+000006e0: 2020 2020 4f62 6a65 6374 5265 6665 7265      ObjectRefere
+000006f0: 6e63 652c 0a20 2020 204f 7269 6769 6e56  nce,.    OriginV
+00000700: 6973 6974 5769 7468 5374 6174 7573 6573  isitWithStatuses
+00000710: 2c0a 2020 2020 5061 6765 6452 6573 756c  ,.    PagedResul
+00000720: 742c 0a20 2020 2050 6172 7469 616c 4272  t,.    PartialBr
+00000730: 616e 6368 6573 2c0a 2020 2020 536e 6170  anches,.    Snap
+00000740: 7368 6f74 4272 616e 6368 4279 4e61 6d65  shotBranchByName
+00000750: 5265 7370 6f6e 7365 2c0a 290a 6672 6f6d  Response,.).from
+00000760: 2073 7768 2e73 746f 7261 6765 2e6f 626a   swh.storage.obj
+00000770: 7374 6f72 6167 6520 696d 706f 7274 204f  storage import O
+00000780: 626a 5374 6f72 6167 650a 6672 6f6d 2073  bjStorage.from s
+00000790: 7768 2e73 746f 7261 6765 2e75 7469 6c73  wh.storage.utils
+000007a0: 2069 6d70 6f72 7420 280a 2020 2020 6578   import (.    ex
+000007b0: 7472 6163 745f 636f 6c6c 6973 696f 6e5f  tract_collision_
+000007c0: 6861 7368 2c0a 2020 2020 6765 745f 7061  hash,.    get_pa
+000007d0: 7274 6974 696f 6e5f 626f 756e 6473 5f62  rtition_bounds_b
+000007e0: 7974 6573 2c0a 2020 2020 6d61 705f 6f70  ytes,.    map_op
+000007f0: 7469 6f6e 616c 2c0a 2020 2020 6e6f 772c  tional,.    now,
+00000800: 0a29 0a66 726f 6d20 7377 682e 7374 6f72  .).from swh.stor
+00000810: 6167 652e 7772 6974 6572 2069 6d70 6f72  age.writer impor
+00000820: 7420 4a6f 7572 6e61 6c57 7269 7465 720a  t JournalWriter.
+00000830: 0a66 726f 6d20 2e20 696d 706f 7274 2063  .from . import c
+00000840: 6f6e 7665 7274 6572 730a 6672 6f6d 202e  onverters.from .
+00000850: 6462 2069 6d70 6f72 7420 4462 0a0a 6c6f  db import Db..lo
+00000860: 6767 6572 203d 206c 6f67 6769 6e67 2e67  gger = logging.g
+00000870: 6574 4c6f 6767 6572 285f 5f6e 616d 655f  etLogger(__name_
+00000880: 5f29 0a0a 2320 4d61 7820 626c 6f63 6b20  _)..# Max block 
+00000890: 7369 7a65 206f 6620 636f 6e74 656e 7473  size of contents
+000008a0: 2074 6f20 7265 7475 726e 0a42 554c 4b5f   to return.BULK_
+000008b0: 424c 4f43 4b5f 434f 4e54 454e 545f 4c45  BLOCK_CONTENT_LE
+000008c0: 4e5f 4d41 5820 3d20 3130 3030 300a 0a45  N_MAX = 10000..E
+000008d0: 4d50 5459 5f53 4e41 5053 484f 545f 4944  MPTY_SNAPSHOT_ID
+000008e0: 203d 2068 6173 685f 746f 5f62 7974 6573   = hash_to_bytes
+000008f0: 2822 3161 3838 3933 6536 6138 3666 3434  ("1a8893e6a86f44
+00000900: 3465 3862 6538 6537 6264 6136 6362 3334  4e8be8e7bda6cb34
+00000910: 6662 3137 3335 6130 3065 2229 0a22 2222  fb1735a00e")."""
+00000920: 4964 656e 7469 6669 6572 2066 6f72 2074  Identifier for t
+00000930: 6865 2065 6d70 7479 2073 6e61 7073 686f  he empty snapsho
+00000940: 7422 2222 0a0a 0a56 414c 4944 4154 494f  t"""...VALIDATIO
+00000950: 4e5f 4558 4345 5054 494f 4e53 203d 2028  N_EXCEPTIONS = (
+00000960: 0a20 2020 204b 6579 4572 726f 722c 0a20  .    KeyError,. 
+00000970: 2020 2054 7970 6545 7272 6f72 2c0a 2020     TypeError,.  
+00000980: 2020 5661 6c75 6545 7272 6f72 2c0a 2020    ValueError,.  
+00000990: 2020 7073 7963 6f70 6732 2e65 7272 6f72    psycopg2.error
+000009a0: 732e 4368 6563 6b56 696f 6c61 7469 6f6e  s.CheckViolation
+000009b0: 2c0a 2020 2020 7073 7963 6f70 6732 2e65  ,.    psycopg2.e
+000009c0: 7272 6f72 732e 496e 7465 6772 6974 7945  rrors.IntegrityE
+000009d0: 7272 6f72 2c0a 2020 2020 7073 7963 6f70  rror,.    psycop
+000009e0: 6732 2e65 7272 6f72 732e 496e 7661 6c69  g2.errors.Invali
+000009f0: 6454 6578 7452 6570 7265 7365 6e74 6174  dTextRepresentat
+00000a00: 696f 6e2c 0a20 2020 2070 7379 636f 7067  ion,.    psycopg
+00000a10: 322e 6572 726f 7273 2e4e 6f74 4e75 6c6c  2.errors.NotNull
+00000a20: 5669 6f6c 6174 696f 6e2c 0a20 2020 2070  Violation,.    p
+00000a30: 7379 636f 7067 322e 6572 726f 7273 2e4e  sycopg2.errors.N
+00000a40: 756d 6572 6963 5661 6c75 654f 7574 4f66  umericValueOutOf
+00000a50: 5261 6e67 652c 0a20 2020 2070 7379 636f  Range,.    psyco
+00000a60: 7067 322e 6572 726f 7273 2e55 6e64 6566  pg2.errors.Undef
+00000a70: 696e 6564 4675 6e63 7469 6f6e 2c20 2023  inedFunction,  #
+00000a80: 2028 7261 6973 6564 206f 6e20 7772 6f6e   (raised on wron
+00000a90: 6720 6172 6775 6d65 6e74 2074 7970 7329  g argument typs)
+00000aa0: 0a20 2020 2070 7379 636f 7067 322e 6572  .    psycopg2.er
+00000ab0: 726f 7273 2e50 726f 6772 616d 4c69 6d69  rors.ProgramLimi
+00000ac0: 7445 7863 6565 6465 642c 2020 2320 7479  tExceeded,  # ty
+00000ad0: 7069 6361 6c6c 7920 7065 7273 6f6e 5f6e  pically person_n
+00000ae0: 616d 655f 6964 780a 290a 2222 2245 7863  ame_idx.)."""Exc
+00000af0: 6570 7469 6f6e 7320 7261 6973 6564 2062  eptions raised b
+00000b00: 7920 706f 7374 6772 6573 716c 2077 6865  y postgresql whe
+00000b10: 6e20 7661 6c69 6461 7469 6f6e 206f 6620  n validation of 
+00000b20: 7468 6520 6172 6775 6d65 6e74 730a 6661  the arguments.fa
+00000b30: 696c 6564 2e22 2222 0a0a 0a40 636f 6e74  iled."""...@cont
+00000b40: 6578 746c 6962 2e63 6f6e 7465 7874 6d61  extlib.contextma
+00000b50: 6e61 6765 720a 6465 6620 636f 6e76 6572  nager.def conver
+00000b60: 745f 7661 6c69 6461 7469 6f6e 5f65 7863  t_validation_exc
+00000b70: 6570 7469 6f6e 7328 293a 0a20 2020 2022  eptions():.    "
+00000b80: 2222 4361 7463 6865 7320 706f 7374 6772  ""Catches postgr
+00000b90: 6573 716c 2065 7272 6f72 7320 7265 6c61  esql errors rela
+00000ba0: 7465 6420 746f 2069 6e76 616c 6964 2061  ted to invalid a
+00000bb0: 7267 756d 656e 7473 2c20 616e 640a 2020  rguments, and.  
+00000bc0: 2020 7265 2d72 6169 7365 7320 6120 5374    re-raises a St
+00000bd0: 6f72 6167 6541 7267 756d 656e 7445 7863  orageArgumentExc
+00000be0: 6570 7469 6f6e 2e22 2222 0a20 2020 2074  eption.""".    t
+00000bf0: 7279 3a0a 2020 2020 2020 2020 7969 656c  ry:.        yiel
+00000c00: 640a 2020 2020 6578 6365 7074 2070 7379  d.    except psy
+00000c10: 636f 7067 322e 6572 726f 7273 2e55 6e69  copg2.errors.Uni
+00000c20: 7175 6556 696f 6c61 7469 6f6e 3a0a 2020  queViolation:.  
+00000c30: 2020 2020 2020 2320 5468 6973 206f 6e6c        # This onl
+00000c40: 7920 6861 7070 656e 7320 6265 6361 7573  y happens becaus
+00000c50: 6520 6f66 2063 6f6e 6375 7272 656e 7420  e of concurrent 
+00000c60: 696e 7365 7274 696f 6e73 2c20 6275 7420  insertions, but 
+00000c70: 6974 2069 730a 2020 2020 2020 2020 2320  it is.        # 
+00000c80: 6120 7375 6263 6c61 7373 206f 6620 496e  a subclass of In
+00000c90: 7465 6772 6974 7945 7272 6f72 3b20 736f  tegrityError; so
+00000ca0: 2077 6520 6e65 6564 2074 6f20 6361 7463   we need to catc
+00000cb0: 6820 616e 6420 7265 7261 6973 6520 6974  h and reraise it
+00000cc0: 0a20 2020 2020 2020 2023 2062 6566 6f72  .        # befor
+00000cd0: 6520 7468 6520 6e65 7874 2063 6c61 7573  e the next claus
+00000ce0: 6520 636f 6e76 6572 7473 2069 7420 746f  e converts it to
+00000cf0: 2053 746f 7261 6765 4172 6775 6d65 6e74   StorageArgument
+00000d00: 4578 6365 7074 696f 6e2e 0a20 2020 2020  Exception..     
+00000d10: 2020 2072 6169 7365 0a20 2020 2065 7863     raise.    exc
+00000d20: 6570 7420 5641 4c49 4441 5449 4f4e 5f45  ept VALIDATION_E
+00000d30: 5843 4550 5449 4f4e 5320 6173 2065 3a0a  XCEPTIONS as e:.
+00000d40: 2020 2020 2020 2020 7261 6973 6520 5374          raise St
+00000d50: 6f72 6167 6541 7267 756d 656e 7445 7863  orageArgumentExc
+00000d60: 6570 7469 6f6e 2873 7472 2865 2929 0a0a  eption(str(e))..
+00000d70: 0a64 6566 2064 625f 7472 616e 7361 6374  .def db_transact
+00000d80: 696f 6e5f 6765 6e65 7261 746f 7228 2a61  ion_generator(*a
+00000d90: 7267 732c 202a 2a6b 7761 7267 7329 3a0a  rgs, **kwargs):.
+00000da0: 2020 2020 6465 6620 6465 636f 7261 746f      def decorato
+00000db0: 7228 6d65 7468 293a 0a20 2020 2020 2020  r(meth):.       
+00000dc0: 206d 6574 6820 3d20 5f64 625f 7472 616e   meth = _db_tran
+00000dd0: 7361 6374 696f 6e5f 6765 6e65 7261 746f  saction_generato
+00000de0: 7228 2a61 7267 732c 202a 2a6b 7761 7267  r(*args, **kwarg
+00000df0: 7329 286d 6574 6829 0a0a 2020 2020 2020  s)(meth)..      
+00000e00: 2020 4066 756e 6374 6f6f 6c73 2e77 7261    @functools.wra
+00000e10: 7073 286d 6574 6829 0a20 2020 2020 2020  ps(meth).       
+00000e20: 2064 6566 205f 6d65 7468 2873 656c 662c   def _meth(self,
+00000e30: 202a 6172 6773 2c20 2a2a 6b77 6172 6773   *args, **kwargs
+00000e40: 293a 0a20 2020 2020 2020 2020 2020 2074  ):.            t
+00000e50: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00000e60: 2020 2020 7969 656c 6420 6672 6f6d 206d      yield from m
+00000e70: 6574 6828 7365 6c66 2c20 2a61 7267 732c  eth(self, *args,
+00000e80: 202a 2a6b 7761 7267 7329 0a20 2020 2020   **kwargs).     
+00000e90: 2020 2020 2020 2065 7863 6570 7420 7073         except ps
+00000ea0: 7963 6f70 6732 2e65 7272 6f72 732e 5175  ycopg2.errors.Qu
+00000eb0: 6572 7943 616e 6365 6c65 6420 6173 2065  eryCanceled as e
+00000ec0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00000ed0: 2020 7261 6973 6520 5175 6572 7954 696d    raise QueryTim
+00000ee0: 656f 7574 282a 652e 6172 6773 290a 0a20  eout(*e.args).. 
+00000ef0: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
+00000f00: 6574 680a 0a20 2020 2072 6574 7572 6e20  eth..    return 
+00000f10: 6465 636f 7261 746f 720a 0a0a 6465 6620  decorator...def 
+00000f20: 6462 5f74 7261 6e73 6163 7469 6f6e 282a  db_transaction(*
+00000f30: 6172 6773 2c20 2a2a 6b77 6172 6773 293a  args, **kwargs):
+00000f40: 0a20 2020 2064 6566 2064 6563 6f72 6174  .    def decorat
+00000f50: 6f72 286d 6574 6829 3a0a 2020 2020 2020  or(meth):.      
+00000f60: 2020 6d65 7468 203d 205f 6462 5f74 7261    meth = _db_tra
+00000f70: 6e73 6163 7469 6f6e 282a 6172 6773 2c20  nsaction(*args, 
+00000f80: 2a2a 6b77 6172 6773 2928 6d65 7468 290a  **kwargs)(meth).
+00000f90: 0a20 2020 2020 2020 2040 6675 6e63 746f  .        @functo
+00000fa0: 6f6c 732e 7772 6170 7328 6d65 7468 290a  ols.wraps(meth).
+00000fb0: 2020 2020 2020 2020 6465 6620 5f6d 6574          def _met
+00000fc0: 6828 7365 6c66 2c20 2a61 7267 732c 202a  h(self, *args, *
+00000fd0: 2a6b 7761 7267 7329 3a0a 2020 2020 2020  *kwargs):.      
+00000fe0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+00000ff0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00001000: 6e20 6d65 7468 2873 656c 662c 202a 6172  n meth(self, *ar
+00001010: 6773 2c20 2a2a 6b77 6172 6773 290a 2020  gs, **kwargs).  
+00001020: 2020 2020 2020 2020 2020 6578 6365 7074            except
+00001030: 2070 7379 636f 7067 322e 6572 726f 7273   psycopg2.errors
+00001040: 2e51 7565 7279 4361 6e63 656c 6564 2061  .QueryCanceled a
+00001050: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
+00001060: 2020 2020 2072 6169 7365 2051 7565 7279       raise Query
+00001070: 5469 6d65 6f75 7428 2a65 2e61 7267 7329  Timeout(*e.args)
+00001080: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00001090: 205f 6d65 7468 0a0a 2020 2020 7265 7475   _meth..    retu
+000010a0: 726e 2064 6563 6f72 6174 6f72 0a0a 0a54  rn decorator...T
+000010b0: 526f 7720 3d20 5479 7065 5661 7228 2254  Row = TypeVar("T
+000010c0: 526f 7722 2c20 626f 756e 643d 5475 706c  Row", bound=Tupl
+000010d0: 6529 0a54 5265 7375 6c74 203d 2054 7970  e).TResult = Typ
+000010e0: 6556 6172 2822 5452 6573 756c 7422 290a  eVar("TResult").
+000010f0: 0a0a 6465 6620 5f67 6574 5f70 6167 696e  ..def _get_pagin
+00001100: 6174 6564 5f73 6861 315f 7061 7274 6974  ated_sha1_partit
+00001110: 696f 6e28 0a20 2020 2063 7572 2c0a 2020  ion(.    cur,.  
+00001120: 2020 7061 7274 6974 696f 6e5f 6964 3a20    partition_id: 
+00001130: 696e 742c 0a20 2020 206e 625f 7061 7274  int,.    nb_part
+00001140: 6974 696f 6e73 3a20 696e 742c 0a20 2020  itions: int,.   
+00001150: 2070 6167 655f 746f 6b65 6e3a 204f 7074   page_token: Opt
+00001160: 696f 6e61 6c5b 7374 725d 2c0a 2020 2020  ional[str],.    
+00001170: 6c69 6d69 743a 2069 6e74 2c0a 2020 2020  limit: int,.    
+00001180: 6765 745f 7261 6e67 653a 2043 616c 6c61  get_range: Calla
+00001190: 626c 655b 5b62 7974 6573 2c20 6279 7465  ble[[bytes, byte
+000011a0: 732c 2069 6e74 2c20 416e 795d 2c20 4974  s, int, Any], It
+000011b0: 6572 6174 6f72 5b54 526f 775d 5d2c 0a20  erator[TRow]],. 
+000011c0: 2020 2063 6f6e 7665 7274 3a20 4361 6c6c     convert: Call
+000011d0: 6162 6c65 5b5b 5452 6f77 5d2c 2054 5265  able[[TRow], TRe
+000011e0: 7375 6c74 5d2c 0a20 2020 2067 6574 5f69  sult],.    get_i
+000011f0: 643a 204f 7074 696f 6e61 6c5b 4361 6c6c  d: Optional[Call
+00001200: 6162 6c65 5b5b 5452 6573 756c 745d 2c20  able[[TResult], 
+00001210: 416e 795d 5d20 3d20 4e6f 6e65 2c0a 2920  Any]] = None,.) 
+00001220: 2d3e 2050 6167 6564 5265 7375 6c74 5b54  -> PagedResult[T
+00001230: 5265 7375 6c74 5d3a 0a20 2020 2022 2222  Result]:.    """
+00001240: 496d 706c 656d 656e 7473 2074 6865 2062  Implements the b
+00001250: 756c 6b20 6f66 2060 6063 6f6e 7465 6e74  ulk of ``content
+00001260: 5f67 6574 5f70 6172 7469 7469 6f6e 6060  _get_partition``
+00001270: 2c20 6060 6469 7265 6374 6f72 795f 6765  , ``directory_ge
+00001280: 745f 7061 7274 6974 696f 6e60 602c 0a20  t_partition``,. 
+00001290: 2020 202e 2e2e 3a0a 0a20 2020 2031 2e20     ...:..    1. 
+000012a0: 636f 6d70 7574 6573 2072 616e 6765 2062  computes range b
+000012b0: 6f75 6e64 730a 2020 2020 322e 2061 7070  ounds.    2. app
+000012c0: 6c69 6573 2070 6167 696e 6174 696f 6e20  lies pagination 
+000012d0: 746f 6b65 6e0a 2020 2020 332e 2063 6f6e  token.    3. con
+000012e0: 7665 7274 7320 746f 2066 696e 616c 206f  verts to final o
+000012f0: 626a 6563 7473 0a20 2020 2034 2e20 6578  bjects.    4. ex
+00001300: 7472 6163 7473 206e 6578 7420 7061 6769  tracts next pagi
+00001310: 6e61 7469 6f6e 2074 6f6b 656e 0a20 2020  nation token.   
+00001320: 2022 2222 0a20 2020 2069 6620 6c69 6d69   """.    if limi
+00001330: 7420 6973 204e 6f6e 653a 0a20 2020 2020  t is None:.     
+00001340: 2020 2072 6169 7365 2053 746f 7261 6765     raise Storage
+00001350: 4172 6775 6d65 6e74 4578 6365 7074 696f  ArgumentExceptio
+00001360: 6e28 226c 696d 6974 2073 686f 756c 6420  n("limit should 
+00001370: 6e6f 7420 6265 204e 6f6e 6522 290a 2020  not be None").  
+00001380: 2020 6966 2067 6574 5f69 6420 6973 204e    if get_id is N
+00001390: 6f6e 653a 0a0a 2020 2020 2020 2020 6465  one:..        de
+000013a0: 6620 6765 745f 6964 286f 626a 3a20 5452  f get_id(obj: TR
+000013b0: 6573 756c 7429 3a0a 2020 2020 2020 2020  esult):.        
+000013c0: 2020 2020 7265 7475 726e 206f 626a 2e69      return obj.i
+000013d0: 6420 2023 2074 7970 653a 2069 676e 6f72  d  # type: ignor
+000013e0: 655b 6174 7472 2d64 6566 696e 6564 5d0a  e[attr-defined].
+000013f0: 0a20 2020 2061 7373 6572 7420 6765 745f  .    assert get_
+00001400: 6964 2069 7320 6e6f 7420 4e6f 6e65 2020  id is not None  
+00001410: 2320 746f 2070 6c65 6173 6520 6d79 7079  # to please mypy
+00001420: 0a0a 2020 2020 2873 7461 7274 2c20 656e  ..    (start, en
+00001430: 6429 203d 2067 6574 5f70 6172 7469 7469  d) = get_partiti
+00001440: 6f6e 5f62 6f75 6e64 735f 6279 7465 7328  on_bounds_bytes(
+00001450: 7061 7274 6974 696f 6e5f 6964 2c20 6e62  partition_id, nb
+00001460: 5f70 6172 7469 7469 6f6e 732c 2053 4841  _partitions, SHA
+00001470: 315f 5349 5a45 290a 2020 2020 6966 2070  1_SIZE).    if p
+00001480: 6167 655f 746f 6b65 6e3a 0a20 2020 2020  age_token:.     
+00001490: 2020 2073 7461 7274 203d 2068 6173 685f     start = hash_
+000014a0: 746f 5f62 7974 6573 2870 6167 655f 746f  to_bytes(page_to
+000014b0: 6b65 6e29 0a20 2020 2069 6620 656e 6420  ken).    if end 
+000014c0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+000014d0: 2065 6e64 203d 2062 225c 7866 6622 202a   end = b"\xff" *
+000014e0: 2053 4841 315f 5349 5a45 0a0a 2020 2020   SHA1_SIZE..    
+000014f0: 6e65 7874 5f70 6167 655f 746f 6b65 6e3a  next_page_token:
+00001500: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+00001510: 204e 6f6e 650a 2020 2020 7265 7375 6c74   None.    result
+00001520: 7320 3d20 5b5d 0a20 2020 2066 6f72 2063  s = [].    for c
+00001530: 6f75 6e74 6572 2c20 726f 7720 696e 2065  ounter, row in e
+00001540: 6e75 6d65 7261 7465 2867 6574 5f72 616e  numerate(get_ran
+00001550: 6765 2873 7461 7274 2c20 656e 642c 206c  ge(start, end, l
+00001560: 696d 6974 202b 2031 2c20 6375 7229 293a  imit + 1, cur)):
+00001570: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+00001580: 3d20 636f 6e76 6572 7428 726f 7729 0a20  = convert(row). 
+00001590: 2020 2020 2020 2069 6620 636f 756e 7465         if counte
+000015a0: 7220 3e3d 206c 696d 6974 3a0a 2020 2020  r >= limit:.    
+000015b0: 2020 2020 2020 2020 2320 7461 6b65 2074          # take t
+000015c0: 6865 206c 6173 7420 636f 6e74 656e 7420  he last content 
+000015d0: 666f 7220 7468 6520 6e65 7874 2070 6167  for the next pag
+000015e0: 6520 7374 6172 7469 6e67 2066 726f 6d20  e starting from 
+000015f0: 7468 6973 0a20 2020 2020 2020 2020 2020  this.           
+00001600: 206e 6578 745f 7061 6765 5f74 6f6b 656e   next_page_token
+00001610: 203d 2068 6173 685f 746f 5f68 6578 2867   = hash_to_hex(g
+00001620: 6574 5f69 6428 7265 7375 6c74 2929 0a20  et_id(result)). 
+00001630: 2020 2020 2020 2020 2020 2062 7265 616b             break
+00001640: 0a20 2020 2020 2020 2072 6573 756c 7473  .        results
+00001650: 2e61 7070 656e 6428 7265 7375 6c74 290a  .append(result).
+00001660: 0a20 2020 2061 7373 6572 7420 6c65 6e28  .    assert len(
+00001670: 7265 7375 6c74 7329 203c 3d20 6c69 6d69  results) <= limi
+00001680: 740a 2020 2020 7265 7475 726e 2050 6167  t.    return Pag
+00001690: 6564 5265 7375 6c74 2872 6573 756c 7473  edResult(results
+000016a0: 3d72 6573 756c 7473 2c20 6e65 7874 5f70  =results, next_p
+000016b0: 6167 655f 746f 6b65 6e3d 6e65 7874 5f70  age_token=next_p
+000016c0: 6167 655f 746f 6b65 6e29 0a0a 0a63 6c61  age_token)...cla
+000016d0: 7373 2053 746f 7261 6765 3a0a 2020 2020  ss Storage:.    
+000016e0: 2222 2253 5748 2073 746f 7261 6765 2064  """SWH storage d
+000016f0: 6174 6173 746f 7265 2070 726f 7879 2c20  atastore proxy, 
+00001700: 656e 636f 6d70 6173 7369 6e67 2044 4220  encompassing DB 
+00001710: 616e 6420 6f62 6a65 6374 2073 746f 7261  and object stora
+00001720: 6765 2222 220a 0a20 2020 2063 7572 7265  ge"""..    curre
+00001730: 6e74 5f76 6572 7369 6f6e 3a20 696e 7420  nt_version: int 
+00001740: 3d20 3139 330a 0a20 2020 2064 6566 205f  = 193..    def _
+00001750: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+00001760: 2073 656c 662c 0a20 2020 2020 2020 2064   self,.        d
+00001770: 622c 0a20 2020 2020 2020 206f 626a 7374  b,.        objst
+00001780: 6f72 6167 653d 4e6f 6e65 2c0a 2020 2020  orage=None,.    
+00001790: 2020 2020 6d69 6e5f 706f 6f6c 5f63 6f6e      min_pool_con
+000017a0: 6e73 3d31 2c0a 2020 2020 2020 2020 6d61  ns=1,.        ma
+000017b0: 785f 706f 6f6c 5f63 6f6e 6e73 3d31 302c  x_pool_conns=10,
+000017c0: 0a20 2020 2020 2020 206a 6f75 726e 616c  .        journal
+000017d0: 5f77 7269 7465 723d 4e6f 6e65 2c0a 2020  _writer=None,.  
+000017e0: 2020 2020 2020 7175 6572 795f 6f70 7469        query_opti
+000017f0: 6f6e 733d 4e6f 6e65 2c0a 2020 2020 293a  ons=None,.    ):
+00001800: 0a20 2020 2020 2020 2022 2222 496e 7374  .        """Inst
+00001810: 616e 7469 6174 6520 6120 7374 6f72 6167  antiate a storag
+00001820: 6520 696e 7374 616e 6365 2062 6163 6b65  e instance backe
+00001830: 6420 6279 2061 2050 6f73 7467 7265 5351  d by a PostgreSQ
+00001840: 4c20 6461 7461 6261 7365 2061 6e64 2061  L database and a
+00001850: 6e0a 2020 2020 2020 2020 6f62 6a73 746f  n.        objsto
+00001860: 7261 6765 2e0a 0a20 2020 2020 2020 2057  rage...        W
+00001870: 6865 6e20 6060 6462 6060 2069 7320 7061  hen ``db`` is pa
+00001880: 7373 6564 2061 7320 6120 636f 6e6e 6563  ssed as a connec
+00001890: 7469 6f6e 2073 7472 696e 672c 2074 6865  tion string, the
+000018a0: 6e20 7468 6973 206d 6f64 756c 6520 6175  n this module au
+000018b0: 746f 6d61 7469 6361 6c6c 790a 2020 2020  tomatically.    
+000018c0: 2020 2020 6d61 6e61 6765 7320 6120 636f      manages a co
+000018d0: 6e6e 6563 7469 6f6e 2070 6f6f 6c20 6265  nnection pool be
+000018e0: 7477 6565 6e20 6060 6d69 6e5f 706f 6f6c  tween ``min_pool
+000018f0: 5f63 6f6e 6e73 6060 2061 6e64 2060 606d  _conns`` and ``m
+00001900: 6178 5f70 6f6f 6c5f 636f 6e6e 7360 602e  ax_pool_conns``.
+00001910: 0a20 2020 2020 2020 2057 6865 6e20 6060  .        When ``
+00001920: 6462 6060 2069 7320 616e 2065 7870 6c69  db`` is an expli
+00001930: 6369 7420 7073 7963 6f70 6732 2063 6f6e  cit psycopg2 con
+00001940: 6e65 6374 696f 6e2c 2074 6865 6e20 6060  nection, then ``
+00001950: 6d69 6e5f 706f 6f6c 5f63 6f6e 6e73 6060  min_pool_conns``
+00001960: 2061 6e64 0a20 2020 2020 2020 2060 606d   and.        ``m
+00001970: 6178 5f70 6f6f 6c5f 636f 6e6e 7360 6020  ax_pool_conns`` 
+00001980: 6172 6520 6967 6e6f 7265 6420 616e 6420  are ignored and 
+00001990: 7468 6520 636f 6e6e 6563 7469 6f6e 2069  the connection i
+000019a0: 7320 7573 6564 2064 6972 6563 746c 792e  s used directly.
+000019b0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+000019c0: 2020 2020 2020 2020 2020 2020 6462 3a20              db: 
+000019d0: 6569 7468 6572 2061 206c 6962 7071 2063  either a libpq c
+000019e0: 6f6e 6e65 6374 696f 6e20 7374 7269 6e67  onnection string
+000019f0: 2c20 6f72 2061 2070 7379 636f 7067 3220  , or a psycopg2 
+00001a00: 636f 6e6e 6563 7469 6f6e 0a20 2020 2020  connection.     
+00001a10: 2020 2020 2020 206f 626a 7374 6f72 6167         objstorag
+00001a20: 653a 2063 6f6e 6669 6775 7261 7469 6f6e  e: configuration
+00001a30: 2066 6f72 2074 6865 2062 6163 6b65 6e64   for the backend
+00001a40: 203a 636c 6173 733a 604f 626a 5374 6f72   :class:`ObjStor
+00001a50: 6167 6560 3b20 6966 2075 6e73 6574 2c0a  age`; if unset,.
+00001a60: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+00001a70: 7365 2061 204e 6f6f 704f 626a 5374 6f72  se a NoopObjStor
+00001a80: 6167 650a 2020 2020 2020 2020 2020 2020  age.            
+00001a90: 6d69 6e5f 706f 6f6c 5f63 6f6e 6e73 3a20  min_pool_conns: 
+00001aa0: 6d69 6e20 6e75 6d62 6572 206f 6620 636f  min number of co
+00001ab0: 6e6e 6563 7469 6f6e 7320 696e 2074 6865  nnections in the
+00001ac0: 2070 7379 636f 7067 3220 706f 6f6c 0a20   psycopg2 pool. 
+00001ad0: 2020 2020 2020 2020 2020 206d 6178 5f70             max_p
+00001ae0: 6f6f 6c5f 636f 6e6e 733a 206d 6178 206e  ool_conns: max n
+00001af0: 756d 6265 7220 6f66 2063 6f6e 6e65 6374  umber of connect
+00001b00: 696f 6e73 2069 6e20 7468 6520 7073 7963  ions in the psyc
+00001b10: 6f70 6732 2070 6f6f 6c0a 2020 2020 2020  opg2 pool.      
+00001b20: 2020 2020 2020 6a6f 7572 6e61 6c5f 7772        journal_wr
+00001b30: 6974 6572 3a20 636f 6e66 6967 7572 6174  iter: configurat
+00001b40: 696f 6e20 666f 7220 7468 6520 3a63 6c61  ion for the :cla
+00001b50: 7373 3a60 4a6f 7572 6e61 6c57 7269 7465  ss:`JournalWrite
+00001b60: 7260 0a20 2020 2020 2020 2020 2020 2071  r`.            q
+00001b70: 7565 7279 5f6f 7074 696f 6e73 3a20 636f  uery_options: co
+00001b80: 6e66 6967 7572 6174 696f 6e20 666f 7220  nfiguration for 
+00001b90: 7468 6520 7371 6c20 636f 6e6e 6563 7469  the sql connecti
+00001ba0: 6f6e 733b 206b 6579 7320 6f66 2074 6865  ons; keys of the
+00001bb0: 2064 6963 7420 6172 650a 2020 2020 2020   dict are.      
+00001bc0: 2020 2020 2020 2020 2074 6865 206d 6574           the met
+00001bd0: 686f 6420 6e61 6d65 7320 6465 636f 7261  hod names decora
+00001be0: 7465 6420 7769 7468 203a 6675 6e63 3a60  ted with :func:`
+00001bf0: 6462 5f74 7261 6e73 6163 7469 6f6e 6020  db_transaction` 
+00001c00: 6f72 0a20 2020 2020 2020 2020 2020 2020  or.             
+00001c10: 2020 3a66 756e 633a 6064 625f 7472 616e    :func:`db_tran
+00001c20: 7361 6374 696f 6e5f 6765 6e65 7261 746f  saction_generato
+00001c30: 7260 2028 6567 2e20 3a66 756e 633a 6063  r` (eg. :func:`c
+00001c40: 6f6e 7465 6e74 5f66 696e 6460 292c 2061  ontent_find`), a
+00001c50: 6e64 2076 616c 7565 730a 2020 2020 2020  nd values.      
+00001c60: 2020 2020 2020 2020 2061 7265 2064 6963           are dic
+00001c70: 7473 2028 636f 6e66 6967 5f6e 616d 652c  ts (config_name,
+00001c80: 2063 6f6e 6669 675f 7661 6c75 6529 2075   config_value) u
+00001c90: 7365 6420 746f 2063 6f6e 6669 6775 7265  sed to configure
+00001ca0: 2074 6865 2073 716c 0a20 2020 2020 2020   the sql.       
+00001cb0: 2020 2020 2020 2020 636f 6e6e 6563 7469          connecti
+00001cc0: 6f6e 2066 6f72 2074 6865 206d 6574 686f  on for the metho
+00001cd0: 645f 6e61 6d65 2e20 466f 7220 6578 616d  d_name. For exam
+00001ce0: 706c 652c 2075 7369 6e67 3a3a 0a0a 2020  ple, using::..  
+00001cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d00: 7b22 636f 6e74 656e 745f 6765 7422 3a20  {"content_get": 
+00001d10: 7b22 7374 6174 656d 656e 745f 7469 6d65  {"statement_time
+00001d20: 6f75 7422 3a20 3530 3030 7d7d 0a0a 2020  out": 5000}}..  
+00001d30: 2020 2020 2020 2020 2020 2020 2077 696c               wil
+00001d40: 6c20 6f76 6572 7269 6465 2074 6865 2064  l override the d
+00001d50: 6566 6175 6c74 2073 7461 7465 6d65 6e74  efault statement
+00001d60: 2074 696d 656f 7574 2066 6f72 2074 6865   timeout for the
+00001d70: 203a 6675 6e63 3a60 636f 6e74 656e 745f   :func:`content_
+00001d80: 6765 7460 0a20 2020 2020 2020 2020 2020  get`.           
+00001d90: 2020 2020 656e 6470 6f69 6e74 2066 726f      endpoint fro
+00001da0: 6d20 3530 306d 7320 746f 2035 3030 306d  m 500ms to 5000m
+00001db0: 732e 0a0a 2020 2020 2020 2020 2020 2020  s...            
+00001dc0: 2020 2053 6565 203a 6d6f 643a 6073 7768     See :mod:`swh
+00001dd0: 2e63 6f72 652e 6462 2e63 6f6d 6d6f 6e60  .core.db.common`
+00001de0: 2066 6f72 206d 6f72 6520 6465 7461 696c   for more detail
+00001df0: 732e 0a0a 2020 2020 2020 2020 2222 220a  s...        """.
+00001e00: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
+00001e10: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
+00001e20: 6e73 7461 6e63 6528 6462 2c20 7073 7963  nstance(db, psyc
+00001e30: 6f70 6732 2e65 7874 656e 7369 6f6e 732e  opg2.extensions.
+00001e40: 636f 6e6e 6563 7469 6f6e 293a 0a20 2020  connection):.   
+00001e50: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00001e60: 662e 5f70 6f6f 6c20 3d20 4e6f 6e65 0a20  f._pool = None. 
+00001e70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00001e80: 656c 662e 5f64 6220 3d20 4462 2864 6229  elf._db = Db(db)
+00001e90: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001ea0: 2020 2320 5365 6520 636f 6d6d 656e 7420    # See comment 
+00001eb0: 6265 6c6f 770a 2020 2020 2020 2020 2020  below.          
+00001ec0: 2020 2020 2020 7365 6c66 2e5f 6462 2e63        self._db.c
+00001ed0: 7572 736f 7228 292e 6578 6563 7574 6528  ursor().execute(
+00001ee0: 2253 4554 2054 494d 4520 5a4f 4e45 2027  "SET TIME ZONE '
+00001ef0: 5554 4327 2229 0a20 2020 2020 2020 2020  UTC'").         
+00001f00: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00001f10: 2020 2020 2020 2020 2073 656c 662e 5f70           self._p
+00001f20: 6f6f 6c20 3d20 7073 7963 6f70 6732 2e70  ool = psycopg2.p
+00001f30: 6f6f 6c2e 5468 7265 6164 6564 436f 6e6e  ool.ThreadedConn
+00001f40: 6563 7469 6f6e 506f 6f6c 280a 2020 2020  ectionPool(.    
+00001f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f60: 6d69 6e5f 706f 6f6c 5f63 6f6e 6e73 2c20  min_pool_conns, 
+00001f70: 6d61 785f 706f 6f6c 5f63 6f6e 6e73 2c20  max_pool_conns, 
+00001f80: 6462 0a20 2020 2020 2020 2020 2020 2020  db.             
+00001f90: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00001fa0: 2020 2020 2073 656c 662e 5f64 6220 3d20       self._db = 
+00001fb0: 4e6f 6e65 0a20 2020 2020 2020 2065 7863  None.        exc
+00001fc0: 6570 7420 7073 7963 6f70 6732 2e4f 7065  ept psycopg2.Ope
+00001fd0: 7261 7469 6f6e 616c 4572 726f 7220 6173  rationalError as
+00001fe0: 2065 3a0a 2020 2020 2020 2020 2020 2020   e:.            
+00001ff0: 7261 6973 6520 5374 6f72 6167 6544 4245  raise StorageDBE
+00002000: 7272 6f72 2865 290a 2020 2020 2020 2020  rror(e).        
+00002010: 7365 6c66 2e6a 6f75 726e 616c 5f77 7269  self.journal_wri
+00002020: 7465 7220 3d20 4a6f 7572 6e61 6c57 7269  ter = JournalWri
+00002030: 7465 7228 6a6f 7572 6e61 6c5f 7772 6974  ter(journal_writ
+00002040: 6572 290a 2020 2020 2020 2020 7365 6c66  er).        self
+00002050: 2e6f 626a 7374 6f72 6167 6520 3d20 4f62  .objstorage = Ob
+00002060: 6a53 746f 7261 6765 2873 656c 662c 206f  jStorage(self, o
+00002070: 626a 7374 6f72 6167 6529 0a20 2020 2020  bjstorage).     
+00002080: 2020 2073 656c 662e 7175 6572 795f 6f70     self.query_op
+00002090: 7469 6f6e 7320 3d20 7175 6572 795f 6f70  tions = query_op
+000020a0: 7469 6f6e 730a 2020 2020 2020 2020 7365  tions.        se
+000020b0: 6c66 2e5f 666c 6176 6f72 3a20 4f70 7469  lf._flavor: Opti
+000020c0: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+000020d0: 0a0a 2020 2020 2323 2323 2323 2323 2323  ..    ##########
+000020e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000020f0: 0a20 2020 2023 2055 7469 6c69 7469 6573  .    # Utilities
+00002100: 0a20 2020 2023 2323 2323 2323 2323 2323  .    ###########
+00002110: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
+00002120: 0a20 2020 2064 6566 2067 6574 5f64 6228  .    def get_db(
+00002130: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
+00002140: 6620 7365 6c66 2e5f 6462 3a0a 2020 2020  f self._db:.    
+00002150: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00002160: 656c 662e 5f64 620a 2020 2020 2020 2020  elf._db.        
+00002170: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00002180: 2020 6462 203d 2044 622e 6672 6f6d 5f70    db = Db.from_p
+00002190: 6f6f 6c28 7365 6c66 2e5f 706f 6f6c 290a  ool(self._pool).
+000021a0: 0a20 2020 2020 2020 2020 2020 2023 2057  .            # W
+000021b0: 6f72 6b61 726f 756e 6420 666f 7220 7073  orkaround for ps
+000021c0: 7963 6f70 6732 203c 2032 2e39 2e30 206e  ycopg2 < 2.9.0 n
+000021d0: 6f74 2068 616e 646c 696e 6720 6672 6163  ot handling frac
+000021e0: 7469 6f6e 616c 2074 696d 657a 6f6e 6573  tional timezones
+000021f0: 2c0a 2020 2020 2020 2020 2020 2020 2320  ,.            # 
+00002200: 7768 6963 6820 6d61 7920 6861 7070 656e  which may happen
+00002210: 206f 6e20 6f6c 6420 7265 7669 7369 6f6e   on old revision
+00002220: 2f72 656c 6561 7365 2064 6174 6573 206f  /release dates o
+00002230: 6e20 7379 7374 656d 7320 636f 6e66 6967  n systems config
+00002240: 7572 6564 0a20 2020 2020 2020 2020 2020  ured.           
+00002250: 2023 2077 6974 6820 6e6f 6e2d 5554 4320   # with non-UTC 
+00002260: 7469 6d65 7a6f 6e65 732e 0a20 2020 2020  timezones..     
+00002270: 2020 2020 2020 2023 2068 7474 7073 3a2f         # https:/
+00002280: 2f77 7777 2e70 7379 636f 7067 2e6f 7267  /www.psycopg.org
+00002290: 2f64 6f63 732f 7573 6167 652e 6874 6d6c  /docs/usage.html
+000022a0: 2374 696d 652d 7a6f 6e65 732d 6861 6e64  #time-zones-hand
+000022b0: 6c69 6e67 0a20 2020 2020 2020 2020 2020  ling.           
+000022c0: 2064 622e 6375 7273 6f72 2829 2e65 7865   db.cursor().exe
+000022d0: 6375 7465 2822 5345 5420 5449 4d45 205a  cute("SET TIME Z
+000022e0: 4f4e 4520 2755 5443 2722 290a 0a20 2020  ONE 'UTC'")..   
+000022f0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00002300: 6462 0a0a 2020 2020 6465 6620 7075 745f  db..    def put_
+00002310: 6462 2873 656c 662c 2064 6229 3a0a 2020  db(self, db):.  
+00002320: 2020 2020 2020 6966 2064 6220 6973 206e        if db is n
+00002330: 6f74 2073 656c 662e 5f64 623a 0a20 2020  ot self._db:.   
+00002340: 2020 2020 2020 2020 2064 622e 7075 745f           db.put_
+00002350: 636f 6e6e 2829 0a0a 2020 2020 4063 6f6e  conn()..    @con
+00002360: 7465 7874 6d61 6e61 6765 720a 2020 2020  textmanager.    
+00002370: 6465 6620 6462 2873 656c 6629 3a0a 2020  def db(self):.  
+00002380: 2020 2020 2020 6462 203d 204e 6f6e 650a        db = None.
+00002390: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+000023a0: 2020 2020 2020 2020 2064 6220 3d20 7365           db = se
+000023b0: 6c66 2e67 6574 5f64 6228 290a 2020 2020  lf.get_db().    
+000023c0: 2020 2020 2020 2020 7969 656c 6420 6462          yield db
+000023d0: 0a20 2020 2020 2020 2066 696e 616c 6c79  .        finally
+000023e0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+000023f0: 2064 623a 0a20 2020 2020 2020 2020 2020   db:.           
+00002400: 2020 2020 2073 656c 662e 7075 745f 6462       self.put_db
+00002410: 2864 6229 0a0a 2020 2020 4064 625f 7472  (db)..    @db_tr
+00002420: 616e 7361 6374 696f 6e28 290a 2020 2020  ansaction().    
+00002430: 6465 6620 6765 745f 666c 6176 6f72 2873  def get_flavor(s
+00002440: 656c 662c 202a 2c20 6462 3a20 4462 2c20  elf, *, db: Db, 
+00002450: 6375 723d 4e6f 6e65 2920 2d3e 2073 7472  cur=None) -> str
+00002460: 3a0a 2020 2020 2020 2020 666c 6176 6f72  :.        flavor
+00002470: 203d 2073 7768 5f64 625f 666c 6176 6f72   = swh_db_flavor
+00002480: 2864 622e 636f 6e6e 2e64 736e 290a 2020  (db.conn.dsn).  
+00002490: 2020 2020 2020 6173 7365 7274 2066 6c61        assert fla
+000024a0: 766f 7220 6973 206e 6f74 204e 6f6e 650a  vor is not None.
+000024b0: 2020 2020 2020 2020 7265 7475 726e 2066          return f
+000024c0: 6c61 766f 720a 0a20 2020 2040 7072 6f70  lavor..    @prop
+000024d0: 6572 7479 0a20 2020 2064 6566 2066 6c61  erty.    def fla
+000024e0: 766f 7228 7365 6c66 2920 2d3e 2073 7472  vor(self) -> str
+000024f0: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
+00002500: 662e 5f66 6c61 766f 7220 6973 204e 6f6e  f._flavor is Non
+00002510: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00002520: 656c 662e 5f66 6c61 766f 7220 3d20 7365  elf._flavor = se
+00002530: 6c66 2e67 6574 5f66 6c61 766f 7228 290a  lf.get_flavor().
+00002540: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
+00002550: 656c 662e 5f66 6c61 766f 7220 6973 206e  elf._flavor is n
+00002560: 6f74 204e 6f6e 650a 2020 2020 2020 2020  ot None.        
+00002570: 7265 7475 726e 2073 656c 662e 5f66 6c61  return self._fla
+00002580: 766f 720a 0a20 2020 2040 6462 5f74 7261  vor..    @db_tra
+00002590: 6e73 6163 7469 6f6e 2829 0a20 2020 2064  nsaction().    d
+000025a0: 6566 2063 6865 636b 5f63 6f6e 6669 6728  ef check_config(
+000025b0: 7365 6c66 2c20 2a2c 2063 6865 636b 5f77  self, *, check_w
+000025c0: 7269 7465 3a20 626f 6f6c 2c20 6462 3a20  rite: bool, db: 
+000025d0: 4462 2c20 6375 723d 4e6f 6e65 2920 2d3e  Db, cur=None) ->
+000025e0: 2062 6f6f 6c3a 0a20 2020 2020 2020 2069   bool:.        i
+000025f0: 6620 6e6f 7420 7365 6c66 2e6f 626a 7374  f not self.objst
+00002600: 6f72 6167 652e 6368 6563 6b5f 636f 6e66  orage.check_conf
+00002610: 6967 2863 6865 636b 5f77 7269 7465 3d63  ig(check_write=c
+00002620: 6865 636b 5f77 7269 7465 293a 0a20 2020  heck_write):.   
+00002630: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00002640: 4661 6c73 650a 0a20 2020 2020 2020 2064  False..        d
+00002650: 6276 6572 7369 6f6e 203d 2073 7768 5f64  bversion = swh_d
+00002660: 625f 7665 7273 696f 6e28 6462 2e63 6f6e  b_version(db.con
+00002670: 6e2e 6473 6e29 0a20 2020 2020 2020 2069  n.dsn).        i
+00002680: 6620 6462 7665 7273 696f 6e20 213d 2073  f dbversion != s
+00002690: 656c 662e 6375 7272 656e 745f 7665 7273  elf.current_vers
+000026a0: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
+000026b0: 206c 6f67 6765 722e 7761 726e 696e 6728   logger.warning(
+000026c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000026d0: 2022 6461 7461 6261 7365 2064 6276 6572   "database dbver
+000026e0: 7369 6f6e 2028 2573 2920 213d 2025 7320  sion (%s) != %s 
+000026f0: 6375 7272 656e 745f 7665 7273 696f 6e20  current_version 
+00002700: 2825 7329 222c 0a20 2020 2020 2020 2020  (%s)",.         
+00002710: 2020 2020 2020 2064 6276 6572 7369 6f6e         dbversion
+00002720: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002730: 2020 5f5f 6e61 6d65 5f5f 2c0a 2020 2020    __name__,.    
+00002740: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00002750: 2e63 7572 7265 6e74 5f76 6572 7369 6f6e  .current_version
+00002760: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+00002770: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00002780: 726e 2046 616c 7365 0a0a 2020 2020 2020  rn False..      
+00002790: 2020 2320 4368 6563 6b20 7065 726d 6973    # Check permis
+000027a0: 7369 6f6e 7320 6f6e 206f 6e65 206f 6620  sions on one of 
+000027b0: 7468 6520 7461 626c 6573 0a20 2020 2020  the tables.     
+000027c0: 2020 2063 6865 636b 203d 2022 494e 5345     check = "INSE
+000027d0: 5254 2220 6966 2063 6865 636b 5f77 7269  RT" if check_wri
+000027e0: 7465 2065 6c73 6520 2253 454c 4543 5422  te else "SELECT"
+000027f0: 0a0a 2020 2020 2020 2020 6375 722e 6578  ..        cur.ex
+00002800: 6563 7574 6528 2273 656c 6563 7420 6861  ecute("select ha
+00002810: 735f 7461 626c 655f 7072 6976 696c 6567  s_table_privileg
+00002820: 6528 6375 7272 656e 745f 7573 6572 2c20  e(current_user, 
+00002830: 2763 6f6e 7465 6e74 272c 2025 7329 222c  'content', %s)",
+00002840: 2028 6368 6563 6b2c 2929 0a20 2020 2020   (check,)).     
+00002850: 2020 2072 6574 7572 6e20 6375 722e 6665     return cur.fe
+00002860: 7463 686f 6e65 2829 5b30 5d0a 0a20 2020  tchone()[0]..   
+00002870: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
+00002880: 2323 2323 2323 2323 2323 230a 2020 2020  ###########.    
+00002890: 2320 436f 6e74 656e 740a 2020 2020 2323  # Content.    ##
 000028a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000028b0: 0a0a 2020 2020 6465 6620 5f63 6f6e 7465  ..    def _conte
-000028c0: 6e74 5f75 6e69 7175 655f 6b65 7928 7365  nt_unique_key(se
-000028d0: 6c66 2c20 6861 7368 2c20 6462 293a 0a20  lf, hash, db):. 
-000028e0: 2020 2020 2020 2022 2222 4769 7665 6e20         """Given 
-000028f0: 6120 6861 7368 2028 7475 706c 6520 6f72  a hash (tuple or
-00002900: 2064 6963 7429 2c20 7265 7475 726e 2061   dict), return a
-00002910: 2075 6e69 7175 6520 6b65 7920 6672 6f6d   unique key from
-00002920: 2074 6865 0a20 2020 2020 2020 2061 6767   the.        agg
-00002930: 7265 6761 7469 6f6e 206f 6620 6b65 7973  regation of keys
-00002940: 2e0a 0a20 2020 2020 2020 2022 2222 0a20  ...        """. 
-00002950: 2020 2020 2020 206b 6579 7320 3d20 6462         keys = db
-00002960: 2e63 6f6e 7465 6e74 5f68 6173 685f 6b65  .content_hash_ke
-00002970: 7973 0a20 2020 2020 2020 2069 6620 6973  ys.        if is
-00002980: 696e 7374 616e 6365 2868 6173 682c 2074  instance(hash, t
-00002990: 7570 6c65 293a 0a20 2020 2020 2020 2020  uple):.         
-000029a0: 2020 2072 6574 7572 6e20 6861 7368 0a20     return hash. 
-000029b0: 2020 2020 2020 2072 6574 7572 6e20 7475         return tu
-000029c0: 706c 6528 5b68 6173 685b 6b5d 2066 6f72  ple([hash[k] for
-000029d0: 206b 2069 6e20 6b65 7973 5d29 0a0a 2020   k in keys])..  
-000029e0: 2020 6465 6620 5f63 6f6e 7465 6e74 5f61    def _content_a
-000029f0: 6464 5f6d 6574 6164 6174 6128 7365 6c66  dd_metadata(self
-00002a00: 2c20 6462 2c20 6375 722c 2063 6f6e 7465  , db, cur, conte
-00002a10: 6e74 293a 0a20 2020 2020 2020 2022 2222  nt):.        """
-00002a20: 4164 6420 636f 6e74 656e 7420 746f 2074  Add content to t
-00002a30: 6865 2070 6f73 7467 7265 7371 6c20 6461  he postgresql da
-00002a40: 7461 6261 7365 2062 7574 206e 6f74 2074  tabase but not t
-00002a50: 6865 206f 626a 6563 7420 7374 6f72 6167  he object storag
-00002a60: 652e 2222 220a 2020 2020 2020 2020 2320  e.""".        # 
-00002a70: 6372 6561 7465 2074 656d 706f 7261 7279  create temporary
-00002a80: 2074 6162 6c65 2066 6f72 206d 6574 6164   table for metad
-00002a90: 6174 6120 696e 6a65 6374 696f 6e0a 2020  ata injection.  
-00002aa0: 2020 2020 2020 6462 2e6d 6b74 656d 7028        db.mktemp(
-00002ab0: 2263 6f6e 7465 6e74 222c 2063 7572 290a  "content", cur).
-00002ac0: 0a20 2020 2020 2020 2064 622e 636f 7079  .        db.copy
-00002ad0: 5f74 6f28 0a20 2020 2020 2020 2020 2020  _to(.           
-00002ae0: 2028 632e 746f 5f64 6963 7428 2920 666f   (c.to_dict() fo
-00002af0: 7220 6320 696e 2063 6f6e 7465 6e74 292c  r c in content),
-00002b00: 2022 746d 705f 636f 6e74 656e 7422 2c20   "tmp_content", 
-00002b10: 6462 2e63 6f6e 7465 6e74 5f61 6464 5f6b  db.content_add_k
-00002b20: 6579 732c 2063 7572 0a20 2020 2020 2020  eys, cur.       
-00002b30: 2029 0a0a 2020 2020 2020 2020 2320 6d6f   )..        # mo
-00002b40: 7665 206d 6574 6164 6174 6120 696e 2070  ve metadata in p
-00002b50: 6c61 6365 0a20 2020 2020 2020 2074 7279  lace.        try
-00002b60: 3a0a 2020 2020 2020 2020 2020 2020 6462  :.            db
-00002b70: 2e63 6f6e 7465 6e74 5f61 6464 5f66 726f  .content_add_fro
-00002b80: 6d5f 7465 6d70 2863 7572 290a 2020 2020  m_temp(cur).    
-00002b90: 2020 2020 6578 6365 7074 2070 7379 636f      except psyco
-00002ba0: 7067 322e 496e 7465 6772 6974 7945 7272  pg2.IntegrityErr
-00002bb0: 6f72 2061 7320 653a 0a20 2020 2020 2020  or as e:.       
-00002bc0: 2020 2020 2069 6620 652e 6469 6167 2e73       if e.diag.s
-00002bd0: 716c 7374 6174 6520 3d3d 2022 3233 3530  qlstate == "2350
-00002be0: 3522 2061 6e64 2065 2e64 6961 672e 7461  5" and e.diag.ta
-00002bf0: 626c 655f 6e61 6d65 203d 3d20 2263 6f6e  ble_name == "con
-00002c00: 7465 6e74 223a 0a20 2020 2020 2020 2020  tent":.         
-00002c10: 2020 2020 2020 206d 6573 7361 6765 5f64         message_d
-00002c20: 6574 6169 6c20 3d20 652e 6469 6167 2e6d  etail = e.diag.m
-00002c30: 6573 7361 6765 5f64 6574 6169 6c0a 2020  essage_detail.  
-00002c40: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00002c50: 206d 6573 7361 6765 5f64 6574 6169 6c3a   message_detail:
-00002c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002c70: 2020 2020 2068 6173 685f 6e61 6d65 2c20       hash_name, 
-00002c80: 6861 7368 5f69 6420 3d20 6578 7472 6163  hash_id = extrac
-00002c90: 745f 636f 6c6c 6973 696f 6e5f 6861 7368  t_collision_hash
-00002ca0: 286d 6573 7361 6765 5f64 6574 6169 6c29  (message_detail)
-00002cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002cc0: 2020 2020 2063 6f6c 6c69 7369 6f6e 5f63       collision_c
-00002cd0: 6f6e 7465 6e74 735f 6861 7368 6573 203d  ontents_hashes =
-00002ce0: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
-00002cf0: 2020 2020 2020 2020 2020 2063 2e68 6173             c.has
-00002d00: 6865 7328 2920 666f 7220 6320 696e 2063  hes() for c in c
-00002d10: 6f6e 7465 6e74 2069 6620 632e 6765 745f  ontent if c.get_
-00002d20: 6861 7368 2868 6173 685f 6e61 6d65 2920  hash(hash_name) 
-00002d30: 3d3d 2068 6173 685f 6964 0a20 2020 2020  == hash_id.     
-00002d40: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-00002d50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002d60: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00002d70: 2020 2020 2020 2020 2020 2063 6f6e 7374             const
-00002d80: 7261 696e 745f 746f 5f68 6173 685f 6e61  raint_to_hash_na
-00002d90: 6d65 203d 207b 0a20 2020 2020 2020 2020  me = {.         
-00002da0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002db0: 636f 6e74 656e 745f 706b 6579 223a 2022  content_pkey": "
-00002dc0: 7368 6131 222c 0a20 2020 2020 2020 2020  sha1",.         
-00002dd0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002de0: 636f 6e74 656e 745f 7368 6131 5f67 6974  content_sha1_git
-00002df0: 5f69 6478 223a 2022 7368 6131 5f67 6974  _idx": "sha1_git
-00002e00: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00002e10: 2020 2020 2020 2020 2020 2022 636f 6e74             "cont
-00002e20: 656e 745f 7368 6132 3536 5f69 6478 223a  ent_sha256_idx":
-00002e30: 2022 7368 6132 3536 222c 0a20 2020 2020   "sha256",.     
-00002e40: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00002e50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002e60: 2020 2020 2068 6173 685f 6e61 6d65 203d       hash_name =
-00002e70: 2063 6f6e 7374 7261 696e 745f 746f 5f68   constraint_to_h
-00002e80: 6173 685f 6e61 6d65 2e67 6574 2865 2e64  ash_name.get(e.d
-00002e90: 6961 672e 636f 6e73 7472 6169 6e74 5f6e  iag.constraint_n
-00002ea0: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
-00002eb0: 2020 2020 2020 2020 2068 6173 685f 6964           hash_id
-00002ec0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-00002ed0: 2020 2020 2020 2020 2020 2020 636f 6c6c              coll
-00002ee0: 6973 696f 6e5f 636f 6e74 656e 7473 5f68  ision_contents_h
-00002ef0: 6173 6865 7320 3d20 4e6f 6e65 0a0a 2020  ashes = None..  
-00002f00: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-00002f10: 6973 6520 4861 7368 436f 6c6c 6973 696f  ise HashCollisio
-00002f20: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
-00002f30: 2020 2020 2020 2068 6173 685f 6e61 6d65         hash_name
-00002f40: 2c20 6861 7368 5f69 642c 2063 6f6c 6c69  , hash_id, colli
-00002f50: 7369 6f6e 5f63 6f6e 7465 6e74 735f 6861  sion_contents_ha
-00002f60: 7368 6573 0a20 2020 2020 2020 2020 2020  shes.           
-00002f70: 2020 2020 2029 2066 726f 6d20 4e6f 6e65       ) from None
-00002f80: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00002f90: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00002fa0: 2020 2072 6169 7365 0a0a 2020 2020 6465     raise..    de
-00002fb0: 6620 636f 6e74 656e 745f 6164 6428 7365  f content_add(se
-00002fc0: 6c66 2c20 636f 6e74 656e 743a 204c 6973  lf, content: Lis
-00002fd0: 745b 436f 6e74 656e 745d 2920 2d3e 2044  t[Content]) -> D
-00002fe0: 6963 745b 7374 722c 2069 6e74 5d3a 0a20  ict[str, int]:. 
-00002ff0: 2020 2020 2020 2063 7469 6d65 203d 206e         ctime = n
-00003000: 6f77 2829 0a0a 2020 2020 2020 2020 636f  ow()..        co
-00003010: 6e74 656e 7473 203d 205b 6174 7472 2e65  ntents = [attr.e
-00003020: 766f 6c76 6528 632c 2063 7469 6d65 3d63  volve(c, ctime=c
-00003030: 7469 6d65 2920 666f 7220 6320 696e 2063  time) for c in c
-00003040: 6f6e 7465 6e74 5d0a 0a20 2020 2020 2020  ontent]..       
-00003050: 2023 204d 7573 7420 6164 6420 746f 2074   # Must add to t
-00003060: 6865 206f 626a 7374 6f72 6167 6520 6265  he objstorage be
-00003070: 666f 7265 2074 6865 2044 4220 616e 6420  fore the DB and 
-00003080: 6a6f 7572 6e61 6c2e 204f 7468 6572 7769  journal. Otherwi
-00003090: 7365 3a0a 2020 2020 2020 2020 2320 312e  se:.        # 1.
-000030a0: 2069 6e20 6361 7365 206f 6620 6120 6372   in case of a cr
-000030b0: 6173 6820 7468 6520 4442 206d 6179 2022  ash the DB may "
-000030c0: 6265 6c69 6576 6522 2077 6520 6861 7665  believe" we have
-000030d0: 2074 6865 2063 6f6e 7465 6e74 2c20 6275   the content, bu
-000030e0: 740a 2020 2020 2020 2020 2320 2020 2077  t.        #    w
-000030f0: 6520 6469 646e 2774 2068 6176 6520 7469  e didn't have ti
-00003100: 6d65 2074 6f20 7772 6974 6520 746f 2074  me to write to t
-00003110: 6865 206f 626a 7374 6f72 6167 6520 6265  he objstorage be
-00003120: 666f 7265 2074 6865 2063 7261 7368 0a20  fore the crash. 
-00003130: 2020 2020 2020 2023 2032 2e20 7468 6520         # 2. the 
-00003140: 6f62 6a73 746f 7261 6765 206d 6972 726f  objstorage mirro
-00003150: 7269 6e67 2c20 7768 6963 6820 7265 6164  ring, which read
-00003160: 7320 6672 6f6d 2074 6865 206a 6f75 726e  s from the journ
-00003170: 616c 2c20 6d61 7920 6174 7465 6d70 7420  al, may attempt 
-00003180: 746f 0a20 2020 2020 2020 2023 2020 2020  to.        #    
-00003190: 7265 6164 2066 726f 6d20 7468 6520 6f62  read from the ob
-000031a0: 6a73 746f 7261 6765 2062 6566 6f72 6520  jstorage before 
-000031b0: 7765 2066 696e 6973 6865 6420 7772 6974  we finished writ
-000031c0: 696e 6720 6974 0a20 2020 2020 2020 206f  ing it.        o
-000031d0: 626a 7374 6f72 6167 655f 7375 6d6d 6172  bjstorage_summar
-000031e0: 7920 3d20 7365 6c66 2e6f 626a 7374 6f72  y = self.objstor
-000031f0: 6167 652e 636f 6e74 656e 745f 6164 6428  age.content_add(
-00003200: 636f 6e74 656e 7473 290a 0a20 2020 2020  contents)..     
-00003210: 2020 2077 6974 6820 7365 6c66 2e64 6228     with self.db(
-00003220: 2920 6173 2064 623a 0a20 2020 2020 2020  ) as db:.       
-00003230: 2020 2020 2077 6974 6820 6462 2e74 7261       with db.tra
-00003240: 6e73 6163 7469 6f6e 2829 2061 7320 6375  nsaction() as cu
-00003250: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
-00003260: 2020 206d 6973 7369 6e67 203d 2073 6574     missing = set
-00003270: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00003280: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
-00003290: 6e74 5f6d 6973 7369 6e67 280a 2020 2020  nt_missing(.    
-000032a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032b0: 2020 2020 5b63 2e74 6f5f 6469 6374 2829      [c.to_dict()
-000032c0: 2066 6f72 2063 2069 6e20 636f 6e74 656e   for c in conten
-000032d0: 7473 5d2c 0a20 2020 2020 2020 2020 2020  ts],.           
-000032e0: 2020 2020 2020 2020 2020 2020 206b 6579               key
-000032f0: 5f68 6173 683d 2273 6861 315f 6769 7422  _hash="sha1_git"
-00003300: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00003310: 2020 2020 2020 2020 2020 6462 3d64 622c            db=db,
-00003320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003330: 2020 2020 2020 2020 2063 7572 3d63 7572           cur=cur
-00003340: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00003350: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00003360: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00003370: 2020 2020 2020 2020 2020 636f 6e74 656e            conten
-00003380: 7473 203d 205b 6320 666f 7220 6320 696e  ts = [c for c in
-00003390: 2063 6f6e 7465 6e74 7320 6966 2063 2e73   contents if c.s
-000033a0: 6861 315f 6769 7420 696e 206d 6973 7369  ha1_git in missi
-000033b0: 6e67 5d0a 0a20 2020 2020 2020 2020 2020  ng]..           
-000033c0: 2020 2020 2073 656c 662e 6a6f 7572 6e61       self.journa
-000033d0: 6c5f 7772 6974 6572 2e63 6f6e 7465 6e74  l_writer.content
-000033e0: 5f61 6464 2863 6f6e 7465 6e74 7329 0a20  _add(contents). 
-000033f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00003400: 656c 662e 5f63 6f6e 7465 6e74 5f61 6464  elf._content_add
-00003410: 5f6d 6574 6164 6174 6128 6462 2c20 6375  _metadata(db, cu
-00003420: 722c 2063 6f6e 7465 6e74 7329 0a0a 2020  r, contents)..  
-00003430: 2020 2020 2020 7265 7475 726e 207b 0a20        return {. 
-00003440: 2020 2020 2020 2020 2020 2022 636f 6e74             "cont
-00003450: 656e 743a 6164 6422 3a20 6c65 6e28 636f  ent:add": len(co
-00003460: 6e74 656e 7473 292c 0a20 2020 2020 2020  ntents),.       
-00003470: 2020 2020 2022 636f 6e74 656e 743a 6164       "content:ad
-00003480: 643a 6279 7465 7322 3a20 6f62 6a73 746f  d:bytes": objsto
-00003490: 7261 6765 5f73 756d 6d61 7279 5b22 636f  rage_summary["co
-000034a0: 6e74 656e 743a 6164 643a 6279 7465 7322  ntent:add:bytes"
-000034b0: 5d2c 0a20 2020 2020 2020 207d 0a0a 2020  ],.        }..  
-000034c0: 2020 4064 625f 7472 616e 7361 6374 696f    @db_transactio
-000034d0: 6e28 290a 2020 2020 6465 6620 636f 6e74  n().    def cont
-000034e0: 656e 745f 7570 6461 7465 280a 2020 2020  ent_update(.    
-000034f0: 2020 2020 7365 6c66 2c20 636f 6e74 656e      self, conten
-00003500: 7473 3a20 4c69 7374 5b44 6963 745b 7374  ts: List[Dict[st
-00003510: 722c 2041 6e79 5d5d 2c20 6b65 7973 3a20  r, Any]], keys: 
-00003520: 4c69 7374 5b73 7472 5d20 3d20 5b5d 2c20  List[str] = [], 
-00003530: 2a2c 2064 623a 2044 622c 2063 7572 3d4e  *, db: Db, cur=N
-00003540: 6f6e 650a 2020 2020 2920 2d3e 204e 6f6e  one.    ) -> Non
-00003550: 653a 0a20 2020 2020 2020 2023 2054 4f44  e:.        # TOD
-00003560: 4f3a 2041 6464 2061 2063 6865 636b 206f  O: Add a check o
-00003570: 6e20 696e 7075 7420 6b65 7973 2e20 486f  n input keys. Ho
-00003580: 7720 746f 2070 726f 7065 726c 7920 696d  w to properly im
-00003590: 706c 656d 656e 740a 2020 2020 2020 2020  plement.        
-000035a0: 2320 7468 6973 3f20 5765 2064 6f6e 2774  # this? We don't
-000035b0: 206b 6e6f 7720 7965 7420 7468 6520 6e65   know yet the ne
-000035c0: 7720 636f 6c75 6d6e 732e 0a20 2020 2020  w columns..     
-000035d0: 2020 2073 656c 662e 6a6f 7572 6e61 6c5f     self.journal_
-000035e0: 7772 6974 6572 2e63 6f6e 7465 6e74 5f75  writer.content_u
-000035f0: 7064 6174 6528 636f 6e74 656e 7473 290a  pdate(contents).
-00003600: 0a20 2020 2020 2020 2064 622e 6d6b 7465  .        db.mkte
-00003610: 6d70 2822 636f 6e74 656e 7422 2c20 6375  mp("content", cu
-00003620: 7229 0a20 2020 2020 2020 2073 656c 6563  r).        selec
-00003630: 745f 6b65 7973 203d 206c 6973 7428 7365  t_keys = list(se
-00003640: 7428 6462 2e63 6f6e 7465 6e74 5f67 6574  t(db.content_get
-00003650: 5f6d 6574 6164 6174 615f 6b65 7973 292e  _metadata_keys).
-00003660: 756e 696f 6e28 7365 7428 6b65 7973 2929  union(set(keys))
-00003670: 290a 2020 2020 2020 2020 7769 7468 2063  ).        with c
-00003680: 6f6e 7665 7274 5f76 616c 6964 6174 696f  onvert_validatio
-00003690: 6e5f 6578 6365 7074 696f 6e73 2829 3a0a  n_exceptions():.
-000036a0: 2020 2020 2020 2020 2020 2020 6462 2e63              db.c
-000036b0: 6f70 795f 746f 2863 6f6e 7465 6e74 732c  opy_to(contents,
-000036c0: 2022 746d 705f 636f 6e74 656e 7422 2c20   "tmp_content", 
-000036d0: 7365 6c65 6374 5f6b 6579 732c 2063 7572  select_keys, cur
-000036e0: 290a 2020 2020 2020 2020 2020 2020 6462  ).            db
-000036f0: 2e63 6f6e 7465 6e74 5f75 7064 6174 655f  .content_update_
-00003700: 6672 6f6d 5f74 656d 7028 6b65 7973 5f74  from_temp(keys_t
-00003710: 6f5f 7570 6461 7465 3d6b 6579 732c 2063  o_update=keys, c
-00003720: 7572 3d63 7572 290a 0a20 2020 2040 6462  ur=cur)..    @db
-00003730: 5f74 7261 6e73 6163 7469 6f6e 2829 0a20  _transaction(). 
-00003740: 2020 2064 6566 2063 6f6e 7465 6e74 5f61     def content_a
-00003750: 6464 5f6d 6574 6164 6174 6128 0a20 2020  dd_metadata(.   
-00003760: 2020 2020 2073 656c 662c 2063 6f6e 7465       self, conte
-00003770: 6e74 3a20 4c69 7374 5b43 6f6e 7465 6e74  nt: List[Content
-00003780: 5d2c 202a 2c20 6462 3a20 4462 2c20 6375  ], *, db: Db, cu
-00003790: 723d 4e6f 6e65 0a20 2020 2029 202d 3e20  r=None.    ) -> 
-000037a0: 4469 6374 5b73 7472 2c20 696e 745d 3a0a  Dict[str, int]:.
-000037b0: 2020 2020 2020 2020 6d69 7373 696e 6720          missing 
-000037c0: 3d20 7365 7428 0a20 2020 2020 2020 2020  = set(.         
-000037d0: 2020 2073 656c 662e 636f 6e74 656e 745f     self.content_
-000037e0: 6d69 7373 696e 6728 0a20 2020 2020 2020  missing(.       
-000037f0: 2020 2020 2020 2020 205b 632e 746f 5f64           [c.to_d
-00003800: 6963 7428 2920 666f 7220 6320 696e 2063  ict() for c in c
-00003810: 6f6e 7465 6e74 5d2c 0a20 2020 2020 2020  ontent],.       
-00003820: 2020 2020 2020 2020 206b 6579 5f68 6173           key_has
-00003830: 683d 2273 6861 315f 6769 7422 2c0a 2020  h="sha1_git",.  
-00003840: 2020 2020 2020 2020 2020 2020 2020 6462                db
-00003850: 3d64 622c 0a20 2020 2020 2020 2020 2020  =db,.           
-00003860: 2020 2020 2063 7572 3d63 7572 2c0a 2020       cur=cur,.  
-00003870: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00003880: 2020 2020 290a 2020 2020 2020 2020 636f      ).        co
-00003890: 6e74 656e 7473 203d 205b 6320 666f 7220  ntents = [c for 
-000038a0: 6320 696e 2063 6f6e 7465 6e74 2069 6620  c in content if 
-000038b0: 632e 7368 6131 5f67 6974 2069 6e20 6d69  c.sha1_git in mi
-000038c0: 7373 696e 675d 0a0a 2020 2020 2020 2020  ssing]..        
-000038d0: 7365 6c66 2e6a 6f75 726e 616c 5f77 7269  self.journal_wri
-000038e0: 7465 722e 636f 6e74 656e 745f 6164 645f  ter.content_add_
-000038f0: 6d65 7461 6461 7461 2863 6f6e 7465 6e74  metadata(content
-00003900: 7329 0a20 2020 2020 2020 2073 656c 662e  s).        self.
-00003910: 5f63 6f6e 7465 6e74 5f61 6464 5f6d 6574  _content_add_met
-00003920: 6164 6174 6128 6462 2c20 6375 722c 2063  adata(db, cur, c
-00003930: 6f6e 7465 6e74 7329 0a0a 2020 2020 2020  ontents)..      
-00003940: 2020 7265 7475 726e 207b 0a20 2020 2020    return {.     
-00003950: 2020 2020 2020 2022 636f 6e74 656e 743a         "content:
-00003960: 6164 6422 3a20 6c65 6e28 636f 6e74 656e  add": len(conten
-00003970: 7473 292c 0a20 2020 2020 2020 207d 0a0a  ts),.        }..
-00003980: 2020 2020 6465 6620 636f 6e74 656e 745f      def content_
-00003990: 6765 745f 6461 7461 2873 656c 662c 2063  get_data(self, c
-000039a0: 6f6e 7465 6e74 3a20 556e 696f 6e5b 4861  ontent: Union[Ha
-000039b0: 7368 4469 6374 2c20 5368 6131 5d29 202d  shDict, Sha1]) -
-000039c0: 3e20 4f70 7469 6f6e 616c 5b62 7974 6573  > Optional[bytes
-000039d0: 5d3a 0a20 2020 2020 2020 2023 2046 4958  ]:.        # FIX
-000039e0: 4d45 3a20 4d61 6b65 2074 6869 7320 6d65  ME: Make this me
-000039f0: 7468 6f64 2073 7570 706f 7274 2073 6c69  thod support sli
-00003a00: 6369 6e67 2074 6865 2060 6461 7461 600a  cing the `data`.
-00003a10: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00003a20: 656c 662e 6f62 6a73 746f 7261 6765 2e63  elf.objstorage.c
-00003a30: 6f6e 7465 6e74 5f67 6574 2863 6f6e 7465  ontent_get(conte
-00003a40: 6e74 290a 0a20 2020 2040 6462 5f74 7261  nt)..    @db_tra
-00003a50: 6e73 6163 7469 6f6e 2829 0a20 2020 2064  nsaction().    d
-00003a60: 6566 2063 6f6e 7465 6e74 5f67 6574 5f70  ef content_get_p
-00003a70: 6172 7469 7469 6f6e 280a 2020 2020 2020  artition(.      
-00003a80: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00003a90: 7061 7274 6974 696f 6e5f 6964 3a20 696e  partition_id: in
-00003aa0: 742c 0a20 2020 2020 2020 206e 625f 7061  t,.        nb_pa
-00003ab0: 7274 6974 696f 6e73 3a20 696e 742c 0a20  rtitions: int,. 
-00003ac0: 2020 2020 2020 2070 6167 655f 746f 6b65         page_toke
-00003ad0: 6e3a 204f 7074 696f 6e61 6c5b 7374 725d  n: Optional[str]
-00003ae0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00003af0: 206c 696d 6974 3a20 696e 7420 3d20 3130   limit: int = 10
-00003b00: 3030 2c0a 2020 2020 2020 2020 2a2c 0a20  00,.        *,. 
-00003b10: 2020 2020 2020 2064 623a 2044 622c 0a20         db: Db,. 
-00003b20: 2020 2020 2020 2063 7572 3d4e 6f6e 652c         cur=None,
-00003b30: 0a20 2020 2029 202d 3e20 5061 6765 6452  .    ) -> PagedR
-00003b40: 6573 756c 745b 436f 6e74 656e 745d 3a0a  esult[Content]:.
-00003b50: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-00003b60: 6765 745f 7061 6769 6e61 7465 645f 7368  get_paginated_sh
-00003b70: 6131 5f70 6172 7469 7469 6f6e 280a 2020  a1_partition(.  
-00003b80: 2020 2020 2020 2020 2020 6375 722c 0a20            cur,. 
-00003b90: 2020 2020 2020 2020 2020 2070 6172 7469             parti
-00003ba0: 7469 6f6e 5f69 642c 0a20 2020 2020 2020  tion_id,.       
-00003bb0: 2020 2020 206e 625f 7061 7274 6974 696f       nb_partitio
-00003bc0: 6e73 2c0a 2020 2020 2020 2020 2020 2020  ns,.            
-00003bd0: 7061 6765 5f74 6f6b 656e 2c0a 2020 2020  page_token,.    
-00003be0: 2020 2020 2020 2020 6c69 6d69 742c 0a20          limit,. 
-00003bf0: 2020 2020 2020 2020 2020 2064 622e 636f             db.co
-00003c00: 6e74 656e 745f 6765 745f 7261 6e67 652c  ntent_get_range,
-00003c10: 0a20 2020 2020 2020 2020 2020 206c 616d  .            lam
-00003c20: 6264 6120 726f 773a 2043 6f6e 7465 6e74  bda row: Content
-00003c30: 282a 2a64 6963 7428 7a69 7028 6462 2e63  (**dict(zip(db.c
-00003c40: 6f6e 7465 6e74 5f67 6574 5f6d 6574 6164  ontent_get_metad
-00003c50: 6174 615f 6b65 7973 2c20 726f 7729 2929  ata_keys, row)))
-00003c60: 2c0a 2020 2020 2020 2020 2020 2020 6c61  ,.            la
-00003c70: 6d62 6461 2072 6f77 3a20 726f 772e 7368  mbda row: row.sh
-00003c80: 6131 2c0a 2020 2020 2020 2020 290a 0a20  a1,.        ).. 
-00003c90: 2020 2040 6462 5f74 7261 6e73 6163 7469     @db_transacti
-00003ca0: 6f6e 2873 7461 7465 6d65 6e74 5f74 696d  on(statement_tim
-00003cb0: 656f 7574 3d35 3030 290a 2020 2020 6465  eout=500).    de
-00003cc0: 6620 636f 6e74 656e 745f 6765 7428 0a20  f content_get(. 
-00003cd0: 2020 2020 2020 2073 656c 662c 2063 6f6e         self, con
-00003ce0: 7465 6e74 733a 204c 6973 745b 6279 7465  tents: List[byte
-00003cf0: 735d 2c20 616c 676f 3a20 7374 7220 3d20  s], algo: str = 
-00003d00: 2273 6861 3122 2c20 2a2c 2064 623a 2044  "sha1", *, db: D
-00003d10: 622c 2063 7572 3d4e 6f6e 650a 2020 2020  b, cur=None.    
-00003d20: 2920 2d3e 204c 6973 745b 4f70 7469 6f6e  ) -> List[Option
-00003d30: 616c 5b43 6f6e 7465 6e74 5d5d 3a0a 2020  al[Content]]:.  
-00003d40: 2020 2020 2020 636f 6e74 656e 7473 5f62        contents_b
-00003d50: 795f 6861 7368 3a20 4469 6374 5b62 7974  y_hash: Dict[byt
-00003d60: 6573 2c20 4f70 7469 6f6e 616c 5b43 6f6e  es, Optional[Con
-00003d70: 7465 6e74 5d5d 203d 207b 7d0a 2020 2020  tent]] = {}.    
-00003d80: 2020 2020 6966 2061 6c67 6f20 6e6f 7420      if algo not 
-00003d90: 696e 2044 4546 4155 4c54 5f41 4c47 4f52  in DEFAULT_ALGOR
-00003da0: 4954 484d 533a 0a20 2020 2020 2020 2020  ITHMS:.         
-00003db0: 2020 2072 6169 7365 2053 746f 7261 6765     raise Storage
-00003dc0: 4172 6775 6d65 6e74 4578 6365 7074 696f  ArgumentExceptio
-00003dd0: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
-00003de0: 2020 2022 616c 676f 2073 686f 756c 6420     "algo should 
-00003df0: 6265 206f 6e65 206f 6620 7b27 2c27 2e6a  be one of {','.j
-00003e00: 6f69 6e28 4445 4641 554c 545f 414c 474f  oin(DEFAULT_ALGO
-00003e10: 5249 5448 4d53 297d 220a 2020 2020 2020  RITHMS)}".      
-00003e20: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00003e30: 2072 6f77 7320 3d20 6462 2e63 6f6e 7465   rows = db.conte
-00003e40: 6e74 5f67 6574 5f6d 6574 6164 6174 615f  nt_get_metadata_
-00003e50: 6672 6f6d 5f68 6173 6865 7328 636f 6e74  from_hashes(cont
-00003e60: 656e 7473 2c20 616c 676f 2c20 6375 7229  ents, algo, cur)
-00003e70: 0a20 2020 2020 2020 206b 6579 203d 206f  .        key = o
-00003e80: 7065 7261 746f 722e 6174 7472 6765 7474  perator.attrgett
-00003e90: 6572 2861 6c67 6f29 0a0a 2020 2020 2020  er(algo)..      
-00003ea0: 2020 666f 7220 726f 7720 696e 2072 6f77    for row in row
-00003eb0: 733a 0a20 2020 2020 2020 2020 2020 2072  s:.            r
-00003ec0: 6f77 5f64 203d 2064 6963 7428 7a69 7028  ow_d = dict(zip(
-00003ed0: 6462 2e63 6f6e 7465 6e74 5f67 6574 5f6d  db.content_get_m
-00003ee0: 6574 6164 6174 615f 6b65 7973 2c20 726f  etadata_keys, ro
-00003ef0: 7729 290a 2020 2020 2020 2020 2020 2020  w)).            
-00003f00: 636f 6e74 656e 7420 3d20 436f 6e74 656e  content = Conten
-00003f10: 7428 2a2a 726f 775f 6429 0a20 2020 2020  t(**row_d).     
-00003f20: 2020 2020 2020 2063 6f6e 7465 6e74 735f         contents_
-00003f30: 6279 5f68 6173 685b 6b65 7928 636f 6e74  by_hash[key(cont
-00003f40: 656e 7429 5d20 3d20 636f 6e74 656e 740a  ent)] = content.
-00003f50: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00003f60: 5b63 6f6e 7465 6e74 735f 6279 5f68 6173  [contents_by_has
-00003f70: 682e 6765 7428 7368 6131 2920 666f 7220  h.get(sha1) for 
-00003f80: 7368 6131 2069 6e20 636f 6e74 656e 7473  sha1 in contents
-00003f90: 5d0a 0a20 2020 2040 6462 5f74 7261 6e73  ]..    @db_trans
-00003fa0: 6163 7469 6f6e 5f67 656e 6572 6174 6f72  action_generator
-00003fb0: 2829 0a20 2020 2064 6566 2063 6f6e 7465  ().    def conte
-00003fc0: 6e74 5f6d 6973 7369 6e67 280a 2020 2020  nt_missing(.    
-00003fd0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-00003fe0: 2020 636f 6e74 656e 7473 3a20 4c69 7374    contents: List
-00003ff0: 5b48 6173 6844 6963 745d 2c0a 2020 2020  [HashDict],.    
-00004000: 2020 2020 6b65 795f 6861 7368 3a20 7374      key_hash: st
-00004010: 7220 3d20 2273 6861 3122 2c0a 2020 2020  r = "sha1",.    
-00004020: 2020 2020 2a2c 0a20 2020 2020 2020 2064      *,.        d
-00004030: 623a 2044 622c 0a20 2020 2020 2020 2063  b: Db,.        c
-00004040: 7572 3d4e 6f6e 652c 0a20 2020 2029 202d  ur=None,.    ) -
-00004050: 3e20 4974 6572 6162 6c65 5b62 7974 6573  > Iterable[bytes
-00004060: 5d3a 0a20 2020 2020 2020 2069 6620 6b65  ]:.        if ke
-00004070: 795f 6861 7368 206e 6f74 2069 6e20 4445  y_hash not in DE
-00004080: 4641 554c 545f 414c 474f 5249 5448 4d53  FAULT_ALGORITHMS
-00004090: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-000040a0: 6973 6520 5374 6f72 6167 6541 7267 756d  ise StorageArgum
-000040b0: 656e 7445 7863 6570 7469 6f6e 280a 2020  entException(.  
-000040c0: 2020 2020 2020 2020 2020 2020 2020 226b                "k
-000040d0: 6579 5f68 6173 6820 7368 6f75 6c64 2062  ey_hash should b
-000040e0: 6520 6f6e 6520 6f66 207b 272c 272e 6a6f  e one of {','.jo
-000040f0: 696e 2844 4546 4155 4c54 5f41 4c47 4f52  in(DEFAULT_ALGOR
-00004100: 4954 484d 5329 7d22 0a20 2020 2020 2020  ITHMS)}".       
-00004110: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-00004120: 6b65 7973 203d 2064 622e 636f 6e74 656e  keys = db.conten
-00004130: 745f 6861 7368 5f6b 6579 730a 2020 2020  t_hash_keys.    
-00004140: 2020 2020 6b65 795f 6861 7368 5f69 6478      key_hash_idx
-00004150: 203d 206b 6579 732e 696e 6465 7828 6b65   = keys.index(ke
-00004160: 795f 6861 7368 290a 0a20 2020 2020 2020  y_hash)..       
-00004170: 2066 6f72 206f 626a 2069 6e20 6462 2e63   for obj in db.c
-00004180: 6f6e 7465 6e74 5f6d 6973 7369 6e67 5f66  ontent_missing_f
-00004190: 726f 6d5f 6c69 7374 2863 6f6e 7465 6e74  rom_list(content
-000041a0: 732c 2063 7572 293a 0a20 2020 2020 2020  s, cur):.       
-000041b0: 2020 2020 2079 6965 6c64 206f 626a 5b6b       yield obj[k
-000041c0: 6579 5f68 6173 685f 6964 785d 0a0a 2020  ey_hash_idx]..  
-000041d0: 2020 4064 625f 7472 616e 7361 6374 696f    @db_transactio
-000041e0: 6e5f 6765 6e65 7261 746f 7228 290a 2020  n_generator().  
-000041f0: 2020 6465 6620 636f 6e74 656e 745f 6d69    def content_mi
-00004200: 7373 696e 675f 7065 725f 7368 6131 280a  ssing_per_sha1(.
-00004210: 2020 2020 2020 2020 7365 6c66 2c20 636f          self, co
-00004220: 6e74 656e 7473 3a20 4c69 7374 5b62 7974  ntents: List[byt
-00004230: 6573 5d2c 202a 2c20 6462 3a20 4462 2c20  es], *, db: Db, 
-00004240: 6375 723d 4e6f 6e65 0a20 2020 2029 202d  cur=None.    ) -
-00004250: 3e20 4974 6572 6162 6c65 5b62 7974 6573  > Iterable[bytes
-00004260: 5d3a 0a20 2020 2020 2020 2066 6f72 206f  ]:.        for o
-00004270: 626a 2069 6e20 6462 2e63 6f6e 7465 6e74  bj in db.content
-00004280: 5f6d 6973 7369 6e67 5f70 6572 5f73 6861  _missing_per_sha
-00004290: 3128 636f 6e74 656e 7473 2c20 6375 7229  1(contents, cur)
-000042a0: 3a0a 2020 2020 2020 2020 2020 2020 7969  :.            yi
-000042b0: 656c 6420 6f62 6a5b 305d 0a0a 2020 2020  eld obj[0]..    
-000042c0: 4064 625f 7472 616e 7361 6374 696f 6e5f  @db_transaction_
-000042d0: 6765 6e65 7261 746f 7228 290a 2020 2020  generator().    
-000042e0: 6465 6620 636f 6e74 656e 745f 6d69 7373  def content_miss
-000042f0: 696e 675f 7065 725f 7368 6131 5f67 6974  ing_per_sha1_git
-00004300: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
-00004310: 636f 6e74 656e 7473 3a20 4c69 7374 5b62  contents: List[b
-00004320: 7974 6573 5d2c 202a 2c20 6462 3a20 4462  ytes], *, db: Db
-00004330: 2c20 6375 723d 4e6f 6e65 0a20 2020 2029  , cur=None.    )
-00004340: 202d 3e20 4974 6572 6162 6c65 5b53 6861   -> Iterable[Sha
-00004350: 3147 6974 5d3a 0a20 2020 2020 2020 2066  1Git]:.        f
-00004360: 6f72 206f 626a 2069 6e20 6462 2e63 6f6e  or obj in db.con
-00004370: 7465 6e74 5f6d 6973 7369 6e67 5f70 6572  tent_missing_per
-00004380: 5f73 6861 315f 6769 7428 636f 6e74 656e  _sha1_git(conten
-00004390: 7473 2c20 6375 7229 3a0a 2020 2020 2020  ts, cur):.      
-000043a0: 2020 2020 2020 7969 656c 6420 6f62 6a5b        yield obj[
-000043b0: 305d 0a0a 2020 2020 4064 625f 7472 616e  0]..    @db_tran
-000043c0: 7361 6374 696f 6e28 290a 2020 2020 6465  saction().    de
-000043d0: 6620 636f 6e74 656e 745f 6669 6e64 2873  f content_find(s
-000043e0: 656c 662c 2063 6f6e 7465 6e74 3a20 4861  elf, content: Ha
-000043f0: 7368 4469 6374 2c20 2a2c 2064 623a 2044  shDict, *, db: D
-00004400: 622c 2063 7572 3d4e 6f6e 6529 202d 3e20  b, cur=None) -> 
-00004410: 4c69 7374 5b43 6f6e 7465 6e74 5d3a 0a20  List[Content]:. 
-00004420: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-00004430: 7428 636f 6e74 656e 7429 2e69 6e74 6572  t(content).inter
-00004440: 7365 6374 696f 6e28 4445 4641 554c 545f  section(DEFAULT_
-00004450: 414c 474f 5249 5448 4d53 293a 0a20 2020  ALGORITHMS):.   
-00004460: 2020 2020 2020 2020 2072 6169 7365 2053           raise S
-00004470: 746f 7261 6765 4172 6775 6d65 6e74 4578  torageArgumentEx
-00004480: 6365 7074 696f 6e28 0a20 2020 2020 2020  ception(.       
-00004490: 2020 2020 2020 2020 2022 636f 6e74 656e           "conten
-000044a0: 7420 6b65 7973 206d 7573 7420 636f 6e74  t keys must cont
-000044b0: 6169 6e20 6174 206c 6561 7374 206f 6e65  ain at least one
-000044c0: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-000044d0: 2020 2066 226f 663a 207b 272c 2027 2e6a     f"of: {', '.j
-000044e0: 6f69 6e28 736f 7274 6564 2844 4546 4155  oin(sorted(DEFAU
-000044f0: 4c54 5f41 4c47 4f52 4954 484d 5329 297d  LT_ALGORITHMS))}
-00004500: 220a 2020 2020 2020 2020 2020 2020 290a  ".            ).
-00004510: 0a20 2020 2020 2020 2072 6f77 7320 3d20  .        rows = 
-00004520: 6462 2e63 6f6e 7465 6e74 5f66 696e 6428  db.content_find(
-00004530: 0a20 2020 2020 2020 2020 2020 2073 6861  .            sha
-00004540: 313d 636f 6e74 656e 742e 6765 7428 2273  1=content.get("s
-00004550: 6861 3122 292c 0a20 2020 2020 2020 2020  ha1"),.         
-00004560: 2020 2073 6861 315f 6769 743d 636f 6e74     sha1_git=cont
-00004570: 656e 742e 6765 7428 2273 6861 315f 6769  ent.get("sha1_gi
-00004580: 7422 292c 0a20 2020 2020 2020 2020 2020  t"),.           
-00004590: 2073 6861 3235 363d 636f 6e74 656e 742e   sha256=content.
-000045a0: 6765 7428 2273 6861 3235 3622 292c 0a20  get("sha256"),. 
-000045b0: 2020 2020 2020 2020 2020 2062 6c61 6b65             blake
-000045c0: 3273 3235 363d 636f 6e74 656e 742e 6765  2s256=content.ge
-000045d0: 7428 2262 6c61 6b65 3273 3235 3622 292c  t("blake2s256"),
-000045e0: 0a20 2020 2020 2020 2020 2020 2063 7572  .            cur
-000045f0: 3d63 7572 2c0a 2020 2020 2020 2020 290a  =cur,.        ).
-00004600: 2020 2020 2020 2020 636f 6e74 656e 7473          contents
-00004610: 203d 205b 5d0a 2020 2020 2020 2020 666f   = [].        fo
-00004620: 7220 726f 7720 696e 2072 6f77 733a 0a20  r row in rows:. 
-00004630: 2020 2020 2020 2020 2020 2072 6f77 5f64             row_d
-00004640: 203d 2064 6963 7428 7a69 7028 6462 2e63   = dict(zip(db.c
-00004650: 6f6e 7465 6e74 5f66 696e 645f 636f 6c73  ontent_find_cols
-00004660: 2c20 726f 7729 290a 2020 2020 2020 2020  , row)).        
-00004670: 2020 2020 636f 6e74 656e 7473 2e61 7070      contents.app
-00004680: 656e 6428 436f 6e74 656e 7428 2a2a 726f  end(Content(**ro
-00004690: 775f 6429 290a 2020 2020 2020 2020 7265  w_d)).        re
-000046a0: 7475 726e 2063 6f6e 7465 6e74 730a 0a20  turn contents.. 
-000046b0: 2020 2040 6462 5f74 7261 6e73 6163 7469     @db_transacti
-000046c0: 6f6e 2829 0a20 2020 2064 6566 2063 6f6e  on().    def con
-000046d0: 7465 6e74 5f67 6574 5f72 616e 646f 6d28  tent_get_random(
-000046e0: 7365 6c66 2c20 2a2c 2064 623a 2044 622c  self, *, db: Db,
-000046f0: 2063 7572 3d4e 6f6e 6529 202d 3e20 5368   cur=None) -> Sh
-00004700: 6131 4769 743a 0a20 2020 2020 2020 2072  a1Git:.        r
-00004710: 6574 7572 6e20 6462 2e63 6f6e 7465 6e74  eturn db.content
-00004720: 5f67 6574 5f72 616e 646f 6d28 6375 7229  _get_random(cur)
-00004730: 0a0a 2020 2020 2323 2323 2323 2323 2323  ..    ##########
+000028b0: 2323 2323 2323 2323 0a0a 2020 2020 6465  ########..    de
+000028c0: 6620 5f63 6f6e 7465 6e74 5f75 6e69 7175  f _content_uniqu
+000028d0: 655f 6b65 7928 7365 6c66 2c20 6861 7368  e_key(self, hash
+000028e0: 2c20 6462 293a 0a20 2020 2020 2020 2022  , db):.        "
+000028f0: 2222 4769 7665 6e20 6120 6861 7368 2028  ""Given a hash (
+00002900: 7475 706c 6520 6f72 2064 6963 7429 2c20  tuple or dict), 
+00002910: 7265 7475 726e 2061 2075 6e69 7175 6520  return a unique 
+00002920: 6b65 7920 6672 6f6d 2074 6865 0a20 2020  key from the.   
+00002930: 2020 2020 2061 6767 7265 6761 7469 6f6e       aggregation
+00002940: 206f 6620 6b65 7973 2e0a 0a20 2020 2020   of keys...     
+00002950: 2020 2022 2222 0a20 2020 2020 2020 206b     """.        k
+00002960: 6579 7320 3d20 6462 2e63 6f6e 7465 6e74  eys = db.content
+00002970: 5f68 6173 685f 6b65 7973 0a20 2020 2020  _hash_keys.     
+00002980: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00002990: 2868 6173 682c 2074 7570 6c65 293a 0a20  (hash, tuple):. 
+000029a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000029b0: 6e20 6861 7368 0a20 2020 2020 2020 2072  n hash.        r
+000029c0: 6574 7572 6e20 7475 706c 6528 5b68 6173  eturn tuple([has
+000029d0: 685b 6b5d 2066 6f72 206b 2069 6e20 6b65  h[k] for k in ke
+000029e0: 7973 5d29 0a0a 2020 2020 6465 6620 5f63  ys])..    def _c
+000029f0: 6f6e 7465 6e74 5f61 6464 5f6d 6574 6164  ontent_add_metad
+00002a00: 6174 6128 7365 6c66 2c20 6462 2c20 6375  ata(self, db, cu
+00002a10: 722c 2063 6f6e 7465 6e74 293a 0a20 2020  r, content):.   
+00002a20: 2020 2020 2022 2222 4164 6420 636f 6e74       """Add cont
+00002a30: 656e 7420 746f 2074 6865 2070 6f73 7467  ent to the postg
+00002a40: 7265 7371 6c20 6461 7461 6261 7365 2062  resql database b
+00002a50: 7574 206e 6f74 2074 6865 206f 626a 6563  ut not the objec
+00002a60: 7420 7374 6f72 6167 652e 2222 220a 2020  t storage.""".  
+00002a70: 2020 2020 2020 2320 6372 6561 7465 2074        # create t
+00002a80: 656d 706f 7261 7279 2074 6162 6c65 2066  emporary table f
+00002a90: 6f72 206d 6574 6164 6174 6120 696e 6a65  or metadata inje
+00002aa0: 6374 696f 6e0a 2020 2020 2020 2020 6462  ction.        db
+00002ab0: 2e6d 6b74 656d 7028 2263 6f6e 7465 6e74  .mktemp("content
+00002ac0: 222c 2063 7572 290a 0a20 2020 2020 2020  ", cur)..       
+00002ad0: 2064 622e 636f 7079 5f74 6f28 0a20 2020   db.copy_to(.   
+00002ae0: 2020 2020 2020 2020 2028 632e 746f 5f64           (c.to_d
+00002af0: 6963 7428 2920 666f 7220 6320 696e 2063  ict() for c in c
+00002b00: 6f6e 7465 6e74 292c 2022 746d 705f 636f  ontent), "tmp_co
+00002b10: 6e74 656e 7422 2c20 6462 2e63 6f6e 7465  ntent", db.conte
+00002b20: 6e74 5f61 6464 5f6b 6579 732c 2063 7572  nt_add_keys, cur
+00002b30: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00002b40: 2020 2020 2320 6d6f 7665 206d 6574 6164      # move metad
+00002b50: 6174 6120 696e 2070 6c61 6365 0a20 2020  ata in place.   
+00002b60: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+00002b70: 2020 2020 2020 6462 2e63 6f6e 7465 6e74        db.content
+00002b80: 5f61 6464 5f66 726f 6d5f 7465 6d70 2863  _add_from_temp(c
+00002b90: 7572 290a 2020 2020 2020 2020 6578 6365  ur).        exce
+00002ba0: 7074 2070 7379 636f 7067 322e 496e 7465  pt psycopg2.Inte
+00002bb0: 6772 6974 7945 7272 6f72 2061 7320 653a  grityError as e:
+00002bc0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00002bd0: 652e 6469 6167 2e73 716c 7374 6174 6520  e.diag.sqlstate 
+00002be0: 3d3d 2022 3233 3530 3522 2061 6e64 2065  == "23505" and e
+00002bf0: 2e64 6961 672e 7461 626c 655f 6e61 6d65  .diag.table_name
+00002c00: 203d 3d20 2263 6f6e 7465 6e74 223a 0a20   == "content":. 
+00002c10: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00002c20: 6573 7361 6765 5f64 6574 6169 6c20 3d20  essage_detail = 
+00002c30: 652e 6469 6167 2e6d 6573 7361 6765 5f64  e.diag.message_d
+00002c40: 6574 6169 6c0a 2020 2020 2020 2020 2020  etail.          
+00002c50: 2020 2020 2020 6966 206d 6573 7361 6765        if message
+00002c60: 5f64 6574 6169 6c3a 0a20 2020 2020 2020  _detail:.       
+00002c70: 2020 2020 2020 2020 2020 2020 2068 6173               has
+00002c80: 685f 6e61 6d65 2c20 6861 7368 5f69 6420  h_name, hash_id 
+00002c90: 3d20 6578 7472 6163 745f 636f 6c6c 6973  = extract_collis
+00002ca0: 696f 6e5f 6861 7368 286d 6573 7361 6765  ion_hash(message
+00002cb0: 5f64 6574 6169 6c29 0a20 2020 2020 2020  _detail).       
+00002cc0: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
+00002cd0: 6c69 7369 6f6e 5f63 6f6e 7465 6e74 735f  lision_contents_
+00002ce0: 6861 7368 6573 203d 205b 0a20 2020 2020  hashes = [.     
+00002cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d00: 2020 2063 2e68 6173 6865 7328 2920 666f     c.hashes() fo
+00002d10: 7220 6320 696e 2063 6f6e 7465 6e74 2069  r c in content i
+00002d20: 6620 632e 6765 745f 6861 7368 2868 6173  f c.get_hash(has
+00002d30: 685f 6e61 6d65 2920 3d3d 2068 6173 685f  h_name) == hash_
+00002d40: 6964 0a20 2020 2020 2020 2020 2020 2020  id.             
+00002d50: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
+00002d60: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00002d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d80: 2020 2063 6f6e 7374 7261 696e 745f 746f     constraint_to
+00002d90: 5f68 6173 685f 6e61 6d65 203d 207b 0a20  _hash_name = {. 
+00002da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002db0: 2020 2020 2020 2022 636f 6e74 656e 745f         "content_
+00002dc0: 706b 6579 223a 2022 7368 6131 222c 0a20  pkey": "sha1",. 
+00002dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002de0: 2020 2020 2020 2022 636f 6e74 656e 745f         "content_
+00002df0: 7368 6131 5f67 6974 5f69 6478 223a 2022  sha1_git_idx": "
+00002e00: 7368 6131 5f67 6974 222c 0a20 2020 2020  sha1_git",.     
+00002e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e20: 2020 2022 636f 6e74 656e 745f 7368 6132     "content_sha2
+00002e30: 3536 5f69 6478 223a 2022 7368 6132 3536  56_idx": "sha256
+00002e40: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00002e50: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00002e60: 2020 2020 2020 2020 2020 2020 2068 6173               has
+00002e70: 685f 6e61 6d65 203d 2063 6f6e 7374 7261  h_name = constra
+00002e80: 696e 745f 746f 5f68 6173 685f 6e61 6d65  int_to_hash_name
+00002e90: 2e67 6574 2865 2e64 6961 672e 636f 6e73  .get(e.diag.cons
+00002ea0: 7472 6169 6e74 5f6e 616d 6529 0a20 2020  traint_name).   
+00002eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ec0: 2068 6173 685f 6964 203d 204e 6f6e 650a   hash_id = None.
+00002ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ee0: 2020 2020 636f 6c6c 6973 696f 6e5f 636f      collision_co
+00002ef0: 6e74 656e 7473 5f68 6173 6865 7320 3d20  ntents_hashes = 
+00002f00: 4e6f 6e65 0a0a 2020 2020 2020 2020 2020  None..          
+00002f10: 2020 2020 2020 7261 6973 6520 4861 7368        raise Hash
+00002f20: 436f 6c6c 6973 696f 6e28 0a20 2020 2020  Collision(.     
+00002f30: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+00002f40: 6173 685f 6e61 6d65 2c20 6861 7368 5f69  ash_name, hash_i
+00002f50: 642c 2063 6f6c 6c69 7369 6f6e 5f63 6f6e  d, collision_con
+00002f60: 7465 6e74 735f 6861 7368 6573 0a20 2020  tents_hashes.   
+00002f70: 2020 2020 2020 2020 2020 2020 2029 2066               ) f
+00002f80: 726f 6d20 4e6f 6e65 0a20 2020 2020 2020  rom None.       
+00002f90: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00002fa0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00002fb0: 0a0a 2020 2020 6465 6620 636f 6e74 656e  ..    def conten
+00002fc0: 745f 6164 6428 7365 6c66 2c20 636f 6e74  t_add(self, cont
+00002fd0: 656e 743a 204c 6973 745b 436f 6e74 656e  ent: List[Conten
+00002fe0: 745d 2920 2d3e 2044 6963 745b 7374 722c  t]) -> Dict[str,
+00002ff0: 2069 6e74 5d3a 0a20 2020 2020 2020 2063   int]:.        c
+00003000: 7469 6d65 203d 206e 6f77 2829 0a0a 2020  time = now()..  
+00003010: 2020 2020 2020 636f 6e74 656e 7473 203d        contents =
+00003020: 205b 6174 7472 2e65 766f 6c76 6528 632c   [attr.evolve(c,
+00003030: 2063 7469 6d65 3d63 7469 6d65 2920 666f   ctime=ctime) fo
+00003040: 7220 6320 696e 2063 6f6e 7465 6e74 5d0a  r c in content].
+00003050: 0a20 2020 2020 2020 2023 204d 7573 7420  .        # Must 
+00003060: 6164 6420 746f 2074 6865 206f 626a 7374  add to the objst
+00003070: 6f72 6167 6520 6265 666f 7265 2074 6865  orage before the
+00003080: 2044 4220 616e 6420 6a6f 7572 6e61 6c2e   DB and journal.
+00003090: 204f 7468 6572 7769 7365 3a0a 2020 2020   Otherwise:.    
+000030a0: 2020 2020 2320 312e 2069 6e20 6361 7365      # 1. in case
+000030b0: 206f 6620 6120 6372 6173 6820 7468 6520   of a crash the 
+000030c0: 4442 206d 6179 2022 6265 6c69 6576 6522  DB may "believe"
+000030d0: 2077 6520 6861 7665 2074 6865 2063 6f6e   we have the con
+000030e0: 7465 6e74 2c20 6275 740a 2020 2020 2020  tent, but.      
+000030f0: 2020 2320 2020 2077 6520 6469 646e 2774    #    we didn't
+00003100: 2068 6176 6520 7469 6d65 2074 6f20 7772   have time to wr
+00003110: 6974 6520 746f 2074 6865 206f 626a 7374  ite to the objst
+00003120: 6f72 6167 6520 6265 666f 7265 2074 6865  orage before the
+00003130: 2063 7261 7368 0a20 2020 2020 2020 2023   crash.        #
+00003140: 2032 2e20 7468 6520 6f62 6a73 746f 7261   2. the objstora
+00003150: 6765 206d 6972 726f 7269 6e67 2c20 7768  ge mirroring, wh
+00003160: 6963 6820 7265 6164 7320 6672 6f6d 2074  ich reads from t
+00003170: 6865 206a 6f75 726e 616c 2c20 6d61 7920  he journal, may 
+00003180: 6174 7465 6d70 7420 746f 0a20 2020 2020  attempt to.     
+00003190: 2020 2023 2020 2020 7265 6164 2066 726f     #    read fro
+000031a0: 6d20 7468 6520 6f62 6a73 746f 7261 6765  m the objstorage
+000031b0: 2062 6566 6f72 6520 7765 2066 696e 6973   before we finis
+000031c0: 6865 6420 7772 6974 696e 6720 6974 0a20  hed writing it. 
+000031d0: 2020 2020 2020 206f 626a 7374 6f72 6167         objstorag
+000031e0: 655f 7375 6d6d 6172 7920 3d20 7365 6c66  e_summary = self
+000031f0: 2e6f 626a 7374 6f72 6167 652e 636f 6e74  .objstorage.cont
+00003200: 656e 745f 6164 6428 636f 6e74 656e 7473  ent_add(contents
+00003210: 290a 0a20 2020 2020 2020 2077 6974 6820  )..        with 
+00003220: 7365 6c66 2e64 6228 2920 6173 2064 623a  self.db() as db:
+00003230: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+00003240: 6820 6462 2e74 7261 6e73 6163 7469 6f6e  h db.transaction
+00003250: 2829 2061 7320 6375 723a 0a20 2020 2020  () as cur:.     
+00003260: 2020 2020 2020 2020 2020 206d 6973 7369             missi
+00003270: 6e67 203d 2073 6574 280a 2020 2020 2020  ng = set(.      
+00003280: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00003290: 6c66 2e63 6f6e 7465 6e74 5f6d 6973 7369  lf.content_missi
+000032a0: 6e67 280a 2020 2020 2020 2020 2020 2020  ng(.            
+000032b0: 2020 2020 2020 2020 2020 2020 5b63 2e74              [c.t
+000032c0: 6f5f 6469 6374 2829 2066 6f72 2063 2069  o_dict() for c i
+000032d0: 6e20 636f 6e74 656e 7473 5d2c 0a20 2020  n contents],.   
+000032e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032f0: 2020 2020 206b 6579 5f68 6173 683d 2273       key_hash="s
+00003300: 6861 315f 6769 7422 2c0a 2020 2020 2020  ha1_git",.      
+00003310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003320: 2020 6462 3d64 622c 0a20 2020 2020 2020    db=db,.       
+00003330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003340: 2063 7572 3d63 7572 2c0a 2020 2020 2020   cur=cur,.      
+00003350: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00003360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003370: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00003380: 2020 636f 6e74 656e 7473 203d 205b 6320    contents = [c 
+00003390: 666f 7220 6320 696e 2063 6f6e 7465 6e74  for c in content
+000033a0: 7320 6966 2063 2e73 6861 315f 6769 7420  s if c.sha1_git 
+000033b0: 696e 206d 6973 7369 6e67 5d0a 0a20 2020  in missing]..   
+000033c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000033d0: 662e 6a6f 7572 6e61 6c5f 7772 6974 6572  f.journal_writer
+000033e0: 2e63 6f6e 7465 6e74 5f61 6464 2863 6f6e  .content_add(con
+000033f0: 7465 6e74 7329 0a20 2020 2020 2020 2020  tents).         
+00003400: 2020 2020 2020 2073 656c 662e 5f63 6f6e         self._con
+00003410: 7465 6e74 5f61 6464 5f6d 6574 6164 6174  tent_add_metadat
+00003420: 6128 6462 2c20 6375 722c 2063 6f6e 7465  a(db, cur, conte
+00003430: 6e74 7329 0a0a 2020 2020 2020 2020 7265  nts)..        re
+00003440: 7475 726e 207b 0a20 2020 2020 2020 2020  turn {.         
+00003450: 2020 2022 636f 6e74 656e 743a 6164 6422     "content:add"
+00003460: 3a20 6c65 6e28 636f 6e74 656e 7473 292c  : len(contents),
+00003470: 0a20 2020 2020 2020 2020 2020 2022 636f  .            "co
+00003480: 6e74 656e 743a 6164 643a 6279 7465 7322  ntent:add:bytes"
+00003490: 3a20 6f62 6a73 746f 7261 6765 5f73 756d  : objstorage_sum
+000034a0: 6d61 7279 5b22 636f 6e74 656e 743a 6164  mary["content:ad
+000034b0: 643a 6279 7465 7322 5d2c 0a20 2020 2020  d:bytes"],.     
+000034c0: 2020 207d 0a0a 2020 2020 4064 625f 7472     }..    @db_tr
+000034d0: 616e 7361 6374 696f 6e28 290a 2020 2020  ansaction().    
+000034e0: 6465 6620 636f 6e74 656e 745f 7570 6461  def content_upda
+000034f0: 7465 280a 2020 2020 2020 2020 7365 6c66  te(.        self
+00003500: 2c20 636f 6e74 656e 7473 3a20 4c69 7374  , contents: List
+00003510: 5b44 6963 745b 7374 722c 2041 6e79 5d5d  [Dict[str, Any]]
+00003520: 2c20 6b65 7973 3a20 4c69 7374 5b73 7472  , keys: List[str
+00003530: 5d20 3d20 5b5d 2c20 2a2c 2064 623a 2044  ] = [], *, db: D
+00003540: 622c 2063 7572 3d4e 6f6e 650a 2020 2020  b, cur=None.    
+00003550: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00003560: 2020 2023 2054 4f44 4f3a 2041 6464 2061     # TODO: Add a
+00003570: 2063 6865 636b 206f 6e20 696e 7075 7420   check on input 
+00003580: 6b65 7973 2e20 486f 7720 746f 2070 726f  keys. How to pro
+00003590: 7065 726c 7920 696d 706c 656d 656e 740a  perly implement.
+000035a0: 2020 2020 2020 2020 2320 7468 6973 3f20          # this? 
+000035b0: 5765 2064 6f6e 2774 206b 6e6f 7720 7965  We don't know ye
+000035c0: 7420 7468 6520 6e65 7720 636f 6c75 6d6e  t the new column
+000035d0: 732e 0a20 2020 2020 2020 2073 656c 662e  s..        self.
+000035e0: 6a6f 7572 6e61 6c5f 7772 6974 6572 2e63  journal_writer.c
+000035f0: 6f6e 7465 6e74 5f75 7064 6174 6528 636f  ontent_update(co
+00003600: 6e74 656e 7473 290a 0a20 2020 2020 2020  ntents)..       
+00003610: 2064 622e 6d6b 7465 6d70 2822 636f 6e74   db.mktemp("cont
+00003620: 656e 7422 2c20 6375 7229 0a20 2020 2020  ent", cur).     
+00003630: 2020 2073 656c 6563 745f 6b65 7973 203d     select_keys =
+00003640: 206c 6973 7428 7365 7428 6462 2e63 6f6e   list(set(db.con
+00003650: 7465 6e74 5f67 6574 5f6d 6574 6164 6174  tent_get_metadat
+00003660: 615f 6b65 7973 292e 756e 696f 6e28 7365  a_keys).union(se
+00003670: 7428 6b65 7973 2929 290a 2020 2020 2020  t(keys))).      
+00003680: 2020 7769 7468 2063 6f6e 7665 7274 5f76    with convert_v
+00003690: 616c 6964 6174 696f 6e5f 6578 6365 7074  alidation_except
+000036a0: 696f 6e73 2829 3a0a 2020 2020 2020 2020  ions():.        
+000036b0: 2020 2020 6462 2e63 6f70 795f 746f 2863      db.copy_to(c
+000036c0: 6f6e 7465 6e74 732c 2022 746d 705f 636f  ontents, "tmp_co
+000036d0: 6e74 656e 7422 2c20 7365 6c65 6374 5f6b  ntent", select_k
+000036e0: 6579 732c 2063 7572 290a 2020 2020 2020  eys, cur).      
+000036f0: 2020 2020 2020 6462 2e63 6f6e 7465 6e74        db.content
+00003700: 5f75 7064 6174 655f 6672 6f6d 5f74 656d  _update_from_tem
+00003710: 7028 6b65 7973 5f74 6f5f 7570 6461 7465  p(keys_to_update
+00003720: 3d6b 6579 732c 2063 7572 3d63 7572 290a  =keys, cur=cur).
+00003730: 0a20 2020 2040 6462 5f74 7261 6e73 6163  .    @db_transac
+00003740: 7469 6f6e 2829 0a20 2020 2064 6566 2063  tion().    def c
+00003750: 6f6e 7465 6e74 5f61 6464 5f6d 6574 6164  ontent_add_metad
+00003760: 6174 6128 0a20 2020 2020 2020 2073 656c  ata(.        sel
+00003770: 662c 2063 6f6e 7465 6e74 3a20 4c69 7374  f, content: List
+00003780: 5b43 6f6e 7465 6e74 5d2c 202a 2c20 6462  [Content], *, db
+00003790: 3a20 4462 2c20 6375 723d 4e6f 6e65 0a20  : Db, cur=None. 
+000037a0: 2020 2029 202d 3e20 4469 6374 5b73 7472     ) -> Dict[str
+000037b0: 2c20 696e 745d 3a0a 2020 2020 2020 2020  , int]:.        
+000037c0: 6d69 7373 696e 6720 3d20 7365 7428 0a20  missing = set(. 
+000037d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000037e0: 636f 6e74 656e 745f 6d69 7373 696e 6728  content_missing(
+000037f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003800: 205b 632e 746f 5f64 6963 7428 2920 666f   [c.to_dict() fo
+00003810: 7220 6320 696e 2063 6f6e 7465 6e74 5d2c  r c in content],
+00003820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003830: 206b 6579 5f68 6173 683d 2273 6861 315f   key_hash="sha1_
+00003840: 6769 7422 2c0a 2020 2020 2020 2020 2020  git",.          
+00003850: 2020 2020 2020 6462 3d64 622c 0a20 2020        db=db,.   
+00003860: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00003870: 3d63 7572 2c0a 2020 2020 2020 2020 2020  =cur,.          
+00003880: 2020 290a 2020 2020 2020 2020 290a 2020    ).        ).  
+00003890: 2020 2020 2020 636f 6e74 656e 7473 203d        contents =
+000038a0: 205b 6320 666f 7220 6320 696e 2063 6f6e   [c for c in con
+000038b0: 7465 6e74 2069 6620 632e 7368 6131 5f67  tent if c.sha1_g
+000038c0: 6974 2069 6e20 6d69 7373 696e 675d 0a0a  it in missing]..
+000038d0: 2020 2020 2020 2020 7365 6c66 2e6a 6f75          self.jou
+000038e0: 726e 616c 5f77 7269 7465 722e 636f 6e74  rnal_writer.cont
+000038f0: 656e 745f 6164 645f 6d65 7461 6461 7461  ent_add_metadata
+00003900: 2863 6f6e 7465 6e74 7329 0a20 2020 2020  (contents).     
+00003910: 2020 2073 656c 662e 5f63 6f6e 7465 6e74     self._content
+00003920: 5f61 6464 5f6d 6574 6164 6174 6128 6462  _add_metadata(db
+00003930: 2c20 6375 722c 2063 6f6e 7465 6e74 7329  , cur, contents)
+00003940: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00003950: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00003960: 636f 6e74 656e 743a 6164 6422 3a20 6c65  content:add": le
+00003970: 6e28 636f 6e74 656e 7473 292c 0a20 2020  n(contents),.   
+00003980: 2020 2020 207d 0a0a 2020 2020 6465 6620       }..    def 
+00003990: 636f 6e74 656e 745f 6765 745f 6461 7461  content_get_data
+000039a0: 2873 656c 662c 2063 6f6e 7465 6e74 3a20  (self, content: 
+000039b0: 556e 696f 6e5b 4861 7368 4469 6374 2c20  Union[HashDict, 
+000039c0: 5368 6131 5d29 202d 3e20 4f70 7469 6f6e  Sha1]) -> Option
+000039d0: 616c 5b62 7974 6573 5d3a 0a20 2020 2020  al[bytes]:.     
+000039e0: 2020 2023 2046 4958 4d45 3a20 4d61 6b65     # FIXME: Make
+000039f0: 2074 6869 7320 6d65 7468 6f64 2073 7570   this method sup
+00003a00: 706f 7274 2073 6c69 6369 6e67 2074 6865  port slicing the
+00003a10: 2060 6461 7461 600a 2020 2020 2020 2020   `data`.        
+00003a20: 7265 7475 726e 2073 656c 662e 6f62 6a73  return self.objs
+00003a30: 746f 7261 6765 2e63 6f6e 7465 6e74 5f67  torage.content_g
+00003a40: 6574 2863 6f6e 7465 6e74 290a 0a20 2020  et(content)..   
+00003a50: 2040 6462 5f74 7261 6e73 6163 7469 6f6e   @db_transaction
+00003a60: 2829 0a20 2020 2064 6566 2063 6f6e 7465  ().    def conte
+00003a70: 6e74 5f67 6574 5f70 6172 7469 7469 6f6e  nt_get_partition
+00003a80: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00003a90: 2020 2020 2020 2020 7061 7274 6974 696f          partitio
+00003aa0: 6e5f 6964 3a20 696e 742c 0a20 2020 2020  n_id: int,.     
+00003ab0: 2020 206e 625f 7061 7274 6974 696f 6e73     nb_partitions
+00003ac0: 3a20 696e 742c 0a20 2020 2020 2020 2070  : int,.        p
+00003ad0: 6167 655f 746f 6b65 6e3a 204f 7074 696f  age_token: Optio
+00003ae0: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
+00003af0: 0a20 2020 2020 2020 206c 696d 6974 3a20  .        limit: 
+00003b00: 696e 7420 3d20 3130 3030 2c0a 2020 2020  int = 1000,.    
+00003b10: 2020 2020 2a2c 0a20 2020 2020 2020 2064      *,.        d
+00003b20: 623a 2044 622c 0a20 2020 2020 2020 2063  b: Db,.        c
+00003b30: 7572 3d4e 6f6e 652c 0a20 2020 2029 202d  ur=None,.    ) -
+00003b40: 3e20 5061 6765 6452 6573 756c 745b 436f  > PagedResult[Co
+00003b50: 6e74 656e 745d 3a0a 2020 2020 2020 2020  ntent]:.        
+00003b60: 7265 7475 726e 205f 6765 745f 7061 6769  return _get_pagi
+00003b70: 6e61 7465 645f 7368 6131 5f70 6172 7469  nated_sha1_parti
+00003b80: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
+00003b90: 2020 6375 722c 0a20 2020 2020 2020 2020    cur,.         
+00003ba0: 2020 2070 6172 7469 7469 6f6e 5f69 642c     partition_id,
+00003bb0: 0a20 2020 2020 2020 2020 2020 206e 625f  .            nb_
+00003bc0: 7061 7274 6974 696f 6e73 2c0a 2020 2020  partitions,.    
+00003bd0: 2020 2020 2020 2020 7061 6765 5f74 6f6b          page_tok
+00003be0: 656e 2c0a 2020 2020 2020 2020 2020 2020  en,.            
+00003bf0: 6c69 6d69 742c 0a20 2020 2020 2020 2020  limit,.         
+00003c00: 2020 2064 622e 636f 6e74 656e 745f 6765     db.content_ge
+00003c10: 745f 7261 6e67 652c 0a20 2020 2020 2020  t_range,.       
+00003c20: 2020 2020 206c 616d 6264 6120 726f 773a       lambda row:
+00003c30: 2043 6f6e 7465 6e74 282a 2a64 6963 7428   Content(**dict(
+00003c40: 7a69 7028 6462 2e63 6f6e 7465 6e74 5f67  zip(db.content_g
+00003c50: 6574 5f6d 6574 6164 6174 615f 6b65 7973  et_metadata_keys
+00003c60: 2c20 726f 7729 2929 2c0a 2020 2020 2020  , row))),.      
+00003c70: 2020 2020 2020 6c61 6d62 6461 2072 6f77        lambda row
+00003c80: 3a20 726f 772e 7368 6131 2c0a 2020 2020  : row.sha1,.    
+00003c90: 2020 2020 290a 0a20 2020 2040 6462 5f74      )..    @db_t
+00003ca0: 7261 6e73 6163 7469 6f6e 2873 7461 7465  ransaction(state
+00003cb0: 6d65 6e74 5f74 696d 656f 7574 3d35 3030  ment_timeout=500
+00003cc0: 290a 2020 2020 6465 6620 636f 6e74 656e  ).    def conten
+00003cd0: 745f 6765 7428 0a20 2020 2020 2020 2073  t_get(.        s
+00003ce0: 656c 662c 2063 6f6e 7465 6e74 733a 204c  elf, contents: L
+00003cf0: 6973 745b 6279 7465 735d 2c20 616c 676f  ist[bytes], algo
+00003d00: 3a20 7374 7220 3d20 2273 6861 3122 2c20  : str = "sha1", 
+00003d10: 2a2c 2064 623a 2044 622c 2063 7572 3d4e  *, db: Db, cur=N
+00003d20: 6f6e 650a 2020 2020 2920 2d3e 204c 6973  one.    ) -> Lis
+00003d30: 745b 4f70 7469 6f6e 616c 5b43 6f6e 7465  t[Optional[Conte
+00003d40: 6e74 5d5d 3a0a 2020 2020 2020 2020 636f  nt]]:.        co
+00003d50: 6e74 656e 7473 5f62 795f 6861 7368 3a20  ntents_by_hash: 
+00003d60: 4469 6374 5b62 7974 6573 2c20 4f70 7469  Dict[bytes, Opti
+00003d70: 6f6e 616c 5b43 6f6e 7465 6e74 5d5d 203d  onal[Content]] =
+00003d80: 207b 7d0a 2020 2020 2020 2020 6966 2061   {}.        if a
+00003d90: 6c67 6f20 6e6f 7420 696e 2044 4546 4155  lgo not in DEFAU
+00003da0: 4c54 5f41 4c47 4f52 4954 484d 533a 0a20  LT_ALGORITHMS:. 
+00003db0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00003dc0: 2053 746f 7261 6765 4172 6775 6d65 6e74   StorageArgument
+00003dd0: 4578 6365 7074 696f 6e28 0a20 2020 2020  Exception(.     
+00003de0: 2020 2020 2020 2020 2020 2022 616c 676f             "algo
+00003df0: 2073 686f 756c 6420 6265 206f 6e65 206f   should be one o
+00003e00: 6620 7b27 2c27 2e6a 6f69 6e28 4445 4641  f {','.join(DEFA
+00003e10: 554c 545f 414c 474f 5249 5448 4d53 297d  ULT_ALGORITHMS)}
+00003e20: 220a 2020 2020 2020 2020 2020 2020 290a  ".            ).
+00003e30: 0a20 2020 2020 2020 2072 6f77 7320 3d20  .        rows = 
+00003e40: 6462 2e63 6f6e 7465 6e74 5f67 6574 5f6d  db.content_get_m
+00003e50: 6574 6164 6174 615f 6672 6f6d 5f68 6173  etadata_from_has
+00003e60: 6865 7328 636f 6e74 656e 7473 2c20 616c  hes(contents, al
+00003e70: 676f 2c20 6375 7229 0a20 2020 2020 2020  go, cur).       
+00003e80: 206b 6579 203d 206f 7065 7261 746f 722e   key = operator.
+00003e90: 6174 7472 6765 7474 6572 2861 6c67 6f29  attrgetter(algo)
+00003ea0: 0a0a 2020 2020 2020 2020 666f 7220 726f  ..        for ro
+00003eb0: 7720 696e 2072 6f77 733a 0a20 2020 2020  w in rows:.     
+00003ec0: 2020 2020 2020 2072 6f77 5f64 203d 2064         row_d = d
+00003ed0: 6963 7428 7a69 7028 6462 2e63 6f6e 7465  ict(zip(db.conte
+00003ee0: 6e74 5f67 6574 5f6d 6574 6164 6174 615f  nt_get_metadata_
+00003ef0: 6b65 7973 2c20 726f 7729 290a 2020 2020  keys, row)).    
+00003f00: 2020 2020 2020 2020 636f 6e74 656e 7420          content 
+00003f10: 3d20 436f 6e74 656e 7428 2a2a 726f 775f  = Content(**row_
+00003f20: 6429 0a20 2020 2020 2020 2020 2020 2063  d).            c
+00003f30: 6f6e 7465 6e74 735f 6279 5f68 6173 685b  ontents_by_hash[
+00003f40: 6b65 7928 636f 6e74 656e 7429 5d20 3d20  key(content)] = 
+00003f50: 636f 6e74 656e 740a 0a20 2020 2020 2020  content..       
+00003f60: 2072 6574 7572 6e20 5b63 6f6e 7465 6e74   return [content
+00003f70: 735f 6279 5f68 6173 682e 6765 7428 7368  s_by_hash.get(sh
+00003f80: 6131 2920 666f 7220 7368 6131 2069 6e20  a1) for sha1 in 
+00003f90: 636f 6e74 656e 7473 5d0a 0a20 2020 2040  contents]..    @
+00003fa0: 6462 5f74 7261 6e73 6163 7469 6f6e 5f67  db_transaction_g
+00003fb0: 656e 6572 6174 6f72 2829 0a20 2020 2064  enerator().    d
+00003fc0: 6566 2063 6f6e 7465 6e74 5f6d 6973 7369  ef content_missi
+00003fd0: 6e67 280a 2020 2020 2020 2020 7365 6c66  ng(.        self
+00003fe0: 2c0a 2020 2020 2020 2020 636f 6e74 656e  ,.        conten
+00003ff0: 7473 3a20 4c69 7374 5b48 6173 6844 6963  ts: List[HashDic
+00004000: 745d 2c0a 2020 2020 2020 2020 6b65 795f  t],.        key_
+00004010: 6861 7368 3a20 7374 7220 3d20 2273 6861  hash: str = "sha
+00004020: 3122 2c0a 2020 2020 2020 2020 2a2c 0a20  1",.        *,. 
+00004030: 2020 2020 2020 2064 623a 2044 622c 0a20         db: Db,. 
+00004040: 2020 2020 2020 2063 7572 3d4e 6f6e 652c         cur=None,
+00004050: 0a20 2020 2029 202d 3e20 4974 6572 6162  .    ) -> Iterab
+00004060: 6c65 5b62 7974 6573 5d3a 0a20 2020 2020  le[bytes]:.     
+00004070: 2020 2069 6620 6b65 795f 6861 7368 206e     if key_hash n
+00004080: 6f74 2069 6e20 4445 4641 554c 545f 414c  ot in DEFAULT_AL
+00004090: 474f 5249 5448 4d53 3a0a 2020 2020 2020  GORITHMS:.      
+000040a0: 2020 2020 2020 7261 6973 6520 5374 6f72        raise Stor
+000040b0: 6167 6541 7267 756d 656e 7445 7863 6570  ageArgumentExcep
+000040c0: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
+000040d0: 2020 2020 2020 226b 6579 5f68 6173 6820        "key_hash 
+000040e0: 7368 6f75 6c64 2062 6520 6f6e 6520 6f66  should be one of
+000040f0: 207b 272c 272e 6a6f 696e 2844 4546 4155   {','.join(DEFAU
+00004100: 4c54 5f41 4c47 4f52 4954 484d 5329 7d22  LT_ALGORITHMS)}"
+00004110: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
+00004120: 2020 2020 2020 2020 6b65 7973 203d 2064          keys = d
+00004130: 622e 636f 6e74 656e 745f 6861 7368 5f6b  b.content_hash_k
+00004140: 6579 730a 2020 2020 2020 2020 6b65 795f  eys.        key_
+00004150: 6861 7368 5f69 6478 203d 206b 6579 732e  hash_idx = keys.
+00004160: 696e 6465 7828 6b65 795f 6861 7368 290a  index(key_hash).
+00004170: 0a20 2020 2020 2020 2066 6f72 206f 626a  .        for obj
+00004180: 2069 6e20 6462 2e63 6f6e 7465 6e74 5f6d   in db.content_m
+00004190: 6973 7369 6e67 5f66 726f 6d5f 6c69 7374  issing_from_list
+000041a0: 2863 6f6e 7465 6e74 732c 2063 7572 293a  (contents, cur):
+000041b0: 0a20 2020 2020 2020 2020 2020 2079 6965  .            yie
+000041c0: 6c64 206f 626a 5b6b 6579 5f68 6173 685f  ld obj[key_hash_
+000041d0: 6964 785d 0a0a 2020 2020 4064 625f 7472  idx]..    @db_tr
+000041e0: 616e 7361 6374 696f 6e5f 6765 6e65 7261  ansaction_genera
+000041f0: 746f 7228 290a 2020 2020 6465 6620 636f  tor().    def co
+00004200: 6e74 656e 745f 6d69 7373 696e 675f 7065  ntent_missing_pe
+00004210: 725f 7368 6131 280a 2020 2020 2020 2020  r_sha1(.        
+00004220: 7365 6c66 2c20 636f 6e74 656e 7473 3a20  self, contents: 
+00004230: 4c69 7374 5b62 7974 6573 5d2c 202a 2c20  List[bytes], *, 
+00004240: 6462 3a20 4462 2c20 6375 723d 4e6f 6e65  db: Db, cur=None
+00004250: 0a20 2020 2029 202d 3e20 4974 6572 6162  .    ) -> Iterab
+00004260: 6c65 5b62 7974 6573 5d3a 0a20 2020 2020  le[bytes]:.     
+00004270: 2020 2066 6f72 206f 626a 2069 6e20 6462     for obj in db
+00004280: 2e63 6f6e 7465 6e74 5f6d 6973 7369 6e67  .content_missing
+00004290: 5f70 6572 5f73 6861 3128 636f 6e74 656e  _per_sha1(conten
+000042a0: 7473 2c20 6375 7229 3a0a 2020 2020 2020  ts, cur):.      
+000042b0: 2020 2020 2020 7969 656c 6420 6f62 6a5b        yield obj[
+000042c0: 305d 0a0a 2020 2020 4064 625f 7472 616e  0]..    @db_tran
+000042d0: 7361 6374 696f 6e5f 6765 6e65 7261 746f  saction_generato
+000042e0: 7228 290a 2020 2020 6465 6620 636f 6e74  r().    def cont
+000042f0: 656e 745f 6d69 7373 696e 675f 7065 725f  ent_missing_per_
+00004300: 7368 6131 5f67 6974 280a 2020 2020 2020  sha1_git(.      
+00004310: 2020 7365 6c66 2c20 636f 6e74 656e 7473    self, contents
+00004320: 3a20 4c69 7374 5b62 7974 6573 5d2c 202a  : List[bytes], *
+00004330: 2c20 6462 3a20 4462 2c20 6375 723d 4e6f  , db: Db, cur=No
+00004340: 6e65 0a20 2020 2029 202d 3e20 4974 6572  ne.    ) -> Iter
+00004350: 6162 6c65 5b53 6861 3147 6974 5d3a 0a20  able[Sha1Git]:. 
+00004360: 2020 2020 2020 2066 6f72 206f 626a 2069         for obj i
+00004370: 6e20 6462 2e63 6f6e 7465 6e74 5f6d 6973  n db.content_mis
+00004380: 7369 6e67 5f70 6572 5f73 6861 315f 6769  sing_per_sha1_gi
+00004390: 7428 636f 6e74 656e 7473 2c20 6375 7229  t(contents, cur)
+000043a0: 3a0a 2020 2020 2020 2020 2020 2020 7969  :.            yi
+000043b0: 656c 6420 6f62 6a5b 305d 0a0a 2020 2020  eld obj[0]..    
+000043c0: 4064 625f 7472 616e 7361 6374 696f 6e28  @db_transaction(
+000043d0: 290a 2020 2020 6465 6620 636f 6e74 656e  ).    def conten
+000043e0: 745f 6669 6e64 2873 656c 662c 2063 6f6e  t_find(self, con
+000043f0: 7465 6e74 3a20 4861 7368 4469 6374 2c20  tent: HashDict, 
+00004400: 2a2c 2064 623a 2044 622c 2063 7572 3d4e  *, db: Db, cur=N
+00004410: 6f6e 6529 202d 3e20 4c69 7374 5b43 6f6e  one) -> List[Con
+00004420: 7465 6e74 5d3a 0a20 2020 2020 2020 2069  tent]:.        i
+00004430: 6620 6e6f 7420 7365 7428 636f 6e74 656e  f not set(conten
+00004440: 7429 2e69 6e74 6572 7365 6374 696f 6e28  t).intersection(
+00004450: 4445 4641 554c 545f 414c 474f 5249 5448  DEFAULT_ALGORITH
+00004460: 4d53 293a 0a20 2020 2020 2020 2020 2020  MS):.           
+00004470: 2072 6169 7365 2053 746f 7261 6765 4172   raise StorageAr
+00004480: 6775 6d65 6e74 4578 6365 7074 696f 6e28  gumentException(
+00004490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000044a0: 2022 636f 6e74 656e 7420 6b65 7973 206d   "content keys m
+000044b0: 7573 7420 636f 6e74 6169 6e20 6174 206c  ust contain at l
+000044c0: 6561 7374 206f 6e65 2022 0a20 2020 2020  east one ".     
+000044d0: 2020 2020 2020 2020 2020 2066 226f 663a             f"of:
+000044e0: 207b 272c 2027 2e6a 6f69 6e28 736f 7274   {', '.join(sort
+000044f0: 6564 2844 4546 4155 4c54 5f41 4c47 4f52  ed(DEFAULT_ALGOR
+00004500: 4954 484d 5329 297d 220a 2020 2020 2020  ITHMS))}".      
+00004510: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00004520: 2072 6f77 7320 3d20 6462 2e63 6f6e 7465   rows = db.conte
+00004530: 6e74 5f66 696e 6428 0a20 2020 2020 2020  nt_find(.       
+00004540: 2020 2020 2073 6861 313d 636f 6e74 656e       sha1=conten
+00004550: 742e 6765 7428 2273 6861 3122 292c 0a20  t.get("sha1"),. 
+00004560: 2020 2020 2020 2020 2020 2073 6861 315f             sha1_
+00004570: 6769 743d 636f 6e74 656e 742e 6765 7428  git=content.get(
+00004580: 2273 6861 315f 6769 7422 292c 0a20 2020  "sha1_git"),.   
+00004590: 2020 2020 2020 2020 2073 6861 3235 363d           sha256=
+000045a0: 636f 6e74 656e 742e 6765 7428 2273 6861  content.get("sha
+000045b0: 3235 3622 292c 0a20 2020 2020 2020 2020  256"),.         
+000045c0: 2020 2062 6c61 6b65 3273 3235 363d 636f     blake2s256=co
+000045d0: 6e74 656e 742e 6765 7428 2262 6c61 6b65  ntent.get("blake
+000045e0: 3273 3235 3622 292c 0a20 2020 2020 2020  2s256"),.       
+000045f0: 2020 2020 2063 7572 3d63 7572 2c0a 2020       cur=cur,.  
+00004600: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00004610: 636f 6e74 656e 7473 203d 205b 5d0a 2020  contents = [].  
+00004620: 2020 2020 2020 666f 7220 726f 7720 696e        for row in
+00004630: 2072 6f77 733a 0a20 2020 2020 2020 2020   rows:.         
+00004640: 2020 2072 6f77 5f64 203d 2064 6963 7428     row_d = dict(
+00004650: 7a69 7028 6462 2e63 6f6e 7465 6e74 5f66  zip(db.content_f
+00004660: 696e 645f 636f 6c73 2c20 726f 7729 290a  ind_cols, row)).
+00004670: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+00004680: 656e 7473 2e61 7070 656e 6428 436f 6e74  ents.append(Cont
+00004690: 656e 7428 2a2a 726f 775f 6429 290a 2020  ent(**row_d)).  
+000046a0: 2020 2020 2020 7265 7475 726e 2063 6f6e        return con
+000046b0: 7465 6e74 730a 0a20 2020 2040 6462 5f74  tents..    @db_t
+000046c0: 7261 6e73 6163 7469 6f6e 2829 0a20 2020  ransaction().   
+000046d0: 2064 6566 2063 6f6e 7465 6e74 5f67 6574   def content_get
+000046e0: 5f72 616e 646f 6d28 7365 6c66 2c20 2a2c  _random(self, *,
+000046f0: 2064 623a 2044 622c 2063 7572 3d4e 6f6e   db: Db, cur=Non
+00004700: 6529 202d 3e20 5368 6131 4769 743a 0a20  e) -> Sha1Git:. 
+00004710: 2020 2020 2020 2072 6574 7572 6e20 6462         return db
+00004720: 2e63 6f6e 7465 6e74 5f67 6574 5f72 616e  .content_get_ran
+00004730: 646f 6d28 6375 7229 0a0a 2020 2020 2323  dom(cur)..    ##
 00004740: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004750: 0a20 2020 2023 2053 6b69 7070 6564 436f  .    # SkippedCo
-00004760: 6e74 656e 740a 2020 2020 2323 2323 2323  ntent.    ######
-00004770: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004780: 2323 2323 0a0a 2020 2020 4073 7461 7469  ####..    @stati
-00004790: 636d 6574 686f 640a 2020 2020 6465 6620  cmethod.    def 
-000047a0: 5f73 6b69 7070 6564 5f63 6f6e 7465 6e74  _skipped_content
-000047b0: 5f6e 6f72 6d61 6c69 7a65 2864 293a 0a20  _normalize(d):. 
-000047c0: 2020 2020 2020 2064 203d 2064 2e63 6f70         d = d.cop
-000047d0: 7928 290a 0a20 2020 2020 2020 2069 6620  y()..        if 
-000047e0: 642e 6765 7428 2273 7461 7475 7322 2920  d.get("status") 
-000047f0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00004800: 2020 2020 2064 5b22 7374 6174 7573 225d       d["status"]
-00004810: 203d 2022 6162 7365 6e74 220a 0a20 2020   = "absent"..   
-00004820: 2020 2020 2069 6620 642e 6765 7428 226c       if d.get("l
-00004830: 656e 6774 6822 2920 6973 204e 6f6e 653a  ength") is None:
-00004840: 0a20 2020 2020 2020 2020 2020 2064 5b22  .            d["
-00004850: 6c65 6e67 7468 225d 203d 202d 310a 0a20  length"] = -1.. 
-00004860: 2020 2020 2020 2072 6574 7572 6e20 640a         return d.
-00004870: 0a20 2020 2064 6566 205f 736b 6970 7065  .    def _skippe
-00004880: 645f 636f 6e74 656e 745f 6164 645f 6d65  d_content_add_me
-00004890: 7461 6461 7461 2873 656c 662c 2064 622c  tadata(self, db,
-000048a0: 2063 7572 2c20 636f 6e74 656e 743a 204c   cur, content: L
-000048b0: 6973 745b 536b 6970 7065 6443 6f6e 7465  ist[SkippedConte
-000048c0: 6e74 5d29 3a0a 2020 2020 2020 2020 6f72  nt]):.        or
-000048d0: 6967 696e 5f69 6473 203d 2064 622e 6f72  igin_ids = db.or
-000048e0: 6967 696e 5f69 645f 6765 745f 6279 5f75  igin_id_get_by_u
-000048f0: 726c 285b 636f 6e74 2e6f 7269 6769 6e20  rl([cont.origin 
-00004900: 666f 7220 636f 6e74 2069 6e20 636f 6e74  for cont in cont
-00004910: 656e 745d 2c20 6375 723d 6375 7229 0a20  ent], cur=cur). 
-00004920: 2020 2020 2020 2063 6f6e 7465 6e74 203d         content =
-00004930: 205b 0a20 2020 2020 2020 2020 2020 2061   [.            a
-00004940: 7474 722e 6576 6f6c 7665 2863 2c20 6f72  ttr.evolve(c, or
-00004950: 6967 696e 3d6f 7269 6769 6e5f 6964 290a  igin=origin_id).
-00004960: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00004970: 2863 2c20 6f72 6967 696e 5f69 6429 2069  (c, origin_id) i
-00004980: 6e20 7a69 7028 636f 6e74 656e 742c 206f  n zip(content, o
-00004990: 7269 6769 6e5f 6964 7329 0a20 2020 2020  rigin_ids).     
-000049a0: 2020 205d 0a20 2020 2020 2020 2064 622e     ].        db.
-000049b0: 6d6b 7465 6d70 2822 736b 6970 7065 645f  mktemp("skipped_
-000049c0: 636f 6e74 656e 7422 2c20 6375 7229 0a20  content", cur). 
-000049d0: 2020 2020 2020 2064 622e 636f 7079 5f74         db.copy_t
-000049e0: 6f28 0a20 2020 2020 2020 2020 2020 205b  o(.            [
-000049f0: 632e 746f 5f64 6963 7428 2920 666f 7220  c.to_dict() for 
-00004a00: 6320 696e 2063 6f6e 7465 6e74 5d2c 0a20  c in content],. 
-00004a10: 2020 2020 2020 2020 2020 2022 746d 705f             "tmp_
-00004a20: 736b 6970 7065 645f 636f 6e74 656e 7422  skipped_content"
-00004a30: 2c0a 2020 2020 2020 2020 2020 2020 6462  ,.            db
-00004a40: 2e73 6b69 7070 6564 5f63 6f6e 7465 6e74  .skipped_content
-00004a50: 5f6b 6579 732c 0a20 2020 2020 2020 2020  _keys,.         
-00004a60: 2020 2063 7572 2c0a 2020 2020 2020 2020     cur,.        
-00004a70: 290a 0a20 2020 2020 2020 2023 206d 6f76  )..        # mov
-00004a80: 6520 6d65 7461 6461 7461 2069 6e20 706c  e metadata in pl
-00004a90: 6163 650a 2020 2020 2020 2020 6462 2e73  ace.        db.s
-00004aa0: 6b69 7070 6564 5f63 6f6e 7465 6e74 5f61  kipped_content_a
-00004ab0: 6464 5f66 726f 6d5f 7465 6d70 2863 7572  dd_from_temp(cur
-00004ac0: 290a 0a20 2020 2040 6462 5f74 7261 6e73  )..    @db_trans
-00004ad0: 6163 7469 6f6e 2829 0a20 2020 2064 6566  action().    def
-00004ae0: 2073 6b69 7070 6564 5f63 6f6e 7465 6e74   skipped_content
-00004af0: 5f61 6464 280a 2020 2020 2020 2020 7365  _add(.        se
-00004b00: 6c66 2c20 636f 6e74 656e 743a 204c 6973  lf, content: Lis
-00004b10: 745b 536b 6970 7065 6443 6f6e 7465 6e74  t[SkippedContent
-00004b20: 5d2c 202a 2c20 6462 3a20 4462 2c20 6375  ], *, db: Db, cu
-00004b30: 723d 4e6f 6e65 0a20 2020 2029 202d 3e20  r=None.    ) -> 
-00004b40: 4469 6374 5b73 7472 2c20 696e 745d 3a0a  Dict[str, int]:.
-00004b50: 2020 2020 2020 2020 6374 696d 6520 3d20          ctime = 
-00004b60: 6e6f 7728 290a 2020 2020 2020 2020 636f  now().        co
-00004b70: 6e74 656e 7420 3d20 5b61 7474 722e 6576  ntent = [attr.ev
-00004b80: 6f6c 7665 2863 2c20 6374 696d 653d 6374  olve(c, ctime=ct
-00004b90: 696d 6529 2066 6f72 2063 2069 6e20 636f  ime) for c in co
-00004ba0: 6e74 656e 745d 0a0a 2020 2020 2020 2020  ntent]..        
-00004bb0: 6d69 7373 696e 675f 636f 6e74 656e 7473  missing_contents
-00004bc0: 203d 2073 656c 662e 736b 6970 7065 645f   = self.skipped_
-00004bd0: 636f 6e74 656e 745f 6d69 7373 696e 6728  content_missing(
-00004be0: 0a20 2020 2020 2020 2020 2020 2028 632e  .            (c.
-00004bf0: 746f 5f64 6963 7428 2920 666f 7220 6320  to_dict() for c 
-00004c00: 696e 2063 6f6e 7465 6e74 292c 0a20 2020  in content),.   
-00004c10: 2020 2020 2020 2020 2064 623d 6462 2c0a           db=db,.
-00004c20: 2020 2020 2020 2020 2020 2020 6375 723d              cur=
-00004c30: 6375 722c 0a20 2020 2020 2020 2029 0a20  cur,.        ). 
-00004c40: 2020 2020 2020 2063 6f6e 7465 6e74 203d         content =
-00004c50: 205b 0a20 2020 2020 2020 2020 2020 2063   [.            c
-00004c60: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00004c70: 2063 2069 6e20 636f 6e74 656e 740a 2020   c in content.  
-00004c80: 2020 2020 2020 2020 2020 6966 2061 6e79            if any
-00004c90: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00004ca0: 2020 616c 6c28 0a20 2020 2020 2020 2020    all(.         
-00004cb0: 2020 2020 2020 2020 2020 2063 2e67 6574             c.get
-00004cc0: 5f68 6173 6828 616c 676f 2920 3d3d 206d  _hash(algo) == m
-00004cd0: 6973 7369 6e67 5f63 6f6e 7465 6e74 2e67  issing_content.g
-00004ce0: 6574 2861 6c67 6f29 0a20 2020 2020 2020  et(algo).       
-00004cf0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00004d00: 2061 6c67 6f20 696e 2044 4546 4155 4c54   algo in DEFAULT
-00004d10: 5f41 4c47 4f52 4954 484d 530a 2020 2020  _ALGORITHMS.    
-00004d20: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00004d30: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00004d40: 7220 6d69 7373 696e 675f 636f 6e74 656e  r missing_conten
-00004d50: 7420 696e 206d 6973 7369 6e67 5f63 6f6e  t in missing_con
-00004d60: 7465 6e74 730a 2020 2020 2020 2020 2020  tents.          
-00004d70: 2020 290a 2020 2020 2020 2020 5d0a 0a20    ).        ].. 
-00004d80: 2020 2020 2020 2073 656c 662e 6a6f 7572         self.jour
-00004d90: 6e61 6c5f 7772 6974 6572 2e73 6b69 7070  nal_writer.skipp
-00004da0: 6564 5f63 6f6e 7465 6e74 5f61 6464 2863  ed_content_add(c
-00004db0: 6f6e 7465 6e74 290a 2020 2020 2020 2020  ontent).        
-00004dc0: 7365 6c66 2e5f 736b 6970 7065 645f 636f  self._skipped_co
-00004dd0: 6e74 656e 745f 6164 645f 6d65 7461 6461  ntent_add_metada
-00004de0: 7461 2864 622c 2063 7572 2c20 636f 6e74  ta(db, cur, cont
-00004df0: 656e 7429 0a0a 2020 2020 2020 2020 7265  ent)..        re
-00004e00: 7475 726e 207b 0a20 2020 2020 2020 2020  turn {.         
-00004e10: 2020 2022 736b 6970 7065 645f 636f 6e74     "skipped_cont
-00004e20: 656e 743a 6164 6422 3a20 6c65 6e28 636f  ent:add": len(co
-00004e30: 6e74 656e 7429 2c0a 2020 2020 2020 2020  ntent),.        
-00004e40: 7d0a 0a20 2020 2040 6462 5f74 7261 6e73  }..    @db_trans
-00004e50: 6163 7469 6f6e 2829 0a20 2020 2064 6566  action().    def
-00004e60: 2073 6b69 7070 6564 5f63 6f6e 7465 6e74   skipped_content
-00004e70: 5f66 696e 6428 0a20 2020 2020 2020 2073  _find(.        s
-00004e80: 656c 662c 2063 6f6e 7465 6e74 3a20 4861  elf, content: Ha
-00004e90: 7368 4469 6374 2c20 2a2c 2064 623a 2044  shDict, *, db: D
-00004ea0: 622c 2063 7572 3d4e 6f6e 650a 2020 2020  b, cur=None.    
-00004eb0: 2920 2d3e 204c 6973 745b 536b 6970 7065  ) -> List[Skippe
-00004ec0: 6443 6f6e 7465 6e74 5d3a 0a20 2020 2020  dContent]:.     
-00004ed0: 2020 2069 6620 6e6f 7420 7365 7428 636f     if not set(co
-00004ee0: 6e74 656e 7429 2e69 6e74 6572 7365 6374  ntent).intersect
-00004ef0: 696f 6e28 4445 4641 554c 545f 414c 474f  ion(DEFAULT_ALGO
-00004f00: 5249 5448 4d53 293a 0a20 2020 2020 2020  RITHMS):.       
-00004f10: 2020 2020 2072 6169 7365 2053 746f 7261       raise Stora
-00004f20: 6765 4172 6775 6d65 6e74 4578 6365 7074  geArgumentExcept
-00004f30: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
-00004f40: 2020 2020 2022 636f 6e74 656e 7420 6b65       "content ke
-00004f50: 7973 206d 7573 7420 636f 6e74 6169 6e20  ys must contain 
-00004f60: 6174 206c 6561 7374 206f 6e65 2022 0a20  at least one ". 
-00004f70: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00004f80: 226f 663a 207b 272c 2027 2e6a 6f69 6e28  "of: {', '.join(
-00004f90: 736f 7274 6564 2844 4546 4155 4c54 5f41  sorted(DEFAULT_A
-00004fa0: 4c47 4f52 4954 484d 5329 297d 220a 2020  LGORITHMS))}".  
-00004fb0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-00004fc0: 2020 2020 2072 6f77 7320 3d20 6462 2e73       rows = db.s
-00004fd0: 6b69 7070 6564 5f63 6f6e 7465 6e74 5f66  kipped_content_f
-00004fe0: 696e 6428 0a20 2020 2020 2020 2020 2020  ind(.           
-00004ff0: 2073 6861 313d 636f 6e74 656e 742e 6765   sha1=content.ge
-00005000: 7428 2273 6861 3122 292c 0a20 2020 2020  t("sha1"),.     
-00005010: 2020 2020 2020 2073 6861 315f 6769 743d         sha1_git=
-00005020: 636f 6e74 656e 742e 6765 7428 2273 6861  content.get("sha
-00005030: 315f 6769 7422 292c 0a20 2020 2020 2020  1_git"),.       
-00005040: 2020 2020 2073 6861 3235 363d 636f 6e74       sha256=cont
-00005050: 656e 742e 6765 7428 2273 6861 3235 3622  ent.get("sha256"
-00005060: 292c 0a20 2020 2020 2020 2020 2020 2062  ),.            b
-00005070: 6c61 6b65 3273 3235 363d 636f 6e74 656e  lake2s256=conten
-00005080: 742e 6765 7428 2262 6c61 6b65 3273 3235  t.get("blake2s25
-00005090: 3622 292c 0a20 2020 2020 2020 2020 2020  6"),.           
-000050a0: 2063 7572 3d63 7572 2c0a 2020 2020 2020   cur=cur,.      
-000050b0: 2020 290a 2020 2020 2020 2020 736b 6970    ).        skip
-000050c0: 7065 645f 636f 6e74 656e 7473 203d 205b  ped_contents = [
-000050d0: 5d0a 2020 2020 2020 2020 666f 7220 726f  ].        for ro
-000050e0: 7720 696e 2072 6f77 733a 0a20 2020 2020  w in rows:.     
-000050f0: 2020 2020 2020 2072 6f77 5f64 203d 2064         row_d = d
-00005100: 6963 7428 7a69 7028 6462 2e73 6b69 7070  ict(zip(db.skipp
-00005110: 6564 5f63 6f6e 7465 6e74 5f66 696e 645f  ed_content_find_
-00005120: 636f 6c73 2c20 726f 7729 290a 2020 2020  cols, row)).    
-00005130: 2020 2020 2020 2020 736b 6970 7065 645f          skipped_
-00005140: 636f 6e74 656e 7473 2e61 7070 656e 6428  contents.append(
-00005150: 536b 6970 7065 6443 6f6e 7465 6e74 282a  SkippedContent(*
-00005160: 2a72 6f77 5f64 2929 0a20 2020 2020 2020  *row_d)).       
-00005170: 2072 6574 7572 6e20 736b 6970 7065 645f   return skipped_
-00005180: 636f 6e74 656e 7473 0a0a 2020 2020 4064  contents..    @d
-00005190: 625f 7472 616e 7361 6374 696f 6e5f 6765  b_transaction_ge
-000051a0: 6e65 7261 746f 7228 290a 2020 2020 6465  nerator().    de
-000051b0: 6620 736b 6970 7065 645f 636f 6e74 656e  f skipped_conten
-000051c0: 745f 6d69 7373 696e 6728 0a20 2020 2020  t_missing(.     
-000051d0: 2020 2073 656c 662c 2063 6f6e 7465 6e74     self, content
-000051e0: 733a 204c 6973 745b 4469 6374 5b73 7472  s: List[Dict[str
-000051f0: 2c20 416e 795d 5d2c 202a 2c20 6462 3a20  , Any]], *, db: 
-00005200: 4462 2c20 6375 723d 4e6f 6e65 0a20 2020  Db, cur=None.   
-00005210: 2029 202d 3e20 4974 6572 6162 6c65 5b44   ) -> Iterable[D
-00005220: 6963 745b 7374 722c 2041 6e79 5d5d 3a0a  ict[str, Any]]:.
-00005230: 2020 2020 2020 2020 636f 6e74 656e 7473          contents
-00005240: 203d 206c 6973 7428 636f 6e74 656e 7473   = list(contents
-00005250: 290a 2020 2020 2020 2020 666f 7220 636f  ).        for co
-00005260: 6e74 656e 7420 696e 2064 622e 736b 6970  ntent in db.skip
-00005270: 7065 645f 636f 6e74 656e 745f 6d69 7373  ped_content_miss
-00005280: 696e 6728 636f 6e74 656e 7473 2c20 6375  ing(contents, cu
-00005290: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-000052a0: 7969 656c 6420 7b0a 2020 2020 2020 2020  yield {.        
-000052b0: 2020 2020 2020 2020 616c 676f 3a20 6861          algo: ha
-000052c0: 7368 0a20 2020 2020 2020 2020 2020 2020  sh.             
-000052d0: 2020 2066 6f72 2028 616c 676f 2c20 6861     for (algo, ha
-000052e0: 7368 2920 696e 207a 6970 2864 622e 636f  sh) in zip(db.co
-000052f0: 6e74 656e 745f 6861 7368 5f6b 6579 732c  ntent_hash_keys,
-00005300: 2063 6f6e 7465 6e74 290a 2020 2020 2020   content).      
-00005310: 2020 2020 2020 2020 2020 6966 2068 6173            if has
-00005320: 680a 2020 2020 2020 2020 2020 2020 7d0a  h.            }.
-00005330: 0a20 2020 2023 2323 2323 2323 2323 2323  .    ###########
-00005340: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
-00005350: 2020 2020 2320 4469 7265 6374 6f72 790a      # Directory.
-00005360: 2020 2020 2323 2323 2323 2323 2323 2323      ############
-00005370: 2323 2323 2323 2323 2323 2323 2323 0a0a  ##############..
-00005380: 2020 2020 4064 625f 7472 616e 7361 6374      @db_transact
-00005390: 696f 6e28 290a 2020 2020 6465 6620 6469  ion().    def di
-000053a0: 7265 6374 6f72 795f 6164 6428 0a20 2020  rectory_add(.   
-000053b0: 2020 2020 2073 656c 662c 2064 6972 6563       self, direc
-000053c0: 746f 7269 6573 3a20 4c69 7374 5b44 6972  tories: List[Dir
-000053d0: 6563 746f 7279 5d2c 202a 2c20 6462 3a20  ectory], *, db: 
-000053e0: 4462 2c20 6375 723d 4e6f 6e65 0a20 2020  Db, cur=None.   
-000053f0: 2029 202d 3e20 4469 6374 5b73 7472 2c20   ) -> Dict[str, 
-00005400: 696e 745d 3a0a 2020 2020 2020 2020 7375  int]:.        su
-00005410: 6d6d 6172 7920 3d20 7b22 6469 7265 6374  mmary = {"direct
-00005420: 6f72 793a 6164 6422 3a20 307d 0a0a 2020  ory:add": 0}..  
-00005430: 2020 2020 2020 6469 7273 203d 2073 6574        dirs = set
-00005440: 2829 0a20 2020 2020 2020 2064 6972 5f65  ().        dir_e
-00005450: 6e74 7269 6573 3a20 4469 6374 5b73 7472  ntries: Dict[str
-00005460: 2c20 6465 6661 756c 7464 6963 745d 203d  , defaultdict] =
-00005470: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
-00005480: 6669 6c65 223a 2064 6566 6175 6c74 6469  file": defaultdi
-00005490: 6374 286c 6973 7429 2c0a 2020 2020 2020  ct(list),.      
-000054a0: 2020 2020 2020 2264 6972 223a 2064 6566        "dir": def
-000054b0: 6175 6c74 6469 6374 286c 6973 7429 2c0a  aultdict(list),.
-000054c0: 2020 2020 2020 2020 2020 2020 2272 6576              "rev
-000054d0: 223a 2064 6566 6175 6c74 6469 6374 286c  ": defaultdict(l
-000054e0: 6973 7429 2c0a 2020 2020 2020 2020 7d0a  ist),.        }.
-000054f0: 0a20 2020 2020 2020 2066 6f72 2063 7572  .        for cur
-00005500: 5f64 6972 2069 6e20 6469 7265 6374 6f72  _dir in director
-00005510: 6965 733a 0a20 2020 2020 2020 2020 2020  ies:.           
-00005520: 2064 6972 5f69 6420 3d20 6375 725f 6469   dir_id = cur_di
-00005530: 722e 6964 0a20 2020 2020 2020 2020 2020  r.id.           
-00005540: 2064 6972 732e 6164 6428 6469 725f 6964   dirs.add(dir_id
-00005550: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
-00005560: 7220 7372 635f 656e 7472 7920 696e 2063  r src_entry in c
-00005570: 7572 5f64 6972 2e65 6e74 7269 6573 3a0a  ur_dir.entries:.
-00005580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005590: 656e 7472 7920 3d20 7372 635f 656e 7472  entry = src_entr
-000055a0: 792e 746f 5f64 6963 7428 290a 2020 2020  y.to_dict().    
-000055b0: 2020 2020 2020 2020 2020 2020 656e 7472              entr
-000055c0: 795b 2264 6972 5f69 6422 5d20 3d20 6469  y["dir_id"] = di
-000055d0: 725f 6964 0a20 2020 2020 2020 2020 2020  r_id.           
-000055e0: 2020 2020 2064 6972 5f65 6e74 7269 6573       dir_entries
-000055f0: 5b65 6e74 7279 5b22 7479 7065 225d 5d5b  [entry["type"]][
-00005600: 6469 725f 6964 5d2e 6170 7065 6e64 2865  dir_id].append(e
-00005610: 6e74 7279 290a 0a20 2020 2020 2020 2064  ntry)..        d
-00005620: 6972 735f 6d69 7373 696e 6720 3d20 7365  irs_missing = se
-00005630: 7428 7365 6c66 2e64 6972 6563 746f 7279  t(self.directory
-00005640: 5f6d 6973 7369 6e67 2864 6972 732c 2064  _missing(dirs, d
-00005650: 623d 6462 2c20 6375 723d 6375 7229 290a  b=db, cur=cur)).
-00005660: 2020 2020 2020 2020 6966 206e 6f74 2064          if not d
-00005670: 6972 735f 6d69 7373 696e 673a 0a20 2020  irs_missing:.   
-00005680: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00005690: 7375 6d6d 6172 790a 0a20 2020 2020 2020  summary..       
-000056a0: 2073 656c 662e 6a6f 7572 6e61 6c5f 7772   self.journal_wr
-000056b0: 6974 6572 2e64 6972 6563 746f 7279 5f61  iter.directory_a
-000056c0: 6464 280a 2020 2020 2020 2020 2020 2020  dd(.            
-000056d0: 6469 725f 2066 6f72 2064 6972 5f20 696e  dir_ for dir_ in
-000056e0: 2064 6972 6563 746f 7269 6573 2069 6620   directories if 
-000056f0: 6469 725f 2e69 6420 696e 2064 6972 735f  dir_.id in dirs_
-00005700: 6d69 7373 696e 670a 2020 2020 2020 2020  missing.        
-00005710: 290a 0a20 2020 2020 2020 2023 2043 6f70  )..        # Cop
-00005720: 7920 6469 7265 6374 6f72 7920 6d65 7461  y directory meta
-00005730: 6461 7461 0a20 2020 2020 2020 2064 6972  data.        dir
-00005740: 735f 6d69 7373 696e 675f 6469 6374 203d  s_missing_dict =
-00005750: 2028 0a20 2020 2020 2020 2020 2020 207b   (.            {
-00005760: 2269 6422 3a20 6469 725f 2e69 642c 2022  "id": dir_.id, "
-00005770: 7261 775f 6d61 6e69 6665 7374 223a 2064  raw_manifest": d
-00005780: 6972 5f2e 7261 775f 6d61 6e69 6665 7374  ir_.raw_manifest
-00005790: 7d0a 2020 2020 2020 2020 2020 2020 666f  }.            fo
-000057a0: 7220 6469 725f 2069 6e20 6469 7265 6374  r dir_ in direct
-000057b0: 6f72 6965 730a 2020 2020 2020 2020 2020  ories.          
-000057c0: 2020 6966 2064 6972 5f2e 6964 2069 6e20    if dir_.id in 
-000057d0: 6469 7273 5f6d 6973 7369 6e67 0a20 2020  dirs_missing.   
-000057e0: 2020 2020 2029 0a20 2020 2020 2020 2064       ).        d
-000057f0: 622e 6d6b 7465 6d70 2822 6469 7265 6374  b.mktemp("direct
-00005800: 6f72 7922 2c20 6375 7229 0a20 2020 2020  ory", cur).     
-00005810: 2020 2064 622e 636f 7079 5f74 6f28 6469     db.copy_to(di
-00005820: 7273 5f6d 6973 7369 6e67 5f64 6963 742c  rs_missing_dict,
-00005830: 2022 746d 705f 6469 7265 6374 6f72 7922   "tmp_directory"
-00005840: 2c20 5b22 6964 222c 2022 7261 775f 6d61  , ["id", "raw_ma
-00005850: 6e69 6665 7374 225d 2c20 6375 7229 0a0a  nifest"], cur)..
-00005860: 2020 2020 2020 2020 2320 436f 7079 2065          # Copy e
-00005870: 6e74 7269 6573 0a20 2020 2020 2020 2066  ntries.        f
-00005880: 6f72 2065 6e74 7279 5f74 7970 652c 2065  or entry_type, e
-00005890: 6e74 7279 5f6c 6973 7420 696e 2064 6972  ntry_list in dir
-000058a0: 5f65 6e74 7269 6573 2e69 7465 6d73 2829  _entries.items()
-000058b0: 3a0a 2020 2020 2020 2020 2020 2020 656e  :.            en
-000058c0: 7472 6965 7320 3d20 6974 6572 746f 6f6c  tries = itertool
-000058d0: 732e 6368 6169 6e2e 6672 6f6d 5f69 7465  s.chain.from_ite
-000058e0: 7261 626c 6528 0a20 2020 2020 2020 2020  rable(.         
-000058f0: 2020 2020 2020 2065 6e74 7269 6573 5f66         entries_f
-00005900: 6f72 5f64 6972 0a20 2020 2020 2020 2020  or_dir.         
-00005910: 2020 2020 2020 2066 6f72 2064 6972 5f69         for dir_i
-00005920: 642c 2065 6e74 7269 6573 5f66 6f72 5f64  d, entries_for_d
-00005930: 6972 2069 6e20 656e 7472 795f 6c69 7374  ir in entry_list
-00005940: 2e69 7465 6d73 2829 0a20 2020 2020 2020  .items().       
-00005950: 2020 2020 2020 2020 2069 6620 6469 725f           if dir_
-00005960: 6964 2069 6e20 6469 7273 5f6d 6973 7369  id in dirs_missi
-00005970: 6e67 0a20 2020 2020 2020 2020 2020 2029  ng.            )
-00005980: 0a0a 2020 2020 2020 2020 2020 2020 6462  ..            db
-00005990: 2e6d 6b74 656d 705f 6469 725f 656e 7472  .mktemp_dir_entr
-000059a0: 7928 656e 7472 795f 7479 7065 290a 0a20  y(entry_type).. 
-000059b0: 2020 2020 2020 2020 2020 2064 622e 636f             db.co
-000059c0: 7079 5f74 6f28 0a20 2020 2020 2020 2020  py_to(.         
-000059d0: 2020 2020 2020 2065 6e74 7269 6573 2c0a         entries,.
-000059e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059f0: 2274 6d70 5f64 6972 6563 746f 7279 5f65  "tmp_directory_e
-00005a00: 6e74 7279 5f25 7322 2025 2065 6e74 7279  ntry_%s" % entry
-00005a10: 5f74 7970 652c 0a20 2020 2020 2020 2020  _type,.         
-00005a20: 2020 2020 2020 205b 2274 6172 6765 7422         ["target"
-00005a30: 2c20 226e 616d 6522 2c20 2270 6572 6d73  , "name", "perms
-00005a40: 222c 2022 6469 725f 6964 225d 2c0a 2020  ", "dir_id"],.  
-00005a50: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00005a60: 722c 0a20 2020 2020 2020 2020 2020 2029  r,.            )
-00005a70: 0a0a 2020 2020 2020 2020 2320 446f 2074  ..        # Do t
-00005a80: 6865 2066 696e 616c 2063 6f70 790a 2020  he final copy.  
-00005a90: 2020 2020 2020 6462 2e64 6972 6563 746f        db.directo
-00005aa0: 7279 5f61 6464 5f66 726f 6d5f 7465 6d70  ry_add_from_temp
-00005ab0: 2863 7572 290a 2020 2020 2020 2020 7375  (cur).        su
-00005ac0: 6d6d 6172 795b 2264 6972 6563 746f 7279  mmary["directory
-00005ad0: 3a61 6464 225d 203d 206c 656e 2864 6972  :add"] = len(dir
-00005ae0: 735f 6d69 7373 696e 6729 0a0a 2020 2020  s_missing)..    
-00005af0: 2020 2020 7265 7475 726e 2073 756d 6d61      return summa
-00005b00: 7279 0a0a 2020 2020 4064 625f 7472 616e  ry..    @db_tran
-00005b10: 7361 6374 696f 6e5f 6765 6e65 7261 746f  saction_generato
-00005b20: 7228 290a 2020 2020 6465 6620 6469 7265  r().    def dire
-00005b30: 6374 6f72 795f 6d69 7373 696e 6728 0a20  ctory_missing(. 
-00005b40: 2020 2020 2020 2073 656c 662c 2064 6972         self, dir
-00005b50: 6563 746f 7269 6573 3a20 4c69 7374 5b53  ectories: List[S
-00005b60: 6861 3147 6974 5d2c 202a 2c20 6462 3a20  ha1Git], *, db: 
-00005b70: 4462 2c20 6375 723d 4e6f 6e65 0a20 2020  Db, cur=None.   
-00005b80: 2029 202d 3e20 4974 6572 6162 6c65 5b53   ) -> Iterable[S
-00005b90: 6861 3147 6974 5d3a 0a20 2020 2020 2020  ha1Git]:.       
-00005ba0: 2066 6f72 206f 626a 2069 6e20 6462 2e64   for obj in db.d
-00005bb0: 6972 6563 746f 7279 5f6d 6973 7369 6e67  irectory_missing
-00005bc0: 5f66 726f 6d5f 6c69 7374 2864 6972 6563  _from_list(direc
-00005bd0: 746f 7269 6573 2c20 6375 7229 3a0a 2020  tories, cur):.  
-00005be0: 2020 2020 2020 2020 2020 7969 656c 6420            yield 
-00005bf0: 6f62 6a5b 305d 0a0a 2020 2020 4064 625f  obj[0]..    @db_
-00005c00: 7472 616e 7361 6374 696f 6e5f 6765 6e65  transaction_gene
-00005c10: 7261 746f 7228 7374 6174 656d 656e 745f  rator(statement_
-00005c20: 7469 6d65 6f75 743d 3230 3030 3029 0a20  timeout=20000). 
-00005c30: 2020 2064 6566 2064 6972 6563 746f 7279     def directory
-00005c40: 5f6c 7328 0a20 2020 2020 2020 2073 656c  _ls(.        sel
-00005c50: 662c 2064 6972 6563 746f 7279 3a20 5368  f, directory: Sh
-00005c60: 6131 4769 742c 2072 6563 7572 7369 7665  a1Git, recursive
-00005c70: 3a20 626f 6f6c 203d 2046 616c 7365 2c20  : bool = False, 
-00005c80: 2a2c 2064 623a 2044 622c 2063 7572 3d4e  *, db: Db, cur=N
-00005c90: 6f6e 650a 2020 2020 2920 2d3e 2049 7465  one.    ) -> Ite
-00005ca0: 7261 626c 655b 4469 6374 5b73 7472 2c20  rable[Dict[str, 
-00005cb0: 416e 795d 5d3a 0a20 2020 2020 2020 2069  Any]]:.        i
-00005cc0: 6620 7265 6375 7273 6976 653a 0a20 2020  f recursive:.   
-00005cd0: 2020 2020 2020 2020 2072 6573 5f67 656e           res_gen
-00005ce0: 203d 2064 622e 6469 7265 6374 6f72 795f   = db.directory_
-00005cf0: 7761 6c6b 2864 6972 6563 746f 7279 2c20  walk(directory, 
-00005d00: 6375 723d 6375 7229 0a20 2020 2020 2020  cur=cur).       
-00005d10: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00005d20: 2020 2072 6573 5f67 656e 203d 2064 622e     res_gen = db.
-00005d30: 6469 7265 6374 6f72 795f 7761 6c6b 5f6f  directory_walk_o
-00005d40: 6e65 2864 6972 6563 746f 7279 2c20 6375  ne(directory, cu
-00005d50: 723d 6375 7229 0a0a 2020 2020 2020 2020  r=cur)..        
-00005d60: 666f 7220 6c69 6e65 2069 6e20 7265 735f  for line in res_
-00005d70: 6765 6e3a 0a20 2020 2020 2020 2020 2020  gen:.           
-00005d80: 2079 6965 6c64 2064 6963 7428 7a69 7028   yield dict(zip(
-00005d90: 6462 2e64 6972 6563 746f 7279 5f6c 735f  db.directory_ls_
-00005da0: 636f 6c73 2c20 6c69 6e65 2929 0a0a 2020  cols, line))..  
-00005db0: 2020 4064 625f 7472 616e 7361 6374 696f    @db_transactio
-00005dc0: 6e28 7374 6174 656d 656e 745f 7469 6d65  n(statement_time
-00005dd0: 6f75 743d 3430 3030 290a 2020 2020 6465  out=4000).    de
-00005de0: 6620 6469 7265 6374 6f72 795f 656e 7472  f directory_entr
-00005df0: 795f 6765 745f 6279 5f70 6174 6828 0a20  y_get_by_path(. 
-00005e00: 2020 2020 2020 2073 656c 662c 2064 6972         self, dir
-00005e10: 6563 746f 7279 3a20 5368 6131 4769 742c  ectory: Sha1Git,
-00005e20: 2070 6174 6873 3a20 4c69 7374 5b62 7974   paths: List[byt
-00005e30: 6573 5d2c 202a 2c20 6462 3a20 4462 2c20  es], *, db: Db, 
-00005e40: 6375 723d 4e6f 6e65 0a20 2020 2029 202d  cur=None.    ) -
-00005e50: 3e20 4f70 7469 6f6e 616c 5b44 6963 745b  > Optional[Dict[
-00005e60: 7374 722c 2041 6e79 5d5d 3a0a 2020 2020  str, Any]]:.    
-00005e70: 2020 2020 7265 7320 3d20 6462 2e64 6972      res = db.dir
-00005e80: 6563 746f 7279 5f65 6e74 7279 5f67 6574  ectory_entry_get
-00005e90: 5f62 795f 7061 7468 2864 6972 6563 746f  _by_path(directo
-00005ea0: 7279 2c20 7061 7468 732c 2063 7572 290a  ry, paths, cur).
-00005eb0: 2020 2020 2020 2020 7265 7475 726e 2064          return d
-00005ec0: 6963 7428 7a69 7028 6462 2e64 6972 6563  ict(zip(db.direc
-00005ed0: 746f 7279 5f6c 735f 636f 6c73 2c20 7265  tory_ls_cols, re
-00005ee0: 7329 2920 6966 2072 6573 2065 6c73 6520  s)) if res else 
-00005ef0: 4e6f 6e65 0a0a 2020 2020 4064 625f 7472  None..    @db_tr
-00005f00: 616e 7361 6374 696f 6e28 290a 2020 2020  ansaction().    
-00005f10: 6465 6620 6469 7265 6374 6f72 795f 6765  def directory_ge
-00005f20: 745f 7261 6e64 6f6d 2873 656c 662c 202a  t_random(self, *
-00005f30: 2c20 6462 3a20 4462 2c20 6375 723d 4e6f  , db: Db, cur=No
-00005f40: 6e65 2920 2d3e 2053 6861 3147 6974 3a0a  ne) -> Sha1Git:.
-00005f50: 2020 2020 2020 2020 7265 7475 726e 2064          return d
-00005f60: 622e 6469 7265 6374 6f72 795f 6765 745f  b.directory_get_
-00005f70: 7261 6e64 6f6d 2863 7572 290a 0a20 2020  random(cur)..   
-00005f80: 2040 6462 5f74 7261 6e73 6163 7469 6f6e   @db_transaction
-00005f90: 2829 0a20 2020 2064 6566 2064 6972 6563  ().    def direc
-00005fa0: 746f 7279 5f67 6574 5f65 6e74 7269 6573  tory_get_entries
-00005fb0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-00005fc0: 2020 2020 2020 2020 6469 7265 6374 6f72          director
-00005fd0: 795f 6964 3a20 5368 6131 4769 742c 0a20  y_id: Sha1Git,. 
-00005fe0: 2020 2020 2020 2070 6167 655f 746f 6b65         page_toke
-00005ff0: 6e3a 204f 7074 696f 6e61 6c5b 6279 7465  n: Optional[byte
-00006000: 735d 203d 204e 6f6e 652c 0a20 2020 2020  s] = None,.     
-00006010: 2020 206c 696d 6974 3a20 696e 7420 3d20     limit: int = 
-00006020: 3130 3030 2c0a 2020 2020 2020 2020 2a2c  1000,.        *,
-00006030: 0a20 2020 2020 2020 2064 623a 2044 622c  .        db: Db,
-00006040: 0a20 2020 2020 2020 2063 7572 3d4e 6f6e  .        cur=Non
-00006050: 652c 0a20 2020 2029 202d 3e20 4f70 7469  e,.    ) -> Opti
-00006060: 6f6e 616c 5b50 6167 6564 5265 7375 6c74  onal[PagedResult
-00006070: 5b44 6972 6563 746f 7279 456e 7472 795d  [DirectoryEntry]
-00006080: 5d3a 0a20 2020 2020 2020 2069 6620 6c69  ]:.        if li
-00006090: 7374 2873 656c 662e 6469 7265 6374 6f72  st(self.director
-000060a0: 795f 6d69 7373 696e 6728 5b64 6972 6563  y_missing([direc
-000060b0: 746f 7279 5f69 645d 2c20 6462 3d64 622c  tory_id], db=db,
-000060c0: 2063 7572 3d63 7572 2929 3a0a 2020 2020   cur=cur)):.    
-000060d0: 2020 2020 2020 2020 7265 7475 726e 204e          return N
-000060e0: 6f6e 650a 0a20 2020 2020 2020 2069 6620  one..        if 
-000060f0: 7061 6765 5f74 6f6b 656e 2069 7320 6e6f  page_token is no
-00006100: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00006110: 2020 2020 7261 6973 6520 5374 6f72 6167      raise Storag
-00006120: 6541 7267 756d 656e 7445 7863 6570 7469  eArgumentExcepti
-00006130: 6f6e 2822 556e 7375 7070 6f72 7465 6420  on("Unsupported 
-00006140: 7061 6765 2074 6f6b 656e 2229 0a0a 2020  page token")..  
-00006150: 2020 2020 2020 2320 544f 444f 3a20 6163        # TODO: ac
-00006160: 7475 616c 6c79 2070 6167 696e 6174 650a  tually paginate.
-00006170: 2020 2020 2020 2020 726f 7773 203d 2064          rows = d
-00006180: 622e 6469 7265 6374 6f72 795f 6765 745f  b.directory_get_
-00006190: 656e 7472 6965 7328 6469 7265 6374 6f72  entries(director
-000061a0: 795f 6964 2c20 6375 723d 6375 7229 0a20  y_id, cur=cur). 
-000061b0: 2020 2020 2020 2072 6574 7572 6e20 5061         return Pa
-000061c0: 6765 6452 6573 756c 7428 0a20 2020 2020  gedResult(.     
-000061d0: 2020 2020 2020 2072 6573 756c 7473 3d5b         results=[
-000061e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000061f0: 2044 6972 6563 746f 7279 456e 7472 7928   DirectoryEntry(
-00006200: 2a2a 6469 6374 287a 6970 2864 622e 6469  **dict(zip(db.di
-00006210: 7265 6374 6f72 795f 6765 745f 656e 7472  rectory_get_entr
-00006220: 6965 735f 636f 6c73 2c20 726f 7729 2929  ies_cols, row)))
-00006230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006240: 2066 6f72 2072 6f77 2069 6e20 726f 7773   for row in rows
-00006250: 0a20 2020 2020 2020 2020 2020 205d 2c0a  .            ],.
-00006260: 2020 2020 2020 2020 2020 2020 6e65 7874              next
-00006270: 5f70 6167 655f 746f 6b65 6e3d 4e6f 6e65  _page_token=None
-00006280: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-00006290: 2040 6462 5f74 7261 6e73 6163 7469 6f6e   @db_transaction
-000062a0: 2829 0a20 2020 2064 6566 2064 6972 6563  ().    def direc
-000062b0: 746f 7279 5f67 6574 5f72 6177 5f6d 616e  tory_get_raw_man
-000062c0: 6966 6573 7428 0a20 2020 2020 2020 2073  ifest(.        s
-000062d0: 656c 662c 2064 6972 6563 746f 7279 5f69  elf, directory_i
-000062e0: 6473 3a20 4c69 7374 5b53 6861 3147 6974  ds: List[Sha1Git
-000062f0: 5d2c 202a 2c20 6462 3a20 4462 2c20 6375  ], *, db: Db, cu
-00006300: 723d 4e6f 6e65 0a20 2020 2029 202d 3e20  r=None.    ) -> 
-00006310: 4469 6374 5b53 6861 3147 6974 2c20 4f70  Dict[Sha1Git, Op
-00006320: 7469 6f6e 616c 5b62 7974 6573 5d5d 3a0a  tional[bytes]]:.
-00006330: 2020 2020 2020 2020 7265 7475 726e 2064          return d
-00006340: 6963 7428 6462 2e64 6972 6563 746f 7279  ict(db.directory
-00006350: 5f67 6574 5f72 6177 5f6d 616e 6966 6573  _get_raw_manifes
-00006360: 7428 6469 7265 6374 6f72 795f 6964 732c  t(directory_ids,
-00006370: 2063 7572 3d63 7572 2929 0a0a 2020 2020   cur=cur))..    
-00006380: 4064 625f 7472 616e 7361 6374 696f 6e28  @db_transaction(
-00006390: 290a 2020 2020 6465 6620 6469 7265 6374  ).    def direct
-000063a0: 6f72 795f 6765 745f 6964 5f70 6172 7469  ory_get_id_parti
-000063b0: 7469 6f6e 280a 2020 2020 2020 2020 7365  tion(.        se
-000063c0: 6c66 2c0a 2020 2020 2020 2020 7061 7274  lf,.        part
-000063d0: 6974 696f 6e5f 6964 3a20 696e 742c 0a20  ition_id: int,. 
-000063e0: 2020 2020 2020 206e 625f 7061 7274 6974         nb_partit
-000063f0: 696f 6e73 3a20 696e 742c 0a20 2020 2020  ions: int,.     
-00006400: 2020 2070 6167 655f 746f 6b65 6e3a 204f     page_token: O
-00006410: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-00006420: 6f6e 652c 0a20 2020 2020 2020 206c 696d  one,.        lim
-00006430: 6974 3a20 696e 7420 3d20 3130 3030 2c0a  it: int = 1000,.
-00006440: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
-00006450: 2020 2064 623a 2044 622c 0a20 2020 2020     db: Db,.     
-00006460: 2020 2063 7572 3d4e 6f6e 652c 0a20 2020     cur=None,.   
-00006470: 2029 202d 3e20 5061 6765 6452 6573 756c   ) -> PagedResul
-00006480: 745b 5368 6131 4769 745d 3a0a 2020 2020  t[Sha1Git]:.    
-00006490: 2020 2020 7265 7475 726e 205f 6765 745f      return _get_
-000064a0: 7061 6769 6e61 7465 645f 7368 6131 5f70  paginated_sha1_p
-000064b0: 6172 7469 7469 6f6e 280a 2020 2020 2020  artition(.      
-000064c0: 2020 2020 2020 6375 722c 0a20 2020 2020        cur,.     
-000064d0: 2020 2020 2020 2070 6172 7469 7469 6f6e         partition
-000064e0: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
-000064f0: 206e 625f 7061 7274 6974 696f 6e73 2c0a   nb_partitions,.
-00006500: 2020 2020 2020 2020 2020 2020 7061 6765              page
-00006510: 5f74 6f6b 656e 2c0a 2020 2020 2020 2020  _token,.        
-00006520: 2020 2020 6c69 6d69 742c 0a20 2020 2020      limit,.     
-00006530: 2020 2020 2020 2064 622e 6469 7265 6374         db.direct
-00006540: 6f72 795f 6765 745f 6964 5f72 616e 6765  ory_get_id_range
-00006550: 2c0a 2020 2020 2020 2020 2020 2020 6f70  ,.            op
-00006560: 6572 6174 6f72 2e69 7465 6d67 6574 7465  erator.itemgette
-00006570: 7228 3029 2c0a 2020 2020 2020 2020 2020  r(0),.          
-00006580: 2020 6c61 6d62 6461 2069 645f 3a20 6964    lambda id_: id
-00006590: 5f2c 0a20 2020 2020 2020 2029 0a0a 2020  _,.        )..  
-000065a0: 2020 2323 2323 2323 2323 2323 2323 2323    ##############
-000065b0: 2323 2323 2323 2323 2323 2323 0a20 2020  ############.   
-000065c0: 2023 2052 6576 6973 696f 6e0a 2020 2020   # Revision.    
-000065d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000065e0: 2323 2323 2323 2323 2323 0a0a 2020 2020  ##########..    
-000065f0: 4064 625f 7472 616e 7361 6374 696f 6e28  @db_transaction(
-00006600: 290a 2020 2020 6465 6620 7265 7669 7369  ).    def revisi
-00006610: 6f6e 5f61 6464 280a 2020 2020 2020 2020  on_add(.        
-00006620: 7365 6c66 2c20 7265 7669 7369 6f6e 733a  self, revisions:
-00006630: 204c 6973 745b 5265 7669 7369 6f6e 5d2c   List[Revision],
-00006640: 202a 2c20 6462 3a20 4462 2c20 6375 723d   *, db: Db, cur=
-00006650: 4e6f 6e65 0a20 2020 2029 202d 3e20 4469  None.    ) -> Di
-00006660: 6374 5b73 7472 2c20 696e 745d 3a0a 2020  ct[str, int]:.  
-00006670: 2020 2020 2020 7375 6d6d 6172 7920 3d20        summary = 
-00006680: 7b22 7265 7669 7369 6f6e 3a61 6464 223a  {"revision:add":
-00006690: 2030 7d0a 0a20 2020 2020 2020 2072 6576   0}..        rev
-000066a0: 6973 696f 6e73 5f6d 6973 7369 6e67 203d  isions_missing =
-000066b0: 2073 6574 280a 2020 2020 2020 2020 2020   set(.          
-000066c0: 2020 7365 6c66 2e72 6576 6973 696f 6e5f    self.revision_
-000066d0: 6d69 7373 696e 6728 0a20 2020 2020 2020  missing(.       
-000066e0: 2020 2020 2020 2020 2073 6574 2872 6576           set(rev
-000066f0: 6973 696f 6e2e 6964 2066 6f72 2072 6576  ision.id for rev
-00006700: 6973 696f 6e20 696e 2072 6576 6973 696f  ision in revisio
-00006710: 6e73 292c 2064 623d 6462 2c20 6375 723d  ns), db=db, cur=
-00006720: 6375 720a 2020 2020 2020 2020 2020 2020  cur.            
-00006730: 290a 2020 2020 2020 2020 290a 0a20 2020  ).        )..   
-00006740: 2020 2020 2069 6620 6e6f 7420 7265 7669       if not revi
-00006750: 7369 6f6e 735f 6d69 7373 696e 673a 0a20  sions_missing:. 
-00006760: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00006770: 6e20 7375 6d6d 6172 790a 0a20 2020 2020  n summary..     
-00006780: 2020 2064 622e 6d6b 7465 6d70 5f72 6576     db.mktemp_rev
-00006790: 6973 696f 6e28 6375 7229 0a0a 2020 2020  ision(cur)..    
-000067a0: 2020 2020 7265 7669 7369 6f6e 735f 6669      revisions_fi
-000067b0: 6c74 6572 6564 203d 205b 0a20 2020 2020  ltered = [.     
-000067c0: 2020 2020 2020 2072 6576 6973 696f 6e20         revision 
-000067d0: 666f 7220 7265 7669 7369 6f6e 2069 6e20  for revision in 
-000067e0: 7265 7669 7369 6f6e 7320 6966 2072 6576  revisions if rev
-000067f0: 6973 696f 6e2e 6964 2069 6e20 7265 7669  ision.id in revi
-00006800: 7369 6f6e 735f 6d69 7373 696e 670a 2020  sions_missing.  
-00006810: 2020 2020 2020 5d0a 0a20 2020 2020 2020        ]..       
-00006820: 2073 656c 662e 6a6f 7572 6e61 6c5f 7772   self.journal_wr
-00006830: 6974 6572 2e72 6576 6973 696f 6e5f 6164  iter.revision_ad
-00006840: 6428 7265 7669 7369 6f6e 735f 6669 6c74  d(revisions_filt
-00006850: 6572 6564 290a 0a20 2020 2020 2020 2064  ered)..        d
-00006860: 625f 7265 7669 7369 6f6e 735f 6669 6c74  b_revisions_filt
-00006870: 6572 6564 203d 206c 6973 7428 6d61 7028  ered = list(map(
-00006880: 636f 6e76 6572 7465 7273 2e72 6576 6973  converters.revis
-00006890: 696f 6e5f 746f 5f64 622c 2072 6576 6973  ion_to_db, revis
-000068a0: 696f 6e73 5f66 696c 7465 7265 6429 290a  ions_filtered)).
-000068b0: 0a20 2020 2020 2020 2070 6172 656e 7473  .        parents
-000068c0: 5f66 696c 7465 7265 643a 204c 6973 745b  _filtered: List[
-000068d0: 4469 6374 5b73 7472 2c20 416e 795d 5d20  Dict[str, Any]] 
-000068e0: 3d20 5b5d 0a0a 2020 2020 2020 2020 7769  = []..        wi
-000068f0: 7468 2063 6f6e 7665 7274 5f76 616c 6964  th convert_valid
-00006900: 6174 696f 6e5f 6578 6365 7074 696f 6e73  ation_exceptions
-00006910: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00006920: 6462 2e63 6f70 795f 746f 280a 2020 2020  db.copy_to(.    
-00006930: 2020 2020 2020 2020 2020 2020 6462 5f72              db_r
-00006940: 6576 6973 696f 6e73 5f66 696c 7465 7265  evisions_filtere
-00006950: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-00006960: 2020 2022 746d 705f 7265 7669 7369 6f6e     "tmp_revision
-00006970: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00006980: 2020 2064 622e 7265 7669 7369 6f6e 5f61     db.revision_a
-00006990: 6464 5f63 6f6c 732c 0a20 2020 2020 2020  dd_cols,.       
-000069a0: 2020 2020 2020 2020 2063 7572 2c0a 2020           cur,.  
-000069b0: 2020 2020 2020 2020 2020 2020 2020 6c61                la
-000069c0: 6d62 6461 2072 6576 3a20 7061 7265 6e74  mbda rev: parent
-000069d0: 735f 6669 6c74 6572 6564 2e65 7874 656e  s_filtered.exten
-000069e0: 6428 7265 765b 2270 6172 656e 7473 225d  d(rev["parents"]
-000069f0: 292c 0a20 2020 2020 2020 2020 2020 2029  ),.            )
-00006a00: 0a0a 2020 2020 2020 2020 2020 2020 6462  ..            db
-00006a10: 2e72 6576 6973 696f 6e5f 6164 645f 6672  .revision_add_fr
-00006a20: 6f6d 5f74 656d 7028 6375 7229 0a0a 2020  om_temp(cur)..  
-00006a30: 2020 2020 2020 2020 2020 6462 2e63 6f70            db.cop
-00006a40: 795f 746f 280a 2020 2020 2020 2020 2020  y_to(.          
-00006a50: 2020 2020 2020 7061 7265 6e74 735f 6669        parents_fi
-00006a60: 6c74 6572 6564 2c0a 2020 2020 2020 2020  ltered,.        
-00006a70: 2020 2020 2020 2020 2272 6576 6973 696f          "revisio
-00006a80: 6e5f 6869 7374 6f72 7922 2c0a 2020 2020  n_history",.    
-00006a90: 2020 2020 2020 2020 2020 2020 5b22 6964              ["id
-00006aa0: 222c 2022 7061 7265 6e74 5f69 6422 2c20  ", "parent_id", 
-00006ab0: 2270 6172 656e 745f 7261 6e6b 225d 2c0a  "parent_rank"],.
-00006ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ad0: 6375 722c 0a20 2020 2020 2020 2020 2020  cur,.           
-00006ae0: 2029 0a0a 2020 2020 2020 2020 7265 7475   )..        retu
-00006af0: 726e 207b 2272 6576 6973 696f 6e3a 6164  rn {"revision:ad
-00006b00: 6422 3a20 6c65 6e28 7265 7669 7369 6f6e  d": len(revision
-00006b10: 735f 6d69 7373 696e 6729 7d0a 0a20 2020  s_missing)}..   
-00006b20: 2040 6462 5f74 7261 6e73 6163 7469 6f6e   @db_transaction
-00006b30: 5f67 656e 6572 6174 6f72 2829 0a20 2020  _generator().   
-00006b40: 2064 6566 2072 6576 6973 696f 6e5f 6d69   def revision_mi
-00006b50: 7373 696e 6728 0a20 2020 2020 2020 2073  ssing(.        s
-00006b60: 656c 662c 2072 6576 6973 696f 6e73 3a20  elf, revisions: 
-00006b70: 4c69 7374 5b53 6861 3147 6974 5d2c 202a  List[Sha1Git], *
-00006b80: 2c20 6462 3a20 4462 2c20 6375 723d 4e6f  , db: Db, cur=No
-00006b90: 6e65 0a20 2020 2029 202d 3e20 4974 6572  ne.    ) -> Iter
-00006ba0: 6162 6c65 5b53 6861 3147 6974 5d3a 0a20  able[Sha1Git]:. 
-00006bb0: 2020 2020 2020 2069 6620 6e6f 7420 7265         if not re
-00006bc0: 7669 7369 6f6e 733a 0a20 2020 2020 2020  visions:.       
-00006bd0: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
-00006be0: 0a0a 2020 2020 2020 2020 666f 7220 6f62  ..        for ob
-00006bf0: 6a20 696e 2064 622e 7265 7669 7369 6f6e  j in db.revision
-00006c00: 5f6d 6973 7369 6e67 5f66 726f 6d5f 6c69  _missing_from_li
-00006c10: 7374 2872 6576 6973 696f 6e73 2c20 6375  st(revisions, cu
-00006c20: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-00006c30: 7969 656c 6420 6f62 6a5b 305d 0a0a 2020  yield obj[0]..  
-00006c40: 2020 4064 625f 7472 616e 7361 6374 696f    @db_transactio
-00006c50: 6e28 290a 2020 2020 6465 6620 7265 7669  n().    def revi
-00006c60: 7369 6f6e 5f67 6574 5f70 6172 7469 7469  sion_get_partiti
-00006c70: 6f6e 280a 2020 2020 2020 2020 7365 6c66  on(.        self
-00006c80: 2c0a 2020 2020 2020 2020 7061 7274 6974  ,.        partit
-00006c90: 696f 6e5f 6964 3a20 696e 742c 0a20 2020  ion_id: int,.   
-00006ca0: 2020 2020 206e 625f 7061 7274 6974 696f       nb_partitio
-00006cb0: 6e73 3a20 696e 742c 0a20 2020 2020 2020  ns: int,.       
-00006cc0: 2070 6167 655f 746f 6b65 6e3a 204f 7074   page_token: Opt
-00006cd0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-00006ce0: 652c 0a20 2020 2020 2020 206c 696d 6974  e,.        limit
-00006cf0: 3a20 696e 7420 3d20 3130 3030 2c0a 2020  : int = 1000,.  
-00006d00: 2020 2020 2020 2a2c 0a20 2020 2020 2020        *,.       
-00006d10: 2064 623a 2044 622c 0a20 2020 2020 2020   db: Db,.       
-00006d20: 2063 7572 3d4e 6f6e 652c 0a20 2020 2029   cur=None,.    )
-00006d30: 202d 3e20 5061 6765 6452 6573 756c 745b   -> PagedResult[
-00006d40: 5265 7669 7369 6f6e 5d3a 0a20 2020 2020  Revision]:.     
-00006d50: 2020 2072 6574 7572 6e20 5f67 6574 5f70     return _get_p
-00006d60: 6167 696e 6174 6564 5f73 6861 315f 7061  aginated_sha1_pa
-00006d70: 7274 6974 696f 6e28 0a20 2020 2020 2020  rtition(.       
-00006d80: 2020 2020 2063 7572 2c0a 2020 2020 2020       cur,.      
-00006d90: 2020 2020 2020 7061 7274 6974 696f 6e5f        partition_
-00006da0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
-00006db0: 6e62 5f70 6172 7469 7469 6f6e 732c 0a20  nb_partitions,. 
-00006dc0: 2020 2020 2020 2020 2020 2070 6167 655f             page_
-00006dd0: 746f 6b65 6e2c 0a20 2020 2020 2020 2020  token,.         
-00006de0: 2020 206c 696d 6974 2c0a 2020 2020 2020     limit,.      
-00006df0: 2020 2020 2020 6462 2e72 6576 6973 696f        db.revisio
-00006e00: 6e5f 6765 745f 7261 6e67 652c 0a20 2020  n_get_range,.   
-00006e10: 2020 2020 2020 2020 206c 616d 6264 6120           lambda 
-00006e20: 726f 773a 2063 6f6e 7665 7274 6572 732e  row: converters.
-00006e30: 6462 5f74 6f5f 7265 7669 7369 6f6e 2864  db_to_revision(d
-00006e40: 6963 7428 7a69 7028 6462 2e72 6576 6973  ict(zip(db.revis
-00006e50: 696f 6e5f 6765 745f 636f 6c73 2c20 726f  ion_get_cols, ro
-00006e60: 7729 2929 2c0a 2020 2020 2020 2020 290a  w))),.        ).
-00006e70: 0a20 2020 2040 6462 5f74 7261 6e73 6163  .    @db_transac
-00006e80: 7469 6f6e 2873 7461 7465 6d65 6e74 5f74  tion(statement_t
-00006e90: 696d 656f 7574 3d32 3030 3029 0a20 2020  imeout=2000).   
-00006ea0: 2064 6566 2072 6576 6973 696f 6e5f 6765   def revision_ge
-00006eb0: 7428 0a20 2020 2020 2020 2073 656c 662c  t(.        self,
-00006ec0: 0a20 2020 2020 2020 2072 6576 6973 696f  .        revisio
-00006ed0: 6e5f 6964 733a 204c 6973 745b 5368 6131  n_ids: List[Sha1
-00006ee0: 4769 745d 2c0a 2020 2020 2020 2020 6967  Git],.        ig
-00006ef0: 6e6f 7265 5f64 6973 706c 6179 6e61 6d65  nore_displayname
-00006f00: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
-00006f10: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
-00006f20: 2020 2064 623a 2044 622c 0a20 2020 2020     db: Db,.     
-00006f30: 2020 2063 7572 3d4e 6f6e 652c 0a20 2020     cur=None,.   
-00006f40: 2029 202d 3e20 4c69 7374 5b4f 7074 696f   ) -> List[Optio
-00006f50: 6e61 6c5b 5265 7669 7369 6f6e 5d5d 3a0a  nal[Revision]]:.
-00006f60: 2020 2020 2020 2020 7265 7669 7369 6f6e          revision
-00006f70: 7320 3d20 5b5d 0a20 2020 2020 2020 2066  s = [].        f
-00006f80: 6f72 206c 696e 6520 696e 2064 622e 7265  or line in db.re
-00006f90: 7669 7369 6f6e 5f67 6574 5f66 726f 6d5f  vision_get_from_
-00006fa0: 6c69 7374 2872 6576 6973 696f 6e5f 6964  list(revision_id
-00006fb0: 732c 2069 676e 6f72 655f 6469 7370 6c61  s, ignore_displa
-00006fc0: 796e 616d 652c 2063 7572 293a 0a20 2020  yname, cur):.   
-00006fd0: 2020 2020 2020 2020 2072 6576 6973 696f           revisio
-00006fe0: 6e20 3d20 636f 6e76 6572 7465 7273 2e64  n = converters.d
-00006ff0: 625f 746f 5f6f 7074 696f 6e61 6c5f 7265  b_to_optional_re
-00007000: 7669 7369 6f6e 280a 2020 2020 2020 2020  vision(.        
-00007010: 2020 2020 2020 2020 6469 6374 287a 6970          dict(zip
-00007020: 2864 622e 7265 7669 7369 6f6e 5f67 6574  (db.revision_get
-00007030: 5f63 6f6c 732c 206c 696e 6529 290a 2020  _cols, line)).  
-00007040: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00007050: 2020 2020 2020 2020 7265 7669 7369 6f6e          revision
-00007060: 732e 6170 7065 6e64 2872 6576 6973 696f  s.append(revisio
-00007070: 6e29 0a0a 2020 2020 2020 2020 7265 7475  n)..        retu
-00007080: 726e 2072 6576 6973 696f 6e73 0a0a 2020  rn revisions..  
-00007090: 2020 4064 625f 7472 616e 7361 6374 696f    @db_transactio
-000070a0: 6e5f 6765 6e65 7261 746f 7228 7374 6174  n_generator(stat
-000070b0: 656d 656e 745f 7469 6d65 6f75 743d 3230  ement_timeout=20
-000070c0: 3030 290a 2020 2020 6465 6620 7265 7669  00).    def revi
-000070d0: 7369 6f6e 5f6c 6f67 280a 2020 2020 2020  sion_log(.      
-000070e0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-000070f0: 7265 7669 7369 6f6e 733a 204c 6973 745b  revisions: List[
-00007100: 5368 6131 4769 745d 2c0a 2020 2020 2020  Sha1Git],.      
-00007110: 2020 6967 6e6f 7265 5f64 6973 706c 6179    ignore_display
-00007120: 6e61 6d65 3a20 626f 6f6c 203d 2046 616c  name: bool = Fal
-00007130: 7365 2c0a 2020 2020 2020 2020 6c69 6d69  se,.        limi
-00007140: 743a 204f 7074 696f 6e61 6c5b 696e 745d  t: Optional[int]
-00007150: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00007160: 202a 2c0a 2020 2020 2020 2020 6462 3a20   *,.        db: 
-00007170: 4462 2c0a 2020 2020 2020 2020 6375 723d  Db,.        cur=
-00007180: 4e6f 6e65 2c0a 2020 2020 2920 2d3e 2049  None,.    ) -> I
-00007190: 7465 7261 626c 655b 4f70 7469 6f6e 616c  terable[Optional
-000071a0: 5b44 6963 745b 7374 722c 2041 6e79 5d5d  [Dict[str, Any]]
-000071b0: 5d3a 0a20 2020 2020 2020 2066 6f72 206c  ]:.        for l
-000071c0: 696e 6520 696e 2064 622e 7265 7669 7369  ine in db.revisi
-000071d0: 6f6e 5f6c 6f67 280a 2020 2020 2020 2020  on_log(.        
-000071e0: 2020 2020 7265 7669 7369 6f6e 732c 2069      revisions, i
-000071f0: 676e 6f72 655f 6469 7370 6c61 796e 616d  gnore_displaynam
-00007200: 653d 6967 6e6f 7265 5f64 6973 706c 6179  e=ignore_display
-00007210: 6e61 6d65 2c20 6c69 6d69 743d 6c69 6d69  name, limit=limi
-00007220: 742c 2063 7572 3d63 7572 0a20 2020 2020  t, cur=cur.     
-00007230: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
-00007240: 2020 6461 7461 203d 2063 6f6e 7665 7274    data = convert
-00007250: 6572 732e 6462 5f74 6f5f 7265 7669 7369  ers.db_to_revisi
-00007260: 6f6e 2864 6963 7428 7a69 7028 6462 2e72  on(dict(zip(db.r
-00007270: 6576 6973 696f 6e5f 6765 745f 636f 6c73  evision_get_cols
-00007280: 2c20 6c69 6e65 2929 290a 2020 2020 2020  , line))).      
-00007290: 2020 2020 2020 6966 206e 6f74 2064 6174        if not dat
-000072a0: 613a 0a20 2020 2020 2020 2020 2020 2020  a:.             
-000072b0: 2020 2079 6965 6c64 204e 6f6e 650a 2020     yield None.  
-000072c0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-000072d0: 6e74 696e 7565 0a20 2020 2020 2020 2020  ntinue.         
-000072e0: 2020 2079 6965 6c64 2064 6174 612e 746f     yield data.to
-000072f0: 5f64 6963 7428 290a 0a20 2020 2040 6462  _dict()..    @db
-00007300: 5f74 7261 6e73 6163 7469 6f6e 5f67 656e  _transaction_gen
-00007310: 6572 6174 6f72 2873 7461 7465 6d65 6e74  erator(statement
-00007320: 5f74 696d 656f 7574 3d32 3030 3029 0a20  _timeout=2000). 
-00007330: 2020 2064 6566 2072 6576 6973 696f 6e5f     def revision_
-00007340: 7368 6f72 746c 6f67 280a 2020 2020 2020  shortlog(.      
-00007350: 2020 7365 6c66 2c20 7265 7669 7369 6f6e    self, revision
-00007360: 733a 204c 6973 745b 5368 6131 4769 745d  s: List[Sha1Git]
-00007370: 2c20 6c69 6d69 743a 204f 7074 696f 6e61  , limit: Optiona
-00007380: 6c5b 696e 745d 203d 204e 6f6e 652c 202a  l[int] = None, *
-00007390: 2c20 6462 3a20 4462 2c20 6375 723d 4e6f  , db: Db, cur=No
-000073a0: 6e65 0a20 2020 2029 202d 3e20 4974 6572  ne.    ) -> Iter
-000073b0: 6162 6c65 5b4f 7074 696f 6e61 6c5b 5475  able[Optional[Tu
-000073c0: 706c 655b 5368 6131 4769 742c 2054 7570  ple[Sha1Git, Tup
-000073d0: 6c65 5b53 6861 3147 6974 2c20 2e2e 2e5d  le[Sha1Git, ...]
-000073e0: 5d5d 5d3a 0a20 2020 2020 2020 2079 6965  ]]]:.        yie
-000073f0: 6c64 2066 726f 6d20 6462 2e72 6576 6973  ld from db.revis
-00007400: 696f 6e5f 7368 6f72 746c 6f67 2872 6576  ion_shortlog(rev
-00007410: 6973 696f 6e73 2c20 6c69 6d69 742c 2063  isions, limit, c
-00007420: 7572 290a 0a20 2020 2040 6462 5f74 7261  ur)..    @db_tra
-00007430: 6e73 6163 7469 6f6e 2829 0a20 2020 2064  nsaction().    d
-00007440: 6566 2072 6576 6973 696f 6e5f 6765 745f  ef revision_get_
-00007450: 7261 6e64 6f6d 2873 656c 662c 202a 2c20  random(self, *, 
-00007460: 6462 3a20 4462 2c20 6375 723d 4e6f 6e65  db: Db, cur=None
-00007470: 2920 2d3e 2053 6861 3147 6974 3a0a 2020  ) -> Sha1Git:.  
-00007480: 2020 2020 2020 7265 7475 726e 2064 622e        return db.
-00007490: 7265 7669 7369 6f6e 5f67 6574 5f72 616e  revision_get_ran
-000074a0: 646f 6d28 6375 7229 0a0a 2020 2020 2323  dom(cur)..    ##
-000074b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000074c0: 2323 2323 2323 2323 0a20 2020 2023 2045  ########.    # E
-000074d0: 7874 4944 0a20 2020 2023 2323 2323 2323  xtID.    #######
-000074e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000074f0: 2323 230a 0a20 2020 2040 6462 5f74 7261  ###..    @db_tra
-00007500: 6e73 6163 7469 6f6e 2829 0a20 2020 2064  nsaction().    d
-00007510: 6566 2065 7874 6964 5f67 6574 5f66 726f  ef extid_get_fro
-00007520: 6d5f 6578 7469 6428 0a20 2020 2020 2020  m_extid(.       
-00007530: 2073 656c 662c 0a20 2020 2020 2020 2069   self,.        i
-00007540: 645f 7479 7065 3a20 7374 722c 0a20 2020  d_type: str,.   
-00007550: 2020 2020 2069 6473 3a20 4c69 7374 5b62       ids: List[b
-00007560: 7974 6573 5d2c 0a20 2020 2020 2020 2076  ytes],.        v
-00007570: 6572 7369 6f6e 3a20 4f70 7469 6f6e 616c  ersion: Optional
-00007580: 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a 2020  [int] = None,.  
-00007590: 2020 2020 2020 2a2c 0a20 2020 2020 2020        *,.       
-000075a0: 2064 623a 2044 622c 0a20 2020 2020 2020   db: Db,.       
-000075b0: 2063 7572 3d4e 6f6e 652c 0a20 2020 2029   cur=None,.    )
-000075c0: 202d 3e20 4c69 7374 5b45 7874 4944 5d3a   -> List[ExtID]:
-000075d0: 0a20 2020 2020 2020 2065 7874 6964 7320  .        extids 
-000075e0: 3d20 5b5d 0a20 2020 2020 2020 2066 6f72  = [].        for
-000075f0: 2072 6f77 2069 6e20 6462 2e65 7874 6964   row in db.extid
-00007600: 5f67 6574 5f66 726f 6d5f 6578 7469 645f  _get_from_extid_
-00007610: 6c69 7374 2869 645f 7479 7065 2c20 6964  list(id_type, id
-00007620: 732c 2076 6572 7369 6f6e 3d76 6572 7369  s, version=versi
-00007630: 6f6e 2c20 6375 723d 6375 7229 3a0a 2020  on, cur=cur):.  
-00007640: 2020 2020 2020 2020 2020 6966 2072 6f77            if row
-00007650: 5b30 5d20 6973 206e 6f74 204e 6f6e 653a  [0] is not None:
-00007660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007670: 2065 7874 6964 732e 6170 7065 6e64 2863   extids.append(c
-00007680: 6f6e 7665 7274 6572 732e 6462 5f74 6f5f  onverters.db_to_
-00007690: 6578 7469 6428 6469 6374 287a 6970 2864  extid(dict(zip(d
-000076a0: 622e 6578 7469 645f 636f 6c73 2c20 726f  b.extid_cols, ro
-000076b0: 7729 2929 290a 2020 2020 2020 2020 7265  w)))).        re
-000076c0: 7475 726e 2065 7874 6964 730a 0a20 2020  turn extids..   
-000076d0: 2040 6462 5f74 7261 6e73 6163 7469 6f6e   @db_transaction
-000076e0: 2829 0a20 2020 2064 6566 2065 7874 6964  ().    def extid
-000076f0: 5f67 6574 5f66 726f 6d5f 7461 7267 6574  _get_from_target
-00007700: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-00007710: 2020 2020 2020 2020 7461 7267 6574 5f74          target_t
-00007720: 7970 653a 204f 626a 6563 7454 7970 652c  ype: ObjectType,
-00007730: 0a20 2020 2020 2020 2069 6473 3a20 4c69  .        ids: Li
-00007740: 7374 5b53 6861 3147 6974 5d2c 0a20 2020  st[Sha1Git],.   
-00007750: 2020 2020 2065 7874 6964 5f74 7970 653a       extid_type:
-00007760: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
-00007770: 204e 6f6e 652c 0a20 2020 2020 2020 2065   None,.        e
-00007780: 7874 6964 5f76 6572 7369 6f6e 3a20 4f70  xtid_version: Op
-00007790: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
-000077a0: 6e65 2c0a 2020 2020 2020 2020 2a2c 0a20  ne,.        *,. 
-000077b0: 2020 2020 2020 2064 623a 2044 622c 0a20         db: Db,. 
-000077c0: 2020 2020 2020 2063 7572 3d4e 6f6e 652c         cur=None,
-000077d0: 0a20 2020 2029 202d 3e20 4c69 7374 5b45  .    ) -> List[E
-000077e0: 7874 4944 5d3a 0a20 2020 2020 2020 2065  xtID]:.        e
-000077f0: 7874 6964 7320 3d20 5b5d 0a20 2020 2020  xtids = [].     
-00007800: 2020 2069 6620 2865 7874 6964 5f76 6572     if (extid_ver
-00007810: 7369 6f6e 2069 7320 6e6f 7420 4e6f 6e65  sion is not None
-00007820: 2061 6e64 2065 7874 6964 5f74 7970 6520   and extid_type 
-00007830: 6973 204e 6f6e 6529 206f 7220 280a 2020  is None) or (.  
-00007840: 2020 2020 2020 2020 2020 6578 7469 645f            extid_
-00007850: 7665 7273 696f 6e20 6973 204e 6f6e 6520  version is None 
-00007860: 616e 6420 6578 7469 645f 7479 7065 2069  and extid_type i
-00007870: 7320 6e6f 7420 4e6f 6e65 0a20 2020 2020  s not None.     
-00007880: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
-00007890: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-000078a0: 6f72 2822 596f 7520 6d75 7374 2070 726f  or("You must pro
-000078b0: 7669 6465 2062 6f74 6820 6578 7469 645f  vide both extid_
-000078c0: 7479 7065 2061 6e64 2065 7874 6964 5f76  type and extid_v
-000078d0: 6572 7369 6f6e 2229 0a0a 2020 2020 2020  ersion")..      
-000078e0: 2020 666f 7220 726f 7720 696e 2064 622e    for row in db.
-000078f0: 6578 7469 645f 6765 745f 6672 6f6d 5f73  extid_get_from_s
-00007900: 7768 6964 5f6c 6973 7428 0a20 2020 2020  whid_list(.     
-00007910: 2020 2020 2020 2074 6172 6765 745f 7479         target_ty
-00007920: 7065 2e76 616c 7565 2c0a 2020 2020 2020  pe.value,.      
-00007930: 2020 2020 2020 6964 732c 0a20 2020 2020        ids,.     
-00007940: 2020 2020 2020 2065 7874 6964 5f76 6572         extid_ver
-00007950: 7369 6f6e 3d65 7874 6964 5f76 6572 7369  sion=extid_versi
-00007960: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
-00007970: 6578 7469 645f 7479 7065 3d65 7874 6964  extid_type=extid
-00007980: 5f74 7970 652c 0a20 2020 2020 2020 2020  _type,.         
-00007990: 2020 2063 7572 3d63 7572 2c0a 2020 2020     cur=cur,.    
-000079a0: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
-000079b0: 2020 2069 6620 726f 775b 305d 2069 7320     if row[0] is 
-000079c0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000079d0: 2020 2020 2020 2020 2020 6578 7469 6473            extids
-000079e0: 2e61 7070 656e 6428 636f 6e76 6572 7465  .append(converte
-000079f0: 7273 2e64 625f 746f 5f65 7874 6964 2864  rs.db_to_extid(d
-00007a00: 6963 7428 7a69 7028 6462 2e65 7874 6964  ict(zip(db.extid
-00007a10: 5f63 6f6c 732c 2072 6f77 2929 2929 0a20  _cols, row)))). 
-00007a20: 2020 2020 2020 2072 6574 7572 6e20 6578         return ex
-00007a30: 7469 6473 0a0a 2020 2020 4064 625f 7472  tids..    @db_tr
-00007a40: 616e 7361 6374 696f 6e28 290a 2020 2020  ansaction().    
-00007a50: 6465 6620 6578 7469 645f 6164 6428 7365  def extid_add(se
-00007a60: 6c66 2c20 6964 733a 204c 6973 745b 4578  lf, ids: List[Ex
-00007a70: 7449 445d 2c20 2a2c 2064 623a 2044 622c  tID], *, db: Db,
-00007a80: 2063 7572 3d4e 6f6e 6529 202d 3e20 4469   cur=None) -> Di
-00007a90: 6374 5b73 7472 2c20 696e 745d 3a0a 2020  ct[str, int]:.  
-00007aa0: 2020 2020 2020 6578 7469 6420 3d20 5b0a        extid = [.
-00007ab0: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
-00007ac0: 2020 2020 2020 2020 2020 2020 2020 2265                "e
-00007ad0: 7874 6964 223a 2065 7874 6964 2e65 7874  xtid": extid.ext
-00007ae0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
-00007af0: 2020 2020 2265 7874 6964 5f74 7970 6522      "extid_type"
-00007b00: 3a20 6578 7469 642e 6578 7469 645f 7479  : extid.extid_ty
-00007b10: 7065 2c0a 2020 2020 2020 2020 2020 2020  pe,.            
-00007b20: 2020 2020 2265 7874 6964 5f76 6572 7369      "extid_versi
-00007b30: 6f6e 223a 2067 6574 6174 7472 2865 7874  on": getattr(ext
-00007b40: 6964 2c20 2265 7874 6964 5f76 6572 7369  id, "extid_versi
-00007b50: 6f6e 222c 2030 292c 0a20 2020 2020 2020  on", 0),.       
-00007b60: 2020 2020 2020 2020 2022 7461 7267 6574           "target
-00007b70: 223a 2065 7874 6964 2e74 6172 6765 742e  ": extid.target.
-00007b80: 6f62 6a65 6374 5f69 642c 0a20 2020 2020  object_id,.     
-00007b90: 2020 2020 2020 2020 2020 2022 7461 7267             "targ
-00007ba0: 6574 5f74 7970 6522 3a20 6578 7469 642e  et_type": extid.
-00007bb0: 7461 7267 6574 2e6f 626a 6563 745f 7479  target.object_ty
-00007bc0: 7065 2e6e 616d 652e 6c6f 7765 7228 292c  pe.name.lower(),
-00007bd0: 2020 2320 6172 6768 680a 2020 2020 2020    # arghh.      
-00007be0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00007bf0: 2020 2020 666f 7220 6578 7469 6420 696e      for extid in
-00007c00: 2069 6473 0a20 2020 2020 2020 205d 0a20   ids.        ]. 
-00007c10: 2020 2020 2020 2064 622e 6d6b 7465 6d70         db.mktemp
-00007c20: 2822 6578 7469 6422 2c20 6375 7229 0a0a  ("extid", cur)..
-00007c30: 2020 2020 2020 2020 7365 6c66 2e6a 6f75          self.jou
-00007c40: 726e 616c 5f77 7269 7465 722e 6578 7469  rnal_writer.exti
-00007c50: 645f 6164 6428 6964 7329 0a0a 2020 2020  d_add(ids)..    
-00007c60: 2020 2020 6462 2e63 6f70 795f 746f 2865      db.copy_to(e
-00007c70: 7874 6964 2c20 2274 6d70 5f65 7874 6964  xtid, "tmp_extid
-00007c80: 222c 2064 622e 6578 7469 645f 636f 6c73  ", db.extid_cols
-00007c90: 2c20 6375 7229 0a0a 2020 2020 2020 2020  , cur)..        
-00007ca0: 2320 6d6f 7665 206d 6574 6164 6174 6120  # move metadata 
-00007cb0: 696e 2070 6c61 6365 0a20 2020 2020 2020  in place.       
-00007cc0: 2064 622e 6578 7469 645f 6164 645f 6672   db.extid_add_fr
-00007cd0: 6f6d 5f74 656d 7028 6375 7229 0a0a 2020  om_temp(cur)..  
-00007ce0: 2020 2020 2020 7265 7475 726e 207b 2265        return {"e
-00007cf0: 7874 6964 3a61 6464 223a 206c 656e 2865  xtid:add": len(e
-00007d00: 7874 6964 297d 0a0a 2020 2020 2323 2323  xtid)}..    ####
-00007d10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007d20: 2323 2323 2323 0a20 2020 2023 2052 656c  ######.    # Rel
-00007d30: 6561 7365 0a20 2020 2023 2323 2323 2323  ease.    #######
-00007d40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007d50: 2323 230a 0a20 2020 2040 6462 5f74 7261  ###..    @db_tra
-00007d60: 6e73 6163 7469 6f6e 2829 0a20 2020 2064  nsaction().    d
-00007d70: 6566 2072 656c 6561 7365 5f61 6464 280a  ef release_add(.
-00007d80: 2020 2020 2020 2020 7365 6c66 2c20 7265          self, re
-00007d90: 6c65 6173 6573 3a20 4c69 7374 5b52 656c  leases: List[Rel
-00007da0: 6561 7365 5d2c 202a 2c20 6462 3a20 4462  ease], *, db: Db
-00007db0: 2c20 6375 723d 4e6f 6e65 0a20 2020 2029  , cur=None.    )
-00007dc0: 202d 3e20 4469 6374 5b73 7472 2c20 696e   -> Dict[str, in
-00007dd0: 745d 3a0a 2020 2020 2020 2020 7375 6d6d  t]:.        summ
-00007de0: 6172 7920 3d20 7b22 7265 6c65 6173 653a  ary = {"release:
-00007df0: 6164 6422 3a20 307d 0a0a 2020 2020 2020  add": 0}..      
-00007e00: 2020 7265 6c65 6173 655f 6964 7320 3d20    release_ids = 
-00007e10: 7365 7428 7265 6c65 6173 652e 6964 2066  set(release.id f
-00007e20: 6f72 2072 656c 6561 7365 2069 6e20 7265  or release in re
-00007e30: 6c65 6173 6573 290a 2020 2020 2020 2020  leases).        
-00007e40: 7265 6c65 6173 6573 5f6d 6973 7369 6e67  releases_missing
-00007e50: 203d 2073 6574 2873 656c 662e 7265 6c65   = set(self.rele
-00007e60: 6173 655f 6d69 7373 696e 6728 7265 6c65  ase_missing(rele
-00007e70: 6173 655f 6964 732c 2064 623d 6462 2c20  ase_ids, db=db, 
-00007e80: 6375 723d 6375 7229 290a 0a20 2020 2020  cur=cur))..     
-00007e90: 2020 2069 6620 6e6f 7420 7265 6c65 6173     if not releas
-00007ea0: 6573 5f6d 6973 7369 6e67 3a0a 2020 2020  es_missing:.    
-00007eb0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00007ec0: 756d 6d61 7279 0a0a 2020 2020 2020 2020  ummary..        
-00007ed0: 6462 2e6d 6b74 656d 705f 7265 6c65 6173  db.mktemp_releas
-00007ee0: 6528 6375 7229 0a0a 2020 2020 2020 2020  e(cur)..        
-00007ef0: 7265 6c65 6173 6573 5f66 696c 7465 7265  releases_filtere
-00007f00: 6420 3d20 5b0a 2020 2020 2020 2020 2020  d = [.          
-00007f10: 2020 7265 6c65 6173 6520 666f 7220 7265    release for re
-00007f20: 6c65 6173 6520 696e 2072 656c 6561 7365  lease in release
-00007f30: 7320 6966 2072 656c 6561 7365 2e69 6420  s if release.id 
-00007f40: 696e 2072 656c 6561 7365 735f 6d69 7373  in releases_miss
-00007f50: 696e 670a 2020 2020 2020 2020 5d0a 0a20  ing.        ].. 
-00007f60: 2020 2020 2020 2073 656c 662e 6a6f 7572         self.jour
-00007f70: 6e61 6c5f 7772 6974 6572 2e72 656c 6561  nal_writer.relea
-00007f80: 7365 5f61 6464 2872 656c 6561 7365 735f  se_add(releases_
-00007f90: 6669 6c74 6572 6564 290a 0a20 2020 2020  filtered)..     
-00007fa0: 2020 2064 625f 7265 6c65 6173 6573 5f66     db_releases_f
-00007fb0: 696c 7465 7265 6420 3d20 6c69 7374 286d  iltered = list(m
-00007fc0: 6170 2863 6f6e 7665 7274 6572 732e 7265  ap(converters.re
-00007fd0: 6c65 6173 655f 746f 5f64 622c 2072 656c  lease_to_db, rel
-00007fe0: 6561 7365 735f 6669 6c74 6572 6564 2929  eases_filtered))
-00007ff0: 0a0a 2020 2020 2020 2020 7769 7468 2063  ..        with c
-00008000: 6f6e 7665 7274 5f76 616c 6964 6174 696f  onvert_validatio
-00008010: 6e5f 6578 6365 7074 696f 6e73 2829 3a0a  n_exceptions():.
-00008020: 2020 2020 2020 2020 2020 2020 6462 2e63              db.c
-00008030: 6f70 795f 746f 2864 625f 7265 6c65 6173  opy_to(db_releas
-00008040: 6573 5f66 696c 7465 7265 642c 2022 746d  es_filtered, "tm
-00008050: 705f 7265 6c65 6173 6522 2c20 6462 2e72  p_release", db.r
-00008060: 656c 6561 7365 5f61 6464 5f63 6f6c 732c  elease_add_cols,
-00008070: 2063 7572 290a 0a20 2020 2020 2020 2020   cur)..         
-00008080: 2020 2064 622e 7265 6c65 6173 655f 6164     db.release_ad
-00008090: 645f 6672 6f6d 5f74 656d 7028 6375 7229  d_from_temp(cur)
-000080a0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000080b0: 207b 2272 656c 6561 7365 3a61 6464 223a   {"release:add":
-000080c0: 206c 656e 2872 656c 6561 7365 735f 6d69   len(releases_mi
-000080d0: 7373 696e 6729 7d0a 0a20 2020 2040 6462  ssing)}..    @db
-000080e0: 5f74 7261 6e73 6163 7469 6f6e 5f67 656e  _transaction_gen
-000080f0: 6572 6174 6f72 2829 0a20 2020 2064 6566  erator().    def
-00008100: 2072 656c 6561 7365 5f6d 6973 7369 6e67   release_missing
-00008110: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
-00008120: 7265 6c65 6173 6573 3a20 4c69 7374 5b53  releases: List[S
-00008130: 6861 3147 6974 5d2c 202a 2c20 6462 3a20  ha1Git], *, db: 
-00008140: 4462 2c20 6375 723d 4e6f 6e65 0a20 2020  Db, cur=None.   
-00008150: 2029 202d 3e20 4974 6572 6162 6c65 5b53   ) -> Iterable[S
-00008160: 6861 3147 6974 5d3a 0a20 2020 2020 2020  ha1Git]:.       
-00008170: 2069 6620 6e6f 7420 7265 6c65 6173 6573   if not releases
-00008180: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00008190: 7475 726e 0a0a 2020 2020 2020 2020 666f  turn..        fo
-000081a0: 7220 6f62 6a20 696e 2064 622e 7265 6c65  r obj in db.rele
-000081b0: 6173 655f 6d69 7373 696e 675f 6672 6f6d  ase_missing_from
-000081c0: 5f6c 6973 7428 7265 6c65 6173 6573 2c20  _list(releases, 
-000081d0: 6375 7229 3a0a 2020 2020 2020 2020 2020  cur):.          
-000081e0: 2020 7969 656c 6420 6f62 6a5b 305d 0a0a    yield obj[0]..
-000081f0: 2020 2020 4064 625f 7472 616e 7361 6374      @db_transact
-00008200: 696f 6e28 7374 6174 656d 656e 745f 7469  ion(statement_ti
-00008210: 6d65 6f75 743d 3130 3030 290a 2020 2020  meout=1000).    
-00008220: 6465 6620 7265 6c65 6173 655f 6765 7428  def release_get(
-00008230: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00008240: 2020 2020 2020 2072 656c 6561 7365 733a         releases:
-00008250: 204c 6973 745b 5368 6131 4769 745d 2c0a   List[Sha1Git],.
-00008260: 2020 2020 2020 2020 6967 6e6f 7265 5f64          ignore_d
-00008270: 6973 706c 6179 6e61 6d65 3a20 626f 6f6c  isplayname: bool
-00008280: 203d 2046 616c 7365 2c0a 2020 2020 2020   = False,.      
-00008290: 2020 2a2c 0a20 2020 2020 2020 2064 623a    *,.        db:
-000082a0: 2044 622c 0a20 2020 2020 2020 2063 7572   Db,.        cur
-000082b0: 3d4e 6f6e 652c 0a20 2020 2029 202d 3e20  =None,.    ) -> 
-000082c0: 4c69 7374 5b4f 7074 696f 6e61 6c5b 5265  List[Optional[Re
-000082d0: 6c65 6173 655d 5d3a 0a20 2020 2020 2020  lease]]:.       
-000082e0: 2072 656c 7320 3d20 5b5d 0a20 2020 2020   rels = [].     
-000082f0: 2020 2066 6f72 2072 656c 6561 7365 2069     for release i
-00008300: 6e20 6462 2e72 656c 6561 7365 5f67 6574  n db.release_get
-00008310: 5f66 726f 6d5f 6c69 7374 2872 656c 6561  _from_list(relea
-00008320: 7365 732c 2069 676e 6f72 655f 6469 7370  ses, ignore_disp
-00008330: 6c61 796e 616d 652c 2063 7572 293a 0a20  layname, cur):. 
-00008340: 2020 2020 2020 2020 2020 2072 656c 203d             rel =
-00008350: 2063 6f6e 7665 7274 6572 732e 6462 5f74   converters.db_t
-00008360: 6f5f 6f70 7469 6f6e 616c 5f72 656c 6561  o_optional_relea
-00008370: 7365 280a 2020 2020 2020 2020 2020 2020  se(.            
-00008380: 2020 2020 6469 6374 287a 6970 2864 622e      dict(zip(db.
-00008390: 7265 6c65 6173 655f 6765 745f 636f 6c73  release_get_cols
-000083a0: 2c20 7265 6c65 6173 6529 290a 2020 2020  , release)).    
-000083b0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000083c0: 2020 2020 2020 7265 6c73 2e61 7070 656e        rels.appen
-000083d0: 6428 7265 6c29 0a20 2020 2020 2020 2072  d(rel).        r
-000083e0: 6574 7572 6e20 7265 6c73 0a0a 2020 2020  eturn rels..    
-000083f0: 4064 625f 7472 616e 7361 6374 696f 6e28  @db_transaction(
-00008400: 290a 2020 2020 6465 6620 7265 6c65 6173  ).    def releas
-00008410: 655f 6765 745f 7061 7274 6974 696f 6e28  e_get_partition(
-00008420: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00008430: 2020 2020 2020 2070 6172 7469 7469 6f6e         partition
-00008440: 5f69 643a 2069 6e74 2c0a 2020 2020 2020  _id: int,.      
-00008450: 2020 6e62 5f70 6172 7469 7469 6f6e 733a    nb_partitions:
-00008460: 2069 6e74 2c0a 2020 2020 2020 2020 7061   int,.        pa
-00008470: 6765 5f74 6f6b 656e 3a20 4f70 7469 6f6e  ge_token: Option
-00008480: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
-00008490: 2020 2020 2020 2020 6c69 6d69 743a 2069          limit: i
-000084a0: 6e74 203d 2031 3030 302c 0a20 2020 2020  nt = 1000,.     
-000084b0: 2020 202a 2c0a 2020 2020 2020 2020 6462     *,.        db
-000084c0: 3a20 4462 2c0a 2020 2020 2020 2020 6375  : Db,.        cu
-000084d0: 723d 4e6f 6e65 2c0a 2020 2020 2920 2d3e  r=None,.    ) ->
-000084e0: 2050 6167 6564 5265 7375 6c74 5b52 656c   PagedResult[Rel
-000084f0: 6561 7365 5d3a 0a20 2020 2020 2020 2072  ease]:.        r
-00008500: 6574 7572 6e20 5f67 6574 5f70 6167 696e  eturn _get_pagin
-00008510: 6174 6564 5f73 6861 315f 7061 7274 6974  ated_sha1_partit
-00008520: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
-00008530: 2063 7572 2c0a 2020 2020 2020 2020 2020   cur,.          
-00008540: 2020 7061 7274 6974 696f 6e5f 6964 2c0a    partition_id,.
-00008550: 2020 2020 2020 2020 2020 2020 6e62 5f70              nb_p
-00008560: 6172 7469 7469 6f6e 732c 0a20 2020 2020  artitions,.     
-00008570: 2020 2020 2020 2070 6167 655f 746f 6b65         page_toke
-00008580: 6e2c 0a20 2020 2020 2020 2020 2020 206c  n,.            l
-00008590: 696d 6974 2c0a 2020 2020 2020 2020 2020  imit,.          
-000085a0: 2020 6462 2e72 656c 6561 7365 5f67 6574    db.release_get
-000085b0: 5f72 616e 6765 2c0a 2020 2020 2020 2020  _range,.        
-000085c0: 2020 2020 6c61 6d62 6461 2072 6f77 3a20      lambda row: 
-000085d0: 636f 6e76 6572 7465 7273 2e64 625f 746f  converters.db_to
-000085e0: 5f72 656c 6561 7365 2864 6963 7428 7a69  _release(dict(zi
-000085f0: 7028 6462 2e72 656c 6561 7365 5f67 6574  p(db.release_get
-00008600: 5f63 6f6c 732c 2072 6f77 2929 292c 0a20  _cols, row))),. 
-00008610: 2020 2020 2020 2029 0a0a 2020 2020 4064         )..    @d
-00008620: 625f 7472 616e 7361 6374 696f 6e28 290a  b_transaction().
-00008630: 2020 2020 6465 6620 7265 6c65 6173 655f      def release_
-00008640: 6765 745f 7261 6e64 6f6d 2873 656c 662c  get_random(self,
-00008650: 202a 2c20 6462 3a20 4462 2c20 6375 723d   *, db: Db, cur=
-00008660: 4e6f 6e65 2920 2d3e 2053 6861 3147 6974  None) -> Sha1Git
-00008670: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00008680: 2064 622e 7265 6c65 6173 655f 6765 745f   db.release_get_
-00008690: 7261 6e64 6f6d 2863 7572 290a 0a20 2020  random(cur)..   
-000086a0: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
-000086b0: 2323 2323 2323 2323 2323 230a 2020 2020  ###########.    
-000086c0: 2320 536e 6170 7368 6f74 0a20 2020 2023  # Snapshot.    #
-000086d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000086e0: 2323 2323 2323 2323 230a 0a20 2020 2040  #########..    @
-000086f0: 6462 5f74 7261 6e73 6163 7469 6f6e 2829  db_transaction()
-00008700: 0a20 2020 2064 6566 2073 6e61 7073 686f  .    def snapsho
-00008710: 745f 6164 6428 0a20 2020 2020 2020 2073  t_add(.        s
-00008720: 656c 662c 2073 6e61 7073 686f 7473 3a20  elf, snapshots: 
-00008730: 4c69 7374 5b53 6e61 7073 686f 745d 2c20  List[Snapshot], 
-00008740: 2a2c 2064 623a 2044 622c 2063 7572 3d4e  *, db: Db, cur=N
-00008750: 6f6e 650a 2020 2020 2920 2d3e 2044 6963  one.    ) -> Dic
-00008760: 745b 7374 722c 2069 6e74 5d3a 0a20 2020  t[str, int]:.   
-00008770: 2020 2020 2063 7265 6174 6564 5f74 656d       created_tem
-00008780: 705f 7461 626c 6520 3d20 4661 6c73 650a  p_table = False.
-00008790: 0a20 2020 2020 2020 2063 6f75 6e74 203d  .        count =
-000087a0: 2030 0a20 2020 2020 2020 2066 6f72 2073   0.        for s
-000087b0: 6e61 7073 686f 7420 696e 2073 6e61 7073  napshot in snaps
-000087c0: 686f 7473 3a0a 2020 2020 2020 2020 2020  hots:.          
-000087d0: 2020 6966 206e 6f74 2064 622e 736e 6170    if not db.snap
-000087e0: 7368 6f74 5f65 7869 7374 7328 736e 6170  shot_exists(snap
-000087f0: 7368 6f74 2e69 642c 2063 7572 293a 0a20  shot.id, cur):. 
-00008800: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00008810: 6620 6e6f 7420 6372 6561 7465 645f 7465  f not created_te
-00008820: 6d70 5f74 6162 6c65 3a0a 2020 2020 2020  mp_table:.      
-00008830: 2020 2020 2020 2020 2020 2020 2020 6462                db
-00008840: 2e6d 6b74 656d 705f 736e 6170 7368 6f74  .mktemp_snapshot
-00008850: 5f62 7261 6e63 6828 6375 7229 0a20 2020  _branch(cur).   
-00008860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008870: 2063 7265 6174 6564 5f74 656d 705f 7461   created_temp_ta
-00008880: 626c 6520 3d20 5472 7565 0a0a 2020 2020  ble = True..    
-00008890: 2020 2020 2020 2020 2020 2020 7769 7468              with
-000088a0: 2063 6f6e 7665 7274 5f76 616c 6964 6174   convert_validat
-000088b0: 696f 6e5f 6578 6365 7074 696f 6e73 2829  ion_exceptions()
-000088c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000088d0: 2020 2020 2020 6462 2e63 6f70 795f 746f        db.copy_to
-000088e0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000088f0: 2020 2020 2020 2020 2020 280a 2020 2020            (.    
-00008900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008910: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-00008920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008930: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
-00008940: 3a20 6e61 6d65 2c0a 2020 2020 2020 2020  : name,.        
+00004750: 2323 2323 2323 2323 0a20 2020 2023 2053  ########.    # S
+00004760: 6b69 7070 6564 436f 6e74 656e 740a 2020  kippedContent.  
+00004770: 2020 2323 2323 2323 2323 2323 2323 2323    ##############
+00004780: 2323 2323 2323 2323 2323 2323 0a0a 2020  ############..  
+00004790: 2020 4073 7461 7469 636d 6574 686f 640a    @staticmethod.
+000047a0: 2020 2020 6465 6620 5f73 6b69 7070 6564      def _skipped
+000047b0: 5f63 6f6e 7465 6e74 5f6e 6f72 6d61 6c69  _content_normali
+000047c0: 7a65 2864 293a 0a20 2020 2020 2020 2064  ze(d):.        d
+000047d0: 203d 2064 2e63 6f70 7928 290a 0a20 2020   = d.copy()..   
+000047e0: 2020 2020 2069 6620 642e 6765 7428 2273       if d.get("s
+000047f0: 7461 7475 7322 2920 6973 204e 6f6e 653a  tatus") is None:
+00004800: 0a20 2020 2020 2020 2020 2020 2064 5b22  .            d["
+00004810: 7374 6174 7573 225d 203d 2022 6162 7365  status"] = "abse
+00004820: 6e74 220a 0a20 2020 2020 2020 2069 6620  nt"..        if 
+00004830: 642e 6765 7428 226c 656e 6774 6822 2920  d.get("length") 
+00004840: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00004850: 2020 2020 2064 5b22 6c65 6e67 7468 225d       d["length"]
+00004860: 203d 202d 310a 0a20 2020 2020 2020 2072   = -1..        r
+00004870: 6574 7572 6e20 640a 0a20 2020 2064 6566  eturn d..    def
+00004880: 205f 736b 6970 7065 645f 636f 6e74 656e   _skipped_conten
+00004890: 745f 6164 645f 6d65 7461 6461 7461 2873  t_add_metadata(s
+000048a0: 656c 662c 2064 622c 2063 7572 2c20 636f  elf, db, cur, co
+000048b0: 6e74 656e 743a 204c 6973 745b 536b 6970  ntent: List[Skip
+000048c0: 7065 6443 6f6e 7465 6e74 5d29 3a0a 2020  pedContent]):.  
+000048d0: 2020 2020 2020 6f72 6967 696e 5f69 6473        origin_ids
+000048e0: 203d 2064 622e 6f72 6967 696e 5f69 645f   = db.origin_id_
+000048f0: 6765 745f 6279 5f75 726c 285b 636f 6e74  get_by_url([cont
+00004900: 2e6f 7269 6769 6e20 666f 7220 636f 6e74  .origin for cont
+00004910: 2069 6e20 636f 6e74 656e 745d 2c20 6375   in content], cu
+00004920: 723d 6375 7229 0a20 2020 2020 2020 2063  r=cur).        c
+00004930: 6f6e 7465 6e74 203d 205b 0a20 2020 2020  ontent = [.     
+00004940: 2020 2020 2020 2061 7474 722e 6576 6f6c         attr.evol
+00004950: 7665 2863 2c20 6f72 6967 696e 3d6f 7269  ve(c, origin=ori
+00004960: 6769 6e5f 6964 290a 2020 2020 2020 2020  gin_id).        
+00004970: 2020 2020 666f 7220 2863 2c20 6f72 6967      for (c, orig
+00004980: 696e 5f69 6429 2069 6e20 7a69 7028 636f  in_id) in zip(co
+00004990: 6e74 656e 742c 206f 7269 6769 6e5f 6964  ntent, origin_id
+000049a0: 7329 0a20 2020 2020 2020 205d 0a20 2020  s).        ].   
+000049b0: 2020 2020 2064 622e 6d6b 7465 6d70 2822       db.mktemp("
+000049c0: 736b 6970 7065 645f 636f 6e74 656e 7422  skipped_content"
+000049d0: 2c20 6375 7229 0a20 2020 2020 2020 2064  , cur).        d
+000049e0: 622e 636f 7079 5f74 6f28 0a20 2020 2020  b.copy_to(.     
+000049f0: 2020 2020 2020 205b 632e 746f 5f64 6963         [c.to_dic
+00004a00: 7428 2920 666f 7220 6320 696e 2063 6f6e  t() for c in con
+00004a10: 7465 6e74 5d2c 0a20 2020 2020 2020 2020  tent],.         
+00004a20: 2020 2022 746d 705f 736b 6970 7065 645f     "tmp_skipped_
+00004a30: 636f 6e74 656e 7422 2c0a 2020 2020 2020  content",.      
+00004a40: 2020 2020 2020 6462 2e73 6b69 7070 6564        db.skipped
+00004a50: 5f63 6f6e 7465 6e74 5f6b 6579 732c 0a20  _content_keys,. 
+00004a60: 2020 2020 2020 2020 2020 2063 7572 2c0a             cur,.
+00004a70: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00004a80: 2020 2023 206d 6f76 6520 6d65 7461 6461     # move metada
+00004a90: 7461 2069 6e20 706c 6163 650a 2020 2020  ta in place.    
+00004aa0: 2020 2020 6462 2e73 6b69 7070 6564 5f63      db.skipped_c
+00004ab0: 6f6e 7465 6e74 5f61 6464 5f66 726f 6d5f  ontent_add_from_
+00004ac0: 7465 6d70 2863 7572 290a 0a20 2020 2040  temp(cur)..    @
+00004ad0: 6462 5f74 7261 6e73 6163 7469 6f6e 2829  db_transaction()
+00004ae0: 0a20 2020 2064 6566 2073 6b69 7070 6564  .    def skipped
+00004af0: 5f63 6f6e 7465 6e74 5f61 6464 280a 2020  _content_add(.  
+00004b00: 2020 2020 2020 7365 6c66 2c20 636f 6e74        self, cont
+00004b10: 656e 743a 204c 6973 745b 536b 6970 7065  ent: List[Skippe
+00004b20: 6443 6f6e 7465 6e74 5d2c 202a 2c20 6462  dContent], *, db
+00004b30: 3a20 4462 2c20 6375 723d 4e6f 6e65 0a20  : Db, cur=None. 
+00004b40: 2020 2029 202d 3e20 4469 6374 5b73 7472     ) -> Dict[str
+00004b50: 2c20 696e 745d 3a0a 2020 2020 2020 2020  , int]:.        
+00004b60: 6374 696d 6520 3d20 6e6f 7728 290a 2020  ctime = now().  
+00004b70: 2020 2020 2020 636f 6e74 656e 7420 3d20        content = 
+00004b80: 5b61 7474 722e 6576 6f6c 7665 2863 2c20  [attr.evolve(c, 
+00004b90: 6374 696d 653d 6374 696d 6529 2066 6f72  ctime=ctime) for
+00004ba0: 2063 2069 6e20 636f 6e74 656e 745d 0a0a   c in content]..
+00004bb0: 2020 2020 2020 2020 6d69 7373 696e 675f          missing_
+00004bc0: 636f 6e74 656e 7473 203d 2073 656c 662e  contents = self.
+00004bd0: 736b 6970 7065 645f 636f 6e74 656e 745f  skipped_content_
+00004be0: 6d69 7373 696e 6728 0a20 2020 2020 2020  missing(.       
+00004bf0: 2020 2020 2028 632e 746f 5f64 6963 7428       (c.to_dict(
+00004c00: 2920 666f 7220 6320 696e 2063 6f6e 7465  ) for c in conte
+00004c10: 6e74 292c 0a20 2020 2020 2020 2020 2020  nt),.           
+00004c20: 2064 623d 6462 2c0a 2020 2020 2020 2020   db=db,.        
+00004c30: 2020 2020 6375 723d 6375 722c 0a20 2020      cur=cur,.   
+00004c40: 2020 2020 2029 0a20 2020 2020 2020 2063       ).        c
+00004c50: 6f6e 7465 6e74 203d 205b 0a20 2020 2020  ontent = [.     
+00004c60: 2020 2020 2020 2063 0a20 2020 2020 2020         c.       
+00004c70: 2020 2020 2066 6f72 2063 2069 6e20 636f       for c in co
+00004c80: 6e74 656e 740a 2020 2020 2020 2020 2020  ntent.          
+00004c90: 2020 6966 2061 6e79 280a 2020 2020 2020    if any(.      
+00004ca0: 2020 2020 2020 2020 2020 616c 6c28 0a20            all(. 
+00004cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004cc0: 2020 2063 2e67 6574 5f68 6173 6828 616c     c.get_hash(al
+00004cd0: 676f 2920 3d3d 206d 6973 7369 6e67 5f63  go) == missing_c
+00004ce0: 6f6e 7465 6e74 2e67 6574 2861 6c67 6f29  ontent.get(algo)
+00004cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004d00: 2020 2020 2066 6f72 2061 6c67 6f20 696e       for algo in
+00004d10: 2044 4546 4155 4c54 5f41 4c47 4f52 4954   DEFAULT_ALGORIT
+00004d20: 484d 530a 2020 2020 2020 2020 2020 2020  HMS.            
+00004d30: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00004d40: 2020 2020 2020 666f 7220 6d69 7373 696e        for missin
+00004d50: 675f 636f 6e74 656e 7420 696e 206d 6973  g_content in mis
+00004d60: 7369 6e67 5f63 6f6e 7465 6e74 730a 2020  sing_contents.  
+00004d70: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00004d80: 2020 2020 5d0a 0a20 2020 2020 2020 2073      ]..        s
+00004d90: 656c 662e 6a6f 7572 6e61 6c5f 7772 6974  elf.journal_writ
+00004da0: 6572 2e73 6b69 7070 6564 5f63 6f6e 7465  er.skipped_conte
+00004db0: 6e74 5f61 6464 2863 6f6e 7465 6e74 290a  nt_add(content).
+00004dc0: 2020 2020 2020 2020 7365 6c66 2e5f 736b          self._sk
+00004dd0: 6970 7065 645f 636f 6e74 656e 745f 6164  ipped_content_ad
+00004de0: 645f 6d65 7461 6461 7461 2864 622c 2063  d_metadata(db, c
+00004df0: 7572 2c20 636f 6e74 656e 7429 0a0a 2020  ur, content)..  
+00004e00: 2020 2020 2020 7265 7475 726e 207b 0a20        return {. 
+00004e10: 2020 2020 2020 2020 2020 2022 736b 6970             "skip
+00004e20: 7065 645f 636f 6e74 656e 743a 6164 6422  ped_content:add"
+00004e30: 3a20 6c65 6e28 636f 6e74 656e 7429 2c0a  : len(content),.
+00004e40: 2020 2020 2020 2020 7d0a 0a20 2020 2040          }..    @
+00004e50: 6462 5f74 7261 6e73 6163 7469 6f6e 2829  db_transaction()
+00004e60: 0a20 2020 2064 6566 2073 6b69 7070 6564  .    def skipped
+00004e70: 5f63 6f6e 7465 6e74 5f66 696e 6428 0a20  _content_find(. 
+00004e80: 2020 2020 2020 2073 656c 662c 2063 6f6e         self, con
+00004e90: 7465 6e74 3a20 4861 7368 4469 6374 2c20  tent: HashDict, 
+00004ea0: 2a2c 2064 623a 2044 622c 2063 7572 3d4e  *, db: Db, cur=N
+00004eb0: 6f6e 650a 2020 2020 2920 2d3e 204c 6973  one.    ) -> Lis
+00004ec0: 745b 536b 6970 7065 6443 6f6e 7465 6e74  t[SkippedContent
+00004ed0: 5d3a 0a20 2020 2020 2020 2069 6620 6e6f  ]:.        if no
+00004ee0: 7420 7365 7428 636f 6e74 656e 7429 2e69  t set(content).i
+00004ef0: 6e74 6572 7365 6374 696f 6e28 4445 4641  ntersection(DEFA
+00004f00: 554c 545f 414c 474f 5249 5448 4d53 293a  ULT_ALGORITHMS):
+00004f10: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00004f20: 7365 2053 746f 7261 6765 4172 6775 6d65  se StorageArgume
+00004f30: 6e74 4578 6365 7074 696f 6e28 0a20 2020  ntException(.   
+00004f40: 2020 2020 2020 2020 2020 2020 2022 636f               "co
+00004f50: 6e74 656e 7420 6b65 7973 206d 7573 7420  ntent keys must 
+00004f60: 636f 6e74 6169 6e20 6174 206c 6561 7374  contain at least
+00004f70: 206f 6e65 2022 0a20 2020 2020 2020 2020   one ".         
+00004f80: 2020 2020 2020 2066 226f 663a 207b 272c         f"of: {',
+00004f90: 2027 2e6a 6f69 6e28 736f 7274 6564 2844   '.join(sorted(D
+00004fa0: 4546 4155 4c54 5f41 4c47 4f52 4954 484d  EFAULT_ALGORITHM
+00004fb0: 5329 297d 220a 2020 2020 2020 2020 2020  S))}".          
+00004fc0: 2020 290a 0a20 2020 2020 2020 2072 6f77    )..        row
+00004fd0: 7320 3d20 6462 2e73 6b69 7070 6564 5f63  s = db.skipped_c
+00004fe0: 6f6e 7465 6e74 5f66 696e 6428 0a20 2020  ontent_find(.   
+00004ff0: 2020 2020 2020 2020 2073 6861 313d 636f           sha1=co
+00005000: 6e74 656e 742e 6765 7428 2273 6861 3122  ntent.get("sha1"
+00005010: 292c 0a20 2020 2020 2020 2020 2020 2073  ),.            s
+00005020: 6861 315f 6769 743d 636f 6e74 656e 742e  ha1_git=content.
+00005030: 6765 7428 2273 6861 315f 6769 7422 292c  get("sha1_git"),
+00005040: 0a20 2020 2020 2020 2020 2020 2073 6861  .            sha
+00005050: 3235 363d 636f 6e74 656e 742e 6765 7428  256=content.get(
+00005060: 2273 6861 3235 3622 292c 0a20 2020 2020  "sha256"),.     
+00005070: 2020 2020 2020 2062 6c61 6b65 3273 3235         blake2s25
+00005080: 363d 636f 6e74 656e 742e 6765 7428 2262  6=content.get("b
+00005090: 6c61 6b65 3273 3235 3622 292c 0a20 2020  lake2s256"),.   
+000050a0: 2020 2020 2020 2020 2063 7572 3d63 7572           cur=cur
+000050b0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+000050c0: 2020 2020 736b 6970 7065 645f 636f 6e74      skipped_cont
+000050d0: 656e 7473 203d 205b 5d0a 2020 2020 2020  ents = [].      
+000050e0: 2020 666f 7220 726f 7720 696e 2072 6f77    for row in row
+000050f0: 733a 0a20 2020 2020 2020 2020 2020 2072  s:.            r
+00005100: 6f77 5f64 203d 2064 6963 7428 7a69 7028  ow_d = dict(zip(
+00005110: 6462 2e73 6b69 7070 6564 5f63 6f6e 7465  db.skipped_conte
+00005120: 6e74 5f66 696e 645f 636f 6c73 2c20 726f  nt_find_cols, ro
+00005130: 7729 290a 2020 2020 2020 2020 2020 2020  w)).            
+00005140: 736b 6970 7065 645f 636f 6e74 656e 7473  skipped_contents
+00005150: 2e61 7070 656e 6428 536b 6970 7065 6443  .append(SkippedC
+00005160: 6f6e 7465 6e74 282a 2a72 6f77 5f64 2929  ontent(**row_d))
+00005170: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00005180: 736b 6970 7065 645f 636f 6e74 656e 7473  skipped_contents
+00005190: 0a0a 2020 2020 4064 625f 7472 616e 7361  ..    @db_transa
+000051a0: 6374 696f 6e5f 6765 6e65 7261 746f 7228  ction_generator(
+000051b0: 290a 2020 2020 6465 6620 736b 6970 7065  ).    def skippe
+000051c0: 645f 636f 6e74 656e 745f 6d69 7373 696e  d_content_missin
+000051d0: 6728 0a20 2020 2020 2020 2073 656c 662c  g(.        self,
+000051e0: 2063 6f6e 7465 6e74 733a 204c 6973 745b   contents: List[
+000051f0: 4469 6374 5b73 7472 2c20 416e 795d 5d2c  Dict[str, Any]],
+00005200: 202a 2c20 6462 3a20 4462 2c20 6375 723d   *, db: Db, cur=
+00005210: 4e6f 6e65 0a20 2020 2029 202d 3e20 4974  None.    ) -> It
+00005220: 6572 6162 6c65 5b44 6963 745b 7374 722c  erable[Dict[str,
+00005230: 2041 6e79 5d5d 3a0a 2020 2020 2020 2020   Any]]:.        
+00005240: 636f 6e74 656e 7473 203d 206c 6973 7428  contents = list(
+00005250: 636f 6e74 656e 7473 290a 2020 2020 2020  contents).      
+00005260: 2020 666f 7220 636f 6e74 656e 7420 696e    for content in
+00005270: 2064 622e 736b 6970 7065 645f 636f 6e74   db.skipped_cont
+00005280: 656e 745f 6d69 7373 696e 6728 636f 6e74  ent_missing(cont
+00005290: 656e 7473 2c20 6375 7229 3a0a 2020 2020  ents, cur):.    
+000052a0: 2020 2020 2020 2020 7969 656c 6420 7b0a          yield {.
+000052b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000052c0: 616c 676f 3a20 6861 7368 0a20 2020 2020  algo: hash.     
+000052d0: 2020 2020 2020 2020 2020 2066 6f72 2028             for (
+000052e0: 616c 676f 2c20 6861 7368 2920 696e 207a  algo, hash) in z
+000052f0: 6970 2864 622e 636f 6e74 656e 745f 6861  ip(db.content_ha
+00005300: 7368 5f6b 6579 732c 2063 6f6e 7465 6e74  sh_keys, content
+00005310: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00005320: 2020 6966 2068 6173 680a 2020 2020 2020    if hash.      
+00005330: 2020 2020 2020 7d0a 0a20 2020 2023 2323        }..    ###
+00005340: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00005350: 2323 2323 2323 230a 2020 2020 2320 4469  #######.    # Di
+00005360: 7265 6374 6f72 790a 2020 2020 2323 2323  rectory.    ####
+00005370: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00005380: 2323 2323 2323 0a0a 2020 2020 4064 625f  ######..    @db_
+00005390: 7472 616e 7361 6374 696f 6e28 290a 2020  transaction().  
+000053a0: 2020 6465 6620 6469 7265 6374 6f72 795f    def directory_
+000053b0: 6164 6428 0a20 2020 2020 2020 2073 656c  add(.        sel
+000053c0: 662c 2064 6972 6563 746f 7269 6573 3a20  f, directories: 
+000053d0: 4c69 7374 5b44 6972 6563 746f 7279 5d2c  List[Directory],
+000053e0: 202a 2c20 6462 3a20 4462 2c20 6375 723d   *, db: Db, cur=
+000053f0: 4e6f 6e65 0a20 2020 2029 202d 3e20 4469  None.    ) -> Di
+00005400: 6374 5b73 7472 2c20 696e 745d 3a0a 2020  ct[str, int]:.  
+00005410: 2020 2020 2020 7375 6d6d 6172 7920 3d20        summary = 
+00005420: 7b22 6469 7265 6374 6f72 793a 6164 6422  {"directory:add"
+00005430: 3a20 307d 0a0a 2020 2020 2020 2020 6469  : 0}..        di
+00005440: 7273 203d 2073 6574 2829 0a20 2020 2020  rs = set().     
+00005450: 2020 2064 6972 5f65 6e74 7269 6573 3a20     dir_entries: 
+00005460: 4469 6374 5b73 7472 2c20 6465 6661 756c  Dict[str, defaul
+00005470: 7464 6963 745d 203d 207b 0a20 2020 2020  tdict] = {.     
+00005480: 2020 2020 2020 2022 6669 6c65 223a 2064         "file": d
+00005490: 6566 6175 6c74 6469 6374 286c 6973 7429  efaultdict(list)
+000054a0: 2c0a 2020 2020 2020 2020 2020 2020 2264  ,.            "d
+000054b0: 6972 223a 2064 6566 6175 6c74 6469 6374  ir": defaultdict
+000054c0: 286c 6973 7429 2c0a 2020 2020 2020 2020  (list),.        
+000054d0: 2020 2020 2272 6576 223a 2064 6566 6175      "rev": defau
+000054e0: 6c74 6469 6374 286c 6973 7429 2c0a 2020  ltdict(list),.  
+000054f0: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
+00005500: 2066 6f72 2063 7572 5f64 6972 2069 6e20   for cur_dir in 
+00005510: 6469 7265 6374 6f72 6965 733a 0a20 2020  directories:.   
+00005520: 2020 2020 2020 2020 2064 6972 5f69 6420           dir_id 
+00005530: 3d20 6375 725f 6469 722e 6964 0a20 2020  = cur_dir.id.   
+00005540: 2020 2020 2020 2020 2064 6972 732e 6164           dirs.ad
+00005550: 6428 6469 725f 6964 290a 2020 2020 2020  d(dir_id).      
+00005560: 2020 2020 2020 666f 7220 7372 635f 656e        for src_en
+00005570: 7472 7920 696e 2063 7572 5f64 6972 2e65  try in cur_dir.e
+00005580: 6e74 7269 6573 3a0a 2020 2020 2020 2020  ntries:.        
+00005590: 2020 2020 2020 2020 656e 7472 7920 3d20          entry = 
+000055a0: 7372 635f 656e 7472 792e 746f 5f64 6963  src_entry.to_dic
+000055b0: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
+000055c0: 2020 2020 656e 7472 795b 2264 6972 5f69      entry["dir_i
+000055d0: 6422 5d20 3d20 6469 725f 6964 0a20 2020  d"] = dir_id.   
+000055e0: 2020 2020 2020 2020 2020 2020 2064 6972               dir
+000055f0: 5f65 6e74 7269 6573 5b65 6e74 7279 5b22  _entries[entry["
+00005600: 7479 7065 225d 5d5b 6469 725f 6964 5d2e  type"]][dir_id].
+00005610: 6170 7065 6e64 2865 6e74 7279 290a 0a20  append(entry).. 
+00005620: 2020 2020 2020 2064 6972 735f 6d69 7373         dirs_miss
+00005630: 696e 6720 3d20 7365 7428 7365 6c66 2e64  ing = set(self.d
+00005640: 6972 6563 746f 7279 5f6d 6973 7369 6e67  irectory_missing
+00005650: 2864 6972 732c 2064 623d 6462 2c20 6375  (dirs, db=db, cu
+00005660: 723d 6375 7229 290a 2020 2020 2020 2020  r=cur)).        
+00005670: 6966 206e 6f74 2064 6972 735f 6d69 7373  if not dirs_miss
+00005680: 696e 673a 0a20 2020 2020 2020 2020 2020  ing:.           
+00005690: 2072 6574 7572 6e20 7375 6d6d 6172 790a   return summary.
+000056a0: 0a20 2020 2020 2020 2073 656c 662e 6a6f  .        self.jo
+000056b0: 7572 6e61 6c5f 7772 6974 6572 2e64 6972  urnal_writer.dir
+000056c0: 6563 746f 7279 5f61 6464 280a 2020 2020  ectory_add(.    
+000056d0: 2020 2020 2020 2020 6469 725f 2066 6f72          dir_ for
+000056e0: 2064 6972 5f20 696e 2064 6972 6563 746f   dir_ in directo
+000056f0: 7269 6573 2069 6620 6469 725f 2e69 6420  ries if dir_.id 
+00005700: 696e 2064 6972 735f 6d69 7373 696e 670a  in dirs_missing.
+00005710: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00005720: 2020 2023 2043 6f70 7920 6469 7265 6374     # Copy direct
+00005730: 6f72 7920 6d65 7461 6461 7461 0a20 2020  ory metadata.   
+00005740: 2020 2020 2064 6972 735f 6d69 7373 696e       dirs_missin
+00005750: 675f 6469 6374 203d 2028 0a20 2020 2020  g_dict = (.     
+00005760: 2020 2020 2020 207b 2269 6422 3a20 6469         {"id": di
+00005770: 725f 2e69 642c 2022 7261 775f 6d61 6e69  r_.id, "raw_mani
+00005780: 6665 7374 223a 2064 6972 5f2e 7261 775f  fest": dir_.raw_
+00005790: 6d61 6e69 6665 7374 7d0a 2020 2020 2020  manifest}.      
+000057a0: 2020 2020 2020 666f 7220 6469 725f 2069        for dir_ i
+000057b0: 6e20 6469 7265 6374 6f72 6965 730a 2020  n directories.  
+000057c0: 2020 2020 2020 2020 2020 6966 2064 6972            if dir
+000057d0: 5f2e 6964 2069 6e20 6469 7273 5f6d 6973  _.id in dirs_mis
+000057e0: 7369 6e67 0a20 2020 2020 2020 2029 0a20  sing.        ). 
+000057f0: 2020 2020 2020 2064 622e 6d6b 7465 6d70         db.mktemp
+00005800: 2822 6469 7265 6374 6f72 7922 2c20 6375  ("directory", cu
+00005810: 7229 0a20 2020 2020 2020 2064 622e 636f  r).        db.co
+00005820: 7079 5f74 6f28 6469 7273 5f6d 6973 7369  py_to(dirs_missi
+00005830: 6e67 5f64 6963 742c 2022 746d 705f 6469  ng_dict, "tmp_di
+00005840: 7265 6374 6f72 7922 2c20 5b22 6964 222c  rectory", ["id",
+00005850: 2022 7261 775f 6d61 6e69 6665 7374 225d   "raw_manifest"]
+00005860: 2c20 6375 7229 0a0a 2020 2020 2020 2020  , cur)..        
+00005870: 2320 436f 7079 2065 6e74 7269 6573 0a20  # Copy entries. 
+00005880: 2020 2020 2020 2066 6f72 2065 6e74 7279         for entry
+00005890: 5f74 7970 652c 2065 6e74 7279 5f6c 6973  _type, entry_lis
+000058a0: 7420 696e 2064 6972 5f65 6e74 7269 6573  t in dir_entries
+000058b0: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
+000058c0: 2020 2020 2020 656e 7472 6965 7320 3d20        entries = 
+000058d0: 6974 6572 746f 6f6c 732e 6368 6169 6e2e  itertools.chain.
+000058e0: 6672 6f6d 5f69 7465 7261 626c 6528 0a20  from_iterable(. 
+000058f0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00005900: 6e74 7269 6573 5f66 6f72 5f64 6972 0a20  ntries_for_dir. 
+00005910: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00005920: 6f72 2064 6972 5f69 642c 2065 6e74 7269  or dir_id, entri
+00005930: 6573 5f66 6f72 5f64 6972 2069 6e20 656e  es_for_dir in en
+00005940: 7472 795f 6c69 7374 2e69 7465 6d73 2829  try_list.items()
+00005950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005960: 2069 6620 6469 725f 6964 2069 6e20 6469   if dir_id in di
+00005970: 7273 5f6d 6973 7369 6e67 0a20 2020 2020  rs_missing.     
+00005980: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00005990: 2020 2020 2020 6462 2e6d 6b74 656d 705f        db.mktemp_
+000059a0: 6469 725f 656e 7472 7928 656e 7472 795f  dir_entry(entry_
+000059b0: 7479 7065 290a 0a20 2020 2020 2020 2020  type)..         
+000059c0: 2020 2064 622e 636f 7079 5f74 6f28 0a20     db.copy_to(. 
+000059d0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000059e0: 6e74 7269 6573 2c0a 2020 2020 2020 2020  ntries,.        
+000059f0: 2020 2020 2020 2020 2274 6d70 5f64 6972          "tmp_dir
+00005a00: 6563 746f 7279 5f65 6e74 7279 5f25 7322  ectory_entry_%s"
+00005a10: 2025 2065 6e74 7279 5f74 7970 652c 0a20   % entry_type,. 
+00005a20: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+00005a30: 2274 6172 6765 7422 2c20 226e 616d 6522  "target", "name"
+00005a40: 2c20 2270 6572 6d73 222c 2022 6469 725f  , "perms", "dir_
+00005a50: 6964 225d 2c0a 2020 2020 2020 2020 2020  id"],.          
+00005a60: 2020 2020 2020 6375 722c 0a20 2020 2020        cur,.     
+00005a70: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00005a80: 2020 2320 446f 2074 6865 2066 696e 616c    # Do the final
+00005a90: 2063 6f70 790a 2020 2020 2020 2020 6462   copy.        db
+00005aa0: 2e64 6972 6563 746f 7279 5f61 6464 5f66  .directory_add_f
+00005ab0: 726f 6d5f 7465 6d70 2863 7572 290a 2020  rom_temp(cur).  
+00005ac0: 2020 2020 2020 7375 6d6d 6172 795b 2264        summary["d
+00005ad0: 6972 6563 746f 7279 3a61 6464 225d 203d  irectory:add"] =
+00005ae0: 206c 656e 2864 6972 735f 6d69 7373 696e   len(dirs_missin
+00005af0: 6729 0a0a 2020 2020 2020 2020 7265 7475  g)..        retu
+00005b00: 726e 2073 756d 6d61 7279 0a0a 2020 2020  rn summary..    
+00005b10: 4064 625f 7472 616e 7361 6374 696f 6e5f  @db_transaction_
+00005b20: 6765 6e65 7261 746f 7228 290a 2020 2020  generator().    
+00005b30: 6465 6620 6469 7265 6374 6f72 795f 6d69  def directory_mi
+00005b40: 7373 696e 6728 0a20 2020 2020 2020 2073  ssing(.        s
+00005b50: 656c 662c 2064 6972 6563 746f 7269 6573  elf, directories
+00005b60: 3a20 4c69 7374 5b53 6861 3147 6974 5d2c  : List[Sha1Git],
+00005b70: 202a 2c20 6462 3a20 4462 2c20 6375 723d   *, db: Db, cur=
+00005b80: 4e6f 6e65 0a20 2020 2029 202d 3e20 4974  None.    ) -> It
+00005b90: 6572 6162 6c65 5b53 6861 3147 6974 5d3a  erable[Sha1Git]:
+00005ba0: 0a20 2020 2020 2020 2066 6f72 206f 626a  .        for obj
+00005bb0: 2069 6e20 6462 2e64 6972 6563 746f 7279   in db.directory
+00005bc0: 5f6d 6973 7369 6e67 5f66 726f 6d5f 6c69  _missing_from_li
+00005bd0: 7374 2864 6972 6563 746f 7269 6573 2c20  st(directories, 
+00005be0: 6375 7229 3a0a 2020 2020 2020 2020 2020  cur):.          
+00005bf0: 2020 7969 656c 6420 6f62 6a5b 305d 0a0a    yield obj[0]..
+00005c00: 2020 2020 4064 625f 7472 616e 7361 6374      @db_transact
+00005c10: 696f 6e5f 6765 6e65 7261 746f 7228 7374  ion_generator(st
+00005c20: 6174 656d 656e 745f 7469 6d65 6f75 743d  atement_timeout=
+00005c30: 3230 3030 3029 0a20 2020 2064 6566 2064  20000).    def d
+00005c40: 6972 6563 746f 7279 5f6c 7328 0a20 2020  irectory_ls(.   
+00005c50: 2020 2020 2073 656c 662c 2064 6972 6563       self, direc
+00005c60: 746f 7279 3a20 5368 6131 4769 742c 2072  tory: Sha1Git, r
+00005c70: 6563 7572 7369 7665 3a20 626f 6f6c 203d  ecursive: bool =
+00005c80: 2046 616c 7365 2c20 2a2c 2064 623a 2044   False, *, db: D
+00005c90: 622c 2063 7572 3d4e 6f6e 650a 2020 2020  b, cur=None.    
+00005ca0: 2920 2d3e 2049 7465 7261 626c 655b 4469  ) -> Iterable[Di
+00005cb0: 6374 5b73 7472 2c20 416e 795d 5d3a 0a20  ct[str, Any]]:. 
+00005cc0: 2020 2020 2020 2069 6620 7265 6375 7273         if recurs
+00005cd0: 6976 653a 0a20 2020 2020 2020 2020 2020  ive:.           
+00005ce0: 2072 6573 5f67 656e 203d 2064 622e 6469   res_gen = db.di
+00005cf0: 7265 6374 6f72 795f 7761 6c6b 2864 6972  rectory_walk(dir
+00005d00: 6563 746f 7279 2c20 6375 723d 6375 7229  ectory, cur=cur)
+00005d10: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00005d20: 2020 2020 2020 2020 2020 2072 6573 5f67             res_g
+00005d30: 656e 203d 2064 622e 6469 7265 6374 6f72  en = db.director
+00005d40: 795f 7761 6c6b 5f6f 6e65 2864 6972 6563  y_walk_one(direc
+00005d50: 746f 7279 2c20 6375 723d 6375 7229 0a0a  tory, cur=cur)..
+00005d60: 2020 2020 2020 2020 666f 7220 6c69 6e65          for line
+00005d70: 2069 6e20 7265 735f 6765 6e3a 0a20 2020   in res_gen:.   
+00005d80: 2020 2020 2020 2020 2079 6965 6c64 2064           yield d
+00005d90: 6963 7428 7a69 7028 6462 2e64 6972 6563  ict(zip(db.direc
+00005da0: 746f 7279 5f6c 735f 636f 6c73 2c20 6c69  tory_ls_cols, li
+00005db0: 6e65 2929 0a0a 2020 2020 4064 625f 7472  ne))..    @db_tr
+00005dc0: 616e 7361 6374 696f 6e28 7374 6174 656d  ansaction(statem
+00005dd0: 656e 745f 7469 6d65 6f75 743d 3430 3030  ent_timeout=4000
+00005de0: 290a 2020 2020 6465 6620 6469 7265 6374  ).    def direct
+00005df0: 6f72 795f 656e 7472 795f 6765 745f 6279  ory_entry_get_by
+00005e00: 5f70 6174 6828 0a20 2020 2020 2020 2073  _path(.        s
+00005e10: 656c 662c 2064 6972 6563 746f 7279 3a20  elf, directory: 
+00005e20: 5368 6131 4769 742c 2070 6174 6873 3a20  Sha1Git, paths: 
+00005e30: 4c69 7374 5b62 7974 6573 5d2c 202a 2c20  List[bytes], *, 
+00005e40: 6462 3a20 4462 2c20 6375 723d 4e6f 6e65  db: Db, cur=None
+00005e50: 0a20 2020 2029 202d 3e20 4f70 7469 6f6e  .    ) -> Option
+00005e60: 616c 5b44 6963 745b 7374 722c 2041 6e79  al[Dict[str, Any
+00005e70: 5d5d 3a0a 2020 2020 2020 2020 7265 7320  ]]:.        res 
+00005e80: 3d20 6462 2e64 6972 6563 746f 7279 5f65  = db.directory_e
+00005e90: 6e74 7279 5f67 6574 5f62 795f 7061 7468  ntry_get_by_path
+00005ea0: 2864 6972 6563 746f 7279 2c20 7061 7468  (directory, path
+00005eb0: 732c 2063 7572 290a 2020 2020 2020 2020  s, cur).        
+00005ec0: 7265 7475 726e 2064 6963 7428 7a69 7028  return dict(zip(
+00005ed0: 6462 2e64 6972 6563 746f 7279 5f6c 735f  db.directory_ls_
+00005ee0: 636f 6c73 2c20 7265 7329 2920 6966 2072  cols, res)) if r
+00005ef0: 6573 2065 6c73 6520 4e6f 6e65 0a0a 2020  es else None..  
+00005f00: 2020 4064 625f 7472 616e 7361 6374 696f    @db_transactio
+00005f10: 6e28 290a 2020 2020 6465 6620 6469 7265  n().    def dire
+00005f20: 6374 6f72 795f 6765 745f 7261 6e64 6f6d  ctory_get_random
+00005f30: 2873 656c 662c 202a 2c20 6462 3a20 4462  (self, *, db: Db
+00005f40: 2c20 6375 723d 4e6f 6e65 2920 2d3e 2053  , cur=None) -> S
+00005f50: 6861 3147 6974 3a0a 2020 2020 2020 2020  ha1Git:.        
+00005f60: 7265 7475 726e 2064 622e 6469 7265 6374  return db.direct
+00005f70: 6f72 795f 6765 745f 7261 6e64 6f6d 2863  ory_get_random(c
+00005f80: 7572 290a 0a20 2020 2040 6462 5f74 7261  ur)..    @db_tra
+00005f90: 6e73 6163 7469 6f6e 2829 0a20 2020 2064  nsaction().    d
+00005fa0: 6566 2064 6972 6563 746f 7279 5f67 6574  ef directory_get
+00005fb0: 5f65 6e74 7269 6573 280a 2020 2020 2020  _entries(.      
+00005fc0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00005fd0: 6469 7265 6374 6f72 795f 6964 3a20 5368  directory_id: Sh
+00005fe0: 6131 4769 742c 0a20 2020 2020 2020 2070  a1Git,.        p
+00005ff0: 6167 655f 746f 6b65 6e3a 204f 7074 696f  age_token: Optio
+00006000: 6e61 6c5b 6279 7465 735d 203d 204e 6f6e  nal[bytes] = Non
+00006010: 652c 0a20 2020 2020 2020 206c 696d 6974  e,.        limit
+00006020: 3a20 696e 7420 3d20 3130 3030 2c0a 2020  : int = 1000,.  
+00006030: 2020 2020 2020 2a2c 0a20 2020 2020 2020        *,.       
+00006040: 2064 623a 2044 622c 0a20 2020 2020 2020   db: Db,.       
+00006050: 2063 7572 3d4e 6f6e 652c 0a20 2020 2029   cur=None,.    )
+00006060: 202d 3e20 4f70 7469 6f6e 616c 5b50 6167   -> Optional[Pag
+00006070: 6564 5265 7375 6c74 5b44 6972 6563 746f  edResult[Directo
+00006080: 7279 456e 7472 795d 5d3a 0a20 2020 2020  ryEntry]]:.     
+00006090: 2020 2069 6620 6c69 7374 2873 656c 662e     if list(self.
+000060a0: 6469 7265 6374 6f72 795f 6d69 7373 696e  directory_missin
+000060b0: 6728 5b64 6972 6563 746f 7279 5f69 645d  g([directory_id]
+000060c0: 2c20 6462 3d64 622c 2063 7572 3d63 7572  , db=db, cur=cur
+000060d0: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+000060e0: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
+000060f0: 2020 2020 2069 6620 7061 6765 5f74 6f6b       if page_tok
+00006100: 656e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  en is not None:.
+00006110: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00006120: 6520 5374 6f72 6167 6541 7267 756d 656e  e StorageArgumen
+00006130: 7445 7863 6570 7469 6f6e 2822 556e 7375  tException("Unsu
+00006140: 7070 6f72 7465 6420 7061 6765 2074 6f6b  pported page tok
+00006150: 656e 2229 0a0a 2020 2020 2020 2020 2320  en")..        # 
+00006160: 544f 444f 3a20 6163 7475 616c 6c79 2070  TODO: actually p
+00006170: 6167 696e 6174 650a 2020 2020 2020 2020  aginate.        
+00006180: 726f 7773 203d 2064 622e 6469 7265 6374  rows = db.direct
+00006190: 6f72 795f 6765 745f 656e 7472 6965 7328  ory_get_entries(
+000061a0: 6469 7265 6374 6f72 795f 6964 2c20 6375  directory_id, cu
+000061b0: 723d 6375 7229 0a20 2020 2020 2020 2072  r=cur).        r
+000061c0: 6574 7572 6e20 5061 6765 6452 6573 756c  eturn PagedResul
+000061d0: 7428 0a20 2020 2020 2020 2020 2020 2072  t(.            r
+000061e0: 6573 756c 7473 3d5b 0a20 2020 2020 2020  esults=[.       
+000061f0: 2020 2020 2020 2020 2044 6972 6563 746f           Directo
+00006200: 7279 456e 7472 7928 2a2a 6469 6374 287a  ryEntry(**dict(z
+00006210: 6970 2864 622e 6469 7265 6374 6f72 795f  ip(db.directory_
+00006220: 6765 745f 656e 7472 6965 735f 636f 6c73  get_entries_cols
+00006230: 2c20 726f 7729 2929 0a20 2020 2020 2020  , row))).       
+00006240: 2020 2020 2020 2020 2066 6f72 2072 6f77           for row
+00006250: 2069 6e20 726f 7773 0a20 2020 2020 2020   in rows.       
+00006260: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
+00006270: 2020 2020 6e65 7874 5f70 6167 655f 746f      next_page_to
+00006280: 6b65 6e3d 4e6f 6e65 2c0a 2020 2020 2020  ken=None,.      
+00006290: 2020 290a 0a20 2020 2040 6462 5f74 7261    )..    @db_tra
+000062a0: 6e73 6163 7469 6f6e 2829 0a20 2020 2064  nsaction().    d
+000062b0: 6566 2064 6972 6563 746f 7279 5f67 6574  ef directory_get
+000062c0: 5f72 6177 5f6d 616e 6966 6573 7428 0a20  _raw_manifest(. 
+000062d0: 2020 2020 2020 2073 656c 662c 2064 6972         self, dir
+000062e0: 6563 746f 7279 5f69 6473 3a20 4c69 7374  ectory_ids: List
+000062f0: 5b53 6861 3147 6974 5d2c 202a 2c20 6462  [Sha1Git], *, db
+00006300: 3a20 4462 2c20 6375 723d 4e6f 6e65 0a20  : Db, cur=None. 
+00006310: 2020 2029 202d 3e20 4469 6374 5b53 6861     ) -> Dict[Sha
+00006320: 3147 6974 2c20 4f70 7469 6f6e 616c 5b62  1Git, Optional[b
+00006330: 7974 6573 5d5d 3a0a 2020 2020 2020 2020  ytes]]:.        
+00006340: 7265 7475 726e 2064 6963 7428 6462 2e64  return dict(db.d
+00006350: 6972 6563 746f 7279 5f67 6574 5f72 6177  irectory_get_raw
+00006360: 5f6d 616e 6966 6573 7428 6469 7265 6374  _manifest(direct
+00006370: 6f72 795f 6964 732c 2063 7572 3d63 7572  ory_ids, cur=cur
+00006380: 2929 0a0a 2020 2020 4064 625f 7472 616e  ))..    @db_tran
+00006390: 7361 6374 696f 6e28 290a 2020 2020 6465  saction().    de
+000063a0: 6620 6469 7265 6374 6f72 795f 6765 745f  f directory_get_
+000063b0: 6964 5f70 6172 7469 7469 6f6e 280a 2020  id_partition(.  
+000063c0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+000063d0: 2020 2020 7061 7274 6974 696f 6e5f 6964      partition_id
+000063e0: 3a20 696e 742c 0a20 2020 2020 2020 206e  : int,.        n
+000063f0: 625f 7061 7274 6974 696f 6e73 3a20 696e  b_partitions: in
+00006400: 742c 0a20 2020 2020 2020 2070 6167 655f  t,.        page_
+00006410: 746f 6b65 6e3a 204f 7074 696f 6e61 6c5b  token: Optional[
+00006420: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
+00006430: 2020 2020 206c 696d 6974 3a20 696e 7420       limit: int 
+00006440: 3d20 3130 3030 2c0a 2020 2020 2020 2020  = 1000,.        
+00006450: 2a2c 0a20 2020 2020 2020 2064 623a 2044  *,.        db: D
+00006460: 622c 0a20 2020 2020 2020 2063 7572 3d4e  b,.        cur=N
+00006470: 6f6e 652c 0a20 2020 2029 202d 3e20 5061  one,.    ) -> Pa
+00006480: 6765 6452 6573 756c 745b 5368 6131 4769  gedResult[Sha1Gi
+00006490: 745d 3a0a 2020 2020 2020 2020 7265 7475  t]:.        retu
+000064a0: 726e 205f 6765 745f 7061 6769 6e61 7465  rn _get_paginate
+000064b0: 645f 7368 6131 5f70 6172 7469 7469 6f6e  d_sha1_partition
+000064c0: 280a 2020 2020 2020 2020 2020 2020 6375  (.            cu
+000064d0: 722c 0a20 2020 2020 2020 2020 2020 2070  r,.            p
+000064e0: 6172 7469 7469 6f6e 5f69 642c 0a20 2020  artition_id,.   
+000064f0: 2020 2020 2020 2020 206e 625f 7061 7274           nb_part
+00006500: 6974 696f 6e73 2c0a 2020 2020 2020 2020  itions,.        
+00006510: 2020 2020 7061 6765 5f74 6f6b 656e 2c0a      page_token,.
+00006520: 2020 2020 2020 2020 2020 2020 6c69 6d69              limi
+00006530: 742c 0a20 2020 2020 2020 2020 2020 2064  t,.            d
+00006540: 622e 6469 7265 6374 6f72 795f 6765 745f  b.directory_get_
+00006550: 6964 5f72 616e 6765 2c0a 2020 2020 2020  id_range,.      
+00006560: 2020 2020 2020 6f70 6572 6174 6f72 2e69        operator.i
+00006570: 7465 6d67 6574 7465 7228 3029 2c0a 2020  temgetter(0),.  
+00006580: 2020 2020 2020 2020 2020 6c61 6d62 6461            lambda
+00006590: 2069 645f 3a20 6964 5f2c 0a20 2020 2020   id_: id_,.     
+000065a0: 2020 2029 0a0a 2020 2020 2323 2323 2323     )..    ######
+000065b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000065c0: 2323 2323 0a20 2020 2023 2052 6576 6973  ####.    # Revis
+000065d0: 696f 6e0a 2020 2020 2323 2323 2323 2323  ion.    ########
+000065e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000065f0: 2323 0a0a 2020 2020 4064 625f 7472 616e  ##..    @db_tran
+00006600: 7361 6374 696f 6e28 290a 2020 2020 6465  saction().    de
+00006610: 6620 7265 7669 7369 6f6e 5f61 6464 280a  f revision_add(.
+00006620: 2020 2020 2020 2020 7365 6c66 2c20 7265          self, re
+00006630: 7669 7369 6f6e 733a 204c 6973 745b 5265  visions: List[Re
+00006640: 7669 7369 6f6e 5d2c 202a 2c20 6462 3a20  vision], *, db: 
+00006650: 4462 2c20 6375 723d 4e6f 6e65 0a20 2020  Db, cur=None.   
+00006660: 2029 202d 3e20 4469 6374 5b73 7472 2c20   ) -> Dict[str, 
+00006670: 696e 745d 3a0a 2020 2020 2020 2020 7375  int]:.        su
+00006680: 6d6d 6172 7920 3d20 7b22 7265 7669 7369  mmary = {"revisi
+00006690: 6f6e 3a61 6464 223a 2030 7d0a 0a20 2020  on:add": 0}..   
+000066a0: 2020 2020 2072 6576 6973 696f 6e73 5f6d       revisions_m
+000066b0: 6973 7369 6e67 203d 2073 6574 280a 2020  issing = set(.  
+000066c0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+000066d0: 6576 6973 696f 6e5f 6d69 7373 696e 6728  evision_missing(
+000066e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000066f0: 2073 6574 2872 6576 6973 696f 6e2e 6964   set(revision.id
+00006700: 2066 6f72 2072 6576 6973 696f 6e20 696e   for revision in
+00006710: 2072 6576 6973 696f 6e73 292c 2064 623d   revisions), db=
+00006720: 6462 2c20 6375 723d 6375 720a 2020 2020  db, cur=cur.    
+00006730: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00006740: 2020 290a 0a20 2020 2020 2020 2069 6620    )..        if 
+00006750: 6e6f 7420 7265 7669 7369 6f6e 735f 6d69  not revisions_mi
+00006760: 7373 696e 673a 0a20 2020 2020 2020 2020  ssing:.         
+00006770: 2020 2072 6574 7572 6e20 7375 6d6d 6172     return summar
+00006780: 790a 0a20 2020 2020 2020 2064 622e 6d6b  y..        db.mk
+00006790: 7465 6d70 5f72 6576 6973 696f 6e28 6375  temp_revision(cu
+000067a0: 7229 0a0a 2020 2020 2020 2020 7265 7669  r)..        revi
+000067b0: 7369 6f6e 735f 6669 6c74 6572 6564 203d  sions_filtered =
+000067c0: 205b 0a20 2020 2020 2020 2020 2020 2072   [.            r
+000067d0: 6576 6973 696f 6e20 666f 7220 7265 7669  evision for revi
+000067e0: 7369 6f6e 2069 6e20 7265 7669 7369 6f6e  sion in revision
+000067f0: 7320 6966 2072 6576 6973 696f 6e2e 6964  s if revision.id
+00006800: 2069 6e20 7265 7669 7369 6f6e 735f 6d69   in revisions_mi
+00006810: 7373 696e 670a 2020 2020 2020 2020 5d0a  ssing.        ].
+00006820: 0a20 2020 2020 2020 2073 656c 662e 6a6f  .        self.jo
+00006830: 7572 6e61 6c5f 7772 6974 6572 2e72 6576  urnal_writer.rev
+00006840: 6973 696f 6e5f 6164 6428 7265 7669 7369  ision_add(revisi
+00006850: 6f6e 735f 6669 6c74 6572 6564 290a 0a20  ons_filtered).. 
+00006860: 2020 2020 2020 2064 625f 7265 7669 7369         db_revisi
+00006870: 6f6e 735f 6669 6c74 6572 6564 203d 206c  ons_filtered = l
+00006880: 6973 7428 6d61 7028 636f 6e76 6572 7465  ist(map(converte
+00006890: 7273 2e72 6576 6973 696f 6e5f 746f 5f64  rs.revision_to_d
+000068a0: 622c 2072 6576 6973 696f 6e73 5f66 696c  b, revisions_fil
+000068b0: 7465 7265 6429 290a 0a20 2020 2020 2020  tered))..       
+000068c0: 2070 6172 656e 7473 5f66 696c 7465 7265   parents_filtere
+000068d0: 643a 204c 6973 745b 4469 6374 5b73 7472  d: List[Dict[str
+000068e0: 2c20 416e 795d 5d20 3d20 5b5d 0a0a 2020  , Any]] = []..  
+000068f0: 2020 2020 2020 7769 7468 2063 6f6e 7665        with conve
+00006900: 7274 5f76 616c 6964 6174 696f 6e5f 6578  rt_validation_ex
+00006910: 6365 7074 696f 6e73 2829 3a0a 2020 2020  ceptions():.    
+00006920: 2020 2020 2020 2020 6462 2e63 6f70 795f          db.copy_
+00006930: 746f 280a 2020 2020 2020 2020 2020 2020  to(.            
+00006940: 2020 2020 6462 5f72 6576 6973 696f 6e73      db_revisions
+00006950: 5f66 696c 7465 7265 642c 0a20 2020 2020  _filtered,.     
+00006960: 2020 2020 2020 2020 2020 2022 746d 705f             "tmp_
+00006970: 7265 7669 7369 6f6e 222c 0a20 2020 2020  revision",.     
+00006980: 2020 2020 2020 2020 2020 2064 622e 7265             db.re
+00006990: 7669 7369 6f6e 5f61 6464 5f63 6f6c 732c  vision_add_cols,
+000069a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000069b0: 2063 7572 2c0a 2020 2020 2020 2020 2020   cur,.          
+000069c0: 2020 2020 2020 6c61 6d62 6461 2072 6576        lambda rev
+000069d0: 3a20 7061 7265 6e74 735f 6669 6c74 6572  : parents_filter
+000069e0: 6564 2e65 7874 656e 6428 7265 765b 2270  ed.extend(rev["p
+000069f0: 6172 656e 7473 225d 292c 0a20 2020 2020  arents"]),.     
+00006a00: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00006a10: 2020 2020 2020 6462 2e72 6576 6973 696f        db.revisio
+00006a20: 6e5f 6164 645f 6672 6f6d 5f74 656d 7028  n_add_from_temp(
+00006a30: 6375 7229 0a0a 2020 2020 2020 2020 2020  cur)..          
+00006a40: 2020 6462 2e63 6f70 795f 746f 280a 2020    db.copy_to(.  
+00006a50: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00006a60: 7265 6e74 735f 6669 6c74 6572 6564 2c0a  rents_filtered,.
+00006a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a80: 2272 6576 6973 696f 6e5f 6869 7374 6f72  "revision_histor
+00006a90: 7922 2c0a 2020 2020 2020 2020 2020 2020  y",.            
+00006aa0: 2020 2020 5b22 6964 222c 2022 7061 7265      ["id", "pare
+00006ab0: 6e74 5f69 6422 2c20 2270 6172 656e 745f  nt_id", "parent_
+00006ac0: 7261 6e6b 225d 2c0a 2020 2020 2020 2020  rank"],.        
+00006ad0: 2020 2020 2020 2020 6375 722c 0a20 2020          cur,.   
+00006ae0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+00006af0: 2020 2020 7265 7475 726e 207b 2272 6576      return {"rev
+00006b00: 6973 696f 6e3a 6164 6422 3a20 6c65 6e28  ision:add": len(
+00006b10: 7265 7669 7369 6f6e 735f 6d69 7373 696e  revisions_missin
+00006b20: 6729 7d0a 0a20 2020 2040 6462 5f74 7261  g)}..    @db_tra
+00006b30: 6e73 6163 7469 6f6e 5f67 656e 6572 6174  nsaction_generat
+00006b40: 6f72 2829 0a20 2020 2064 6566 2072 6576  or().    def rev
+00006b50: 6973 696f 6e5f 6d69 7373 696e 6728 0a20  ision_missing(. 
+00006b60: 2020 2020 2020 2073 656c 662c 2072 6576         self, rev
+00006b70: 6973 696f 6e73 3a20 4c69 7374 5b53 6861  isions: List[Sha
+00006b80: 3147 6974 5d2c 202a 2c20 6462 3a20 4462  1Git], *, db: Db
+00006b90: 2c20 6375 723d 4e6f 6e65 0a20 2020 2029  , cur=None.    )
+00006ba0: 202d 3e20 4974 6572 6162 6c65 5b53 6861   -> Iterable[Sha
+00006bb0: 3147 6974 5d3a 0a20 2020 2020 2020 2069  1Git]:.        i
+00006bc0: 6620 6e6f 7420 7265 7669 7369 6f6e 733a  f not revisions:
+00006bd0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00006be0: 7572 6e20 4e6f 6e65 0a0a 2020 2020 2020  urn None..      
+00006bf0: 2020 666f 7220 6f62 6a20 696e 2064 622e    for obj in db.
+00006c00: 7265 7669 7369 6f6e 5f6d 6973 7369 6e67  revision_missing
+00006c10: 5f66 726f 6d5f 6c69 7374 2872 6576 6973  _from_list(revis
+00006c20: 696f 6e73 2c20 6375 7229 3a0a 2020 2020  ions, cur):.    
+00006c30: 2020 2020 2020 2020 7969 656c 6420 6f62          yield ob
+00006c40: 6a5b 305d 0a0a 2020 2020 4064 625f 7472  j[0]..    @db_tr
+00006c50: 616e 7361 6374 696f 6e28 290a 2020 2020  ansaction().    
+00006c60: 6465 6620 7265 7669 7369 6f6e 5f67 6574  def revision_get
+00006c70: 5f70 6172 7469 7469 6f6e 280a 2020 2020  _partition(.    
+00006c80: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00006c90: 2020 7061 7274 6974 696f 6e5f 6964 3a20    partition_id: 
+00006ca0: 696e 742c 0a20 2020 2020 2020 206e 625f  int,.        nb_
+00006cb0: 7061 7274 6974 696f 6e73 3a20 696e 742c  partitions: int,
+00006cc0: 0a20 2020 2020 2020 2070 6167 655f 746f  .        page_to
+00006cd0: 6b65 6e3a 204f 7074 696f 6e61 6c5b 7374  ken: Optional[st
+00006ce0: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
+00006cf0: 2020 206c 696d 6974 3a20 696e 7420 3d20     limit: int = 
+00006d00: 3130 3030 2c0a 2020 2020 2020 2020 2a2c  1000,.        *,
+00006d10: 0a20 2020 2020 2020 2064 623a 2044 622c  .        db: Db,
+00006d20: 0a20 2020 2020 2020 2063 7572 3d4e 6f6e  .        cur=Non
+00006d30: 652c 0a20 2020 2029 202d 3e20 5061 6765  e,.    ) -> Page
+00006d40: 6452 6573 756c 745b 5265 7669 7369 6f6e  dResult[Revision
+00006d50: 5d3a 0a20 2020 2020 2020 2072 6574 7572  ]:.        retur
+00006d60: 6e20 5f67 6574 5f70 6167 696e 6174 6564  n _get_paginated
+00006d70: 5f73 6861 315f 7061 7274 6974 696f 6e28  _sha1_partition(
+00006d80: 0a20 2020 2020 2020 2020 2020 2063 7572  .            cur
+00006d90: 2c0a 2020 2020 2020 2020 2020 2020 7061  ,.            pa
+00006da0: 7274 6974 696f 6e5f 6964 2c0a 2020 2020  rtition_id,.    
+00006db0: 2020 2020 2020 2020 6e62 5f70 6172 7469          nb_parti
+00006dc0: 7469 6f6e 732c 0a20 2020 2020 2020 2020  tions,.         
+00006dd0: 2020 2070 6167 655f 746f 6b65 6e2c 0a20     page_token,. 
+00006de0: 2020 2020 2020 2020 2020 206c 696d 6974             limit
+00006df0: 2c0a 2020 2020 2020 2020 2020 2020 6462  ,.            db
+00006e00: 2e72 6576 6973 696f 6e5f 6765 745f 7261  .revision_get_ra
+00006e10: 6e67 652c 0a20 2020 2020 2020 2020 2020  nge,.           
+00006e20: 206c 616d 6264 6120 726f 773a 2063 6f6e   lambda row: con
+00006e30: 7665 7274 6572 732e 6462 5f74 6f5f 7265  verters.db_to_re
+00006e40: 7669 7369 6f6e 2864 6963 7428 7a69 7028  vision(dict(zip(
+00006e50: 6462 2e72 6576 6973 696f 6e5f 6765 745f  db.revision_get_
+00006e60: 636f 6c73 2c20 726f 7729 2929 2c0a 2020  cols, row))),.  
+00006e70: 2020 2020 2020 290a 0a20 2020 2040 6462        )..    @db
+00006e80: 5f74 7261 6e73 6163 7469 6f6e 2873 7461  _transaction(sta
+00006e90: 7465 6d65 6e74 5f74 696d 656f 7574 3d32  tement_timeout=2
+00006ea0: 3030 3029 0a20 2020 2064 6566 2072 6576  000).    def rev
+00006eb0: 6973 696f 6e5f 6765 7428 0a20 2020 2020  ision_get(.     
+00006ec0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00006ed0: 2072 6576 6973 696f 6e5f 6964 733a 204c   revision_ids: L
+00006ee0: 6973 745b 5368 6131 4769 745d 2c0a 2020  ist[Sha1Git],.  
+00006ef0: 2020 2020 2020 6967 6e6f 7265 5f64 6973        ignore_dis
+00006f00: 706c 6179 6e61 6d65 3a20 626f 6f6c 203d  playname: bool =
+00006f10: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
+00006f20: 2a2c 0a20 2020 2020 2020 2064 623a 2044  *,.        db: D
+00006f30: 622c 0a20 2020 2020 2020 2063 7572 3d4e  b,.        cur=N
+00006f40: 6f6e 652c 0a20 2020 2029 202d 3e20 4c69  one,.    ) -> Li
+00006f50: 7374 5b4f 7074 696f 6e61 6c5b 5265 7669  st[Optional[Revi
+00006f60: 7369 6f6e 5d5d 3a0a 2020 2020 2020 2020  sion]]:.        
+00006f70: 7265 7669 7369 6f6e 7320 3d20 5b5d 0a20  revisions = []. 
+00006f80: 2020 2020 2020 2066 6f72 206c 696e 6520         for line 
+00006f90: 696e 2064 622e 7265 7669 7369 6f6e 5f67  in db.revision_g
+00006fa0: 6574 5f66 726f 6d5f 6c69 7374 2872 6576  et_from_list(rev
+00006fb0: 6973 696f 6e5f 6964 732c 2069 676e 6f72  ision_ids, ignor
+00006fc0: 655f 6469 7370 6c61 796e 616d 652c 2063  e_displayname, c
+00006fd0: 7572 293a 0a20 2020 2020 2020 2020 2020  ur):.           
+00006fe0: 2072 6576 6973 696f 6e20 3d20 636f 6e76   revision = conv
+00006ff0: 6572 7465 7273 2e64 625f 746f 5f6f 7074  erters.db_to_opt
+00007000: 696f 6e61 6c5f 7265 7669 7369 6f6e 280a  ional_revision(.
+00007010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007020: 6469 6374 287a 6970 2864 622e 7265 7669  dict(zip(db.revi
+00007030: 7369 6f6e 5f67 6574 5f63 6f6c 732c 206c  sion_get_cols, l
+00007040: 696e 6529 290a 2020 2020 2020 2020 2020  ine)).          
+00007050: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00007060: 7265 7669 7369 6f6e 732e 6170 7065 6e64  revisions.append
+00007070: 2872 6576 6973 696f 6e29 0a0a 2020 2020  (revision)..    
+00007080: 2020 2020 7265 7475 726e 2072 6576 6973      return revis
+00007090: 696f 6e73 0a0a 2020 2020 4064 625f 7472  ions..    @db_tr
+000070a0: 616e 7361 6374 696f 6e5f 6765 6e65 7261  ansaction_genera
+000070b0: 746f 7228 7374 6174 656d 656e 745f 7469  tor(statement_ti
+000070c0: 6d65 6f75 743d 3230 3030 290a 2020 2020  meout=2000).    
+000070d0: 6465 6620 7265 7669 7369 6f6e 5f6c 6f67  def revision_log
+000070e0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+000070f0: 2020 2020 2020 2020 7265 7669 7369 6f6e          revision
+00007100: 733a 204c 6973 745b 5368 6131 4769 745d  s: List[Sha1Git]
+00007110: 2c0a 2020 2020 2020 2020 6967 6e6f 7265  ,.        ignore
+00007120: 5f64 6973 706c 6179 6e61 6d65 3a20 626f  _displayname: bo
+00007130: 6f6c 203d 2046 616c 7365 2c0a 2020 2020  ol = False,.    
+00007140: 2020 2020 6c69 6d69 743a 204f 7074 696f      limit: Optio
+00007150: 6e61 6c5b 696e 745d 203d 204e 6f6e 652c  nal[int] = None,
+00007160: 0a20 2020 2020 2020 202a 2c0a 2020 2020  .        *,.    
+00007170: 2020 2020 6462 3a20 4462 2c0a 2020 2020      db: Db,.    
+00007180: 2020 2020 6375 723d 4e6f 6e65 2c0a 2020      cur=None,.  
+00007190: 2020 2920 2d3e 2049 7465 7261 626c 655b    ) -> Iterable[
+000071a0: 4f70 7469 6f6e 616c 5b44 6963 745b 7374  Optional[Dict[st
+000071b0: 722c 2041 6e79 5d5d 5d3a 0a20 2020 2020  r, Any]]]:.     
+000071c0: 2020 2066 6f72 206c 696e 6520 696e 2064     for line in d
+000071d0: 622e 7265 7669 7369 6f6e 5f6c 6f67 280a  b.revision_log(.
+000071e0: 2020 2020 2020 2020 2020 2020 7265 7669              revi
+000071f0: 7369 6f6e 732c 2069 676e 6f72 655f 6469  sions, ignore_di
+00007200: 7370 6c61 796e 616d 653d 6967 6e6f 7265  splayname=ignore
+00007210: 5f64 6973 706c 6179 6e61 6d65 2c20 6c69  _displayname, li
+00007220: 6d69 743d 6c69 6d69 742c 2063 7572 3d63  mit=limit, cur=c
+00007230: 7572 0a20 2020 2020 2020 2029 3a0a 2020  ur.        ):.  
+00007240: 2020 2020 2020 2020 2020 6461 7461 203d            data =
+00007250: 2063 6f6e 7665 7274 6572 732e 6462 5f74   converters.db_t
+00007260: 6f5f 7265 7669 7369 6f6e 2864 6963 7428  o_revision(dict(
+00007270: 7a69 7028 6462 2e72 6576 6973 696f 6e5f  zip(db.revision_
+00007280: 6765 745f 636f 6c73 2c20 6c69 6e65 2929  get_cols, line))
+00007290: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+000072a0: 206e 6f74 2064 6174 613a 0a20 2020 2020   not data:.     
+000072b0: 2020 2020 2020 2020 2020 2079 6965 6c64             yield
+000072c0: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+000072d0: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
+000072e0: 2020 2020 2020 2020 2020 2079 6965 6c64             yield
+000072f0: 2064 6174 612e 746f 5f64 6963 7428 290a   data.to_dict().
+00007300: 0a20 2020 2040 6462 5f74 7261 6e73 6163  .    @db_transac
+00007310: 7469 6f6e 5f67 656e 6572 6174 6f72 2873  tion_generator(s
+00007320: 7461 7465 6d65 6e74 5f74 696d 656f 7574  tatement_timeout
+00007330: 3d32 3030 3029 0a20 2020 2064 6566 2072  =2000).    def r
+00007340: 6576 6973 696f 6e5f 7368 6f72 746c 6f67  evision_shortlog
+00007350: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
+00007360: 7265 7669 7369 6f6e 733a 204c 6973 745b  revisions: List[
+00007370: 5368 6131 4769 745d 2c20 6c69 6d69 743a  Sha1Git], limit:
+00007380: 204f 7074 696f 6e61 6c5b 696e 745d 203d   Optional[int] =
+00007390: 204e 6f6e 652c 202a 2c20 6462 3a20 4462   None, *, db: Db
+000073a0: 2c20 6375 723d 4e6f 6e65 0a20 2020 2029  , cur=None.    )
+000073b0: 202d 3e20 4974 6572 6162 6c65 5b4f 7074   -> Iterable[Opt
+000073c0: 696f 6e61 6c5b 5475 706c 655b 5368 6131  ional[Tuple[Sha1
+000073d0: 4769 742c 2054 7570 6c65 5b53 6861 3147  Git, Tuple[Sha1G
+000073e0: 6974 2c20 2e2e 2e5d 5d5d 5d3a 0a20 2020  it, ...]]]]:.   
+000073f0: 2020 2020 2079 6965 6c64 2066 726f 6d20       yield from 
+00007400: 6462 2e72 6576 6973 696f 6e5f 7368 6f72  db.revision_shor
+00007410: 746c 6f67 2872 6576 6973 696f 6e73 2c20  tlog(revisions, 
+00007420: 6c69 6d69 742c 2063 7572 290a 0a20 2020  limit, cur)..   
+00007430: 2040 6462 5f74 7261 6e73 6163 7469 6f6e   @db_transaction
+00007440: 2829 0a20 2020 2064 6566 2072 6576 6973  ().    def revis
+00007450: 696f 6e5f 6765 745f 7261 6e64 6f6d 2873  ion_get_random(s
+00007460: 656c 662c 202a 2c20 6462 3a20 4462 2c20  elf, *, db: Db, 
+00007470: 6375 723d 4e6f 6e65 2920 2d3e 2053 6861  cur=None) -> Sha
+00007480: 3147 6974 3a0a 2020 2020 2020 2020 7265  1Git:.        re
+00007490: 7475 726e 2064 622e 7265 7669 7369 6f6e  turn db.revision
+000074a0: 5f67 6574 5f72 616e 646f 6d28 6375 7229  _get_random(cur)
+000074b0: 0a0a 2020 2020 2323 2323 2323 2323 2323  ..    ##########
+000074c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000074d0: 0a20 2020 2023 2045 7874 4944 0a20 2020  .    # ExtID.   
+000074e0: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
+000074f0: 2323 2323 2323 2323 2323 230a 0a20 2020  ###########..   
+00007500: 2040 6462 5f74 7261 6e73 6163 7469 6f6e   @db_transaction
+00007510: 2829 0a20 2020 2064 6566 2065 7874 6964  ().    def extid
+00007520: 5f67 6574 5f66 726f 6d5f 6578 7469 6428  _get_from_extid(
+00007530: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00007540: 2020 2020 2020 2069 645f 7479 7065 3a20         id_type: 
+00007550: 7374 722c 0a20 2020 2020 2020 2069 6473  str,.        ids
+00007560: 3a20 4c69 7374 5b62 7974 6573 5d2c 0a20  : List[bytes],. 
+00007570: 2020 2020 2020 2076 6572 7369 6f6e 3a20         version: 
+00007580: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+00007590: 4e6f 6e65 2c0a 2020 2020 2020 2020 2a2c  None,.        *,
+000075a0: 0a20 2020 2020 2020 2064 623a 2044 622c  .        db: Db,
+000075b0: 0a20 2020 2020 2020 2063 7572 3d4e 6f6e  .        cur=Non
+000075c0: 652c 0a20 2020 2029 202d 3e20 4c69 7374  e,.    ) -> List
+000075d0: 5b45 7874 4944 5d3a 0a20 2020 2020 2020  [ExtID]:.       
+000075e0: 2065 7874 6964 7320 3d20 5b5d 0a20 2020   extids = [].   
+000075f0: 2020 2020 2066 6f72 2072 6f77 2069 6e20       for row in 
+00007600: 6462 2e65 7874 6964 5f67 6574 5f66 726f  db.extid_get_fro
+00007610: 6d5f 6578 7469 645f 6c69 7374 2869 645f  m_extid_list(id_
+00007620: 7479 7065 2c20 6964 732c 2076 6572 7369  type, ids, versi
+00007630: 6f6e 3d76 6572 7369 6f6e 2c20 6375 723d  on=version, cur=
+00007640: 6375 7229 3a0a 2020 2020 2020 2020 2020  cur):.          
+00007650: 2020 6966 2072 6f77 5b30 5d20 6973 206e    if row[0] is n
+00007660: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00007670: 2020 2020 2020 2020 2065 7874 6964 732e           extids.
+00007680: 6170 7065 6e64 2863 6f6e 7665 7274 6572  append(converter
+00007690: 732e 6462 5f74 6f5f 6578 7469 6428 6469  s.db_to_extid(di
+000076a0: 6374 287a 6970 2864 622e 6578 7469 645f  ct(zip(db.extid_
+000076b0: 636f 6c73 2c20 726f 7729 2929 290a 2020  cols, row)))).  
+000076c0: 2020 2020 2020 7265 7475 726e 2065 7874        return ext
+000076d0: 6964 730a 0a20 2020 2040 6462 5f74 7261  ids..    @db_tra
+000076e0: 6e73 6163 7469 6f6e 2829 0a20 2020 2064  nsaction().    d
+000076f0: 6566 2065 7874 6964 5f67 6574 5f66 726f  ef extid_get_fro
+00007700: 6d5f 7461 7267 6574 280a 2020 2020 2020  m_target(.      
+00007710: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00007720: 7461 7267 6574 5f74 7970 653a 204f 626a  target_type: Obj
+00007730: 6563 7454 7970 652c 0a20 2020 2020 2020  ectType,.       
+00007740: 2069 6473 3a20 4c69 7374 5b53 6861 3147   ids: List[Sha1G
+00007750: 6974 5d2c 0a20 2020 2020 2020 2065 7874  it],.        ext
+00007760: 6964 5f74 7970 653a 204f 7074 696f 6e61  id_type: Optiona
+00007770: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
+00007780: 2020 2020 2020 2065 7874 6964 5f76 6572         extid_ver
+00007790: 7369 6f6e 3a20 4f70 7469 6f6e 616c 5b69  sion: Optional[i
+000077a0: 6e74 5d20 3d20 4e6f 6e65 2c0a 2020 2020  nt] = None,.    
+000077b0: 2020 2020 2a2c 0a20 2020 2020 2020 2064      *,.        d
+000077c0: 623a 2044 622c 0a20 2020 2020 2020 2063  b: Db,.        c
+000077d0: 7572 3d4e 6f6e 652c 0a20 2020 2029 202d  ur=None,.    ) -
+000077e0: 3e20 4c69 7374 5b45 7874 4944 5d3a 0a20  > List[ExtID]:. 
+000077f0: 2020 2020 2020 2065 7874 6964 7320 3d20         extids = 
+00007800: 5b5d 0a20 2020 2020 2020 2069 6620 2865  [].        if (e
+00007810: 7874 6964 5f76 6572 7369 6f6e 2069 7320  xtid_version is 
+00007820: 6e6f 7420 4e6f 6e65 2061 6e64 2065 7874  not None and ext
+00007830: 6964 5f74 7970 6520 6973 204e 6f6e 6529  id_type is None)
+00007840: 206f 7220 280a 2020 2020 2020 2020 2020   or (.          
+00007850: 2020 6578 7469 645f 7665 7273 696f 6e20    extid_version 
+00007860: 6973 204e 6f6e 6520 616e 6420 6578 7469  is None and exti
+00007870: 645f 7479 7065 2069 7320 6e6f 7420 4e6f  d_type is not No
+00007880: 6e65 0a20 2020 2020 2020 2029 3a0a 2020  ne.        ):.  
+00007890: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000078a0: 5661 6c75 6545 7272 6f72 2822 596f 7520  ValueError("You 
+000078b0: 6d75 7374 2070 726f 7669 6465 2062 6f74  must provide bot
+000078c0: 6820 6578 7469 645f 7479 7065 2061 6e64  h extid_type and
+000078d0: 2065 7874 6964 5f76 6572 7369 6f6e 2229   extid_version")
+000078e0: 0a0a 2020 2020 2020 2020 666f 7220 726f  ..        for ro
+000078f0: 7720 696e 2064 622e 6578 7469 645f 6765  w in db.extid_ge
+00007900: 745f 6672 6f6d 5f73 7768 6964 5f6c 6973  t_from_swhid_lis
+00007910: 7428 0a20 2020 2020 2020 2020 2020 2074  t(.            t
+00007920: 6172 6765 745f 7479 7065 2e76 616c 7565  arget_type.value
+00007930: 2c0a 2020 2020 2020 2020 2020 2020 6964  ,.            id
+00007940: 732c 0a20 2020 2020 2020 2020 2020 2065  s,.            e
+00007950: 7874 6964 5f76 6572 7369 6f6e 3d65 7874  xtid_version=ext
+00007960: 6964 5f76 6572 7369 6f6e 2c0a 2020 2020  id_version,.    
+00007970: 2020 2020 2020 2020 6578 7469 645f 7479          extid_ty
+00007980: 7065 3d65 7874 6964 5f74 7970 652c 0a20  pe=extid_type,. 
+00007990: 2020 2020 2020 2020 2020 2063 7572 3d63             cur=c
+000079a0: 7572 2c0a 2020 2020 2020 2020 293a 0a20  ur,.        ):. 
+000079b0: 2020 2020 2020 2020 2020 2069 6620 726f             if ro
+000079c0: 775b 305d 2069 7320 6e6f 7420 4e6f 6e65  w[0] is not None
+000079d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000079e0: 2020 6578 7469 6473 2e61 7070 656e 6428    extids.append(
+000079f0: 636f 6e76 6572 7465 7273 2e64 625f 746f  converters.db_to
+00007a00: 5f65 7874 6964 2864 6963 7428 7a69 7028  _extid(dict(zip(
+00007a10: 6462 2e65 7874 6964 5f63 6f6c 732c 2072  db.extid_cols, r
+00007a20: 6f77 2929 2929 0a20 2020 2020 2020 2072  ow)))).        r
+00007a30: 6574 7572 6e20 6578 7469 6473 0a0a 2020  eturn extids..  
+00007a40: 2020 4064 625f 7472 616e 7361 6374 696f    @db_transactio
+00007a50: 6e28 290a 2020 2020 6465 6620 6578 7469  n().    def exti
+00007a60: 645f 6164 6428 7365 6c66 2c20 6964 733a  d_add(self, ids:
+00007a70: 204c 6973 745b 4578 7449 445d 2c20 2a2c   List[ExtID], *,
+00007a80: 2064 623a 2044 622c 2063 7572 3d4e 6f6e   db: Db, cur=Non
+00007a90: 6529 202d 3e20 4469 6374 5b73 7472 2c20  e) -> Dict[str, 
+00007aa0: 696e 745d 3a0a 2020 2020 2020 2020 6578  int]:.        ex
+00007ab0: 7469 6420 3d20 5b0a 2020 2020 2020 2020  tid = [.        
+00007ac0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+00007ad0: 2020 2020 2020 2265 7874 6964 223a 2065        "extid": e
+00007ae0: 7874 6964 2e65 7874 6964 2c0a 2020 2020  xtid.extid,.    
+00007af0: 2020 2020 2020 2020 2020 2020 2265 7874              "ext
+00007b00: 6964 5f74 7970 6522 3a20 6578 7469 642e  id_type": extid.
+00007b10: 6578 7469 645f 7479 7065 2c0a 2020 2020  extid_type,.    
+00007b20: 2020 2020 2020 2020 2020 2020 2265 7874              "ext
+00007b30: 6964 5f76 6572 7369 6f6e 223a 2067 6574  id_version": get
+00007b40: 6174 7472 2865 7874 6964 2c20 2265 7874  attr(extid, "ext
+00007b50: 6964 5f76 6572 7369 6f6e 222c 2030 292c  id_version", 0),
+00007b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007b70: 2022 7461 7267 6574 223a 2065 7874 6964   "target": extid
+00007b80: 2e74 6172 6765 742e 6f62 6a65 6374 5f69  .target.object_i
+00007b90: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
+00007ba0: 2020 2022 7461 7267 6574 5f74 7970 6522     "target_type"
+00007bb0: 3a20 6578 7469 642e 7461 7267 6574 2e6f  : extid.target.o
+00007bc0: 626a 6563 745f 7479 7065 2e6e 616d 652e  bject_type.name.
+00007bd0: 6c6f 7765 7228 292c 2020 2320 6172 6768  lower(),  # argh
+00007be0: 680a 2020 2020 2020 2020 2020 2020 7d0a  h.            }.
+00007bf0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00007c00: 6578 7469 6420 696e 2069 6473 0a20 2020  extid in ids.   
+00007c10: 2020 2020 205d 0a20 2020 2020 2020 2064       ].        d
+00007c20: 622e 6d6b 7465 6d70 2822 6578 7469 6422  b.mktemp("extid"
+00007c30: 2c20 6375 7229 0a0a 2020 2020 2020 2020  , cur)..        
+00007c40: 7365 6c66 2e6a 6f75 726e 616c 5f77 7269  self.journal_wri
+00007c50: 7465 722e 6578 7469 645f 6164 6428 6964  ter.extid_add(id
+00007c60: 7329 0a0a 2020 2020 2020 2020 6462 2e63  s)..        db.c
+00007c70: 6f70 795f 746f 2865 7874 6964 2c20 2274  opy_to(extid, "t
+00007c80: 6d70 5f65 7874 6964 222c 2064 622e 6578  mp_extid", db.ex
+00007c90: 7469 645f 636f 6c73 2c20 6375 7229 0a0a  tid_cols, cur)..
+00007ca0: 2020 2020 2020 2020 2320 6d6f 7665 206d          # move m
+00007cb0: 6574 6164 6174 6120 696e 2070 6c61 6365  etadata in place
+00007cc0: 0a20 2020 2020 2020 2064 622e 6578 7469  .        db.exti
+00007cd0: 645f 6164 645f 6672 6f6d 5f74 656d 7028  d_add_from_temp(
+00007ce0: 6375 7229 0a0a 2020 2020 2020 2020 7265  cur)..        re
+00007cf0: 7475 726e 207b 2265 7874 6964 3a61 6464  turn {"extid:add
+00007d00: 223a 206c 656e 2865 7874 6964 297d 0a0a  ": len(extid)}..
+00007d10: 2020 2020 2323 2323 2323 2323 2323 2323      ############
+00007d20: 2323 2323 2323 2323 2323 2323 2323 0a20  ##############. 
+00007d30: 2020 2023 2052 656c 6561 7365 0a20 2020     # Release.   
+00007d40: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
+00007d50: 2323 2323 2323 2323 2323 230a 0a20 2020  ###########..   
+00007d60: 2040 6462 5f74 7261 6e73 6163 7469 6f6e   @db_transaction
+00007d70: 2829 0a20 2020 2064 6566 2072 656c 6561  ().    def relea
+00007d80: 7365 5f61 6464 280a 2020 2020 2020 2020  se_add(.        
+00007d90: 7365 6c66 2c20 7265 6c65 6173 6573 3a20  self, releases: 
+00007da0: 4c69 7374 5b52 656c 6561 7365 5d2c 202a  List[Release], *
+00007db0: 2c20 6462 3a20 4462 2c20 6375 723d 4e6f  , db: Db, cur=No
+00007dc0: 6e65 0a20 2020 2029 202d 3e20 4469 6374  ne.    ) -> Dict
+00007dd0: 5b73 7472 2c20 696e 745d 3a0a 2020 2020  [str, int]:.    
+00007de0: 2020 2020 7375 6d6d 6172 7920 3d20 7b22      summary = {"
+00007df0: 7265 6c65 6173 653a 6164 6422 3a20 307d  release:add": 0}
+00007e00: 0a0a 2020 2020 2020 2020 7265 6c65 6173  ..        releas
+00007e10: 655f 6964 7320 3d20 7365 7428 7265 6c65  e_ids = set(rele
+00007e20: 6173 652e 6964 2066 6f72 2072 656c 6561  ase.id for relea
+00007e30: 7365 2069 6e20 7265 6c65 6173 6573 290a  se in releases).
+00007e40: 2020 2020 2020 2020 7265 6c65 6173 6573          releases
+00007e50: 5f6d 6973 7369 6e67 203d 2073 6574 2873  _missing = set(s
+00007e60: 656c 662e 7265 6c65 6173 655f 6d69 7373  elf.release_miss
+00007e70: 696e 6728 7265 6c65 6173 655f 6964 732c  ing(release_ids,
+00007e80: 2064 623d 6462 2c20 6375 723d 6375 7229   db=db, cur=cur)
+00007e90: 290a 0a20 2020 2020 2020 2069 6620 6e6f  )..        if no
+00007ea0: 7420 7265 6c65 6173 6573 5f6d 6973 7369  t releases_missi
+00007eb0: 6e67 3a0a 2020 2020 2020 2020 2020 2020  ng:.            
+00007ec0: 7265 7475 726e 2073 756d 6d61 7279 0a0a  return summary..
+00007ed0: 2020 2020 2020 2020 6462 2e6d 6b74 656d          db.mktem
+00007ee0: 705f 7265 6c65 6173 6528 6375 7229 0a0a  p_release(cur)..
+00007ef0: 2020 2020 2020 2020 7265 6c65 6173 6573          releases
+00007f00: 5f66 696c 7465 7265 6420 3d20 5b0a 2020  _filtered = [.  
+00007f10: 2020 2020 2020 2020 2020 7265 6c65 6173            releas
+00007f20: 6520 666f 7220 7265 6c65 6173 6520 696e  e for release in
+00007f30: 2072 656c 6561 7365 7320 6966 2072 656c   releases if rel
+00007f40: 6561 7365 2e69 6420 696e 2072 656c 6561  ease.id in relea
+00007f50: 7365 735f 6d69 7373 696e 670a 2020 2020  ses_missing.    
+00007f60: 2020 2020 5d0a 0a20 2020 2020 2020 2073      ]..        s
+00007f70: 656c 662e 6a6f 7572 6e61 6c5f 7772 6974  elf.journal_writ
+00007f80: 6572 2e72 656c 6561 7365 5f61 6464 2872  er.release_add(r
+00007f90: 656c 6561 7365 735f 6669 6c74 6572 6564  eleases_filtered
+00007fa0: 290a 0a20 2020 2020 2020 2064 625f 7265  )..        db_re
+00007fb0: 6c65 6173 6573 5f66 696c 7465 7265 6420  leases_filtered 
+00007fc0: 3d20 6c69 7374 286d 6170 2863 6f6e 7665  = list(map(conve
+00007fd0: 7274 6572 732e 7265 6c65 6173 655f 746f  rters.release_to
+00007fe0: 5f64 622c 2072 656c 6561 7365 735f 6669  _db, releases_fi
+00007ff0: 6c74 6572 6564 2929 0a0a 2020 2020 2020  ltered))..      
+00008000: 2020 7769 7468 2063 6f6e 7665 7274 5f76    with convert_v
+00008010: 616c 6964 6174 696f 6e5f 6578 6365 7074  alidation_except
+00008020: 696f 6e73 2829 3a0a 2020 2020 2020 2020  ions():.        
+00008030: 2020 2020 6462 2e63 6f70 795f 746f 2864      db.copy_to(d
+00008040: 625f 7265 6c65 6173 6573 5f66 696c 7465  b_releases_filte
+00008050: 7265 642c 2022 746d 705f 7265 6c65 6173  red, "tmp_releas
+00008060: 6522 2c20 6462 2e72 656c 6561 7365 5f61  e", db.release_a
+00008070: 6464 5f63 6f6c 732c 2063 7572 290a 0a20  dd_cols, cur).. 
+00008080: 2020 2020 2020 2020 2020 2064 622e 7265             db.re
+00008090: 6c65 6173 655f 6164 645f 6672 6f6d 5f74  lease_add_from_t
+000080a0: 656d 7028 6375 7229 0a0a 2020 2020 2020  emp(cur)..      
+000080b0: 2020 7265 7475 726e 207b 2272 656c 6561    return {"relea
+000080c0: 7365 3a61 6464 223a 206c 656e 2872 656c  se:add": len(rel
+000080d0: 6561 7365 735f 6d69 7373 696e 6729 7d0a  eases_missing)}.
+000080e0: 0a20 2020 2040 6462 5f74 7261 6e73 6163  .    @db_transac
+000080f0: 7469 6f6e 5f67 656e 6572 6174 6f72 2829  tion_generator()
+00008100: 0a20 2020 2064 6566 2072 656c 6561 7365  .    def release
+00008110: 5f6d 6973 7369 6e67 280a 2020 2020 2020  _missing(.      
+00008120: 2020 7365 6c66 2c20 7265 6c65 6173 6573    self, releases
+00008130: 3a20 4c69 7374 5b53 6861 3147 6974 5d2c  : List[Sha1Git],
+00008140: 202a 2c20 6462 3a20 4462 2c20 6375 723d   *, db: Db, cur=
+00008150: 4e6f 6e65 0a20 2020 2029 202d 3e20 4974  None.    ) -> It
+00008160: 6572 6162 6c65 5b53 6861 3147 6974 5d3a  erable[Sha1Git]:
+00008170: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00008180: 7265 6c65 6173 6573 3a0a 2020 2020 2020  releases:.      
+00008190: 2020 2020 2020 7265 7475 726e 0a0a 2020        return..  
+000081a0: 2020 2020 2020 666f 7220 6f62 6a20 696e        for obj in
+000081b0: 2064 622e 7265 6c65 6173 655f 6d69 7373   db.release_miss
+000081c0: 696e 675f 6672 6f6d 5f6c 6973 7428 7265  ing_from_list(re
+000081d0: 6c65 6173 6573 2c20 6375 7229 3a0a 2020  leases, cur):.  
+000081e0: 2020 2020 2020 2020 2020 7969 656c 6420            yield 
+000081f0: 6f62 6a5b 305d 0a0a 2020 2020 4064 625f  obj[0]..    @db_
+00008200: 7472 616e 7361 6374 696f 6e28 7374 6174  transaction(stat
+00008210: 656d 656e 745f 7469 6d65 6f75 743d 3130  ement_timeout=10
+00008220: 3030 290a 2020 2020 6465 6620 7265 6c65  00).    def rele
+00008230: 6173 655f 6765 7428 0a20 2020 2020 2020  ase_get(.       
+00008240: 2073 656c 662c 0a20 2020 2020 2020 2072   self,.        r
+00008250: 656c 6561 7365 733a 204c 6973 745b 5368  eleases: List[Sh
+00008260: 6131 4769 745d 2c0a 2020 2020 2020 2020  a1Git],.        
+00008270: 6967 6e6f 7265 5f64 6973 706c 6179 6e61  ignore_displayna
+00008280: 6d65 3a20 626f 6f6c 203d 2046 616c 7365  me: bool = False
+00008290: 2c0a 2020 2020 2020 2020 2a2c 0a20 2020  ,.        *,.   
+000082a0: 2020 2020 2064 623a 2044 622c 0a20 2020       db: Db,.   
+000082b0: 2020 2020 2063 7572 3d4e 6f6e 652c 0a20       cur=None,. 
+000082c0: 2020 2029 202d 3e20 4c69 7374 5b4f 7074     ) -> List[Opt
+000082d0: 696f 6e61 6c5b 5265 6c65 6173 655d 5d3a  ional[Release]]:
+000082e0: 0a20 2020 2020 2020 2072 656c 7320 3d20  .        rels = 
+000082f0: 5b5d 0a20 2020 2020 2020 2066 6f72 2072  [].        for r
+00008300: 656c 6561 7365 2069 6e20 6462 2e72 656c  elease in db.rel
+00008310: 6561 7365 5f67 6574 5f66 726f 6d5f 6c69  ease_get_from_li
+00008320: 7374 2872 656c 6561 7365 732c 2069 676e  st(releases, ign
+00008330: 6f72 655f 6469 7370 6c61 796e 616d 652c  ore_displayname,
+00008340: 2063 7572 293a 0a20 2020 2020 2020 2020   cur):.         
+00008350: 2020 2072 656c 203d 2063 6f6e 7665 7274     rel = convert
+00008360: 6572 732e 6462 5f74 6f5f 6f70 7469 6f6e  ers.db_to_option
+00008370: 616c 5f72 656c 6561 7365 280a 2020 2020  al_release(.    
+00008380: 2020 2020 2020 2020 2020 2020 6469 6374              dict
+00008390: 287a 6970 2864 622e 7265 6c65 6173 655f  (zip(db.release_
+000083a0: 6765 745f 636f 6c73 2c20 7265 6c65 6173  get_cols, releas
+000083b0: 6529 290a 2020 2020 2020 2020 2020 2020  e)).            
+000083c0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+000083d0: 6c73 2e61 7070 656e 6428 7265 6c29 0a20  ls.append(rel). 
+000083e0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+000083f0: 6c73 0a0a 2020 2020 4064 625f 7472 616e  ls..    @db_tran
+00008400: 7361 6374 696f 6e28 290a 2020 2020 6465  saction().    de
+00008410: 6620 7265 6c65 6173 655f 6765 745f 7061  f release_get_pa
+00008420: 7274 6974 696f 6e28 0a20 2020 2020 2020  rtition(.       
+00008430: 2073 656c 662c 0a20 2020 2020 2020 2070   self,.        p
+00008440: 6172 7469 7469 6f6e 5f69 643a 2069 6e74  artition_id: int
+00008450: 2c0a 2020 2020 2020 2020 6e62 5f70 6172  ,.        nb_par
+00008460: 7469 7469 6f6e 733a 2069 6e74 2c0a 2020  titions: int,.  
+00008470: 2020 2020 2020 7061 6765 5f74 6f6b 656e        page_token
+00008480: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+00008490: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+000084a0: 6c69 6d69 743a 2069 6e74 203d 2031 3030  limit: int = 100
+000084b0: 302c 0a20 2020 2020 2020 202a 2c0a 2020  0,.        *,.  
+000084c0: 2020 2020 2020 6462 3a20 4462 2c0a 2020        db: Db,.  
+000084d0: 2020 2020 2020 6375 723d 4e6f 6e65 2c0a        cur=None,.
+000084e0: 2020 2020 2920 2d3e 2050 6167 6564 5265      ) -> PagedRe
+000084f0: 7375 6c74 5b52 656c 6561 7365 5d3a 0a20  sult[Release]:. 
+00008500: 2020 2020 2020 2072 6574 7572 6e20 5f67         return _g
+00008510: 6574 5f70 6167 696e 6174 6564 5f73 6861  et_paginated_sha
+00008520: 315f 7061 7274 6974 696f 6e28 0a20 2020  1_partition(.   
+00008530: 2020 2020 2020 2020 2063 7572 2c0a 2020           cur,.  
+00008540: 2020 2020 2020 2020 2020 7061 7274 6974            partit
+00008550: 696f 6e5f 6964 2c0a 2020 2020 2020 2020  ion_id,.        
+00008560: 2020 2020 6e62 5f70 6172 7469 7469 6f6e      nb_partition
+00008570: 732c 0a20 2020 2020 2020 2020 2020 2070  s,.            p
+00008580: 6167 655f 746f 6b65 6e2c 0a20 2020 2020  age_token,.     
+00008590: 2020 2020 2020 206c 696d 6974 2c0a 2020         limit,.  
+000085a0: 2020 2020 2020 2020 2020 6462 2e72 656c            db.rel
+000085b0: 6561 7365 5f67 6574 5f72 616e 6765 2c0a  ease_get_range,.
+000085c0: 2020 2020 2020 2020 2020 2020 6c61 6d62              lamb
+000085d0: 6461 2072 6f77 3a20 636f 6e76 6572 7465  da row: converte
+000085e0: 7273 2e64 625f 746f 5f72 656c 6561 7365  rs.db_to_release
+000085f0: 2864 6963 7428 7a69 7028 6462 2e72 656c  (dict(zip(db.rel
+00008600: 6561 7365 5f67 6574 5f63 6f6c 732c 2072  ease_get_cols, r
+00008610: 6f77 2929 292c 0a20 2020 2020 2020 2029  ow))),.        )
+00008620: 0a0a 2020 2020 4064 625f 7472 616e 7361  ..    @db_transa
+00008630: 6374 696f 6e28 290a 2020 2020 6465 6620  ction().    def 
+00008640: 7265 6c65 6173 655f 6765 745f 7261 6e64  release_get_rand
+00008650: 6f6d 2873 656c 662c 202a 2c20 6462 3a20  om(self, *, db: 
+00008660: 4462 2c20 6375 723d 4e6f 6e65 2920 2d3e  Db, cur=None) ->
+00008670: 2053 6861 3147 6974 3a0a 2020 2020 2020   Sha1Git:.      
+00008680: 2020 7265 7475 726e 2064 622e 7265 6c65    return db.rele
+00008690: 6173 655f 6765 745f 7261 6e64 6f6d 2863  ase_get_random(c
+000086a0: 7572 290a 0a20 2020 2023 2323 2323 2323  ur)..    #######
+000086b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000086c0: 2323 230a 2020 2020 2320 536e 6170 7368  ###.    # Snapsh
+000086d0: 6f74 0a20 2020 2023 2323 2323 2323 2323  ot.    #########
+000086e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000086f0: 230a 0a20 2020 2040 6462 5f74 7261 6e73  #..    @db_trans
+00008700: 6163 7469 6f6e 2829 0a20 2020 2064 6566  action().    def
+00008710: 2073 6e61 7073 686f 745f 6164 6428 0a20   snapshot_add(. 
+00008720: 2020 2020 2020 2073 656c 662c 2073 6e61         self, sna
+00008730: 7073 686f 7473 3a20 4c69 7374 5b53 6e61  pshots: List[Sna
+00008740: 7073 686f 745d 2c20 2a2c 2064 623a 2044  pshot], *, db: D
+00008750: 622c 2063 7572 3d4e 6f6e 650a 2020 2020  b, cur=None.    
+00008760: 2920 2d3e 2044 6963 745b 7374 722c 2069  ) -> Dict[str, i
+00008770: 6e74 5d3a 0a20 2020 2020 2020 2063 7265  nt]:.        cre
+00008780: 6174 6564 5f74 656d 705f 7461 626c 6520  ated_temp_table 
+00008790: 3d20 4661 6c73 650a 0a20 2020 2020 2020  = False..       
+000087a0: 2063 6f75 6e74 203d 2030 0a20 2020 2020   count = 0.     
+000087b0: 2020 2066 6f72 2073 6e61 7073 686f 7420     for snapshot 
+000087c0: 696e 2073 6e61 7073 686f 7473 3a0a 2020  in snapshots:.  
+000087d0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+000087e0: 2064 622e 736e 6170 7368 6f74 5f65 7869   db.snapshot_exi
+000087f0: 7374 7328 736e 6170 7368 6f74 2e69 642c  sts(snapshot.id,
+00008800: 2063 7572 293a 0a20 2020 2020 2020 2020   cur):.         
+00008810: 2020 2020 2020 2069 6620 6e6f 7420 6372         if not cr
+00008820: 6561 7465 645f 7465 6d70 5f74 6162 6c65  eated_temp_table
+00008830: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00008840: 2020 2020 2020 6462 2e6d 6b74 656d 705f        db.mktemp_
+00008850: 736e 6170 7368 6f74 5f62 7261 6e63 6828  snapshot_branch(
+00008860: 6375 7229 0a20 2020 2020 2020 2020 2020  cur).           
+00008870: 2020 2020 2020 2020 2063 7265 6174 6564           created
+00008880: 5f74 656d 705f 7461 626c 6520 3d20 5472  _temp_table = Tr
+00008890: 7565 0a0a 2020 2020 2020 2020 2020 2020  ue..            
+000088a0: 2020 2020 7769 7468 2063 6f6e 7665 7274      with convert
+000088b0: 5f76 616c 6964 6174 696f 6e5f 6578 6365  _validation_exce
+000088c0: 7074 696f 6e73 2829 3a0a 2020 2020 2020  ptions():.      
+000088d0: 2020 2020 2020 2020 2020 2020 2020 6462                db
+000088e0: 2e63 6f70 795f 746f 280a 2020 2020 2020  .copy_to(.      
+000088f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008900: 2020 280a 2020 2020 2020 2020 2020 2020    (.            
+00008910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008920: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00008930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008940: 2020 226e 616d 6522 3a20 6e61 6d65 2c0a    "name": name,.
 00008950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008960: 2020 2020 2020 2020 2274 6172 6765 7422          "target"
-00008970: 3a20 696e 666f 2e74 6172 6765 7420 6966  : info.target if
-00008980: 2069 6e66 6f20 656c 7365 204e 6f6e 652c   info else None,
-00008990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008970: 2274 6172 6765 7422 3a20 696e 666f 2e74  "target": info.t
+00008980: 6172 6765 7420 6966 2069 6e66 6f20 656c  arget if info el
+00008990: 7365 204e 6f6e 652c 0a20 2020 2020 2020  se None,.       
 000089a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089b0: 2022 7461 7267 6574 5f74 7970 6522 3a20   "target_type": 
-000089c0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000089b0: 2020 2020 2020 2020 2022 7461 7267 6574           "target
+000089c0: 5f74 7970 6522 3a20 280a 2020 2020 2020  _type": (.      
 000089d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089e0: 2020 2020 2020 696e 666f 2e74 6172 6765        info.targe
-000089f0: 745f 7479 7065 2e76 616c 7565 2069 6620  t_type.value if 
-00008a00: 696e 666f 2065 6c73 6520 4e6f 6e65 0a20  info else None. 
-00008a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a20: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00008a30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00008a40: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
-00008a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a60: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00008a70: 6e61 6d65 2c20 696e 666f 2069 6e20 736e  name, info in sn
-00008a80: 6170 7368 6f74 2e62 7261 6e63 6865 732e  apshot.branches.
-00008a90: 6974 656d 7328 290a 2020 2020 2020 2020  items().        
+000089e0: 2020 2020 2020 2020 2020 2020 2020 696e                in
+000089f0: 666f 2e74 6172 6765 745f 7479 7065 2e76  fo.target_type.v
+00008a00: 616c 7565 2069 6620 696e 666f 2065 6c73  alue if info els
+00008a10: 6520 4e6f 6e65 0a20 2020 2020 2020 2020  e None.         
+00008a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a30: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
+00008a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a50: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00008a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a70: 2020 2020 666f 7220 6e61 6d65 2c20 696e      for name, in
+00008a80: 666f 2069 6e20 736e 6170 7368 6f74 2e62  fo in snapshot.b
+00008a90: 7261 6e63 6865 732e 6974 656d 7328 290a  ranches.items().
 00008aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ab0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00008ac0: 2020 2020 2020 2020 2020 2022 746d 705f             "tmp_
-00008ad0: 736e 6170 7368 6f74 5f62 7261 6e63 6822  snapshot_branch"
-00008ae0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00008af0: 2020 2020 2020 2020 2020 5b22 6e61 6d65            ["name
-00008b00: 222c 2022 7461 7267 6574 222c 2022 7461  ", "target", "ta
-00008b10: 7267 6574 5f74 7970 6522 5d2c 0a20 2020  rget_type"],.   
-00008b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b30: 2020 2020 2063 7572 2c0a 2020 2020 2020       cur,.      
-00008b40: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00008b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008b60: 2073 656c 662e 6a6f 7572 6e61 6c5f 7772   self.journal_wr
-00008b70: 6974 6572 2e73 6e61 7073 686f 745f 6164  iter.snapshot_ad
-00008b80: 6428 5b73 6e61 7073 686f 745d 290a 0a20  d([snapshot]).. 
-00008b90: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00008ba0: 622e 736e 6170 7368 6f74 5f61 6464 2873  b.snapshot_add(s
-00008bb0: 6e61 7073 686f 742e 6964 2c20 6375 7229  napshot.id, cur)
-00008bc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008bd0: 2063 6f75 6e74 202b 3d20 310a 0a20 2020   count += 1..   
-00008be0: 2020 2020 2072 6574 7572 6e20 7b22 736e       return {"sn
-00008bf0: 6170 7368 6f74 3a61 6464 223a 2063 6f75  apshot:add": cou
-00008c00: 6e74 7d0a 0a20 2020 2040 6462 5f74 7261  nt}..    @db_tra
-00008c10: 6e73 6163 7469 6f6e 5f67 656e 6572 6174  nsaction_generat
-00008c20: 6f72 2829 0a20 2020 2064 6566 2073 6e61  or().    def sna
-00008c30: 7073 686f 745f 6d69 7373 696e 6728 0a20  pshot_missing(. 
-00008c40: 2020 2020 2020 2073 656c 662c 2073 6e61         self, sna
-00008c50: 7073 686f 7473 3a20 4c69 7374 5b53 6861  pshots: List[Sha
-00008c60: 3147 6974 5d2c 202a 2c20 6462 3a20 4462  1Git], *, db: Db
-00008c70: 2c20 6375 723d 4e6f 6e65 0a20 2020 2029  , cur=None.    )
-00008c80: 202d 3e20 4974 6572 6162 6c65 5b53 6861   -> Iterable[Sha
-00008c90: 3147 6974 5d3a 0a20 2020 2020 2020 2066  1Git]:.        f
-00008ca0: 6f72 206f 626a 2069 6e20 6462 2e73 6e61  or obj in db.sna
-00008cb0: 7073 686f 745f 6d69 7373 696e 675f 6672  pshot_missing_fr
-00008cc0: 6f6d 5f6c 6973 7428 736e 6170 7368 6f74  om_list(snapshot
-00008cd0: 732c 2063 7572 293a 0a20 2020 2020 2020  s, cur):.       
-00008ce0: 2020 2020 2079 6965 6c64 206f 626a 5b30       yield obj[0
-00008cf0: 5d0a 0a20 2020 2040 6462 5f74 7261 6e73  ]..    @db_trans
-00008d00: 6163 7469 6f6e 2873 7461 7465 6d65 6e74  action(statement
-00008d10: 5f74 696d 656f 7574 3d32 3030 3029 0a20  _timeout=2000). 
-00008d20: 2020 2064 6566 2073 6e61 7073 686f 745f     def snapshot_
-00008d30: 6765 7428 0a20 2020 2020 2020 2073 656c  get(.        sel
-00008d40: 662c 2073 6e61 7073 686f 745f 6964 3a20  f, snapshot_id: 
-00008d50: 5368 6131 4769 742c 202a 2c20 6462 3a20  Sha1Git, *, db: 
-00008d60: 4462 2c20 6375 723d 4e6f 6e65 0a20 2020  Db, cur=None.   
-00008d70: 2029 202d 3e20 4f70 7469 6f6e 616c 5b44   ) -> Optional[D
-00008d80: 6963 745b 7374 722c 2041 6e79 5d5d 3a0a  ict[str, Any]]:.
-00008d90: 2020 2020 2020 2020 6420 3d20 7365 6c66          d = self
-00008da0: 2e73 6e61 7073 686f 745f 6765 745f 6272  .snapshot_get_br
-00008db0: 616e 6368 6573 2873 6e61 7073 686f 745f  anches(snapshot_
-00008dc0: 6964 290a 2020 2020 2020 2020 6966 2064  id).        if d
-00008dd0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00008de0: 2020 2020 2020 7265 7475 726e 2064 0a20        return d. 
-00008df0: 2020 2020 2020 2072 6574 7572 6e20 7b0a         return {.
-00008e00: 2020 2020 2020 2020 2020 2020 2269 6422              "id"
-00008e10: 3a20 645b 2269 6422 5d2c 0a20 2020 2020  : d["id"],.     
-00008e20: 2020 2020 2020 2022 6272 616e 6368 6573         "branches
-00008e30: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-00008e40: 2020 2020 206e 616d 653a 2062 7261 6e63       name: branc
-00008e50: 682e 746f 5f64 6963 7428 2920 6966 2062  h.to_dict() if b
-00008e60: 7261 6e63 6820 656c 7365 204e 6f6e 650a  ranch else None.
-00008e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e80: 666f 7220 286e 616d 652c 2062 7261 6e63  for (name, branc
-00008e90: 6829 2069 6e20 645b 2262 7261 6e63 6865  h) in d["branche
-00008ea0: 7322 5d2e 6974 656d 7328 290a 2020 2020  s"].items().    
-00008eb0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00008ec0: 2020 2020 2020 2022 6e65 7874 5f62 7261         "next_bra
-00008ed0: 6e63 6822 3a20 645b 226e 6578 745f 6272  nch": d["next_br
-00008ee0: 616e 6368 225d 2c0a 2020 2020 2020 2020  anch"],.        
-00008ef0: 7d0a 0a20 2020 2040 6462 5f74 7261 6e73  }..    @db_trans
-00008f00: 6163 7469 6f6e 2829 0a20 2020 2064 6566  action().    def
-00008f10: 2073 6e61 7073 686f 745f 6765 745f 6964   snapshot_get_id
-00008f20: 5f70 6172 7469 7469 6f6e 280a 2020 2020  _partition(.    
-00008f30: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-00008f40: 2020 7061 7274 6974 696f 6e5f 6964 3a20    partition_id: 
-00008f50: 696e 742c 0a20 2020 2020 2020 206e 625f  int,.        nb_
-00008f60: 7061 7274 6974 696f 6e73 3a20 696e 742c  partitions: int,
-00008f70: 0a20 2020 2020 2020 2070 6167 655f 746f  .        page_to
-00008f80: 6b65 6e3a 204f 7074 696f 6e61 6c5b 7374  ken: Optional[st
-00008f90: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-00008fa0: 2020 206c 696d 6974 3a20 696e 7420 3d20     limit: int = 
-00008fb0: 3130 3030 2c0a 2020 2020 2020 2020 2a2c  1000,.        *,
-00008fc0: 0a20 2020 2020 2020 2064 623a 2044 622c  .        db: Db,
-00008fd0: 0a20 2020 2020 2020 2063 7572 3d4e 6f6e  .        cur=Non
-00008fe0: 652c 0a20 2020 2029 202d 3e20 5061 6765  e,.    ) -> Page
-00008ff0: 6452 6573 756c 745b 5368 6131 4769 745d  dResult[Sha1Git]
-00009000: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00009010: 205f 6765 745f 7061 6769 6e61 7465 645f   _get_paginated_
-00009020: 7368 6131 5f70 6172 7469 7469 6f6e 280a  sha1_partition(.
-00009030: 2020 2020 2020 2020 2020 2020 6375 722c              cur,
-00009040: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
-00009050: 7469 7469 6f6e 5f69 642c 0a20 2020 2020  tition_id,.     
-00009060: 2020 2020 2020 206e 625f 7061 7274 6974         nb_partit
-00009070: 696f 6e73 2c0a 2020 2020 2020 2020 2020  ions,.          
-00009080: 2020 7061 6765 5f74 6f6b 656e 2c0a 2020    page_token,.  
-00009090: 2020 2020 2020 2020 2020 6c69 6d69 742c            limit,
-000090a0: 0a20 2020 2020 2020 2020 2020 2064 622e  .            db.
-000090b0: 736e 6170 7368 6f74 5f67 6574 5f69 645f  snapshot_get_id_
-000090c0: 7261 6e67 652c 0a20 2020 2020 2020 2020  range,.         
-000090d0: 2020 206f 7065 7261 746f 722e 6974 656d     operator.item
-000090e0: 6765 7474 6572 2830 292c 0a20 2020 2020  getter(0),.     
-000090f0: 2020 2020 2020 206c 616d 6264 6120 6964         lambda id
-00009100: 5f3a 2069 645f 2c0a 2020 2020 2020 2020  _: id_,.        
-00009110: 290a 0a20 2020 2040 6462 5f74 7261 6e73  )..    @db_trans
-00009120: 6163 7469 6f6e 2873 7461 7465 6d65 6e74  action(statement
-00009130: 5f74 696d 656f 7574 3d32 3030 3029 0a20  _timeout=2000). 
-00009140: 2020 2064 6566 2073 6e61 7073 686f 745f     def snapshot_
-00009150: 636f 756e 745f 6272 616e 6368 6573 280a  count_branches(.
-00009160: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-00009170: 2020 2020 2020 736e 6170 7368 6f74 5f69        snapshot_i
-00009180: 643a 2053 6861 3147 6974 2c0a 2020 2020  d: Sha1Git,.    
-00009190: 2020 2020 6272 616e 6368 5f6e 616d 655f      branch_name_
-000091a0: 6578 636c 7564 655f 7072 6566 6978 3a20  exclude_prefix: 
-000091b0: 4f70 7469 6f6e 616c 5b62 7974 6573 5d20  Optional[bytes] 
-000091c0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-000091d0: 2a2c 0a20 2020 2020 2020 2064 623a 2044  *,.        db: D
-000091e0: 622c 0a20 2020 2020 2020 2063 7572 3d4e  b,.        cur=N
-000091f0: 6f6e 652c 0a20 2020 2029 202d 3e20 4f70  one,.    ) -> Op
-00009200: 7469 6f6e 616c 5b44 6963 745b 4f70 7469  tional[Dict[Opti
-00009210: 6f6e 616c 5b73 7472 5d2c 2069 6e74 5d5d  onal[str], int]]
-00009220: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00009230: 2064 6963 7428 0a20 2020 2020 2020 2020   dict(.         
-00009240: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
-00009250: 2020 2020 2062 630a 2020 2020 2020 2020       bc.        
-00009260: 2020 2020 2020 2020 666f 7220 6263 2069          for bc i
-00009270: 6e20 6462 2e73 6e61 7073 686f 745f 636f  n db.snapshot_co
-00009280: 756e 745f 6272 616e 6368 6573 280a 2020  unt_branches(.  
-00009290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000092a0: 2020 736e 6170 7368 6f74 5f69 642c 0a20    snapshot_id,. 
-000092b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000092c0: 2020 2062 7261 6e63 685f 6e61 6d65 5f65     branch_name_e
-000092d0: 7863 6c75 6465 5f70 7265 6669 782c 0a20  xclude_prefix,. 
-000092e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000092f0: 2020 2063 7572 2c0a 2020 2020 2020 2020     cur,.        
-00009300: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00009310: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
-00009320: 290a 0a20 2020 2040 6462 5f74 7261 6e73  )..    @db_trans
-00009330: 6163 7469 6f6e 2873 7461 7465 6d65 6e74  action(statement
-00009340: 5f74 696d 656f 7574 3d32 3030 3029 0a20  _timeout=2000). 
-00009350: 2020 2064 6566 2073 6e61 7073 686f 745f     def snapshot_
-00009360: 6765 745f 6272 616e 6368 6573 280a 2020  get_branches(.  
-00009370: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00009380: 2020 2020 736e 6170 7368 6f74 5f69 643a      snapshot_id:
-00009390: 2053 6861 3147 6974 2c0a 2020 2020 2020   Sha1Git,.      
-000093a0: 2020 6272 616e 6368 6573 5f66 726f 6d3a    branches_from:
-000093b0: 2062 7974 6573 203d 2062 2222 2c0a 2020   bytes = b"",.  
-000093c0: 2020 2020 2020 6272 616e 6368 6573 5f63        branches_c
-000093d0: 6f75 6e74 3a20 696e 7420 3d20 3130 3030  ount: int = 1000
-000093e0: 2c0a 2020 2020 2020 2020 7461 7267 6574  ,.        target
-000093f0: 5f74 7970 6573 3a20 4f70 7469 6f6e 616c  _types: Optional
-00009400: 5b4c 6973 745b 7374 725d 5d20 3d20 4e6f  [List[str]] = No
-00009410: 6e65 2c0a 2020 2020 2020 2020 6272 616e  ne,.        bran
-00009420: 6368 5f6e 616d 655f 696e 636c 7564 655f  ch_name_include_
-00009430: 7375 6273 7472 696e 673a 204f 7074 696f  substring: Optio
-00009440: 6e61 6c5b 6279 7465 735d 203d 204e 6f6e  nal[bytes] = Non
-00009450: 652c 0a20 2020 2020 2020 2062 7261 6e63  e,.        branc
-00009460: 685f 6e61 6d65 5f65 7863 6c75 6465 5f70  h_name_exclude_p
-00009470: 7265 6669 783a 204f 7074 696f 6e61 6c5b  refix: Optional[
-00009480: 6279 7465 735d 203d 204e 6f6e 652c 0a20  bytes] = None,. 
-00009490: 2020 2020 2020 202a 2c0a 2020 2020 2020         *,.      
-000094a0: 2020 6462 3a20 4462 2c0a 2020 2020 2020    db: Db,.      
-000094b0: 2020 6375 723d 4e6f 6e65 2c0a 2020 2020    cur=None,.    
-000094c0: 2920 2d3e 204f 7074 696f 6e61 6c5b 5061  ) -> Optional[Pa
-000094d0: 7274 6961 6c42 7261 6e63 6865 735d 3a0a  rtialBranches]:.
-000094e0: 2020 2020 2020 2020 6966 2073 6e61 7073          if snaps
-000094f0: 686f 745f 6964 203d 3d20 454d 5054 595f  hot_id == EMPTY_
-00009500: 534e 4150 5348 4f54 5f49 443a 0a20 2020  SNAPSHOT_ID:.   
-00009510: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00009520: 5061 7274 6961 6c42 7261 6e63 6865 7328  PartialBranches(
-00009530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009540: 2069 643d 736e 6170 7368 6f74 5f69 642c   id=snapshot_id,
-00009550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009560: 2062 7261 6e63 6865 733d 7b7d 2c0a 2020   branches={},.  
-00009570: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-00009580: 7874 5f62 7261 6e63 683d 4e6f 6e65 2c0a  xt_branch=None,.
-00009590: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-000095a0: 2020 2020 2020 2069 6620 6c69 7374 2873         if list(s
-000095b0: 656c 662e 736e 6170 7368 6f74 5f6d 6973  elf.snapshot_mis
-000095c0: 7369 6e67 285b 736e 6170 7368 6f74 5f69  sing([snapshot_i
-000095d0: 645d 2929 3a0a 2020 2020 2020 2020 2020  d])):.          
-000095e0: 2020 7265 7475 726e 204e 6f6e 650a 0a20    return None.. 
-000095f0: 2020 2020 2020 2062 7261 6e63 6865 7320         branches 
-00009600: 3d20 7b7d 0a20 2020 2020 2020 206e 6578  = {}.        nex
-00009610: 745f 6272 616e 6368 203d 204e 6f6e 650a  t_branch = None.
-00009620: 0a20 2020 2020 2020 2066 6574 6368 6564  .        fetched
-00009630: 5f62 7261 6e63 6865 7320 3d20 6c69 7374  _branches = list
-00009640: 280a 2020 2020 2020 2020 2020 2020 6462  (.            db
-00009650: 2e73 6e61 7073 686f 745f 6765 745f 6279  .snapshot_get_by
-00009660: 5f69 6428 0a20 2020 2020 2020 2020 2020  _id(.           
-00009670: 2020 2020 2073 6e61 7073 686f 745f 6964       snapshot_id
-00009680: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00009690: 2020 6272 616e 6368 6573 5f66 726f 6d3d    branches_from=
-000096a0: 6272 616e 6368 6573 5f66 726f 6d2c 0a20  branches_from,. 
-000096b0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-000096c0: 2074 6865 2075 6e64 6572 6c79 696e 6720   the underlying 
-000096d0: 5351 4c20 7175 6572 7920 6361 6e20 6265  SQL query can be
-000096e0: 2071 7569 7465 2065 7870 656e 7369 7665   quite expensive
-000096f0: 2074 6f20 6578 6563 7574 6520 666f 7220   to execute for 
-00009700: 736d 616c 6c0a 2020 2020 2020 2020 2020  small.          
-00009710: 2020 2020 2020 2320 6272 616e 6368 6573        # branches
-00009720: 5f63 6f75 6e74 2076 616c 7565 2c20 736f  _count value, so
-00009730: 2077 6520 656e 7375 7265 2061 206d 696e   we ensure a min
-00009740: 696d 756d 2062 7261 6e63 6865 7320 6c69  imum branches li
-00009750: 6d69 7420 6f66 2031 3020 666f 720a 2020  mit of 10 for.  
-00009760: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00009770: 6f70 7469 6d61 6c20 7065 7266 6f72 6d61  optimal performa
-00009780: 6e63 6573 0a20 2020 2020 2020 2020 2020  nces.           
-00009790: 2020 2020 2062 7261 6e63 6865 735f 636f       branches_co
-000097a0: 756e 743d 6d61 7828 6272 616e 6368 6573  unt=max(branches
-000097b0: 5f63 6f75 6e74 202b 2031 2c20 3130 292c  _count + 1, 10),
-000097c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000097d0: 2074 6172 6765 745f 7479 7065 733d 7461   target_types=ta
-000097e0: 7267 6574 5f74 7970 6573 2c0a 2020 2020  rget_types,.    
-000097f0: 2020 2020 2020 2020 2020 2020 6272 616e              bran
-00009800: 6368 5f6e 616d 655f 696e 636c 7564 655f  ch_name_include_
-00009810: 7375 6273 7472 696e 673d 6272 616e 6368  substring=branch
-00009820: 5f6e 616d 655f 696e 636c 7564 655f 7375  _name_include_su
-00009830: 6273 7472 696e 672c 0a20 2020 2020 2020  bstring,.       
-00009840: 2020 2020 2020 2020 2062 7261 6e63 685f           branch_
-00009850: 6e61 6d65 5f65 7863 6c75 6465 5f70 7265  name_exclude_pre
-00009860: 6669 783d 6272 616e 6368 5f6e 616d 655f  fix=branch_name_
-00009870: 6578 636c 7564 655f 7072 6566 6978 2c0a  exclude_prefix,.
-00009880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009890: 6375 723d 6375 722c 0a20 2020 2020 2020  cur=cur,.       
-000098a0: 2020 2020 2029 0a20 2020 2020 2020 2029       ).        )
-000098b0: 0a20 2020 2020 2020 2066 6f72 2072 6f77  .        for row
-000098c0: 2069 6e20 6665 7463 6865 645f 6272 616e   in fetched_bran
-000098d0: 6368 6573 5b3a 6272 616e 6368 6573 5f63  ches[:branches_c
-000098e0: 6f75 6e74 5d3a 0a20 2020 2020 2020 2020  ount]:.         
-000098f0: 2020 2062 7261 6e63 685f 6420 3d20 6469     branch_d = di
-00009900: 6374 287a 6970 2864 622e 736e 6170 7368  ct(zip(db.snapsh
-00009910: 6f74 5f67 6574 5f63 6f6c 732c 2072 6f77  ot_get_cols, row
-00009920: 2929 0a20 2020 2020 2020 2020 2020 2064  )).            d
-00009930: 656c 2062 7261 6e63 685f 645b 2273 6e61  el branch_d["sna
-00009940: 7073 686f 745f 6964 225d 0a20 2020 2020  pshot_id"].     
-00009950: 2020 2020 2020 206e 616d 6520 3d20 6272         name = br
-00009960: 616e 6368 5f64 2e70 6f70 2822 6e61 6d65  anch_d.pop("name
-00009970: 2229 0a20 2020 2020 2020 2020 2020 2069  ").            i
-00009980: 6620 6272 616e 6368 5f64 5b22 7461 7267  f branch_d["targ
-00009990: 6574 225d 2069 7320 4e6f 6e65 2061 6e64  et"] is None and
-000099a0: 2062 7261 6e63 685f 645b 2274 6172 6765   branch_d["targe
-000099b0: 745f 7479 7065 225d 2069 7320 4e6f 6e65  t_type"] is None
-000099c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000099d0: 2020 6272 616e 6368 203d 204e 6f6e 650a    branch = None.
-000099e0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-000099f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00009a00: 2020 6173 7365 7274 2062 7261 6e63 685f    assert branch_
-00009a10: 645b 2274 6172 6765 745f 7479 7065 225d  d["target_type"]
-00009a20: 2069 7320 6e6f 7420 4e6f 6e65 0a20 2020   is not None.   
-00009a30: 2020 2020 2020 2020 2020 2020 2062 7261               bra
-00009a40: 6e63 6820 3d20 536e 6170 7368 6f74 4272  nch = SnapshotBr
-00009a50: 616e 6368 280a 2020 2020 2020 2020 2020  anch(.          
-00009a60: 2020 2020 2020 2020 2020 7461 7267 6574            target
-00009a70: 3d62 7261 6e63 685f 645b 2274 6172 6765  =branch_d["targe
-00009a80: 7422 5d2c 0a20 2020 2020 2020 2020 2020  t"],.           
-00009a90: 2020 2020 2020 2020 2074 6172 6765 745f           target_
-00009aa0: 7479 7065 3d54 6172 6765 7454 7970 6528  type=TargetType(
-00009ab0: 6272 616e 6368 5f64 5b22 7461 7267 6574  branch_d["target
-00009ac0: 5f74 7970 6522 5d29 2c0a 2020 2020 2020  _type"]),.      
-00009ad0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00009ae0: 2020 2020 2020 2020 6272 616e 6368 6573          branches
-00009af0: 5b6e 616d 655d 203d 2062 7261 6e63 680a  [name] = branch.
-00009b00: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-00009b10: 6665 7463 6865 645f 6272 616e 6368 6573  fetched_branches
-00009b20: 2920 3e20 6272 616e 6368 6573 5f63 6f75  ) > branches_cou
-00009b30: 6e74 3a0a 2020 2020 2020 2020 2020 2020  nt:.            
-00009b40: 6e65 7874 5f62 7261 6e63 6820 3d20 6469  next_branch = di
-00009b50: 6374 280a 2020 2020 2020 2020 2020 2020  ct(.            
-00009b60: 2020 2020 7a69 7028 6462 2e73 6e61 7073      zip(db.snaps
-00009b70: 686f 745f 6765 745f 636f 6c73 2c20 6665  hot_get_cols, fe
-00009b80: 7463 6865 645f 6272 616e 6368 6573 5b62  tched_branches[b
-00009b90: 7261 6e63 6865 735f 636f 756e 745d 290a  ranches_count]).
-00009ba0: 2020 2020 2020 2020 2020 2020 295b 226e              )["n
-00009bb0: 616d 6522 5d0a 0a20 2020 2020 2020 2072  ame"]..        r
-00009bc0: 6574 7572 6e20 5061 7274 6961 6c42 7261  eturn PartialBra
-00009bd0: 6e63 6865 7328 0a20 2020 2020 2020 2020  nches(.         
-00009be0: 2020 2069 643d 736e 6170 7368 6f74 5f69     id=snapshot_i
-00009bf0: 642c 0a20 2020 2020 2020 2020 2020 2062  d,.            b
-00009c00: 7261 6e63 6865 733d 6272 616e 6368 6573  ranches=branches
-00009c10: 2c0a 2020 2020 2020 2020 2020 2020 6e65  ,.            ne
-00009c20: 7874 5f62 7261 6e63 683d 6e65 7874 5f62  xt_branch=next_b
-00009c30: 7261 6e63 682c 0a20 2020 2020 2020 2029  ranch,.        )
-00009c40: 0a0a 2020 2020 4064 625f 7472 616e 7361  ..    @db_transa
-00009c50: 6374 696f 6e28 290a 2020 2020 6465 6620  ction().    def 
-00009c60: 736e 6170 7368 6f74 5f67 6574 5f72 616e  snapshot_get_ran
-00009c70: 646f 6d28 7365 6c66 2c20 2a2c 2064 623a  dom(self, *, db:
-00009c80: 2044 622c 2063 7572 3d4e 6f6e 6529 202d   Db, cur=None) -
-00009c90: 3e20 5368 6131 4769 743a 0a20 2020 2020  > Sha1Git:.     
-00009ca0: 2020 2072 6574 7572 6e20 6462 2e73 6e61     return db.sna
-00009cb0: 7073 686f 745f 6765 745f 7261 6e64 6f6d  pshot_get_random
-00009cc0: 2863 7572 290a 0a20 2020 2040 6462 5f74  (cur)..    @db_t
-00009cd0: 7261 6e73 6163 7469 6f6e 2873 7461 7465  ransaction(state
-00009ce0: 6d65 6e74 5f74 696d 656f 7574 3d32 3030  ment_timeout=200
-00009cf0: 3029 0a20 2020 2064 6566 2073 6e61 7073  0).    def snaps
-00009d00: 686f 745f 6272 616e 6368 5f67 6574 5f62  hot_branch_get_b
-00009d10: 795f 6e61 6d65 280a 2020 2020 2020 2020  y_name(.        
-00009d20: 7365 6c66 2c0a 2020 2020 2020 2020 736e  self,.        sn
-00009d30: 6170 7368 6f74 5f69 643a 2053 6861 3147  apshot_id: Sha1G
-00009d40: 6974 2c0a 2020 2020 2020 2020 6272 616e  it,.        bran
-00009d50: 6368 5f6e 616d 653a 2062 7974 6573 2c0a  ch_name: bytes,.
-00009d60: 2020 2020 2020 2020 6462 3a20 4462 2c0a          db: Db,.
-00009d70: 2020 2020 2020 2020 6375 723d 4e6f 6e65          cur=None
-00009d80: 2c0a 2020 2020 2020 2020 666f 6c6c 6f77  ,.        follow
-00009d90: 5f61 6c69 6173 5f63 6861 696e 3a20 626f  _alias_chain: bo
-00009da0: 6f6c 203d 2054 7275 652c 0a20 2020 2020  ol = True,.     
-00009db0: 2020 206d 6178 5f61 6c69 6173 5f63 6861     max_alias_cha
-00009dc0: 696e 5f6c 656e 6774 683a 2069 6e74 203d  in_length: int =
-00009dd0: 2031 3030 2c0a 2020 2020 2920 2d3e 204f   100,.    ) -> O
-00009de0: 7074 696f 6e61 6c5b 536e 6170 7368 6f74  ptional[Snapshot
-00009df0: 4272 616e 6368 4279 4e61 6d65 5265 7370  BranchByNameResp
-00009e00: 6f6e 7365 5d3a 0a20 2020 2020 2020 2069  onse]:.        i
-00009e10: 6620 6c69 7374 2873 656c 662e 736e 6170  f list(self.snap
-00009e20: 7368 6f74 5f6d 6973 7369 6e67 285b 736e  shot_missing([sn
-00009e30: 6170 7368 6f74 5f69 645d 2929 3a0a 2020  apshot_id])):.  
-00009e40: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00009e50: 204e 6f6e 650a 0a20 2020 2020 2020 2069   None..        i
-00009e60: 6620 736e 6170 7368 6f74 5f69 6420 3d3d  f snapshot_id ==
-00009e70: 2045 4d50 5459 5f53 4e41 5053 484f 545f   EMPTY_SNAPSHOT_
-00009e80: 4944 3a0a 2020 2020 2020 2020 2020 2020  ID:.            
-00009e90: 7265 7475 726e 2053 6e61 7073 686f 7442  return SnapshotB
-00009ea0: 7261 6e63 6842 794e 616d 6552 6573 706f  ranchByNameRespo
-00009eb0: 6e73 6528 0a20 2020 2020 2020 2020 2020  nse(.           
-00009ec0: 2020 2020 2062 7261 6e63 685f 666f 756e       branch_foun
-00009ed0: 643d 4661 6c73 652c 0a20 2020 2020 2020  d=False,.       
-00009ee0: 2020 2020 2020 2020 2074 6172 6765 743d           target=
-00009ef0: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00009f00: 2020 2020 2020 616c 6961 7365 735f 666f        aliases_fo
-00009f10: 6c6c 6f77 6564 3d5b 5d2c 0a20 2020 2020  llowed=[],.     
-00009f20: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00009f30: 2020 636f 6c73 5f74 6f5f 6665 7463 6820    cols_to_fetch 
-00009f40: 3d20 5b22 7461 7267 6574 222c 2022 7461  = ["target", "ta
-00009f50: 7267 6574 5f74 7970 6522 5d0a 2020 2020  rget_type"].    
-00009f60: 2020 2020 7265 736f 6c76 655f 6368 6169      resolve_chai
-00009f70: 6e3a 204c 6973 745b 6279 7465 735d 203d  n: List[bytes] =
-00009f80: 205b 5d0a 2020 2020 2020 2020 7768 696c   [].        whil
-00009f90: 6520 5472 7565 3a0a 2020 2020 2020 2020  e True:.        
-00009fa0: 2020 2020 6272 616e 6368 203d 2064 622e      branch = db.
-00009fb0: 736e 6170 7368 6f74 5f62 7261 6e63 685f  snapshot_branch_
-00009fc0: 6765 745f 6279 5f6e 616d 6528 0a20 2020  get_by_name(.   
-00009fd0: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
-00009fe0: 735f 746f 5f66 6574 6368 3d63 6f6c 735f  s_to_fetch=cols_
-00009ff0: 746f 5f66 6574 6368 2c0a 2020 2020 2020  to_fetch,.      
-0000a000: 2020 2020 2020 2020 2020 736e 6170 7368            snapsh
-0000a010: 6f74 5f69 643d 736e 6170 7368 6f74 5f69  ot_id=snapshot_i
-0000a020: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-0000a030: 2020 2062 7261 6e63 685f 6e61 6d65 3d62     branch_name=b
-0000a040: 7261 6e63 685f 6e61 6d65 2c0a 2020 2020  ranch_name,.    
-0000a050: 2020 2020 2020 2020 2020 2020 6375 723d              cur=
-0000a060: 6375 722c 0a20 2020 2020 2020 2020 2020  cur,.           
-0000a070: 2029 0a20 2020 2020 2020 2020 2020 2069   ).            i
-0000a080: 6620 6272 616e 6368 2069 7320 4e6f 6e65  f branch is None
-0000a090: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000a0a0: 2020 2320 7461 7267 6574 2062 7261 6e63    # target branc
-0000a0b0: 6820 6973 204e 6f6e 652c 2074 6865 7265  h is None, there
-0000a0c0: 2063 6f75 6c64 2062 6520 6974 656d 7320   could be items 
-0000a0d0: 696e 2061 6c69 6173 6573 5f66 6f6c 6c6f  in aliases_follo
-0000a0e0: 7765 640a 2020 2020 2020 2020 2020 2020  wed.            
-0000a0f0: 2020 2020 7461 7267 6574 203d 204e 6f6e      target = Non
-0000a100: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-0000a110: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
-0000a120: 2020 2020 6272 616e 6368 5f64 203d 2064      branch_d = d
-0000a130: 6963 7428 7a69 7028 636f 6c73 5f74 6f5f  ict(zip(cols_to_
-0000a140: 6665 7463 682c 2062 7261 6e63 6829 290a  fetch, branch)).
-0000a150: 2020 2020 2020 2020 2020 2020 7265 736f              reso
-0000a160: 6c76 655f 6368 6169 6e2e 6170 7065 6e64  lve_chain.append
-0000a170: 2862 7261 6e63 685f 6e61 6d65 290a 2020  (branch_name).  
-0000a180: 2020 2020 2020 2020 2020 6966 2028 0a20            if (. 
-0000a190: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-0000a1a0: 7261 6e63 685f 645b 2274 6172 6765 745f  ranch_d["target_
-0000a1b0: 7479 7065 225d 2021 3d20 5461 7267 6574  type"] != Target
-0000a1c0: 5479 7065 2e41 4c49 4153 2e76 616c 7565  Type.ALIAS.value
-0000a1d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a1e0: 206f 7220 6e6f 7420 666f 6c6c 6f77 5f61   or not follow_a
-0000a1f0: 6c69 6173 5f63 6861 696e 0a20 2020 2020  lias_chain.     
-0000a200: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
-0000a210: 2020 2020 2020 2020 2020 2320 6669 7273            # firs
-0000a220: 7420 6e6f 6e20 616c 6961 7320 6272 616e  t non alias bran
-0000a230: 6368 206f 7220 7468 6520 6669 7273 7420  ch or the first 
-0000a240: 6272 616e 6368 2077 6865 6e20 666f 6c6c  branch when foll
-0000a250: 6f77 5f61 6c69 6173 5f63 6861 696e 2069  ow_alias_chain i
-0000a260: 7320 4661 6c73 650a 2020 2020 2020 2020  s False.        
-0000a270: 2020 2020 2020 2020 7461 7267 6574 203d          target =
-0000a280: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
-0000a290: 2020 2020 2020 2053 6e61 7073 686f 7442         SnapshotB
-0000a2a0: 7261 6e63 6828 0a20 2020 2020 2020 2020  ranch(.         
-0000a2b0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000a2c0: 6172 6765 743d 6272 616e 6368 5f64 5b22  arget=branch_d["
-0000a2d0: 7461 7267 6574 225d 2c0a 2020 2020 2020  target"],.      
-0000a2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2f0: 2020 7461 7267 6574 5f74 7970 653d 5461    target_type=Ta
-0000a300: 7267 6574 5479 7065 2862 7261 6e63 685f  rgetType(branch_
-0000a310: 645b 2274 6172 6765 745f 7479 7065 225d  d["target_type"]
-0000a320: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0000a330: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000a340: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000a350: 6272 616e 6368 5f64 5b22 7461 7267 6574  branch_d["target
-0000a360: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
-0000a370: 2020 2020 2020 2065 6c73 6520 4e6f 6e65         else None
-0000a380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a390: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-0000a3a0: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
-0000a3b0: 2020 2020 2065 6c69 6620 280a 2020 2020       elif (.    
-0000a3c0: 2020 2020 2020 2020 2020 2020 2320 4369              # Ci
-0000a3d0: 7263 756c 6172 2072 6566 6572 656e 6365  rcular reference
-0000a3e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a3f0: 2072 6573 6f6c 7665 5f63 6861 696e 2e63   resolve_chain.c
-0000a400: 6f75 6e74 2862 7261 6e63 685f 6e61 6d65  ount(branch_name
-0000a410: 2920 3e20 310a 2020 2020 2020 2020 2020  ) > 1.          
-0000a420: 2020 2020 2020 2320 546f 6f20 6d61 6e79        # Too many
-0000a430: 2072 652d 6469 7265 6374 730a 2020 2020   re-directs.    
-0000a440: 2020 2020 2020 2020 2020 2020 6f72 206c              or l
-0000a450: 656e 2872 6573 6f6c 7665 5f63 6861 696e  en(resolve_chain
-0000a460: 2920 3e3d 206d 6178 5f61 6c69 6173 5f63  ) >= max_alias_c
-0000a470: 6861 696e 5f6c 656e 6774 680a 2020 2020  hain_length.    
-0000a480: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
-0000a490: 2020 2020 2020 2020 2020 2074 6172 6765             targe
-0000a4a0: 7420 3d20 4e6f 6e65 0a20 2020 2020 2020  t = None.       
-0000a4b0: 2020 2020 2020 2020 2062 7265 616b 0a20           break. 
-0000a4c0: 2020 2020 2020 2020 2020 2023 2042 7261             # Bra
-0000a4d0: 6e63 6820 6861 7320 6120 6e6f 6e2d 4e6f  nch has a non-No
-0000a4e0: 6e65 2074 6172 6765 7420 7769 7468 2074  ne target with t
-0000a4f0: 7970 6520 616c 6961 730a 2020 2020 2020  ype alias.      
-0000a500: 2020 2020 2020 6272 616e 6368 5f6e 616d        branch_nam
-0000a510: 6520 3d20 6272 616e 6368 5f64 5b22 7461  e = branch_d["ta
-0000a520: 7267 6574 225d 0a0a 2020 2020 2020 2020  rget"]..        
-0000a530: 7265 7475 726e 2053 6e61 7073 686f 7442  return SnapshotB
-0000a540: 7261 6e63 6842 794e 616d 6552 6573 706f  ranchByNameRespo
-0000a550: 6e73 6528 0a20 2020 2020 2020 2020 2020  nse(.           
-0000a560: 2023 2072 6573 6f6c 7665 5f63 6869 616e   # resolve_chian
-0000a570: 2068 6173 2069 7465 6d73 2c20 6272 6163   has items, brac
-0000a580: 685f 666f 756e 6420 6d75 7374 2062 6520  h_found must be 
-0000a590: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
-0000a5a0: 2062 7261 6e63 685f 666f 756e 643d 626f   branch_found=bo
-0000a5b0: 6f6c 2872 6573 6f6c 7665 5f63 6861 696e  ol(resolve_chain
-0000a5c0: 292c 0a20 2020 2020 2020 2020 2020 2074  ),.            t
-0000a5d0: 6172 6765 743d 7461 7267 6574 2c0a 2020  arget=target,.  
-0000a5e0: 2020 2020 2020 2020 2020 616c 6961 7365            aliase
-0000a5f0: 735f 666f 6c6c 6f77 6564 3d72 6573 6f6c  s_followed=resol
-0000a600: 7665 5f63 6861 696e 2c0a 2020 2020 2020  ve_chain,.      
-0000a610: 2020 290a 0a20 2020 2023 2323 2323 2323    )..    #######
-0000a620: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000a630: 2323 230a 2020 2020 2320 4f72 6967 696e  ###.    # Origin
-0000a640: 5669 7369 7420 616e 6420 4f72 6967 696e  Visit and Origin
-0000a650: 5669 7369 7453 7461 7475 730a 2020 2020  VisitStatus.    
-0000a660: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000a670: 2323 2323 2323 2323 2323 0a0a 2020 2020  ##########..    
-0000a680: 4064 625f 7472 616e 7361 6374 696f 6e28  @db_transaction(
-0000a690: 290a 2020 2020 6465 6620 6f72 6967 696e  ).    def origin
-0000a6a0: 5f76 6973 6974 5f61 6464 280a 2020 2020  _visit_add(.    
-0000a6b0: 2020 2020 7365 6c66 2c20 7669 7369 7473      self, visits
-0000a6c0: 3a20 4c69 7374 5b4f 7269 6769 6e56 6973  : List[OriginVis
-0000a6d0: 6974 5d2c 202a 2c20 6462 3a20 4462 2c20  it], *, db: Db, 
-0000a6e0: 6375 723d 4e6f 6e65 0a20 2020 2029 202d  cur=None.    ) -
-0000a6f0: 3e20 4974 6572 6162 6c65 5b4f 7269 6769  > Iterable[Origi
-0000a700: 6e56 6973 6974 5d3a 0a20 2020 2020 2020  nVisit]:.       
-0000a710: 2066 6f72 2076 6973 6974 2069 6e20 7669   for visit in vi
-0000a720: 7369 7473 3a0a 2020 2020 2020 2020 2020  sits:.          
-0000a730: 2020 6f72 6967 696e 203d 2073 656c 662e    origin = self.
-0000a740: 6f72 6967 696e 5f67 6574 285b 7669 7369  origin_get([visi
-0000a750: 742e 6f72 6967 696e 5d2c 2064 623d 6462  t.origin], db=db
-0000a760: 2c20 6375 723d 6375 7229 5b30 5d0a 2020  , cur=cur)[0].  
-0000a770: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-0000a780: 206f 7269 6769 6e3a 2020 2320 4361 6e6e   origin:  # Cann
-0000a790: 6f74 2061 6464 2061 2076 6973 6974 2077  ot add a visit w
-0000a7a0: 6974 686f 7574 2061 6e20 6f72 6967 696e  ithout an origin
-0000a7b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a7c0: 2072 6169 7365 2053 746f 7261 6765 4172   raise StorageAr
-0000a7d0: 6775 6d65 6e74 4578 6365 7074 696f 6e28  gumentException(
-0000a7e0: 2255 6e6b 6e6f 776e 206f 7269 6769 6e20  "Unknown origin 
-0000a7f0: 2573 222c 2076 6973 6974 2e6f 7269 6769  %s", visit.origi
-0000a800: 6e29 0a0a 2020 2020 2020 2020 616c 6c5f  n)..        all_
-0000a810: 7669 7369 7473 203d 205b 5d0a 2020 2020  visits = [].    
-0000a820: 2020 2020 666f 7220 7669 7369 7420 696e      for visit in
-0000a830: 2076 6973 6974 733a 0a20 2020 2020 2020   visits:.       
-0000a840: 2020 2020 2069 6620 7669 7369 742e 7669       if visit.vi
-0000a850: 7369 743a 0a20 2020 2020 2020 2020 2020  sit:.           
-0000a860: 2020 2020 2073 656c 662e 6a6f 7572 6e61       self.journa
-0000a870: 6c5f 7772 6974 6572 2e6f 7269 6769 6e5f  l_writer.origin_
-0000a880: 7669 7369 745f 6164 6428 5b76 6973 6974  visit_add([visit
-0000a890: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-0000a8a0: 2020 2064 622e 6f72 6967 696e 5f76 6973     db.origin_vis
-0000a8b0: 6974 5f61 6464 5f77 6974 685f 6964 2876  it_add_with_id(v
-0000a8c0: 6973 6974 2c20 6375 723d 6375 7229 0a20  isit, cur=cur). 
-0000a8d0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000a8e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a8f0: 2023 2076 6973 6974 5f69 6420 6973 206e   # visit_id is n
-0000a900: 6f74 2067 6976 656e 2c20 6974 206e 6565  ot given, it nee
-0000a910: 6473 2074 6f20 6265 2073 6574 2062 7920  ds to be set by 
-0000a920: 7468 6520 6462 0a20 2020 2020 2020 2020  the db.         
-0000a930: 2020 2020 2020 2077 6974 6820 636f 6e76         with conv
-0000a940: 6572 745f 7661 6c69 6461 7469 6f6e 5f65  ert_validation_e
-0000a950: 7863 6570 7469 6f6e 7328 293a 0a20 2020  xceptions():.   
-0000a960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a970: 2076 6973 6974 5f69 6420 3d20 6462 2e6f   visit_id = db.o
-0000a980: 7269 6769 6e5f 7669 7369 745f 6164 6428  rigin_visit_add(
-0000a990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a9a0: 2020 2020 2020 2020 2076 6973 6974 2e6f           visit.o
-0000a9b0: 7269 6769 6e2c 2076 6973 6974 2e64 6174  rigin, visit.dat
-0000a9c0: 652c 2076 6973 6974 2e74 7970 652c 2063  e, visit.type, c
-0000a9d0: 7572 3d63 7572 0a20 2020 2020 2020 2020  ur=cur.         
-0000a9e0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0000a9f0: 2020 2020 2020 2020 2020 2020 2076 6973               vis
-0000aa00: 6974 203d 2061 7474 722e 6576 6f6c 7665  it = attr.evolve
-0000aa10: 2876 6973 6974 2c20 7669 7369 743d 7669  (visit, visit=vi
-0000aa20: 7369 745f 6964 290a 2020 2020 2020 2020  sit_id).        
-0000aa30: 2020 2020 2020 2020 2320 466f 7263 6564          # Forced
-0000aa40: 2074 6f20 7772 6974 6520 696e 2074 6865   to write in the
-0000aa50: 206a 6f75 726e 616c 2061 6674 6572 2074   journal after t
-0000aa60: 6865 2064 6220 2873 696e 6365 2069 7473  he db (since its
-0000aa70: 2074 6865 2064 620a 2020 2020 2020 2020   the db.        
-0000aa80: 2020 2020 2020 2020 2320 6361 6c6c 2074          # call t
-0000aa90: 6861 7420 7365 7420 7468 6520 7669 7369  hat set the visi
-0000aaa0: 7420 6964 290a 2020 2020 2020 2020 2020  t id).          
-0000aab0: 2020 2020 2020 7365 6c66 2e6a 6f75 726e        self.journ
-0000aac0: 616c 5f77 7269 7465 722e 6f72 6967 696e  al_writer.origin
-0000aad0: 5f76 6973 6974 5f61 6464 285b 7669 7369  _visit_add([visi
-0000aae0: 745d 290a 2020 2020 2020 2020 2020 2020  t]).            
-0000aaf0: 2020 2020 2320 496e 2074 6869 7320 6361      # In this ca
-0000ab00: 7365 2c20 7765 2061 6c73 6f20 7761 6e74  se, we also want
-0000ab10: 2074 6f20 6372 6561 7465 2074 6865 2069   to create the i
-0000ab20: 6e69 7469 616c 204f 5653 206f 626a 6563  nitial OVS objec
-0000ab30: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
-0000ab40: 2020 7669 7369 745f 7374 6174 7573 203d    visit_status =
-0000ab50: 204f 7269 6769 6e56 6973 6974 5374 6174   OriginVisitStat
-0000ab60: 7573 280a 2020 2020 2020 2020 2020 2020  us(.            
-0000ab70: 2020 2020 2020 2020 6f72 6967 696e 3d76          origin=v
-0000ab80: 6973 6974 2e6f 7269 6769 6e2c 0a20 2020  isit.origin,.   
-0000ab90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aba0: 2076 6973 6974 3d76 6973 6974 5f69 642c   visit=visit_id,
-0000abb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000abc0: 2020 2020 2064 6174 653d 7669 7369 742e       date=visit.
-0000abd0: 6461 7465 2c0a 2020 2020 2020 2020 2020  date,.          
-0000abe0: 2020 2020 2020 2020 2020 7479 7065 3d76            type=v
-0000abf0: 6973 6974 2e74 7970 652c 0a20 2020 2020  isit.type,.     
-0000ac00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000ac10: 7461 7475 733d 2263 7265 6174 6564 222c  tatus="created",
-0000ac20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ac30: 2020 2020 2073 6e61 7073 686f 743d 4e6f       snapshot=No
-0000ac40: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-0000ac50: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0000ac60: 2020 2020 2020 7365 6c66 2e5f 6f72 6967        self._orig
-0000ac70: 696e 5f76 6973 6974 5f73 7461 7475 735f  in_visit_status_
-0000ac80: 6164 6428 7669 7369 745f 7374 6174 7573  add(visit_status
-0000ac90: 2c20 6462 3d64 622c 2063 7572 3d63 7572  , db=db, cur=cur
-0000aca0: 290a 2020 2020 2020 2020 2020 2020 6173  ).            as
-0000acb0: 7365 7274 2076 6973 6974 2e76 6973 6974  sert visit.visit
-0000acc0: 2069 7320 6e6f 7420 4e6f 6e65 0a20 2020   is not None.   
-0000acd0: 2020 2020 2020 2020 2061 6c6c 5f76 6973           all_vis
-0000ace0: 6974 732e 6170 7065 6e64 2876 6973 6974  its.append(visit
-0000acf0: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-0000ad00: 6e20 616c 6c5f 7669 7369 7473 0a0a 2020  n all_visits..  
-0000ad10: 2020 6465 6620 5f6f 7269 6769 6e5f 7669    def _origin_vi
-0000ad20: 7369 745f 7374 6174 7573 5f61 6464 280a  sit_status_add(.
-0000ad30: 2020 2020 2020 2020 7365 6c66 2c20 7669          self, vi
-0000ad40: 7369 745f 7374 6174 7573 3a20 4f72 6967  sit_status: Orig
-0000ad50: 696e 5669 7369 7453 7461 7475 732c 2064  inVisitStatus, d
-0000ad60: 622c 2063 7572 0a20 2020 2029 202d 3e20  b, cur.    ) -> 
-0000ad70: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-0000ad80: 2241 6464 2061 6e20 6f72 6967 696e 2076  "Add an origin v
-0000ad90: 6973 6974 2073 7461 7475 7322 2222 0a20  isit status""". 
-0000ada0: 2020 2020 2020 2073 656c 662e 6a6f 7572         self.jour
-0000adb0: 6e61 6c5f 7772 6974 6572 2e6f 7269 6769  nal_writer.origi
-0000adc0: 6e5f 7669 7369 745f 7374 6174 7573 5f61  n_visit_status_a
-0000add0: 6464 285b 7669 7369 745f 7374 6174 7573  dd([visit_status
-0000ade0: 5d29 0a20 2020 2020 2020 2064 622e 6f72  ]).        db.or
-0000adf0: 6967 696e 5f76 6973 6974 5f73 7461 7475  igin_visit_statu
-0000ae00: 735f 6164 6428 7669 7369 745f 7374 6174  s_add(visit_stat
-0000ae10: 7573 2c20 6375 723d 6375 7229 0a0a 2020  us, cur=cur)..  
-0000ae20: 2020 4064 625f 7472 616e 7361 6374 696f    @db_transactio
-0000ae30: 6e28 290a 2020 2020 6465 6620 6f72 6967  n().    def orig
-0000ae40: 696e 5f76 6973 6974 5f73 7461 7475 735f  in_visit_status_
-0000ae50: 6164 6428 0a20 2020 2020 2020 2073 656c  add(.        sel
-0000ae60: 662c 0a20 2020 2020 2020 2076 6973 6974  f,.        visit
-0000ae70: 5f73 7461 7475 7365 733a 204c 6973 745b  _statuses: List[
-0000ae80: 4f72 6967 696e 5669 7369 7453 7461 7475  OriginVisitStatu
-0000ae90: 735d 2c0a 2020 2020 2020 2020 2a2c 0a20  s],.        *,. 
-0000aea0: 2020 2020 2020 2064 623a 2044 622c 0a20         db: Db,. 
-0000aeb0: 2020 2020 2020 2063 7572 3d4e 6f6e 652c         cur=None,
-0000aec0: 0a20 2020 2029 202d 3e20 4469 6374 5b73  .    ) -> Dict[s
-0000aed0: 7472 2c20 696e 745d 3a0a 2020 2020 2020  tr, int]:.      
-0000aee0: 2020 7669 7369 745f 7374 6174 7573 6573    visit_statuses
-0000aef0: 5f20 3d20 5b5d 0a0a 2020 2020 2020 2020  _ = []..        
-0000af00: 2320 4669 7273 7420 726f 756e 6420 746f  # First round to
-0000af10: 2063 6865 636b 2065 7869 7374 656e 6365   check existence
-0000af20: 2028 6661 696c 2065 6172 6c79 2069 6620   (fail early if 
-0000af30: 616e 7920 6973 206b 6f29 0a20 2020 2020  any is ko).     
-0000af40: 2020 2066 6f72 2076 6973 6974 5f73 7461     for visit_sta
-0000af50: 7475 7320 696e 2076 6973 6974 5f73 7461  tus in visit_sta
-0000af60: 7475 7365 733a 0a20 2020 2020 2020 2020  tuses:.         
-0000af70: 2020 206f 7269 6769 6e5f 7572 6c20 3d20     origin_url = 
-0000af80: 7365 6c66 2e6f 7269 6769 6e5f 6765 7428  self.origin_get(
-0000af90: 5b76 6973 6974 5f73 7461 7475 732e 6f72  [visit_status.or
-0000afa0: 6967 696e 5d2c 2064 623d 6462 2c20 6375  igin], db=db, cu
-0000afb0: 723d 6375 7229 5b30 5d0a 2020 2020 2020  r=cur)[0].      
-0000afc0: 2020 2020 2020 6966 206e 6f74 206f 7269        if not ori
-0000afd0: 6769 6e5f 7572 6c3a 0a20 2020 2020 2020  gin_url:.       
-0000afe0: 2020 2020 2020 2020 2072 6169 7365 2053           raise S
-0000aff0: 746f 7261 6765 4172 6775 6d65 6e74 4578  torageArgumentEx
-0000b000: 6365 7074 696f 6e28 6622 556e 6b6e 6f77  ception(f"Unknow
-0000b010: 6e20 6f72 6967 696e 207b 7669 7369 745f  n origin {visit_
-0000b020: 7374 6174 7573 2e6f 7269 6769 6e7d 2229  status.origin}")
-0000b030: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-0000b040: 2076 6973 6974 5f73 7461 7475 732e 7479   visit_status.ty
-0000b050: 7065 2069 7320 4e6f 6e65 3a0a 2020 2020  pe is None:.    
-0000b060: 2020 2020 2020 2020 2020 2020 6f72 6967              orig
-0000b070: 696e 5f76 6973 6974 203d 2073 656c 662e  in_visit = self.
-0000b080: 6f72 6967 696e 5f76 6973 6974 5f67 6574  origin_visit_get
-0000b090: 5f62 7928 0a20 2020 2020 2020 2020 2020  _by(.           
-0000b0a0: 2020 2020 2020 2020 2076 6973 6974 5f73           visit_s
-0000b0b0: 7461 7475 732e 6f72 6967 696e 2c20 7669  tatus.origin, vi
-0000b0c0: 7369 745f 7374 6174 7573 2e76 6973 6974  sit_status.visit
-0000b0d0: 2c20 6462 3d64 622c 2063 7572 3d63 7572  , db=db, cur=cur
-0000b0e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b0f0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-0000b100: 2020 2069 6620 6f72 6967 696e 5f76 6973     if origin_vis
-0000b110: 6974 2069 7320 4e6f 6e65 3a0a 2020 2020  it is None:.    
-0000b120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b130: 7261 6973 6520 5374 6f72 6167 6541 7267  raise StorageArg
-0000b140: 756d 656e 7445 7863 6570 7469 6f6e 280a  umentException(.
-0000b150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b160: 2020 2020 2020 2020 6622 556e 6b6e 6f77          f"Unknow
-0000b170: 6e20 6f72 6967 696e 2076 6973 6974 207b  n origin visit {
-0000b180: 7669 7369 745f 7374 6174 7573 2e76 6973  visit_status.vis
-0000b190: 6974 7d20 220a 2020 2020 2020 2020 2020  it} ".          
-0000b1a0: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-0000b1b0: 6f66 206f 7269 6769 6e20 7b76 6973 6974  of origin {visit
-0000b1c0: 5f73 7461 7475 732e 6f72 6967 696e 7d22  _status.origin}"
-0000b1d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b1e0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-0000b1f0: 2020 2020 2020 2020 6f72 6967 696e 5f76          origin_v
-0000b200: 6973 6974 5f73 7461 7475 7320 3d20 6174  isit_status = at
-0000b210: 7472 2e65 766f 6c76 6528 7669 7369 745f  tr.evolve(visit_
-0000b220: 7374 6174 7573 2c20 7479 7065 3d6f 7269  status, type=ori
-0000b230: 6769 6e5f 7669 7369 742e 7479 7065 290a  gin_visit.type).
-0000b240: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000b250: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000b260: 2020 6f72 6967 696e 5f76 6973 6974 5f73    origin_visit_s
-0000b270: 7461 7475 7320 3d20 7669 7369 745f 7374  tatus = visit_st
-0000b280: 6174 7573 0a0a 2020 2020 2020 2020 2020  atus..          
-0000b290: 2020 7669 7369 745f 7374 6174 7573 6573    visit_statuses
-0000b2a0: 5f2e 6170 7065 6e64 286f 7269 6769 6e5f  _.append(origin_
-0000b2b0: 7669 7369 745f 7374 6174 7573 290a 0a20  visit_status).. 
-0000b2c0: 2020 2020 2020 2066 6f72 2076 6973 6974         for visit
-0000b2d0: 5f73 7461 7475 7320 696e 2076 6973 6974  _status in visit
-0000b2e0: 5f73 7461 7475 7365 735f 3a0a 2020 2020  _statuses_:.    
-0000b2f0: 2020 2020 2020 2020 7365 6c66 2e5f 6f72          self._or
-0000b300: 6967 696e 5f76 6973 6974 5f73 7461 7475  igin_visit_statu
-0000b310: 735f 6164 6428 7669 7369 745f 7374 6174  s_add(visit_stat
-0000b320: 7573 2c20 6462 2c20 6375 7229 0a20 2020  us, db, cur).   
-0000b330: 2020 2020 2072 6574 7572 6e20 7b22 6f72       return {"or
-0000b340: 6967 696e 5f76 6973 6974 5f73 7461 7475  igin_visit_statu
-0000b350: 733a 6164 6422 3a20 6c65 6e28 7669 7369  s:add": len(visi
-0000b360: 745f 7374 6174 7573 6573 5f29 7d0a 0a20  t_statuses_)}.. 
-0000b370: 2020 2040 6462 5f74 7261 6e73 6163 7469     @db_transacti
-0000b380: 6f6e 2829 0a20 2020 2064 6566 206f 7269  on().    def ori
-0000b390: 6769 6e5f 7669 7369 745f 7374 6174 7573  gin_visit_status
-0000b3a0: 5f67 6574 5f6c 6174 6573 7428 0a20 2020  _get_latest(.   
-0000b3b0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0000b3c0: 2020 206f 7269 6769 6e5f 7572 6c3a 2073     origin_url: s
-0000b3d0: 7472 2c0a 2020 2020 2020 2020 7669 7369  tr,.        visi
-0000b3e0: 743a 2069 6e74 2c0a 2020 2020 2020 2020  t: int,.        
-0000b3f0: 616c 6c6f 7765 645f 7374 6174 7573 6573  allowed_statuses
-0000b400: 3a20 4f70 7469 6f6e 616c 5b4c 6973 745b  : Optional[List[
-0000b410: 7374 725d 5d20 3d20 4e6f 6e65 2c0a 2020  str]] = None,.  
-0000b420: 2020 2020 2020 7265 7175 6972 655f 736e        require_sn
-0000b430: 6170 7368 6f74 3a20 626f 6f6c 203d 2046  apshot: bool = F
-0000b440: 616c 7365 2c0a 2020 2020 2020 2020 2a2c  alse,.        *,
-0000b450: 0a20 2020 2020 2020 2064 623a 2044 622c  .        db: Db,
-0000b460: 0a20 2020 2020 2020 2063 7572 3d4e 6f6e  .        cur=Non
-0000b470: 652c 0a20 2020 2029 202d 3e20 4f70 7469  e,.    ) -> Opti
-0000b480: 6f6e 616c 5b4f 7269 6769 6e56 6973 6974  onal[OriginVisit
-0000b490: 5374 6174 7573 5d3a 0a20 2020 2020 2020  Status]:.       
-0000b4a0: 2069 6620 616c 6c6f 7765 645f 7374 6174   if allowed_stat
-0000b4b0: 7573 6573 2061 6e64 206e 6f74 2073 6574  uses and not set
-0000b4c0: 2861 6c6c 6f77 6564 5f73 7461 7475 7365  (allowed_statuse
-0000b4d0: 7329 2e69 6e74 6572 7365 6374 696f 6e28  s).intersection(
-0000b4e0: 5649 5349 545f 5354 4154 5553 4553 293a  VISIT_STATUSES):
-0000b4f0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-0000b500: 7365 2053 746f 7261 6765 4172 6775 6d65  se StorageArgume
-0000b510: 6e74 4578 6365 7074 696f 6e28 0a20 2020  ntException(.   
-0000b520: 2020 2020 2020 2020 2020 2020 2066 2255               f"U
-0000b530: 6e6b 6e6f 776e 2061 6c6c 6f77 6564 2073  nknown allowed s
-0000b540: 7461 7475 7365 7320 7b27 2c27 2e6a 6f69  tatuses {','.joi
-0000b550: 6e28 616c 6c6f 7765 645f 7374 6174 7573  n(allowed_status
-0000b560: 6573 297d 2c20 6f6e 6c79 2022 0a20 2020  es)}, only ".   
-0000b570: 2020 2020 2020 2020 2020 2020 2066 227b               f"{
-0000b580: 272c 272e 6a6f 696e 2856 4953 4954 5f53  ','.join(VISIT_S
-0000b590: 5441 5455 5345 5329 7d20 6175 7468 6f72  TATUSES)} author
-0000b5a0: 697a 6564 220a 2020 2020 2020 2020 2020  ized".          
-0000b5b0: 2020 290a 0a20 2020 2020 2020 2072 6f77    )..        row
-0000b5c0: 5f64 203d 2064 622e 6f72 6967 696e 5f76  _d = db.origin_v
-0000b5d0: 6973 6974 5f73 7461 7475 735f 6765 745f  isit_status_get_
-0000b5e0: 6c61 7465 7374 280a 2020 2020 2020 2020  latest(.        
-0000b5f0: 2020 2020 6f72 6967 696e 5f75 726c 2c20      origin_url, 
-0000b600: 7669 7369 742c 2061 6c6c 6f77 6564 5f73  visit, allowed_s
-0000b610: 7461 7475 7365 732c 2072 6571 7569 7265  tatuses, require
-0000b620: 5f73 6e61 7073 686f 742c 2063 7572 3d63  _snapshot, cur=c
-0000b630: 7572 0a20 2020 2020 2020 2029 0a20 2020  ur.        ).   
-0000b640: 2020 2020 2069 6620 6e6f 7420 726f 775f       if not row_
-0000b650: 643a 0a20 2020 2020 2020 2020 2020 2072  d:.            r
-0000b660: 6574 7572 6e20 4e6f 6e65 0a20 2020 2020  eturn None.     
-0000b670: 2020 2072 6574 7572 6e20 4f72 6967 696e     return Origin
-0000b680: 5669 7369 7453 7461 7475 7328 2a2a 726f  VisitStatus(**ro
-0000b690: 775f 6429 0a0a 2020 2020 4064 625f 7472  w_d)..    @db_tr
-0000b6a0: 616e 7361 6374 696f 6e28 7374 6174 656d  ansaction(statem
-0000b6b0: 656e 745f 7469 6d65 6f75 743d 3530 3029  ent_timeout=500)
-0000b6c0: 0a20 2020 2064 6566 206f 7269 6769 6e5f  .    def origin_
-0000b6d0: 7669 7369 745f 6765 7428 0a20 2020 2020  visit_get(.     
-0000b6e0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-0000b6f0: 206f 7269 6769 6e3a 2073 7472 2c0a 2020   origin: str,.  
-0000b700: 2020 2020 2020 7061 6765 5f74 6f6b 656e        page_token
-0000b710: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-0000b720: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000b730: 6f72 6465 723a 204c 6973 744f 7264 6572  order: ListOrder
-0000b740: 203d 204c 6973 744f 7264 6572 2e41 5343   = ListOrder.ASC
-0000b750: 2c0a 2020 2020 2020 2020 6c69 6d69 743a  ,.        limit:
-0000b760: 2069 6e74 203d 2031 302c 0a20 2020 2020   int = 10,.     
-0000b770: 2020 202a 2c0a 2020 2020 2020 2020 6462     *,.        db
-0000b780: 3a20 4462 2c0a 2020 2020 2020 2020 6375  : Db,.        cu
-0000b790: 723d 4e6f 6e65 2c0a 2020 2020 2920 2d3e  r=None,.    ) ->
-0000b7a0: 2050 6167 6564 5265 7375 6c74 5b4f 7269   PagedResult[Ori
-0000b7b0: 6769 6e56 6973 6974 5d3a 0a20 2020 2020  ginVisit]:.     
-0000b7c0: 2020 2070 6167 655f 746f 6b65 6e20 3d20     page_token = 
-0000b7d0: 7061 6765 5f74 6f6b 656e 206f 7220 2230  page_token or "0
-0000b7e0: 220a 2020 2020 2020 2020 6966 206e 6f74  ".        if not
-0000b7f0: 2069 7369 6e73 7461 6e63 6528 6f72 6465   isinstance(orde
-0000b800: 722c 204c 6973 744f 7264 6572 293a 0a20  r, ListOrder):. 
-0000b810: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-0000b820: 2053 746f 7261 6765 4172 6775 6d65 6e74   StorageArgument
-0000b830: 4578 6365 7074 696f 6e28 226f 7264 6572  Exception("order
-0000b840: 206d 7573 7420 6265 2061 204c 6973 744f   must be a ListO
-0000b850: 7264 6572 2076 616c 7565 2229 0a20 2020  rder value").   
-0000b860: 2020 2020 2069 6620 6e6f 7420 6973 696e       if not isin
-0000b870: 7374 616e 6365 2870 6167 655f 746f 6b65  stance(page_toke
-0000b880: 6e2c 2073 7472 293a 0a20 2020 2020 2020  n, str):.       
-0000b890: 2020 2020 2072 6169 7365 2053 746f 7261       raise Stora
-0000b8a0: 6765 4172 6775 6d65 6e74 4578 6365 7074  geArgumentExcept
-0000b8b0: 696f 6e28 2270 6167 655f 746f 6b65 6e20  ion("page_token 
-0000b8c0: 6d75 7374 2062 6520 6120 7374 7269 6e67  must be a string
-0000b8d0: 2e22 290a 0a20 2020 2020 2020 206e 6578  .")..        nex
-0000b8e0: 745f 7061 6765 5f74 6f6b 656e 203d 204e  t_page_token = N
-0000b8f0: 6f6e 650a 2020 2020 2020 2020 7669 7369  one.        visi
-0000b900: 745f 6672 6f6d 203d 2069 6e74 2870 6167  t_from = int(pag
-0000b910: 655f 746f 6b65 6e29 0a20 2020 2020 2020  e_token).       
-0000b920: 2076 6973 6974 733a 204c 6973 745b 4f72   visits: List[Or
-0000b930: 6967 696e 5669 7369 745d 203d 205b 5d0a  iginVisit] = [].
-0000b940: 2020 2020 2020 2020 6578 7472 615f 6c69          extra_li
-0000b950: 6d69 7420 3d20 6c69 6d69 7420 2b20 310a  mit = limit + 1.
-0000b960: 2020 2020 2020 2020 666f 7220 726f 7720          for row 
-0000b970: 696e 2064 622e 6f72 6967 696e 5f76 6973  in db.origin_vis
-0000b980: 6974 5f67 6574 5f72 616e 6765 280a 2020  it_get_range(.  
-0000b990: 2020 2020 2020 2020 2020 6f72 6967 696e            origin
-0000b9a0: 2c20 7669 7369 745f 6672 6f6d 3d76 6973  , visit_from=vis
-0000b9b0: 6974 5f66 726f 6d2c 206f 7264 6572 3d6f  it_from, order=o
-0000b9c0: 7264 6572 2c20 6c69 6d69 743d 6578 7472  rder, limit=extr
-0000b9d0: 615f 6c69 6d69 742c 2063 7572 3d63 7572  a_limit, cur=cur
-0000b9e0: 0a20 2020 2020 2020 2029 3a0a 2020 2020  .        ):.    
-0000b9f0: 2020 2020 2020 2020 726f 775f 6420 3d20          row_d = 
-0000ba00: 6469 6374 287a 6970 2864 622e 6f72 6967  dict(zip(db.orig
-0000ba10: 696e 5f76 6973 6974 5f63 6f6c 732c 2072  in_visit_cols, r
-0000ba20: 6f77 2929 0a20 2020 2020 2020 2020 2020  ow)).           
-0000ba30: 2076 6973 6974 732e 6170 7065 6e64 280a   visits.append(.
-0000ba40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba50: 4f72 6967 696e 5669 7369 7428 0a20 2020  OriginVisit(.   
+00008ab0: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
+00008ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ad0: 2020 2022 746d 705f 736e 6170 7368 6f74     "tmp_snapshot
+00008ae0: 5f62 7261 6e63 6822 2c0a 2020 2020 2020  _branch",.      
+00008af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b00: 2020 5b22 6e61 6d65 222c 2022 7461 7267    ["name", "targ
+00008b10: 6574 222c 2022 7461 7267 6574 5f74 7970  et", "target_typ
+00008b20: 6522 5d2c 0a20 2020 2020 2020 2020 2020  e"],.           
+00008b30: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00008b40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00008b50: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00008b60: 2020 2020 2020 2020 2073 656c 662e 6a6f           self.jo
+00008b70: 7572 6e61 6c5f 7772 6974 6572 2e73 6e61  urnal_writer.sna
+00008b80: 7073 686f 745f 6164 6428 5b73 6e61 7073  pshot_add([snaps
+00008b90: 686f 745d 290a 0a20 2020 2020 2020 2020  hot])..         
+00008ba0: 2020 2020 2020 2064 622e 736e 6170 7368         db.snapsh
+00008bb0: 6f74 5f61 6464 2873 6e61 7073 686f 742e  ot_add(snapshot.
+00008bc0: 6964 2c20 6375 7229 0a20 2020 2020 2020  id, cur).       
+00008bd0: 2020 2020 2020 2020 2063 6f75 6e74 202b           count +
+00008be0: 3d20 310a 0a20 2020 2020 2020 2072 6574  = 1..        ret
+00008bf0: 7572 6e20 7b22 736e 6170 7368 6f74 3a61  urn {"snapshot:a
+00008c00: 6464 223a 2063 6f75 6e74 7d0a 0a20 2020  dd": count}..   
+00008c10: 2040 6462 5f74 7261 6e73 6163 7469 6f6e   @db_transaction
+00008c20: 5f67 656e 6572 6174 6f72 2829 0a20 2020  _generator().   
+00008c30: 2064 6566 2073 6e61 7073 686f 745f 6d69   def snapshot_mi
+00008c40: 7373 696e 6728 0a20 2020 2020 2020 2073  ssing(.        s
+00008c50: 656c 662c 2073 6e61 7073 686f 7473 3a20  elf, snapshots: 
+00008c60: 4c69 7374 5b53 6861 3147 6974 5d2c 202a  List[Sha1Git], *
+00008c70: 2c20 6462 3a20 4462 2c20 6375 723d 4e6f  , db: Db, cur=No
+00008c80: 6e65 0a20 2020 2029 202d 3e20 4974 6572  ne.    ) -> Iter
+00008c90: 6162 6c65 5b53 6861 3147 6974 5d3a 0a20  able[Sha1Git]:. 
+00008ca0: 2020 2020 2020 2066 6f72 206f 626a 2069         for obj i
+00008cb0: 6e20 6462 2e73 6e61 7073 686f 745f 6d69  n db.snapshot_mi
+00008cc0: 7373 696e 675f 6672 6f6d 5f6c 6973 7428  ssing_from_list(
+00008cd0: 736e 6170 7368 6f74 732c 2063 7572 293a  snapshots, cur):
+00008ce0: 0a20 2020 2020 2020 2020 2020 2079 6965  .            yie
+00008cf0: 6c64 206f 626a 5b30 5d0a 0a20 2020 2040  ld obj[0]..    @
+00008d00: 6462 5f74 7261 6e73 6163 7469 6f6e 2873  db_transaction(s
+00008d10: 7461 7465 6d65 6e74 5f74 696d 656f 7574  tatement_timeout
+00008d20: 3d32 3030 3029 0a20 2020 2064 6566 2073  =2000).    def s
+00008d30: 6e61 7073 686f 745f 6765 7428 0a20 2020  napshot_get(.   
+00008d40: 2020 2020 2073 656c 662c 2073 6e61 7073       self, snaps
+00008d50: 686f 745f 6964 3a20 5368 6131 4769 742c  hot_id: Sha1Git,
+00008d60: 202a 2c20 6462 3a20 4462 2c20 6375 723d   *, db: Db, cur=
+00008d70: 4e6f 6e65 0a20 2020 2029 202d 3e20 4f70  None.    ) -> Op
+00008d80: 7469 6f6e 616c 5b44 6963 745b 7374 722c  tional[Dict[str,
+00008d90: 2041 6e79 5d5d 3a0a 2020 2020 2020 2020   Any]]:.        
+00008da0: 6420 3d20 7365 6c66 2e73 6e61 7073 686f  d = self.snapsho
+00008db0: 745f 6765 745f 6272 616e 6368 6573 2873  t_get_branches(s
+00008dc0: 6e61 7073 686f 745f 6964 290a 2020 2020  napshot_id).    
+00008dd0: 2020 2020 6966 2064 2069 7320 4e6f 6e65      if d is None
+00008de0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00008df0: 7475 726e 2064 0a20 2020 2020 2020 2072  turn d.        r
+00008e00: 6574 7572 6e20 7b0a 2020 2020 2020 2020  eturn {.        
+00008e10: 2020 2020 2269 6422 3a20 645b 2269 6422      "id": d["id"
+00008e20: 5d2c 0a20 2020 2020 2020 2020 2020 2022  ],.            "
+00008e30: 6272 616e 6368 6573 223a 207b 0a20 2020  branches": {.   
+00008e40: 2020 2020 2020 2020 2020 2020 206e 616d               nam
+00008e50: 653a 2062 7261 6e63 682e 746f 5f64 6963  e: branch.to_dic
+00008e60: 7428 2920 6966 2062 7261 6e63 6820 656c  t() if branch el
+00008e70: 7365 204e 6f6e 650a 2020 2020 2020 2020  se None.        
+00008e80: 2020 2020 2020 2020 666f 7220 286e 616d          for (nam
+00008e90: 652c 2062 7261 6e63 6829 2069 6e20 645b  e, branch) in d[
+00008ea0: 2262 7261 6e63 6865 7322 5d2e 6974 656d  "branches"].item
+00008eb0: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
+00008ec0: 7d2c 0a20 2020 2020 2020 2020 2020 2022  },.            "
+00008ed0: 6e65 7874 5f62 7261 6e63 6822 3a20 645b  next_branch": d[
+00008ee0: 226e 6578 745f 6272 616e 6368 225d 2c0a  "next_branch"],.
+00008ef0: 2020 2020 2020 2020 7d0a 0a20 2020 2040          }..    @
+00008f00: 6462 5f74 7261 6e73 6163 7469 6f6e 2829  db_transaction()
+00008f10: 0a20 2020 2064 6566 2073 6e61 7073 686f  .    def snapsho
+00008f20: 745f 6765 745f 6964 5f70 6172 7469 7469  t_get_id_partiti
+00008f30: 6f6e 280a 2020 2020 2020 2020 7365 6c66  on(.        self
+00008f40: 2c0a 2020 2020 2020 2020 7061 7274 6974  ,.        partit
+00008f50: 696f 6e5f 6964 3a20 696e 742c 0a20 2020  ion_id: int,.   
+00008f60: 2020 2020 206e 625f 7061 7274 6974 696f       nb_partitio
+00008f70: 6e73 3a20 696e 742c 0a20 2020 2020 2020  ns: int,.       
+00008f80: 2070 6167 655f 746f 6b65 6e3a 204f 7074   page_token: Opt
+00008f90: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+00008fa0: 652c 0a20 2020 2020 2020 206c 696d 6974  e,.        limit
+00008fb0: 3a20 696e 7420 3d20 3130 3030 2c0a 2020  : int = 1000,.  
+00008fc0: 2020 2020 2020 2a2c 0a20 2020 2020 2020        *,.       
+00008fd0: 2064 623a 2044 622c 0a20 2020 2020 2020   db: Db,.       
+00008fe0: 2063 7572 3d4e 6f6e 652c 0a20 2020 2029   cur=None,.    )
+00008ff0: 202d 3e20 5061 6765 6452 6573 756c 745b   -> PagedResult[
+00009000: 5368 6131 4769 745d 3a0a 2020 2020 2020  Sha1Git]:.      
+00009010: 2020 7265 7475 726e 205f 6765 745f 7061    return _get_pa
+00009020: 6769 6e61 7465 645f 7368 6131 5f70 6172  ginated_sha1_par
+00009030: 7469 7469 6f6e 280a 2020 2020 2020 2020  tition(.        
+00009040: 2020 2020 6375 722c 0a20 2020 2020 2020      cur,.       
+00009050: 2020 2020 2070 6172 7469 7469 6f6e 5f69       partition_i
+00009060: 642c 0a20 2020 2020 2020 2020 2020 206e  d,.            n
+00009070: 625f 7061 7274 6974 696f 6e73 2c0a 2020  b_partitions,.  
+00009080: 2020 2020 2020 2020 2020 7061 6765 5f74            page_t
+00009090: 6f6b 656e 2c0a 2020 2020 2020 2020 2020  oken,.          
+000090a0: 2020 6c69 6d69 742c 0a20 2020 2020 2020    limit,.       
+000090b0: 2020 2020 2064 622e 736e 6170 7368 6f74       db.snapshot
+000090c0: 5f67 6574 5f69 645f 7261 6e67 652c 0a20  _get_id_range,. 
+000090d0: 2020 2020 2020 2020 2020 206f 7065 7261             opera
+000090e0: 746f 722e 6974 656d 6765 7474 6572 2830  tor.itemgetter(0
+000090f0: 292c 0a20 2020 2020 2020 2020 2020 206c  ),.            l
+00009100: 616d 6264 6120 6964 5f3a 2069 645f 2c0a  ambda id_: id_,.
+00009110: 2020 2020 2020 2020 290a 0a20 2020 2040          )..    @
+00009120: 6462 5f74 7261 6e73 6163 7469 6f6e 2873  db_transaction(s
+00009130: 7461 7465 6d65 6e74 5f74 696d 656f 7574  tatement_timeout
+00009140: 3d32 3030 3029 0a20 2020 2064 6566 2073  =2000).    def s
+00009150: 6e61 7073 686f 745f 636f 756e 745f 6272  napshot_count_br
+00009160: 616e 6368 6573 280a 2020 2020 2020 2020  anches(.        
+00009170: 7365 6c66 2c0a 2020 2020 2020 2020 736e  self,.        sn
+00009180: 6170 7368 6f74 5f69 643a 2053 6861 3147  apshot_id: Sha1G
+00009190: 6974 2c0a 2020 2020 2020 2020 6272 616e  it,.        bran
+000091a0: 6368 5f6e 616d 655f 6578 636c 7564 655f  ch_name_exclude_
+000091b0: 7072 6566 6978 3a20 4f70 7469 6f6e 616c  prefix: Optional
+000091c0: 5b62 7974 6573 5d20 3d20 4e6f 6e65 2c0a  [bytes] = None,.
+000091d0: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
+000091e0: 2020 2064 623a 2044 622c 0a20 2020 2020     db: Db,.     
+000091f0: 2020 2063 7572 3d4e 6f6e 652c 0a20 2020     cur=None,.   
+00009200: 2029 202d 3e20 4f70 7469 6f6e 616c 5b44   ) -> Optional[D
+00009210: 6963 745b 4f70 7469 6f6e 616c 5b73 7472  ict[Optional[str
+00009220: 5d2c 2069 6e74 5d5d 3a0a 2020 2020 2020  ], int]]:.      
+00009230: 2020 7265 7475 726e 2064 6963 7428 0a20    return dict(. 
+00009240: 2020 2020 2020 2020 2020 205b 0a20 2020             [.   
+00009250: 2020 2020 2020 2020 2020 2020 2062 630a               bc.
+00009260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009270: 666f 7220 6263 2069 6e20 6462 2e73 6e61  for bc in db.sna
+00009280: 7073 686f 745f 636f 756e 745f 6272 616e  pshot_count_bran
+00009290: 6368 6573 280a 2020 2020 2020 2020 2020  ches(.          
+000092a0: 2020 2020 2020 2020 2020 736e 6170 7368            snapsh
+000092b0: 6f74 5f69 642c 0a20 2020 2020 2020 2020  ot_id,.         
+000092c0: 2020 2020 2020 2020 2020 2062 7261 6e63             branc
+000092d0: 685f 6e61 6d65 5f65 7863 6c75 6465 5f70  h_name_exclude_p
+000092e0: 7265 6669 782c 0a20 2020 2020 2020 2020  refix,.         
+000092f0: 2020 2020 2020 2020 2020 2063 7572 2c0a             cur,.
+00009300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009310: 290a 2020 2020 2020 2020 2020 2020 5d0a  ).            ].
+00009320: 2020 2020 2020 2020 290a 0a20 2020 2040          )..    @
+00009330: 6462 5f74 7261 6e73 6163 7469 6f6e 2873  db_transaction(s
+00009340: 7461 7465 6d65 6e74 5f74 696d 656f 7574  tatement_timeout
+00009350: 3d32 3030 3029 0a20 2020 2064 6566 2073  =2000).    def s
+00009360: 6e61 7073 686f 745f 6765 745f 6272 616e  napshot_get_bran
+00009370: 6368 6573 280a 2020 2020 2020 2020 7365  ches(.        se
+00009380: 6c66 2c0a 2020 2020 2020 2020 736e 6170  lf,.        snap
+00009390: 7368 6f74 5f69 643a 2053 6861 3147 6974  shot_id: Sha1Git
+000093a0: 2c0a 2020 2020 2020 2020 6272 616e 6368  ,.        branch
+000093b0: 6573 5f66 726f 6d3a 2062 7974 6573 203d  es_from: bytes =
+000093c0: 2062 2222 2c0a 2020 2020 2020 2020 6272   b"",.        br
+000093d0: 616e 6368 6573 5f63 6f75 6e74 3a20 696e  anches_count: in
+000093e0: 7420 3d20 3130 3030 2c0a 2020 2020 2020  t = 1000,.      
+000093f0: 2020 7461 7267 6574 5f74 7970 6573 3a20    target_types: 
+00009400: 4f70 7469 6f6e 616c 5b4c 6973 745b 7374  Optional[List[st
+00009410: 725d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  r]] = None,.    
+00009420: 2020 2020 6272 616e 6368 5f6e 616d 655f      branch_name_
+00009430: 696e 636c 7564 655f 7375 6273 7472 696e  include_substrin
+00009440: 673a 204f 7074 696f 6e61 6c5b 6279 7465  g: Optional[byte
+00009450: 735d 203d 204e 6f6e 652c 0a20 2020 2020  s] = None,.     
+00009460: 2020 2062 7261 6e63 685f 6e61 6d65 5f65     branch_name_e
+00009470: 7863 6c75 6465 5f70 7265 6669 783a 204f  xclude_prefix: O
+00009480: 7074 696f 6e61 6c5b 6279 7465 735d 203d  ptional[bytes] =
+00009490: 204e 6f6e 652c 0a20 2020 2020 2020 202a   None,.        *
+000094a0: 2c0a 2020 2020 2020 2020 6462 3a20 4462  ,.        db: Db
+000094b0: 2c0a 2020 2020 2020 2020 6375 723d 4e6f  ,.        cur=No
+000094c0: 6e65 2c0a 2020 2020 2920 2d3e 204f 7074  ne,.    ) -> Opt
+000094d0: 696f 6e61 6c5b 5061 7274 6961 6c42 7261  ional[PartialBra
+000094e0: 6e63 6865 735d 3a0a 2020 2020 2020 2020  nches]:.        
+000094f0: 6966 2073 6e61 7073 686f 745f 6964 203d  if snapshot_id =
+00009500: 3d20 454d 5054 595f 534e 4150 5348 4f54  = EMPTY_SNAPSHOT
+00009510: 5f49 443a 0a20 2020 2020 2020 2020 2020  _ID:.           
+00009520: 2072 6574 7572 6e20 5061 7274 6961 6c42   return PartialB
+00009530: 7261 6e63 6865 7328 0a20 2020 2020 2020  ranches(.       
+00009540: 2020 2020 2020 2020 2069 643d 736e 6170           id=snap
+00009550: 7368 6f74 5f69 642c 0a20 2020 2020 2020  shot_id,.       
+00009560: 2020 2020 2020 2020 2062 7261 6e63 6865           branche
+00009570: 733d 7b7d 2c0a 2020 2020 2020 2020 2020  s={},.          
+00009580: 2020 2020 2020 6e65 7874 5f62 7261 6e63        next_branc
+00009590: 683d 4e6f 6e65 2c0a 2020 2020 2020 2020  h=None,.        
+000095a0: 2020 2020 290a 0a20 2020 2020 2020 2069      )..        i
+000095b0: 6620 6c69 7374 2873 656c 662e 736e 6170  f list(self.snap
+000095c0: 7368 6f74 5f6d 6973 7369 6e67 285b 736e  shot_missing([sn
+000095d0: 6170 7368 6f74 5f69 645d 2929 3a0a 2020  apshot_id])):.  
+000095e0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000095f0: 204e 6f6e 650a 0a20 2020 2020 2020 2062   None..        b
+00009600: 7261 6e63 6865 7320 3d20 7b7d 0a20 2020  ranches = {}.   
+00009610: 2020 2020 206e 6578 745f 6272 616e 6368       next_branch
+00009620: 203d 204e 6f6e 650a 0a20 2020 2020 2020   = None..       
+00009630: 2066 6574 6368 6564 5f62 7261 6e63 6865   fetched_branche
+00009640: 7320 3d20 6c69 7374 280a 2020 2020 2020  s = list(.      
+00009650: 2020 2020 2020 6462 2e73 6e61 7073 686f        db.snapsho
+00009660: 745f 6765 745f 6279 5f69 6428 0a20 2020  t_get_by_id(.   
+00009670: 2020 2020 2020 2020 2020 2020 2073 6e61               sna
+00009680: 7073 686f 745f 6964 2c0a 2020 2020 2020  pshot_id,.      
+00009690: 2020 2020 2020 2020 2020 6272 616e 6368            branch
+000096a0: 6573 5f66 726f 6d3d 6272 616e 6368 6573  es_from=branches
+000096b0: 5f66 726f 6d2c 0a20 2020 2020 2020 2020  _from,.         
+000096c0: 2020 2020 2020 2023 2074 6865 2075 6e64         # the und
+000096d0: 6572 6c79 696e 6720 5351 4c20 7175 6572  erlying SQL quer
+000096e0: 7920 6361 6e20 6265 2071 7569 7465 2065  y can be quite e
+000096f0: 7870 656e 7369 7665 2074 6f20 6578 6563  xpensive to exec
+00009700: 7574 6520 666f 7220 736d 616c 6c0a 2020  ute for small.  
+00009710: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00009720: 6272 616e 6368 6573 5f63 6f75 6e74 2076  branches_count v
+00009730: 616c 7565 2c20 736f 2077 6520 656e 7375  alue, so we ensu
+00009740: 7265 2061 206d 696e 696d 756d 2062 7261  re a minimum bra
+00009750: 6e63 6865 7320 6c69 6d69 7420 6f66 2031  nches limit of 1
+00009760: 3020 666f 720a 2020 2020 2020 2020 2020  0 for.          
+00009770: 2020 2020 2020 2320 6f70 7469 6d61 6c20        # optimal 
+00009780: 7065 7266 6f72 6d61 6e63 6573 0a20 2020  performances.   
+00009790: 2020 2020 2020 2020 2020 2020 2062 7261               bra
+000097a0: 6e63 6865 735f 636f 756e 743d 6d61 7828  nches_count=max(
+000097b0: 6272 616e 6368 6573 5f63 6f75 6e74 202b  branches_count +
+000097c0: 2031 2c20 3130 292c 0a20 2020 2020 2020   1, 10),.       
+000097d0: 2020 2020 2020 2020 2074 6172 6765 745f           target_
+000097e0: 7479 7065 733d 7461 7267 6574 5f74 7970  types=target_typ
+000097f0: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
+00009800: 2020 2020 6272 616e 6368 5f6e 616d 655f      branch_name_
+00009810: 696e 636c 7564 655f 7375 6273 7472 696e  include_substrin
+00009820: 673d 6272 616e 6368 5f6e 616d 655f 696e  g=branch_name_in
+00009830: 636c 7564 655f 7375 6273 7472 696e 672c  clude_substring,
+00009840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009850: 2062 7261 6e63 685f 6e61 6d65 5f65 7863   branch_name_exc
+00009860: 6c75 6465 5f70 7265 6669 783d 6272 616e  lude_prefix=bran
+00009870: 6368 5f6e 616d 655f 6578 636c 7564 655f  ch_name_exclude_
+00009880: 7072 6566 6978 2c0a 2020 2020 2020 2020  prefix,.        
+00009890: 2020 2020 2020 2020 6375 723d 6375 722c          cur=cur,
+000098a0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+000098b0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000098c0: 2066 6f72 2072 6f77 2069 6e20 6665 7463   for row in fetc
+000098d0: 6865 645f 6272 616e 6368 6573 5b3a 6272  hed_branches[:br
+000098e0: 616e 6368 6573 5f63 6f75 6e74 5d3a 0a20  anches_count]:. 
+000098f0: 2020 2020 2020 2020 2020 2062 7261 6e63             branc
+00009900: 685f 6420 3d20 6469 6374 287a 6970 2864  h_d = dict(zip(d
+00009910: 622e 736e 6170 7368 6f74 5f67 6574 5f63  b.snapshot_get_c
+00009920: 6f6c 732c 2072 6f77 2929 0a20 2020 2020  ols, row)).     
+00009930: 2020 2020 2020 2064 656c 2062 7261 6e63         del branc
+00009940: 685f 645b 2273 6e61 7073 686f 745f 6964  h_d["snapshot_id
+00009950: 225d 0a20 2020 2020 2020 2020 2020 206e  "].            n
+00009960: 616d 6520 3d20 6272 616e 6368 5f64 2e70  ame = branch_d.p
+00009970: 6f70 2822 6e61 6d65 2229 0a20 2020 2020  op("name").     
+00009980: 2020 2020 2020 2069 6620 6272 616e 6368         if branch
+00009990: 5f64 5b22 7461 7267 6574 225d 2069 7320  _d["target"] is 
+000099a0: 4e6f 6e65 2061 6e64 2062 7261 6e63 685f  None and branch_
+000099b0: 645b 2274 6172 6765 745f 7479 7065 225d  d["target_type"]
+000099c0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+000099d0: 2020 2020 2020 2020 2020 6272 616e 6368            branch
+000099e0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+000099f0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00009a00: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+00009a10: 2062 7261 6e63 685f 645b 2274 6172 6765   branch_d["targe
+00009a20: 745f 7479 7065 225d 2069 7320 6e6f 7420  t_type"] is not 
+00009a30: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
+00009a40: 2020 2020 2062 7261 6e63 6820 3d20 536e       branch = Sn
+00009a50: 6170 7368 6f74 4272 616e 6368 280a 2020  apshotBranch(.  
+00009a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a70: 2020 7461 7267 6574 3d62 7261 6e63 685f    target=branch_
+00009a80: 645b 2274 6172 6765 7422 5d2c 0a20 2020  d["target"],.   
+00009a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009aa0: 2074 6172 6765 745f 7479 7065 3d53 6e61   target_type=Sna
+00009ab0: 7073 686f 7454 6172 6765 7454 7970 6528  pshotTargetType(
+00009ac0: 6272 616e 6368 5f64 5b22 7461 7267 6574  branch_d["target
+00009ad0: 5f74 7970 6522 5d29 2c0a 2020 2020 2020  _type"]),.      
+00009ae0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00009af0: 2020 2020 2020 2020 6272 616e 6368 6573          branches
+00009b00: 5b6e 616d 655d 203d 2062 7261 6e63 680a  [name] = branch.
+00009b10: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+00009b20: 6665 7463 6865 645f 6272 616e 6368 6573  fetched_branches
+00009b30: 2920 3e20 6272 616e 6368 6573 5f63 6f75  ) > branches_cou
+00009b40: 6e74 3a0a 2020 2020 2020 2020 2020 2020  nt:.            
+00009b50: 6e65 7874 5f62 7261 6e63 6820 3d20 6469  next_branch = di
+00009b60: 6374 280a 2020 2020 2020 2020 2020 2020  ct(.            
+00009b70: 2020 2020 7a69 7028 6462 2e73 6e61 7073      zip(db.snaps
+00009b80: 686f 745f 6765 745f 636f 6c73 2c20 6665  hot_get_cols, fe
+00009b90: 7463 6865 645f 6272 616e 6368 6573 5b62  tched_branches[b
+00009ba0: 7261 6e63 6865 735f 636f 756e 745d 290a  ranches_count]).
+00009bb0: 2020 2020 2020 2020 2020 2020 295b 226e              )["n
+00009bc0: 616d 6522 5d0a 0a20 2020 2020 2020 2072  ame"]..        r
+00009bd0: 6574 7572 6e20 5061 7274 6961 6c42 7261  eturn PartialBra
+00009be0: 6e63 6865 7328 0a20 2020 2020 2020 2020  nches(.         
+00009bf0: 2020 2069 643d 736e 6170 7368 6f74 5f69     id=snapshot_i
+00009c00: 642c 0a20 2020 2020 2020 2020 2020 2062  d,.            b
+00009c10: 7261 6e63 6865 733d 6272 616e 6368 6573  ranches=branches
+00009c20: 2c0a 2020 2020 2020 2020 2020 2020 6e65  ,.            ne
+00009c30: 7874 5f62 7261 6e63 683d 6e65 7874 5f62  xt_branch=next_b
+00009c40: 7261 6e63 682c 0a20 2020 2020 2020 2029  ranch,.        )
+00009c50: 0a0a 2020 2020 4064 625f 7472 616e 7361  ..    @db_transa
+00009c60: 6374 696f 6e28 290a 2020 2020 6465 6620  ction().    def 
+00009c70: 736e 6170 7368 6f74 5f67 6574 5f72 616e  snapshot_get_ran
+00009c80: 646f 6d28 7365 6c66 2c20 2a2c 2064 623a  dom(self, *, db:
+00009c90: 2044 622c 2063 7572 3d4e 6f6e 6529 202d   Db, cur=None) -
+00009ca0: 3e20 5368 6131 4769 743a 0a20 2020 2020  > Sha1Git:.     
+00009cb0: 2020 2072 6574 7572 6e20 6462 2e73 6e61     return db.sna
+00009cc0: 7073 686f 745f 6765 745f 7261 6e64 6f6d  pshot_get_random
+00009cd0: 2863 7572 290a 0a20 2020 2040 6462 5f74  (cur)..    @db_t
+00009ce0: 7261 6e73 6163 7469 6f6e 2873 7461 7465  ransaction(state
+00009cf0: 6d65 6e74 5f74 696d 656f 7574 3d32 3030  ment_timeout=200
+00009d00: 3029 0a20 2020 2064 6566 2073 6e61 7073  0).    def snaps
+00009d10: 686f 745f 6272 616e 6368 5f67 6574 5f62  hot_branch_get_b
+00009d20: 795f 6e61 6d65 280a 2020 2020 2020 2020  y_name(.        
+00009d30: 7365 6c66 2c0a 2020 2020 2020 2020 736e  self,.        sn
+00009d40: 6170 7368 6f74 5f69 643a 2053 6861 3147  apshot_id: Sha1G
+00009d50: 6974 2c0a 2020 2020 2020 2020 6272 616e  it,.        bran
+00009d60: 6368 5f6e 616d 653a 2062 7974 6573 2c0a  ch_name: bytes,.
+00009d70: 2020 2020 2020 2020 6462 3a20 4462 2c0a          db: Db,.
+00009d80: 2020 2020 2020 2020 6375 723d 4e6f 6e65          cur=None
+00009d90: 2c0a 2020 2020 2020 2020 666f 6c6c 6f77  ,.        follow
+00009da0: 5f61 6c69 6173 5f63 6861 696e 3a20 626f  _alias_chain: bo
+00009db0: 6f6c 203d 2054 7275 652c 0a20 2020 2020  ol = True,.     
+00009dc0: 2020 206d 6178 5f61 6c69 6173 5f63 6861     max_alias_cha
+00009dd0: 696e 5f6c 656e 6774 683a 2069 6e74 203d  in_length: int =
+00009de0: 2031 3030 2c0a 2020 2020 2920 2d3e 204f   100,.    ) -> O
+00009df0: 7074 696f 6e61 6c5b 536e 6170 7368 6f74  ptional[Snapshot
+00009e00: 4272 616e 6368 4279 4e61 6d65 5265 7370  BranchByNameResp
+00009e10: 6f6e 7365 5d3a 0a20 2020 2020 2020 2069  onse]:.        i
+00009e20: 6620 6c69 7374 2873 656c 662e 736e 6170  f list(self.snap
+00009e30: 7368 6f74 5f6d 6973 7369 6e67 285b 736e  shot_missing([sn
+00009e40: 6170 7368 6f74 5f69 645d 2929 3a0a 2020  apshot_id])):.  
+00009e50: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00009e60: 204e 6f6e 650a 0a20 2020 2020 2020 2069   None..        i
+00009e70: 6620 736e 6170 7368 6f74 5f69 6420 3d3d  f snapshot_id ==
+00009e80: 2045 4d50 5459 5f53 4e41 5053 484f 545f   EMPTY_SNAPSHOT_
+00009e90: 4944 3a0a 2020 2020 2020 2020 2020 2020  ID:.            
+00009ea0: 7265 7475 726e 2053 6e61 7073 686f 7442  return SnapshotB
+00009eb0: 7261 6e63 6842 794e 616d 6552 6573 706f  ranchByNameRespo
+00009ec0: 6e73 6528 0a20 2020 2020 2020 2020 2020  nse(.           
+00009ed0: 2020 2020 2062 7261 6e63 685f 666f 756e       branch_foun
+00009ee0: 643d 4661 6c73 652c 0a20 2020 2020 2020  d=False,.       
+00009ef0: 2020 2020 2020 2020 2074 6172 6765 743d           target=
+00009f00: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+00009f10: 2020 2020 2020 616c 6961 7365 735f 666f        aliases_fo
+00009f20: 6c6c 6f77 6564 3d5b 5d2c 0a20 2020 2020  llowed=[],.     
+00009f30: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00009f40: 2020 636f 6c73 5f74 6f5f 6665 7463 6820    cols_to_fetch 
+00009f50: 3d20 5b22 7461 7267 6574 222c 2022 7461  = ["target", "ta
+00009f60: 7267 6574 5f74 7970 6522 5d0a 2020 2020  rget_type"].    
+00009f70: 2020 2020 7265 736f 6c76 655f 6368 6169      resolve_chai
+00009f80: 6e3a 204c 6973 745b 6279 7465 735d 203d  n: List[bytes] =
+00009f90: 205b 5d0a 2020 2020 2020 2020 7768 696c   [].        whil
+00009fa0: 6520 5472 7565 3a0a 2020 2020 2020 2020  e True:.        
+00009fb0: 2020 2020 6272 616e 6368 203d 2064 622e      branch = db.
+00009fc0: 736e 6170 7368 6f74 5f62 7261 6e63 685f  snapshot_branch_
+00009fd0: 6765 745f 6279 5f6e 616d 6528 0a20 2020  get_by_name(.   
+00009fe0: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
+00009ff0: 735f 746f 5f66 6574 6368 3d63 6f6c 735f  s_to_fetch=cols_
+0000a000: 746f 5f66 6574 6368 2c0a 2020 2020 2020  to_fetch,.      
+0000a010: 2020 2020 2020 2020 2020 736e 6170 7368            snapsh
+0000a020: 6f74 5f69 643d 736e 6170 7368 6f74 5f69  ot_id=snapshot_i
+0000a030: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
+0000a040: 2020 2062 7261 6e63 685f 6e61 6d65 3d62     branch_name=b
+0000a050: 7261 6e63 685f 6e61 6d65 2c0a 2020 2020  ranch_name,.    
+0000a060: 2020 2020 2020 2020 2020 2020 6375 723d              cur=
+0000a070: 6375 722c 0a20 2020 2020 2020 2020 2020  cur,.           
+0000a080: 2029 0a20 2020 2020 2020 2020 2020 2069   ).            i
+0000a090: 6620 6272 616e 6368 2069 7320 4e6f 6e65  f branch is None
+0000a0a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000a0b0: 2020 2320 7461 7267 6574 2062 7261 6e63    # target branc
+0000a0c0: 6820 6973 204e 6f6e 652c 2074 6865 7265  h is None, there
+0000a0d0: 2063 6f75 6c64 2062 6520 6974 656d 7320   could be items 
+0000a0e0: 696e 2061 6c69 6173 6573 5f66 6f6c 6c6f  in aliases_follo
+0000a0f0: 7765 640a 2020 2020 2020 2020 2020 2020  wed.            
+0000a100: 2020 2020 7461 7267 6574 203d 204e 6f6e      target = Non
+0000a110: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0000a120: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
+0000a130: 2020 2020 6272 616e 6368 5f64 203d 2064      branch_d = d
+0000a140: 6963 7428 7a69 7028 636f 6c73 5f74 6f5f  ict(zip(cols_to_
+0000a150: 6665 7463 682c 2062 7261 6e63 6829 290a  fetch, branch)).
+0000a160: 2020 2020 2020 2020 2020 2020 7265 736f              reso
+0000a170: 6c76 655f 6368 6169 6e2e 6170 7065 6e64  lve_chain.append
+0000a180: 2862 7261 6e63 685f 6e61 6d65 290a 2020  (branch_name).  
+0000a190: 2020 2020 2020 2020 2020 6966 2028 0a20            if (. 
+0000a1a0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+0000a1b0: 7261 6e63 685f 645b 2274 6172 6765 745f  ranch_d["target_
+0000a1c0: 7479 7065 225d 2021 3d20 536e 6170 7368  type"] != Snapsh
+0000a1d0: 6f74 5461 7267 6574 5479 7065 2e41 4c49  otTargetType.ALI
+0000a1e0: 4153 2e76 616c 7565 0a20 2020 2020 2020  AS.value.       
+0000a1f0: 2020 2020 2020 2020 206f 7220 6e6f 7420           or not 
+0000a200: 666f 6c6c 6f77 5f61 6c69 6173 5f63 6861  follow_alias_cha
+0000a210: 696e 0a20 2020 2020 2020 2020 2020 2029  in.            )
+0000a220: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000a230: 2020 2320 6669 7273 7420 6e6f 6e20 616c    # first non al
+0000a240: 6961 7320 6272 616e 6368 206f 7220 7468  ias branch or th
+0000a250: 6520 6669 7273 7420 6272 616e 6368 2077  e first branch w
+0000a260: 6865 6e20 666f 6c6c 6f77 5f61 6c69 6173  hen follow_alias
+0000a270: 5f63 6861 696e 2069 7320 4661 6c73 650a  _chain is False.
+0000a280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a290: 7461 7267 6574 203d 2028 0a20 2020 2020  target = (.     
+0000a2a0: 2020 2020 2020 2020 2020 2020 2020 2053                 S
+0000a2b0: 6e61 7073 686f 7442 7261 6e63 6828 0a20  napshotBranch(. 
+0000a2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a2d0: 2020 2020 2020 2074 6172 6765 743d 6272         target=br
+0000a2e0: 616e 6368 5f64 5b22 7461 7267 6574 225d  anch_d["target"]
+0000a2f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000a300: 2020 2020 2020 2020 2020 7461 7267 6574            target
+0000a310: 5f74 7970 653d 536e 6170 7368 6f74 5461  _type=SnapshotTa
+0000a320: 7267 6574 5479 7065 2862 7261 6e63 685f  rgetType(branch_
+0000a330: 645b 2274 6172 6765 745f 7479 7065 225d  d["target_type"]
+0000a340: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0000a350: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000a360: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000a370: 6272 616e 6368 5f64 5b22 7461 7267 6574  branch_d["target
+0000a380: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+0000a390: 2020 2020 2020 2065 6c73 6520 4e6f 6e65         else None
+0000a3a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a3b0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+0000a3c0: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
+0000a3d0: 2020 2020 2065 6c69 6620 280a 2020 2020       elif (.    
+0000a3e0: 2020 2020 2020 2020 2020 2020 2320 4369              # Ci
+0000a3f0: 7263 756c 6172 2072 6566 6572 656e 6365  rcular reference
+0000a400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a410: 2072 6573 6f6c 7665 5f63 6861 696e 2e63   resolve_chain.c
+0000a420: 6f75 6e74 2862 7261 6e63 685f 6e61 6d65  ount(branch_name
+0000a430: 2920 3e20 310a 2020 2020 2020 2020 2020  ) > 1.          
+0000a440: 2020 2020 2020 2320 546f 6f20 6d61 6e79        # Too many
+0000a450: 2072 652d 6469 7265 6374 730a 2020 2020   re-directs.    
+0000a460: 2020 2020 2020 2020 2020 2020 6f72 206c              or l
+0000a470: 656e 2872 6573 6f6c 7665 5f63 6861 696e  en(resolve_chain
+0000a480: 2920 3e3d 206d 6178 5f61 6c69 6173 5f63  ) >= max_alias_c
+0000a490: 6861 696e 5f6c 656e 6774 680a 2020 2020  hain_length.    
+0000a4a0: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
+0000a4b0: 2020 2020 2020 2020 2020 2074 6172 6765             targe
+0000a4c0: 7420 3d20 4e6f 6e65 0a20 2020 2020 2020  t = None.       
+0000a4d0: 2020 2020 2020 2020 2062 7265 616b 0a20           break. 
+0000a4e0: 2020 2020 2020 2020 2020 2023 2042 7261             # Bra
+0000a4f0: 6e63 6820 6861 7320 6120 6e6f 6e2d 4e6f  nch has a non-No
+0000a500: 6e65 2074 6172 6765 7420 7769 7468 2074  ne target with t
+0000a510: 7970 6520 616c 6961 730a 2020 2020 2020  ype alias.      
+0000a520: 2020 2020 2020 6272 616e 6368 5f6e 616d        branch_nam
+0000a530: 6520 3d20 6272 616e 6368 5f64 5b22 7461  e = branch_d["ta
+0000a540: 7267 6574 225d 0a0a 2020 2020 2020 2020  rget"]..        
+0000a550: 7265 7475 726e 2053 6e61 7073 686f 7442  return SnapshotB
+0000a560: 7261 6e63 6842 794e 616d 6552 6573 706f  ranchByNameRespo
+0000a570: 6e73 6528 0a20 2020 2020 2020 2020 2020  nse(.           
+0000a580: 2023 2072 6573 6f6c 7665 5f63 6869 616e   # resolve_chian
+0000a590: 2068 6173 2069 7465 6d73 2c20 6272 6163   has items, brac
+0000a5a0: 685f 666f 756e 6420 6d75 7374 2062 6520  h_found must be 
+0000a5b0: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
+0000a5c0: 2062 7261 6e63 685f 666f 756e 643d 626f   branch_found=bo
+0000a5d0: 6f6c 2872 6573 6f6c 7665 5f63 6861 696e  ol(resolve_chain
+0000a5e0: 292c 0a20 2020 2020 2020 2020 2020 2074  ),.            t
+0000a5f0: 6172 6765 743d 7461 7267 6574 2c0a 2020  arget=target,.  
+0000a600: 2020 2020 2020 2020 2020 616c 6961 7365            aliase
+0000a610: 735f 666f 6c6c 6f77 6564 3d72 6573 6f6c  s_followed=resol
+0000a620: 7665 5f63 6861 696e 2c0a 2020 2020 2020  ve_chain,.      
+0000a630: 2020 290a 0a20 2020 2023 2323 2323 2323    )..    #######
+0000a640: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000a650: 2323 230a 2020 2020 2320 4f72 6967 696e  ###.    # Origin
+0000a660: 5669 7369 7420 616e 6420 4f72 6967 696e  Visit and Origin
+0000a670: 5669 7369 7453 7461 7475 730a 2020 2020  VisitStatus.    
+0000a680: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000a690: 2323 2323 2323 2323 2323 0a0a 2020 2020  ##########..    
+0000a6a0: 4064 625f 7472 616e 7361 6374 696f 6e28  @db_transaction(
+0000a6b0: 290a 2020 2020 6465 6620 6f72 6967 696e  ).    def origin
+0000a6c0: 5f76 6973 6974 5f61 6464 280a 2020 2020  _visit_add(.    
+0000a6d0: 2020 2020 7365 6c66 2c20 7669 7369 7473      self, visits
+0000a6e0: 3a20 4c69 7374 5b4f 7269 6769 6e56 6973  : List[OriginVis
+0000a6f0: 6974 5d2c 202a 2c20 6462 3a20 4462 2c20  it], *, db: Db, 
+0000a700: 6375 723d 4e6f 6e65 0a20 2020 2029 202d  cur=None.    ) -
+0000a710: 3e20 4974 6572 6162 6c65 5b4f 7269 6769  > Iterable[Origi
+0000a720: 6e56 6973 6974 5d3a 0a20 2020 2020 2020  nVisit]:.       
+0000a730: 2066 6f72 2076 6973 6974 2069 6e20 7669   for visit in vi
+0000a740: 7369 7473 3a0a 2020 2020 2020 2020 2020  sits:.          
+0000a750: 2020 6f72 6967 696e 203d 2073 656c 662e    origin = self.
+0000a760: 6f72 6967 696e 5f67 6574 285b 7669 7369  origin_get([visi
+0000a770: 742e 6f72 6967 696e 5d2c 2064 623d 6462  t.origin], db=db
+0000a780: 2c20 6375 723d 6375 7229 5b30 5d0a 2020  , cur=cur)[0].  
+0000a790: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+0000a7a0: 206f 7269 6769 6e3a 2020 2320 4361 6e6e   origin:  # Cann
+0000a7b0: 6f74 2061 6464 2061 2076 6973 6974 2077  ot add a visit w
+0000a7c0: 6974 686f 7574 2061 6e20 6f72 6967 696e  ithout an origin
+0000a7d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a7e0: 2072 6169 7365 2053 746f 7261 6765 4172   raise StorageAr
+0000a7f0: 6775 6d65 6e74 4578 6365 7074 696f 6e28  gumentException(
+0000a800: 2255 6e6b 6e6f 776e 206f 7269 6769 6e20  "Unknown origin 
+0000a810: 2573 222c 2076 6973 6974 2e6f 7269 6769  %s", visit.origi
+0000a820: 6e29 0a0a 2020 2020 2020 2020 616c 6c5f  n)..        all_
+0000a830: 7669 7369 7473 203d 205b 5d0a 2020 2020  visits = [].    
+0000a840: 2020 2020 666f 7220 7669 7369 7420 696e      for visit in
+0000a850: 2076 6973 6974 733a 0a20 2020 2020 2020   visits:.       
+0000a860: 2020 2020 2069 6620 7669 7369 742e 7669       if visit.vi
+0000a870: 7369 743a 0a20 2020 2020 2020 2020 2020  sit:.           
+0000a880: 2020 2020 2073 656c 662e 6a6f 7572 6e61       self.journa
+0000a890: 6c5f 7772 6974 6572 2e6f 7269 6769 6e5f  l_writer.origin_
+0000a8a0: 7669 7369 745f 6164 6428 5b76 6973 6974  visit_add([visit
+0000a8b0: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+0000a8c0: 2020 2064 622e 6f72 6967 696e 5f76 6973     db.origin_vis
+0000a8d0: 6974 5f61 6464 5f77 6974 685f 6964 2876  it_add_with_id(v
+0000a8e0: 6973 6974 2c20 6375 723d 6375 7229 0a20  isit, cur=cur). 
+0000a8f0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000a900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a910: 2023 2076 6973 6974 5f69 6420 6973 206e   # visit_id is n
+0000a920: 6f74 2067 6976 656e 2c20 6974 206e 6565  ot given, it nee
+0000a930: 6473 2074 6f20 6265 2073 6574 2062 7920  ds to be set by 
+0000a940: 7468 6520 6462 0a20 2020 2020 2020 2020  the db.         
+0000a950: 2020 2020 2020 2077 6974 6820 636f 6e76         with conv
+0000a960: 6572 745f 7661 6c69 6461 7469 6f6e 5f65  ert_validation_e
+0000a970: 7863 6570 7469 6f6e 7328 293a 0a20 2020  xceptions():.   
+0000a980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a990: 2076 6973 6974 5f69 6420 3d20 6462 2e6f   visit_id = db.o
+0000a9a0: 7269 6769 6e5f 7669 7369 745f 6164 6428  rigin_visit_add(
+0000a9b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a9c0: 2020 2020 2020 2020 2076 6973 6974 2e6f           visit.o
+0000a9d0: 7269 6769 6e2c 2076 6973 6974 2e64 6174  rigin, visit.dat
+0000a9e0: 652c 2076 6973 6974 2e74 7970 652c 2063  e, visit.type, c
+0000a9f0: 7572 3d63 7572 0a20 2020 2020 2020 2020  ur=cur.         
+0000aa00: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000aa10: 2020 2020 2020 2020 2020 2020 2076 6973               vis
+0000aa20: 6974 203d 2061 7474 722e 6576 6f6c 7665  it = attr.evolve
+0000aa30: 2876 6973 6974 2c20 7669 7369 743d 7669  (visit, visit=vi
+0000aa40: 7369 745f 6964 290a 2020 2020 2020 2020  sit_id).        
+0000aa50: 2020 2020 2020 2020 2320 466f 7263 6564          # Forced
+0000aa60: 2074 6f20 7772 6974 6520 696e 2074 6865   to write in the
+0000aa70: 206a 6f75 726e 616c 2061 6674 6572 2074   journal after t
+0000aa80: 6865 2064 6220 2873 696e 6365 2069 7473  he db (since its
+0000aa90: 2074 6865 2064 620a 2020 2020 2020 2020   the db.        
+0000aaa0: 2020 2020 2020 2020 2320 6361 6c6c 2074          # call t
+0000aab0: 6861 7420 7365 7420 7468 6520 7669 7369  hat set the visi
+0000aac0: 7420 6964 290a 2020 2020 2020 2020 2020  t id).          
+0000aad0: 2020 2020 2020 7365 6c66 2e6a 6f75 726e        self.journ
+0000aae0: 616c 5f77 7269 7465 722e 6f72 6967 696e  al_writer.origin
+0000aaf0: 5f76 6973 6974 5f61 6464 285b 7669 7369  _visit_add([visi
+0000ab00: 745d 290a 2020 2020 2020 2020 2020 2020  t]).            
+0000ab10: 2020 2020 2320 496e 2074 6869 7320 6361      # In this ca
+0000ab20: 7365 2c20 7765 2061 6c73 6f20 7761 6e74  se, we also want
+0000ab30: 2074 6f20 6372 6561 7465 2074 6865 2069   to create the i
+0000ab40: 6e69 7469 616c 204f 5653 206f 626a 6563  nitial OVS objec
+0000ab50: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+0000ab60: 2020 7669 7369 745f 7374 6174 7573 203d    visit_status =
+0000ab70: 204f 7269 6769 6e56 6973 6974 5374 6174   OriginVisitStat
+0000ab80: 7573 280a 2020 2020 2020 2020 2020 2020  us(.            
+0000ab90: 2020 2020 2020 2020 6f72 6967 696e 3d76          origin=v
+0000aba0: 6973 6974 2e6f 7269 6769 6e2c 0a20 2020  isit.origin,.   
+0000abb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000abc0: 2076 6973 6974 3d76 6973 6974 5f69 642c   visit=visit_id,
+0000abd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000abe0: 2020 2020 2064 6174 653d 7669 7369 742e       date=visit.
+0000abf0: 6461 7465 2c0a 2020 2020 2020 2020 2020  date,.          
+0000ac00: 2020 2020 2020 2020 2020 7479 7065 3d76            type=v
+0000ac10: 6973 6974 2e74 7970 652c 0a20 2020 2020  isit.type,.     
+0000ac20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000ac30: 7461 7475 733d 2263 7265 6174 6564 222c  tatus="created",
+0000ac40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ac50: 2020 2020 2073 6e61 7073 686f 743d 4e6f       snapshot=No
+0000ac60: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+0000ac70: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0000ac80: 2020 2020 2020 7365 6c66 2e5f 6f72 6967        self._orig
+0000ac90: 696e 5f76 6973 6974 5f73 7461 7475 735f  in_visit_status_
+0000aca0: 6164 6428 7669 7369 745f 7374 6174 7573  add(visit_status
+0000acb0: 2c20 6462 3d64 622c 2063 7572 3d63 7572  , db=db, cur=cur
+0000acc0: 290a 2020 2020 2020 2020 2020 2020 6173  ).            as
+0000acd0: 7365 7274 2076 6973 6974 2e76 6973 6974  sert visit.visit
+0000ace0: 2069 7320 6e6f 7420 4e6f 6e65 0a20 2020   is not None.   
+0000acf0: 2020 2020 2020 2020 2061 6c6c 5f76 6973           all_vis
+0000ad00: 6974 732e 6170 7065 6e64 2876 6973 6974  its.append(visit
+0000ad10: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+0000ad20: 6e20 616c 6c5f 7669 7369 7473 0a0a 2020  n all_visits..  
+0000ad30: 2020 6465 6620 5f6f 7269 6769 6e5f 7669    def _origin_vi
+0000ad40: 7369 745f 7374 6174 7573 5f61 6464 280a  sit_status_add(.
+0000ad50: 2020 2020 2020 2020 7365 6c66 2c20 7669          self, vi
+0000ad60: 7369 745f 7374 6174 7573 3a20 4f72 6967  sit_status: Orig
+0000ad70: 696e 5669 7369 7453 7461 7475 732c 2064  inVisitStatus, d
+0000ad80: 622c 2063 7572 0a20 2020 2029 202d 3e20  b, cur.    ) -> 
+0000ad90: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+0000ada0: 2241 6464 2061 6e20 6f72 6967 696e 2076  "Add an origin v
+0000adb0: 6973 6974 2073 7461 7475 7322 2222 0a20  isit status""". 
+0000adc0: 2020 2020 2020 2073 656c 662e 6a6f 7572         self.jour
+0000add0: 6e61 6c5f 7772 6974 6572 2e6f 7269 6769  nal_writer.origi
+0000ade0: 6e5f 7669 7369 745f 7374 6174 7573 5f61  n_visit_status_a
+0000adf0: 6464 285b 7669 7369 745f 7374 6174 7573  dd([visit_status
+0000ae00: 5d29 0a20 2020 2020 2020 2064 622e 6f72  ]).        db.or
+0000ae10: 6967 696e 5f76 6973 6974 5f73 7461 7475  igin_visit_statu
+0000ae20: 735f 6164 6428 7669 7369 745f 7374 6174  s_add(visit_stat
+0000ae30: 7573 2c20 6375 723d 6375 7229 0a0a 2020  us, cur=cur)..  
+0000ae40: 2020 4064 625f 7472 616e 7361 6374 696f    @db_transactio
+0000ae50: 6e28 290a 2020 2020 6465 6620 6f72 6967  n().    def orig
+0000ae60: 696e 5f76 6973 6974 5f73 7461 7475 735f  in_visit_status_
+0000ae70: 6164 6428 0a20 2020 2020 2020 2073 656c  add(.        sel
+0000ae80: 662c 0a20 2020 2020 2020 2076 6973 6974  f,.        visit
+0000ae90: 5f73 7461 7475 7365 733a 204c 6973 745b  _statuses: List[
+0000aea0: 4f72 6967 696e 5669 7369 7453 7461 7475  OriginVisitStatu
+0000aeb0: 735d 2c0a 2020 2020 2020 2020 2a2c 0a20  s],.        *,. 
+0000aec0: 2020 2020 2020 2064 623a 2044 622c 0a20         db: Db,. 
+0000aed0: 2020 2020 2020 2063 7572 3d4e 6f6e 652c         cur=None,
+0000aee0: 0a20 2020 2029 202d 3e20 4469 6374 5b73  .    ) -> Dict[s
+0000aef0: 7472 2c20 696e 745d 3a0a 2020 2020 2020  tr, int]:.      
+0000af00: 2020 7669 7369 745f 7374 6174 7573 6573    visit_statuses
+0000af10: 5f20 3d20 5b5d 0a0a 2020 2020 2020 2020  _ = []..        
+0000af20: 2320 4669 7273 7420 726f 756e 6420 746f  # First round to
+0000af30: 2063 6865 636b 2065 7869 7374 656e 6365   check existence
+0000af40: 2028 6661 696c 2065 6172 6c79 2069 6620   (fail early if 
+0000af50: 616e 7920 6973 206b 6f29 0a20 2020 2020  any is ko).     
+0000af60: 2020 2066 6f72 2076 6973 6974 5f73 7461     for visit_sta
+0000af70: 7475 7320 696e 2076 6973 6974 5f73 7461  tus in visit_sta
+0000af80: 7475 7365 733a 0a20 2020 2020 2020 2020  tuses:.         
+0000af90: 2020 206f 7269 6769 6e5f 7572 6c20 3d20     origin_url = 
+0000afa0: 7365 6c66 2e6f 7269 6769 6e5f 6765 7428  self.origin_get(
+0000afb0: 5b76 6973 6974 5f73 7461 7475 732e 6f72  [visit_status.or
+0000afc0: 6967 696e 5d2c 2064 623d 6462 2c20 6375  igin], db=db, cu
+0000afd0: 723d 6375 7229 5b30 5d0a 2020 2020 2020  r=cur)[0].      
+0000afe0: 2020 2020 2020 6966 206e 6f74 206f 7269        if not ori
+0000aff0: 6769 6e5f 7572 6c3a 0a20 2020 2020 2020  gin_url:.       
+0000b000: 2020 2020 2020 2020 2072 6169 7365 2053           raise S
+0000b010: 746f 7261 6765 4172 6775 6d65 6e74 4578  torageArgumentEx
+0000b020: 6365 7074 696f 6e28 6622 556e 6b6e 6f77  ception(f"Unknow
+0000b030: 6e20 6f72 6967 696e 207b 7669 7369 745f  n origin {visit_
+0000b040: 7374 6174 7573 2e6f 7269 6769 6e7d 2229  status.origin}")
+0000b050: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+0000b060: 2076 6973 6974 5f73 7461 7475 732e 7479   visit_status.ty
+0000b070: 7065 2069 7320 4e6f 6e65 3a0a 2020 2020  pe is None:.    
+0000b080: 2020 2020 2020 2020 2020 2020 6f72 6967              orig
+0000b090: 696e 5f76 6973 6974 203d 2073 656c 662e  in_visit = self.
+0000b0a0: 6f72 6967 696e 5f76 6973 6974 5f67 6574  origin_visit_get
+0000b0b0: 5f62 7928 0a20 2020 2020 2020 2020 2020  _by(.           
+0000b0c0: 2020 2020 2020 2020 2076 6973 6974 5f73           visit_s
+0000b0d0: 7461 7475 732e 6f72 6967 696e 2c20 7669  tatus.origin, vi
+0000b0e0: 7369 745f 7374 6174 7573 2e76 6973 6974  sit_status.visit
+0000b0f0: 2c20 6462 3d64 622c 2063 7572 3d63 7572  , db=db, cur=cur
+0000b100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b110: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+0000b120: 2020 2069 6620 6f72 6967 696e 5f76 6973     if origin_vis
+0000b130: 6974 2069 7320 4e6f 6e65 3a0a 2020 2020  it is None:.    
+0000b140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b150: 7261 6973 6520 5374 6f72 6167 6541 7267  raise StorageArg
+0000b160: 756d 656e 7445 7863 6570 7469 6f6e 280a  umentException(.
+0000b170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b180: 2020 2020 2020 2020 6622 556e 6b6e 6f77          f"Unknow
+0000b190: 6e20 6f72 6967 696e 2076 6973 6974 207b  n origin visit {
+0000b1a0: 7669 7369 745f 7374 6174 7573 2e76 6973  visit_status.vis
+0000b1b0: 6974 7d20 220a 2020 2020 2020 2020 2020  it} ".          
+0000b1c0: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+0000b1d0: 6f66 206f 7269 6769 6e20 7b76 6973 6974  of origin {visit
+0000b1e0: 5f73 7461 7475 732e 6f72 6967 696e 7d22  _status.origin}"
+0000b1f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b200: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+0000b210: 2020 2020 2020 2020 6f72 6967 696e 5f76          origin_v
+0000b220: 6973 6974 5f73 7461 7475 7320 3d20 6174  isit_status = at
+0000b230: 7472 2e65 766f 6c76 6528 7669 7369 745f  tr.evolve(visit_
+0000b240: 7374 6174 7573 2c20 7479 7065 3d6f 7269  status, type=ori
+0000b250: 6769 6e5f 7669 7369 742e 7479 7065 290a  gin_visit.type).
+0000b260: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0000b270: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000b280: 2020 6f72 6967 696e 5f76 6973 6974 5f73    origin_visit_s
+0000b290: 7461 7475 7320 3d20 7669 7369 745f 7374  tatus = visit_st
+0000b2a0: 6174 7573 0a0a 2020 2020 2020 2020 2020  atus..          
+0000b2b0: 2020 7669 7369 745f 7374 6174 7573 6573    visit_statuses
+0000b2c0: 5f2e 6170 7065 6e64 286f 7269 6769 6e5f  _.append(origin_
+0000b2d0: 7669 7369 745f 7374 6174 7573 290a 0a20  visit_status).. 
+0000b2e0: 2020 2020 2020 2066 6f72 2076 6973 6974         for visit
+0000b2f0: 5f73 7461 7475 7320 696e 2076 6973 6974  _status in visit
+0000b300: 5f73 7461 7475 7365 735f 3a0a 2020 2020  _statuses_:.    
+0000b310: 2020 2020 2020 2020 7365 6c66 2e5f 6f72          self._or
+0000b320: 6967 696e 5f76 6973 6974 5f73 7461 7475  igin_visit_statu
+0000b330: 735f 6164 6428 7669 7369 745f 7374 6174  s_add(visit_stat
+0000b340: 7573 2c20 6462 2c20 6375 7229 0a20 2020  us, db, cur).   
+0000b350: 2020 2020 2072 6574 7572 6e20 7b22 6f72       return {"or
+0000b360: 6967 696e 5f76 6973 6974 5f73 7461 7475  igin_visit_statu
+0000b370: 733a 6164 6422 3a20 6c65 6e28 7669 7369  s:add": len(visi
+0000b380: 745f 7374 6174 7573 6573 5f29 7d0a 0a20  t_statuses_)}.. 
+0000b390: 2020 2040 6462 5f74 7261 6e73 6163 7469     @db_transacti
+0000b3a0: 6f6e 2829 0a20 2020 2064 6566 206f 7269  on().    def ori
+0000b3b0: 6769 6e5f 7669 7369 745f 7374 6174 7573  gin_visit_status
+0000b3c0: 5f67 6574 5f6c 6174 6573 7428 0a20 2020  _get_latest(.   
+0000b3d0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0000b3e0: 2020 206f 7269 6769 6e5f 7572 6c3a 2073     origin_url: s
+0000b3f0: 7472 2c0a 2020 2020 2020 2020 7669 7369  tr,.        visi
+0000b400: 743a 2069 6e74 2c0a 2020 2020 2020 2020  t: int,.        
+0000b410: 616c 6c6f 7765 645f 7374 6174 7573 6573  allowed_statuses
+0000b420: 3a20 4f70 7469 6f6e 616c 5b4c 6973 745b  : Optional[List[
+0000b430: 7374 725d 5d20 3d20 4e6f 6e65 2c0a 2020  str]] = None,.  
+0000b440: 2020 2020 2020 7265 7175 6972 655f 736e        require_sn
+0000b450: 6170 7368 6f74 3a20 626f 6f6c 203d 2046  apshot: bool = F
+0000b460: 616c 7365 2c0a 2020 2020 2020 2020 2a2c  alse,.        *,
+0000b470: 0a20 2020 2020 2020 2064 623a 2044 622c  .        db: Db,
+0000b480: 0a20 2020 2020 2020 2063 7572 3d4e 6f6e  .        cur=Non
+0000b490: 652c 0a20 2020 2029 202d 3e20 4f70 7469  e,.    ) -> Opti
+0000b4a0: 6f6e 616c 5b4f 7269 6769 6e56 6973 6974  onal[OriginVisit
+0000b4b0: 5374 6174 7573 5d3a 0a20 2020 2020 2020  Status]:.       
+0000b4c0: 2069 6620 616c 6c6f 7765 645f 7374 6174   if allowed_stat
+0000b4d0: 7573 6573 2061 6e64 206e 6f74 2073 6574  uses and not set
+0000b4e0: 2861 6c6c 6f77 6564 5f73 7461 7475 7365  (allowed_statuse
+0000b4f0: 7329 2e69 6e74 6572 7365 6374 696f 6e28  s).intersection(
+0000b500: 5649 5349 545f 5354 4154 5553 4553 293a  VISIT_STATUSES):
+0000b510: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+0000b520: 7365 2053 746f 7261 6765 4172 6775 6d65  se StorageArgume
+0000b530: 6e74 4578 6365 7074 696f 6e28 0a20 2020  ntException(.   
+0000b540: 2020 2020 2020 2020 2020 2020 2066 2255               f"U
+0000b550: 6e6b 6e6f 776e 2061 6c6c 6f77 6564 2073  nknown allowed s
+0000b560: 7461 7475 7365 7320 7b27 2c27 2e6a 6f69  tatuses {','.joi
+0000b570: 6e28 616c 6c6f 7765 645f 7374 6174 7573  n(allowed_status
+0000b580: 6573 297d 2c20 6f6e 6c79 2022 0a20 2020  es)}, only ".   
+0000b590: 2020 2020 2020 2020 2020 2020 2066 227b               f"{
+0000b5a0: 272c 272e 6a6f 696e 2856 4953 4954 5f53  ','.join(VISIT_S
+0000b5b0: 5441 5455 5345 5329 7d20 6175 7468 6f72  TATUSES)} author
+0000b5c0: 697a 6564 220a 2020 2020 2020 2020 2020  ized".          
+0000b5d0: 2020 290a 0a20 2020 2020 2020 2072 6f77    )..        row
+0000b5e0: 5f64 203d 2064 622e 6f72 6967 696e 5f76  _d = db.origin_v
+0000b5f0: 6973 6974 5f73 7461 7475 735f 6765 745f  isit_status_get_
+0000b600: 6c61 7465 7374 280a 2020 2020 2020 2020  latest(.        
+0000b610: 2020 2020 6f72 6967 696e 5f75 726c 2c20      origin_url, 
+0000b620: 7669 7369 742c 2061 6c6c 6f77 6564 5f73  visit, allowed_s
+0000b630: 7461 7475 7365 732c 2072 6571 7569 7265  tatuses, require
+0000b640: 5f73 6e61 7073 686f 742c 2063 7572 3d63  _snapshot, cur=c
+0000b650: 7572 0a20 2020 2020 2020 2029 0a20 2020  ur.        ).   
+0000b660: 2020 2020 2069 6620 6e6f 7420 726f 775f       if not row_
+0000b670: 643a 0a20 2020 2020 2020 2020 2020 2072  d:.            r
+0000b680: 6574 7572 6e20 4e6f 6e65 0a20 2020 2020  eturn None.     
+0000b690: 2020 2072 6574 7572 6e20 4f72 6967 696e     return Origin
+0000b6a0: 5669 7369 7453 7461 7475 7328 2a2a 726f  VisitStatus(**ro
+0000b6b0: 775f 6429 0a0a 2020 2020 4064 625f 7472  w_d)..    @db_tr
+0000b6c0: 616e 7361 6374 696f 6e28 7374 6174 656d  ansaction(statem
+0000b6d0: 656e 745f 7469 6d65 6f75 743d 3530 3029  ent_timeout=500)
+0000b6e0: 0a20 2020 2064 6566 206f 7269 6769 6e5f  .    def origin_
+0000b6f0: 7669 7369 745f 6765 7428 0a20 2020 2020  visit_get(.     
+0000b700: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+0000b710: 206f 7269 6769 6e3a 2073 7472 2c0a 2020   origin: str,.  
+0000b720: 2020 2020 2020 7061 6765 5f74 6f6b 656e        page_token
+0000b730: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+0000b740: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0000b750: 6f72 6465 723a 204c 6973 744f 7264 6572  order: ListOrder
+0000b760: 203d 204c 6973 744f 7264 6572 2e41 5343   = ListOrder.ASC
+0000b770: 2c0a 2020 2020 2020 2020 6c69 6d69 743a  ,.        limit:
+0000b780: 2069 6e74 203d 2031 302c 0a20 2020 2020   int = 10,.     
+0000b790: 2020 202a 2c0a 2020 2020 2020 2020 6462     *,.        db
+0000b7a0: 3a20 4462 2c0a 2020 2020 2020 2020 6375  : Db,.        cu
+0000b7b0: 723d 4e6f 6e65 2c0a 2020 2020 2920 2d3e  r=None,.    ) ->
+0000b7c0: 2050 6167 6564 5265 7375 6c74 5b4f 7269   PagedResult[Ori
+0000b7d0: 6769 6e56 6973 6974 5d3a 0a20 2020 2020  ginVisit]:.     
+0000b7e0: 2020 2070 6167 655f 746f 6b65 6e20 3d20     page_token = 
+0000b7f0: 7061 6765 5f74 6f6b 656e 206f 7220 2230  page_token or "0
+0000b800: 220a 2020 2020 2020 2020 6966 206e 6f74  ".        if not
+0000b810: 2069 7369 6e73 7461 6e63 6528 6f72 6465   isinstance(orde
+0000b820: 722c 204c 6973 744f 7264 6572 293a 0a20  r, ListOrder):. 
+0000b830: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+0000b840: 2053 746f 7261 6765 4172 6775 6d65 6e74   StorageArgument
+0000b850: 4578 6365 7074 696f 6e28 226f 7264 6572  Exception("order
+0000b860: 206d 7573 7420 6265 2061 204c 6973 744f   must be a ListO
+0000b870: 7264 6572 2076 616c 7565 2229 0a20 2020  rder value").   
+0000b880: 2020 2020 2069 6620 6e6f 7420 6973 696e       if not isin
+0000b890: 7374 616e 6365 2870 6167 655f 746f 6b65  stance(page_toke
+0000b8a0: 6e2c 2073 7472 293a 0a20 2020 2020 2020  n, str):.       
+0000b8b0: 2020 2020 2072 6169 7365 2053 746f 7261       raise Stora
+0000b8c0: 6765 4172 6775 6d65 6e74 4578 6365 7074  geArgumentExcept
+0000b8d0: 696f 6e28 2270 6167 655f 746f 6b65 6e20  ion("page_token 
+0000b8e0: 6d75 7374 2062 6520 6120 7374 7269 6e67  must be a string
+0000b8f0: 2e22 290a 0a20 2020 2020 2020 206e 6578  .")..        nex
+0000b900: 745f 7061 6765 5f74 6f6b 656e 203d 204e  t_page_token = N
+0000b910: 6f6e 650a 2020 2020 2020 2020 7669 7369  one.        visi
+0000b920: 745f 6672 6f6d 203d 2069 6e74 2870 6167  t_from = int(pag
+0000b930: 655f 746f 6b65 6e29 0a20 2020 2020 2020  e_token).       
+0000b940: 2076 6973 6974 733a 204c 6973 745b 4f72   visits: List[Or
+0000b950: 6967 696e 5669 7369 745d 203d 205b 5d0a  iginVisit] = [].
+0000b960: 2020 2020 2020 2020 6578 7472 615f 6c69          extra_li
+0000b970: 6d69 7420 3d20 6c69 6d69 7420 2b20 310a  mit = limit + 1.
+0000b980: 2020 2020 2020 2020 666f 7220 726f 7720          for row 
+0000b990: 696e 2064 622e 6f72 6967 696e 5f76 6973  in db.origin_vis
+0000b9a0: 6974 5f67 6574 5f72 616e 6765 280a 2020  it_get_range(.  
+0000b9b0: 2020 2020 2020 2020 2020 6f72 6967 696e            origin
+0000b9c0: 2c20 7669 7369 745f 6672 6f6d 3d76 6973  , visit_from=vis
+0000b9d0: 6974 5f66 726f 6d2c 206f 7264 6572 3d6f  it_from, order=o
+0000b9e0: 7264 6572 2c20 6c69 6d69 743d 6578 7472  rder, limit=extr
+0000b9f0: 615f 6c69 6d69 742c 2063 7572 3d63 7572  a_limit, cur=cur
+0000ba00: 0a20 2020 2020 2020 2029 3a0a 2020 2020  .        ):.    
+0000ba10: 2020 2020 2020 2020 726f 775f 6420 3d20          row_d = 
+0000ba20: 6469 6374 287a 6970 2864 622e 6f72 6967  dict(zip(db.orig
+0000ba30: 696e 5f76 6973 6974 5f63 6f6c 732c 2072  in_visit_cols, r
+0000ba40: 6f77 2929 0a20 2020 2020 2020 2020 2020  ow)).           
+0000ba50: 2076 6973 6974 732e 6170 7065 6e64 280a   visits.append(.
 0000ba60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba70: 206f 7269 6769 6e3d 726f 775f 645b 226f   origin=row_d["o
-0000ba80: 7269 6769 6e22 5d2c 0a20 2020 2020 2020  rigin"],.       
-0000ba90: 2020 2020 2020 2020 2020 2020 2076 6973               vis
-0000baa0: 6974 3d72 6f77 5f64 5b22 7669 7369 7422  it=row_d["visit"
-0000bab0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-0000bac0: 2020 2020 2020 2064 6174 653d 726f 775f         date=row_
-0000bad0: 645b 2264 6174 6522 5d2c 0a20 2020 2020  d["date"],.     
-0000bae0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000baf0: 7970 653d 726f 775f 645b 2274 7970 6522  ype=row_d["type"
-0000bb00: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-0000bb10: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0000bb20: 2029 0a0a 2020 2020 2020 2020 6173 7365   )..        asse
-0000bb30: 7274 206c 656e 2876 6973 6974 7329 203c  rt len(visits) <
-0000bb40: 3d20 6578 7472 615f 6c69 6d69 740a 0a20  = extra_limit.. 
-0000bb50: 2020 2020 2020 2069 6620 6c65 6e28 7669         if len(vi
-0000bb60: 7369 7473 2920 3d3d 2065 7874 7261 5f6c  sits) == extra_l
-0000bb70: 696d 6974 3a0a 2020 2020 2020 2020 2020  imit:.          
-0000bb80: 2020 7669 7369 7473 203d 2076 6973 6974    visits = visit
-0000bb90: 735b 3a6c 696d 6974 5d0a 2020 2020 2020  s[:limit].      
-0000bba0: 2020 2020 2020 6e65 7874 5f70 6167 655f        next_page_
-0000bbb0: 746f 6b65 6e20 3d20 7374 7228 7669 7369  token = str(visi
-0000bbc0: 7473 5b2d 315d 2e76 6973 6974 290a 0a20  ts[-1].visit).. 
-0000bbd0: 2020 2020 2020 2072 6574 7572 6e20 5061         return Pa
-0000bbe0: 6765 6452 6573 756c 7428 7265 7375 6c74  gedResult(result
-0000bbf0: 733d 7669 7369 7473 2c20 6e65 7874 5f70  s=visits, next_p
-0000bc00: 6167 655f 746f 6b65 6e3d 6e65 7874 5f70  age_token=next_p
-0000bc10: 6167 655f 746f 6b65 6e29 0a0a 2020 2020  age_token)..    
-0000bc20: 4064 625f 7472 616e 7361 6374 696f 6e28  @db_transaction(
-0000bc30: 7374 6174 656d 656e 745f 7469 6d65 6f75  statement_timeou
-0000bc40: 743d 3230 3030 290a 2020 2020 6465 6620  t=2000).    def 
-0000bc50: 6f72 6967 696e 5f76 6973 6974 5f67 6574  origin_visit_get
-0000bc60: 5f77 6974 685f 7374 6174 7573 6573 280a  _with_statuses(.
-0000bc70: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-0000bc80: 2020 2020 2020 6f72 6967 696e 3a20 7374        origin: st
-0000bc90: 722c 0a20 2020 2020 2020 2061 6c6c 6f77  r,.        allow
-0000bca0: 6564 5f73 7461 7475 7365 733a 204f 7074  ed_statuses: Opt
-0000bcb0: 696f 6e61 6c5b 4c69 7374 5b73 7472 5d5d  ional[List[str]]
-0000bcc0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0000bcd0: 2072 6571 7569 7265 5f73 6e61 7073 686f   require_snapsho
-0000bce0: 743a 2062 6f6f 6c20 3d20 4661 6c73 652c  t: bool = False,
-0000bcf0: 0a20 2020 2020 2020 2070 6167 655f 746f  .        page_to
-0000bd00: 6b65 6e3a 204f 7074 696f 6e61 6c5b 7374  ken: Optional[st
-0000bd10: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-0000bd20: 2020 206f 7264 6572 3a20 4c69 7374 4f72     order: ListOr
-0000bd30: 6465 7220 3d20 4c69 7374 4f72 6465 722e  der = ListOrder.
-0000bd40: 4153 432c 0a20 2020 2020 2020 206c 696d  ASC,.        lim
-0000bd50: 6974 3a20 696e 7420 3d20 3130 2c0a 2020  it: int = 10,.  
-0000bd60: 2020 2020 2020 2a2c 0a20 2020 2020 2020        *,.       
-0000bd70: 2064 623a 2044 622c 0a20 2020 2020 2020   db: Db,.       
-0000bd80: 2063 7572 3d4e 6f6e 652c 0a20 2020 2029   cur=None,.    )
-0000bd90: 202d 3e20 5061 6765 6452 6573 756c 745b   -> PagedResult[
-0000bda0: 4f72 6967 696e 5669 7369 7457 6974 6853  OriginVisitWithS
-0000bdb0: 7461 7475 7365 735d 3a0a 2020 2020 2020  tatuses]:.      
-0000bdc0: 2020 7061 6765 5f74 6f6b 656e 203d 2070    page_token = p
-0000bdd0: 6167 655f 746f 6b65 6e20 6f72 2022 3022  age_token or "0"
-0000bde0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-0000bdf0: 6973 696e 7374 616e 6365 286f 7264 6572  isinstance(order
-0000be00: 2c20 4c69 7374 4f72 6465 7229 3a0a 2020  , ListOrder):.  
-0000be10: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000be20: 5374 6f72 6167 6541 7267 756d 656e 7445  StorageArgumentE
-0000be30: 7863 6570 7469 6f6e 2822 6f72 6465 7220  xception("order 
-0000be40: 6d75 7374 2062 6520 6120 4c69 7374 4f72  must be a ListOr
-0000be50: 6465 7220 7661 6c75 6522 290a 2020 2020  der value").    
-0000be60: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
-0000be70: 7461 6e63 6528 7061 6765 5f74 6f6b 656e  tance(page_token
-0000be80: 2c20 7374 7229 3a0a 2020 2020 2020 2020  , str):.        
-0000be90: 2020 2020 7261 6973 6520 5374 6f72 6167      raise Storag
-0000bea0: 6541 7267 756d 656e 7445 7863 6570 7469  eArgumentExcepti
-0000beb0: 6f6e 2822 7061 6765 5f74 6f6b 656e 206d  on("page_token m
-0000bec0: 7573 7420 6265 2061 2073 7472 696e 672e  ust be a string.
-0000bed0: 2229 0a0a 2020 2020 2020 2020 2320 4669  ")..        # Fi
-0000bee0: 7273 7420 6765 7420 7669 7369 7473 2028  rst get visits (
-0000bef0: 706c 7573 206f 6e65 2073 6f20 7765 2063  plus one so we c
-0000bf00: 616e 2075 7365 2069 7420 6173 2074 6865  an use it as the
-0000bf10: 206e 6578 7420 7061 6765 2074 6f6b 656e   next page token
-0000bf20: 2069 6620 616e 7929 0a20 2020 2020 2020   if any).       
-0000bf30: 2076 6973 6974 735f 7061 6765 203d 2073   visits_page = s
-0000bf40: 656c 662e 6f72 6967 696e 5f76 6973 6974  elf.origin_visit
-0000bf50: 5f67 6574 280a 2020 2020 2020 2020 2020  _get(.          
-0000bf60: 2020 6f72 6967 696e 3d6f 7269 6769 6e2c    origin=origin,
-0000bf70: 0a20 2020 2020 2020 2020 2020 2070 6167  .            pag
-0000bf80: 655f 746f 6b65 6e3d 7061 6765 5f74 6f6b  e_token=page_tok
-0000bf90: 656e 2c0a 2020 2020 2020 2020 2020 2020  en,.            
-0000bfa0: 6f72 6465 723d 6f72 6465 722c 0a20 2020  order=order,.   
-0000bfb0: 2020 2020 2020 2020 206c 696d 6974 3d6c           limit=l
-0000bfc0: 696d 6974 2c0a 2020 2020 2020 2020 2020  imit,.          
-0000bfd0: 2020 6462 3d64 622c 0a20 2020 2020 2020    db=db,.       
-0000bfe0: 2020 2020 2063 7572 3d63 7572 2c0a 2020       cur=cur,.  
-0000bff0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-0000c000: 2076 6973 6974 7320 3d20 7669 7369 7473   visits = visits
-0000c010: 5f70 6167 652e 7265 7375 6c74 730a 2020  _page.results.  
-0000c020: 2020 2020 2020 6e65 7874 5f70 6167 655f        next_page_
-0000c030: 746f 6b65 6e20 3d20 7669 7369 7473 5f70  token = visits_p
-0000c040: 6167 652e 6e65 7874 5f70 6167 655f 746f  age.next_page_to
-0000c050: 6b65 6e0a 0a20 2020 2020 2020 2069 6620  ken..        if 
-0000c060: 7669 7369 7473 3a0a 2020 2020 2020 2020  visits:.        
-0000c070: 2020 2020 7669 7369 745f 6672 6f6d 203d      visit_from =
-0000c080: 206d 696e 2876 6973 6974 735b 305d 2e76   min(visits[0].v
-0000c090: 6973 6974 2c20 7669 7369 7473 5b2d 315d  isit, visits[-1]
-0000c0a0: 2e76 6973 6974 290a 2020 2020 2020 2020  .visit).        
-0000c0b0: 2020 2020 7669 7369 745f 746f 203d 206d      visit_to = m
-0000c0c0: 6178 2876 6973 6974 735b 305d 2e76 6973  ax(visits[0].vis
-0000c0d0: 6974 2c20 7669 7369 7473 5b2d 315d 2e76  it, visits[-1].v
-0000c0e0: 6973 6974 290a 0a20 2020 2020 2020 2020  isit)..         
-0000c0f0: 2020 2023 2054 6865 6e2c 2066 6574 6368     # Then, fetch
-0000c100: 2061 6c6c 2073 7461 7475 7365 7320 6173   all statuses as
-0000c110: 736f 6369 6174 6564 2074 6f20 7468 6573  sociated to thes
-0000c120: 6520 7669 7369 7473 0a20 2020 2020 2020  e visits.       
-0000c130: 2020 2020 2076 6973 6974 5f73 7461 7475       visit_statu
-0000c140: 7365 733a 2044 6963 745b 696e 742c 204c  ses: Dict[int, L
-0000c150: 6973 745b 4f72 6967 696e 5669 7369 7453  ist[OriginVisitS
-0000c160: 7461 7475 735d 5d20 3d20 6465 6661 756c  tatus]] = defaul
-0000c170: 7464 6963 7428 6c69 7374 290a 2020 2020  tdict(list).    
-0000c180: 2020 2020 2020 2020 666f 7220 726f 7720          for row 
-0000c190: 696e 2064 622e 6f72 6967 696e 5f76 6973  in db.origin_vis
-0000c1a0: 6974 5f73 7461 7475 735f 6765 745f 616c  it_status_get_al
-0000c1b0: 6c5f 696e 5f72 616e 6765 280a 2020 2020  l_in_range(.    
-0000c1c0: 2020 2020 2020 2020 2020 2020 6f72 6967              orig
-0000c1d0: 696e 2c0a 2020 2020 2020 2020 2020 2020  in,.            
-0000c1e0: 2020 2020 616c 6c6f 7765 645f 7374 6174      allowed_stat
-0000c1f0: 7573 6573 2c0a 2020 2020 2020 2020 2020  uses,.          
-0000c200: 2020 2020 2020 7265 7175 6972 655f 736e        require_sn
-0000c210: 6170 7368 6f74 2c0a 2020 2020 2020 2020  apshot,.        
-0000c220: 2020 2020 2020 2020 7669 7369 745f 6672          visit_fr
-0000c230: 6f6d 3d76 6973 6974 5f66 726f 6d2c 0a20  om=visit_from,. 
-0000c240: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-0000c250: 6973 6974 5f74 6f3d 7669 7369 745f 746f  isit_to=visit_to
-0000c260: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000c270: 2020 6375 723d 6375 722c 0a20 2020 2020    cur=cur,.     
-0000c280: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
-0000c290: 2020 2020 2020 2020 2020 726f 775f 6420            row_d 
-0000c2a0: 3d20 6469 6374 287a 6970 2864 622e 6f72  = dict(zip(db.or
-0000c2b0: 6967 696e 5f76 6973 6974 5f73 7461 7475  igin_visit_statu
-0000c2c0: 735f 636f 6c73 2c20 726f 7729 290a 0a20  s_cols, row)).. 
-0000c2d0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-0000c2e0: 6973 6974 5f73 7461 7475 7365 735b 726f  isit_statuses[ro
-0000c2f0: 775f 645b 2276 6973 6974 225d 5d2e 6170  w_d["visit"]].ap
-0000c300: 7065 6e64 284f 7269 6769 6e56 6973 6974  pend(OriginVisit
-0000c310: 5374 6174 7573 282a 2a72 6f77 5f64 2929  Status(**row_d))
-0000c320: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-0000c330: 7320 3d20 5b0a 2020 2020 2020 2020 2020  s = [.          
-0000c340: 2020 4f72 6967 696e 5669 7369 7457 6974    OriginVisitWit
-0000c350: 6853 7461 7475 7365 7328 7669 7369 743d  hStatuses(visit=
-0000c360: 7669 7369 742c 2073 7461 7475 7365 733d  visit, statuses=
-0000c370: 7669 7369 745f 7374 6174 7573 6573 5b76  visit_statuses[v
-0000c380: 6973 6974 2e76 6973 6974 5d29 0a20 2020  isit.visit]).   
-0000c390: 2020 2020 2020 2020 2066 6f72 2076 6973           for vis
-0000c3a0: 6974 2069 6e20 7669 7369 7473 0a20 2020  it in visits.   
-0000c3b0: 2020 2020 205d 0a0a 2020 2020 2020 2020       ]..        
-0000c3c0: 7265 7475 726e 2050 6167 6564 5265 7375  return PagedResu
-0000c3d0: 6c74 2872 6573 756c 7473 3d72 6573 756c  lt(results=resul
-0000c3e0: 7473 2c20 6e65 7874 5f70 6167 655f 746f  ts, next_page_to
-0000c3f0: 6b65 6e3d 6e65 7874 5f70 6167 655f 746f  ken=next_page_to
-0000c400: 6b65 6e29 0a0a 2020 2020 4064 625f 7472  ken)..    @db_tr
-0000c410: 616e 7361 6374 696f 6e28 7374 6174 656d  ansaction(statem
-0000c420: 656e 745f 7469 6d65 6f75 743d 3230 3030  ent_timeout=2000
-0000c430: 290a 2020 2020 6465 6620 6f72 6967 696e  ).    def origin
-0000c440: 5f76 6973 6974 5f66 696e 645f 6279 5f64  _visit_find_by_d
-0000c450: 6174 6528 0a20 2020 2020 2020 2073 656c  ate(.        sel
-0000c460: 662c 0a20 2020 2020 2020 206f 7269 6769  f,.        origi
-0000c470: 6e3a 2073 7472 2c0a 2020 2020 2020 2020  n: str,.        
-0000c480: 7669 7369 745f 6461 7465 3a20 6461 7465  visit_date: date
-0000c490: 7469 6d65 2e64 6174 6574 696d 652c 0a20  time.datetime,. 
-0000c4a0: 2020 2020 2020 2074 7970 653a 204f 7074         type: Opt
-0000c4b0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-0000c4c0: 652c 0a20 2020 2020 2020 202a 2c0a 2020  e,.        *,.  
-0000c4d0: 2020 2020 2020 6462 3a20 4462 2c0a 2020        db: Db,.  
-0000c4e0: 2020 2020 2020 6375 723d 4e6f 6e65 2c0a        cur=None,.
-0000c4f0: 2020 2020 2920 2d3e 204f 7074 696f 6e61      ) -> Optiona
-0000c500: 6c5b 4f72 6967 696e 5669 7369 745d 3a0a  l[OriginVisit]:.
-0000c510: 2020 2020 2020 2020 726f 775f 6420 3d20          row_d = 
-0000c520: 6462 2e6f 7269 6769 6e5f 7669 7369 745f  db.origin_visit_
-0000c530: 6669 6e64 5f62 795f 6461 7465 286f 7269  find_by_date(ori
-0000c540: 6769 6e2c 2076 6973 6974 5f64 6174 652c  gin, visit_date,
-0000c550: 2074 7970 653d 7479 7065 2c20 6375 723d   type=type, cur=
-0000c560: 6375 7229 0a20 2020 2020 2020 2069 6620  cur).        if 
-0000c570: 6e6f 7420 726f 775f 643a 0a20 2020 2020  not row_d:.     
-0000c580: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
-0000c590: 6e65 0a20 2020 2020 2020 2072 6574 7572  ne.        retur
-0000c5a0: 6e20 4f72 6967 696e 5669 7369 7428 0a20  n OriginVisit(. 
-0000c5b0: 2020 2020 2020 2020 2020 206f 7269 6769             origi
-0000c5c0: 6e3d 726f 775f 645b 226f 7269 6769 6e22  n=row_d["origin"
-0000c5d0: 5d2c 0a20 2020 2020 2020 2020 2020 2076  ],.            v
-0000c5e0: 6973 6974 3d72 6f77 5f64 5b22 7669 7369  isit=row_d["visi
-0000c5f0: 7422 5d2c 0a20 2020 2020 2020 2020 2020  t"],.           
-0000c600: 2064 6174 653d 726f 775f 645b 2264 6174   date=row_d["dat
-0000c610: 6522 5d2c 0a20 2020 2020 2020 2020 2020  e"],.           
-0000c620: 2074 7970 653d 726f 775f 645b 2274 7970   type=row_d["typ
-0000c630: 6522 5d2c 0a20 2020 2020 2020 2029 0a0a  e"],.        )..
-0000c640: 2020 2020 4064 625f 7472 616e 7361 6374      @db_transact
-0000c650: 696f 6e28 7374 6174 656d 656e 745f 7469  ion(statement_ti
-0000c660: 6d65 6f75 743d 3530 3029 0a20 2020 2064  meout=500).    d
-0000c670: 6566 206f 7269 6769 6e5f 7669 7369 745f  ef origin_visit_
-0000c680: 6765 745f 6279 280a 2020 2020 2020 2020  get_by(.        
-0000c690: 7365 6c66 2c20 6f72 6967 696e 3a20 7374  self, origin: st
-0000c6a0: 722c 2076 6973 6974 3a20 696e 742c 202a  r, visit: int, *
-0000c6b0: 2c20 6462 3a20 4462 2c20 6375 723d 4e6f  , db: Db, cur=No
-0000c6c0: 6e65 0a20 2020 2029 202d 3e20 4f70 7469  ne.    ) -> Opti
-0000c6d0: 6f6e 616c 5b4f 7269 6769 6e56 6973 6974  onal[OriginVisit
-0000c6e0: 5d3a 0a20 2020 2020 2020 2072 6f77 203d  ]:.        row =
-0000c6f0: 2064 622e 6f72 6967 696e 5f76 6973 6974   db.origin_visit
-0000c700: 5f67 6574 286f 7269 6769 6e2c 2076 6973  _get(origin, vis
-0000c710: 6974 2c20 6375 7229 0a20 2020 2020 2020  it, cur).       
-0000c720: 2069 6620 726f 773a 0a20 2020 2020 2020   if row:.       
-0000c730: 2020 2020 2072 6f77 5f64 203d 2064 6963       row_d = dic
-0000c740: 7428 7a69 7028 6462 2e6f 7269 6769 6e5f  t(zip(db.origin_
-0000c750: 7669 7369 745f 6765 745f 636f 6c73 2c20  visit_get_cols, 
-0000c760: 726f 7729 290a 2020 2020 2020 2020 2020  row)).          
-0000c770: 2020 7265 7475 726e 204f 7269 6769 6e56    return OriginV
-0000c780: 6973 6974 280a 2020 2020 2020 2020 2020  isit(.          
-0000c790: 2020 2020 2020 6f72 6967 696e 3d72 6f77        origin=row
-0000c7a0: 5f64 5b22 6f72 6967 696e 225d 2c0a 2020  _d["origin"],.  
-0000c7b0: 2020 2020 2020 2020 2020 2020 2020 7669                vi
-0000c7c0: 7369 743d 726f 775f 645b 2276 6973 6974  sit=row_d["visit
-0000c7d0: 225d 2c0a 2020 2020 2020 2020 2020 2020  "],.            
-0000c7e0: 2020 2020 6461 7465 3d72 6f77 5f64 5b22      date=row_d["
-0000c7f0: 6461 7465 225d 2c0a 2020 2020 2020 2020  date"],.        
-0000c800: 2020 2020 2020 2020 7479 7065 3d72 6f77          type=row
-0000c810: 5f64 5b22 7479 7065 225d 2c0a 2020 2020  _d["type"],.    
-0000c820: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000c830: 2020 7265 7475 726e 204e 6f6e 650a 0a20    return None.. 
-0000c840: 2020 2040 6462 5f74 7261 6e73 6163 7469     @db_transacti
-0000c850: 6f6e 2873 7461 7465 6d65 6e74 5f74 696d  on(statement_tim
-0000c860: 656f 7574 3d34 3030 3029 0a20 2020 2064  eout=4000).    d
-0000c870: 6566 206f 7269 6769 6e5f 7669 7369 745f  ef origin_visit_
-0000c880: 6765 745f 6c61 7465 7374 280a 2020 2020  get_latest(.    
-0000c890: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0000c8a0: 2020 6f72 6967 696e 3a20 7374 722c 0a20    origin: str,. 
-0000c8b0: 2020 2020 2020 2074 7970 653a 204f 7074         type: Opt
-0000c8c0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-0000c8d0: 652c 0a20 2020 2020 2020 2061 6c6c 6f77  e,.        allow
-0000c8e0: 6564 5f73 7461 7475 7365 733a 204f 7074  ed_statuses: Opt
-0000c8f0: 696f 6e61 6c5b 4c69 7374 5b73 7472 5d5d  ional[List[str]]
-0000c900: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0000c910: 2072 6571 7569 7265 5f73 6e61 7073 686f   require_snapsho
-0000c920: 743a 2062 6f6f 6c20 3d20 4661 6c73 652c  t: bool = False,
-0000c930: 0a20 2020 2020 2020 202a 2c0a 2020 2020  .        *,.    
-0000c940: 2020 2020 6462 3a20 4462 2c0a 2020 2020      db: Db,.    
-0000c950: 2020 2020 6375 723d 4e6f 6e65 2c0a 2020      cur=None,.  
-0000c960: 2020 2920 2d3e 204f 7074 696f 6e61 6c5b    ) -> Optional[
-0000c970: 4f72 6967 696e 5669 7369 745d 3a0a 2020  OriginVisit]:.  
-0000c980: 2020 2020 2020 6966 2061 6c6c 6f77 6564        if allowed
-0000c990: 5f73 7461 7475 7365 7320 616e 6420 6e6f  _statuses and no
-0000c9a0: 7420 7365 7428 616c 6c6f 7765 645f 7374  t set(allowed_st
-0000c9b0: 6174 7573 6573 292e 696e 7465 7273 6563  atuses).intersec
-0000c9c0: 7469 6f6e 2856 4953 4954 5f53 5441 5455  tion(VISIT_STATU
-0000c9d0: 5345 5329 3a0a 2020 2020 2020 2020 2020  SES):.          
-0000c9e0: 2020 7261 6973 6520 5374 6f72 6167 6541    raise StorageA
-0000c9f0: 7267 756d 656e 7445 7863 6570 7469 6f6e  rgumentException
-0000ca00: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000ca10: 2020 6622 556e 6b6e 6f77 6e20 616c 6c6f    f"Unknown allo
-0000ca20: 7765 6420 7374 6174 7573 6573 207b 272c  wed statuses {',
-0000ca30: 272e 6a6f 696e 2861 6c6c 6f77 6564 5f73  '.join(allowed_s
-0000ca40: 7461 7475 7365 7329 7d2c 206f 6e6c 7920  tatuses)}, only 
-0000ca50: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0000ca60: 2020 6622 7b27 2c27 2e6a 6f69 6e28 5649    f"{','.join(VI
-0000ca70: 5349 545f 5354 4154 5553 4553 297d 2061  SIT_STATUSES)} a
-0000ca80: 7574 686f 7269 7a65 6422 0a20 2020 2020  uthorized".     
-0000ca90: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-0000caa0: 2020 726f 7720 3d20 6462 2e6f 7269 6769    row = db.origi
-0000cab0: 6e5f 7669 7369 745f 6765 745f 6c61 7465  n_visit_get_late
-0000cac0: 7374 280a 2020 2020 2020 2020 2020 2020  st(.            
-0000cad0: 6f72 6967 696e 2c0a 2020 2020 2020 2020  origin,.        
-0000cae0: 2020 2020 7479 7065 3d74 7970 652c 0a20      type=type,. 
-0000caf0: 2020 2020 2020 2020 2020 2061 6c6c 6f77             allow
-0000cb00: 6564 5f73 7461 7475 7365 733d 616c 6c6f  ed_statuses=allo
-0000cb10: 7765 645f 7374 6174 7573 6573 2c0a 2020  wed_statuses,.  
-0000cb20: 2020 2020 2020 2020 2020 7265 7175 6972            requir
-0000cb30: 655f 736e 6170 7368 6f74 3d72 6571 7569  e_snapshot=requi
-0000cb40: 7265 5f73 6e61 7073 686f 742c 0a20 2020  re_snapshot,.   
-0000cb50: 2020 2020 2020 2020 2063 7572 3d63 7572           cur=cur
-0000cb60: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-0000cb70: 2020 2020 6966 2072 6f77 3a0a 2020 2020      if row:.    
-0000cb80: 2020 2020 2020 2020 726f 775f 6420 3d20          row_d = 
-0000cb90: 6469 6374 287a 6970 2864 622e 6f72 6967  dict(zip(db.orig
-0000cba0: 696e 5f76 6973 6974 5f67 6574 5f63 6f6c  in_visit_get_col
-0000cbb0: 732c 2072 6f77 2929 0a20 2020 2020 2020  s, row)).       
-0000cbc0: 2020 2020 2061 7373 6572 7420 280a 2020       assert (.  
-0000cbd0: 2020 2020 2020 2020 2020 2020 2020 726f                ro
-0000cbe0: 775f 645b 2276 6973 6974 225d 2069 7320  w_d["visit"] is 
-0000cbf0: 6e6f 7420 4e6f 6e65 0a20 2020 2020 2020  not None.       
-0000cc00: 2020 2020 2029 2c20 226f 7269 6769 6e5f       ), "origin_
-0000cc10: 7669 7369 745f 7374 6174 7573 204c 4546  visit_status LEF
-0000cc20: 5420 4a4f 494e 206f 7269 6769 6e5f 7669  T JOIN origin_vi
-0000cc30: 7369 7420 7265 7475 726e 6564 204e 554c  sit returned NUL
-0000cc40: 4c22 0a20 2020 2020 2020 2020 2020 2076  L".            v
-0000cc50: 6973 6974 203d 204f 7269 6769 6e56 6973  isit = OriginVis
-0000cc60: 6974 280a 2020 2020 2020 2020 2020 2020  it(.            
-0000cc70: 2020 2020 6f72 6967 696e 3d72 6f77 5f64      origin=row_d
-0000cc80: 5b22 6f72 6967 696e 225d 2c0a 2020 2020  ["origin"],.    
-0000cc90: 2020 2020 2020 2020 2020 2020 7669 7369              visi
-0000cca0: 743d 726f 775f 645b 2276 6973 6974 225d  t=row_d["visit"]
-0000ccb0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000ccc0: 2020 6461 7465 3d72 6f77 5f64 5b22 6461    date=row_d["da
-0000ccd0: 7465 225d 2c0a 2020 2020 2020 2020 2020  te"],.          
-0000cce0: 2020 2020 2020 7479 7065 3d72 6f77 5f64        type=row_d
-0000ccf0: 5b22 7479 7065 225d 2c0a 2020 2020 2020  ["type"],.      
-0000cd00: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000cd10: 2020 2020 7265 7475 726e 2076 6973 6974      return visit
-0000cd20: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000cd30: 4e6f 6e65 0a0a 2020 2020 4064 625f 7472  None..    @db_tr
-0000cd40: 616e 7361 6374 696f 6e28 7374 6174 656d  ansaction(statem
-0000cd50: 656e 745f 7469 6d65 6f75 743d 3530 3029  ent_timeout=500)
-0000cd60: 0a20 2020 2064 6566 206f 7269 6769 6e5f  .    def origin_
-0000cd70: 7669 7369 745f 7374 6174 7573 5f67 6574  visit_status_get
-0000cd80: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-0000cd90: 2020 2020 2020 2020 6f72 6967 696e 3a20          origin: 
-0000cda0: 7374 722c 0a20 2020 2020 2020 2076 6973  str,.        vis
-0000cdb0: 6974 3a20 696e 742c 0a20 2020 2020 2020  it: int,.       
-0000cdc0: 2070 6167 655f 746f 6b65 6e3a 204f 7074   page_token: Opt
-0000cdd0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-0000cde0: 652c 0a20 2020 2020 2020 206f 7264 6572  e,.        order
-0000cdf0: 3a20 4c69 7374 4f72 6465 7220 3d20 4c69  : ListOrder = Li
-0000ce00: 7374 4f72 6465 722e 4153 432c 0a20 2020  stOrder.ASC,.   
-0000ce10: 2020 2020 206c 696d 6974 3a20 696e 7420       limit: int 
-0000ce20: 3d20 3130 2c0a 2020 2020 2020 2020 2a2c  = 10,.        *,
-0000ce30: 0a20 2020 2020 2020 2064 623a 2044 622c  .        db: Db,
-0000ce40: 0a20 2020 2020 2020 2063 7572 3d4e 6f6e  .        cur=Non
-0000ce50: 652c 0a20 2020 2029 202d 3e20 5061 6765  e,.    ) -> Page
-0000ce60: 6452 6573 756c 745b 4f72 6967 696e 5669  dResult[OriginVi
-0000ce70: 7369 7453 7461 7475 735d 3a0a 2020 2020  sitStatus]:.    
-0000ce80: 2020 2020 6e65 7874 5f70 6167 655f 746f      next_page_to
-0000ce90: 6b65 6e20 3d20 4e6f 6e65 0a20 2020 2020  ken = None.     
-0000cea0: 2020 2064 6174 655f 6672 6f6d 203d 204e     date_from = N
-0000ceb0: 6f6e 650a 2020 2020 2020 2020 6966 2070  one.        if p
-0000cec0: 6167 655f 746f 6b65 6e20 6973 206e 6f74  age_token is not
-0000ced0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000cee0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-0000cef0: 2020 2020 2020 2020 6461 7465 5f66 726f          date_fro
-0000cf00: 6d20 3d20 6461 7465 7469 6d65 2e64 6174  m = datetime.dat
-0000cf10: 6574 696d 652e 6672 6f6d 6973 6f66 6f72  etime.fromisofor
-0000cf20: 6d61 7428 7061 6765 5f74 6f6b 656e 290a  mat(page_token).
-0000cf30: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-0000cf40: 7074 2056 616c 7565 4572 726f 723a 0a20  pt ValueError:. 
-0000cf50: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000cf60: 6169 7365 2053 746f 7261 6765 4172 6775  aise StorageArgu
-0000cf70: 6d65 6e74 4578 6365 7074 696f 6e28 0a20  mentException(. 
-0000cf80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf90: 2020 2022 496e 7661 6c69 6420 7061 6765     "Invalid page
-0000cfa0: 5f74 6f6b 656e 2061 7267 756d 656e 7420  _token argument 
-0000cfb0: 746f 206f 7269 6769 6e5f 7669 7369 745f  to origin_visit_
-0000cfc0: 7374 6174 7573 5f67 6574 2e22 0a20 2020  status_get.".   
-0000cfd0: 2020 2020 2020 2020 2020 2020 2029 2066               ) f
-0000cfe0: 726f 6d20 4e6f 6e65 0a0a 2020 2020 2020  rom None..      
-0000cff0: 2020 7669 7369 745f 7374 6174 7573 6573    visit_statuses
-0000d000: 3a20 4c69 7374 5b4f 7269 6769 6e56 6973  : List[OriginVis
-0000d010: 6974 5374 6174 7573 5d20 3d20 5b5d 0a20  itStatus] = []. 
-0000d020: 2020 2020 2020 2023 2054 616b 6520 6f6e         # Take on
-0000d030: 6520 6d6f 7265 2076 6973 6974 2073 7461  e more visit sta
-0000d040: 7475 7320 736f 2077 6520 6361 6e20 7265  tus so we can re
-0000d050: 7573 6520 6974 2061 7320 7468 6520 6e65  use it as the ne
-0000d060: 7874 2070 6167 6520 746f 6b65 6e20 6966  xt page token if
-0000d070: 2061 6e79 0a20 2020 2020 2020 2066 6f72   any.        for
-0000d080: 2072 6f77 2069 6e20 6462 2e6f 7269 6769   row in db.origi
-0000d090: 6e5f 7669 7369 745f 7374 6174 7573 5f67  n_visit_status_g
-0000d0a0: 6574 5f72 616e 6765 280a 2020 2020 2020  et_range(.      
-0000d0b0: 2020 2020 2020 6f72 6967 696e 2c0a 2020        origin,.  
-0000d0c0: 2020 2020 2020 2020 2020 7669 7369 742c            visit,
-0000d0d0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-0000d0e0: 655f 6672 6f6d 3d64 6174 655f 6672 6f6d  e_from=date_from
-0000d0f0: 2c0a 2020 2020 2020 2020 2020 2020 6f72  ,.            or
-0000d100: 6465 723d 6f72 6465 722c 0a20 2020 2020  der=order,.     
-0000d110: 2020 2020 2020 206c 696d 6974 3d6c 696d         limit=lim
-0000d120: 6974 202b 2031 2c0a 2020 2020 2020 2020  it + 1,.        
-0000d130: 2020 2020 6375 723d 6375 722c 0a20 2020      cur=cur,.   
-0000d140: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
-0000d150: 2020 2020 726f 775f 6420 3d20 6469 6374      row_d = dict
-0000d160: 287a 6970 2864 622e 6f72 6967 696e 5f76  (zip(db.origin_v
-0000d170: 6973 6974 5f73 7461 7475 735f 636f 6c73  isit_status_cols
-0000d180: 2c20 726f 7729 290a 2020 2020 2020 2020  , row)).        
-0000d190: 2020 2020 7669 7369 745f 7374 6174 7573      visit_status
-0000d1a0: 6573 2e61 7070 656e 6428 4f72 6967 696e  es.append(Origin
-0000d1b0: 5669 7369 7453 7461 7475 7328 2a2a 726f  VisitStatus(**ro
-0000d1c0: 775f 6429 290a 0a20 2020 2020 2020 2069  w_d))..        i
-0000d1d0: 6620 6c65 6e28 7669 7369 745f 7374 6174  f len(visit_stat
-0000d1e0: 7573 6573 2920 3e20 6c69 6d69 743a 0a20  uses) > limit:. 
-0000d1f0: 2020 2020 2020 2020 2020 2023 206c 6173             # las
-0000d200: 7420 7669 7369 7420 7374 6174 7573 2064  t visit status d
-0000d210: 6174 6520 6973 2074 6865 206e 6578 7420  ate is the next 
-0000d220: 7061 6765 2074 6f6b 656e 0a20 2020 2020  page token.     
-0000d230: 2020 2020 2020 206e 6578 745f 7061 6765         next_page
-0000d240: 5f74 6f6b 656e 203d 2073 7472 2876 6973  _token = str(vis
-0000d250: 6974 5f73 7461 7475 7365 735b 2d31 5d2e  it_statuses[-1].
-0000d260: 6461 7465 290a 2020 2020 2020 2020 2020  date).          
-0000d270: 2020 2320 6578 636c 7564 696e 6720 7468    # excluding th
-0000d280: 6174 2076 6973 6974 2073 7461 7475 7320  at visit status 
-0000d290: 6672 6f6d 2074 6865 2072 6573 756c 7420  from the result 
-0000d2a0: 746f 2072 6573 7065 6374 2074 6865 206c  to respect the l
-0000d2b0: 696d 6974 2073 697a 650a 2020 2020 2020  imit size.      
-0000d2c0: 2020 2020 2020 7669 7369 745f 7374 6174        visit_stat
-0000d2d0: 7573 6573 203d 2076 6973 6974 5f73 7461  uses = visit_sta
-0000d2e0: 7475 7365 735b 3a6c 696d 6974 5d0a 0a20  tuses[:limit].. 
-0000d2f0: 2020 2020 2020 2072 6574 7572 6e20 5061         return Pa
-0000d300: 6765 6452 6573 756c 7428 7265 7375 6c74  gedResult(result
-0000d310: 733d 7669 7369 745f 7374 6174 7573 6573  s=visit_statuses
-0000d320: 2c20 6e65 7874 5f70 6167 655f 746f 6b65  , next_page_toke
-0000d330: 6e3d 6e65 7874 5f70 6167 655f 746f 6b65  n=next_page_toke
-0000d340: 6e29 0a0a 2020 2020 4064 625f 7472 616e  n)..    @db_tran
-0000d350: 7361 6374 696f 6e28 290a 2020 2020 6465  saction().    de
-0000d360: 6620 6f72 6967 696e 5f76 6973 6974 5f73  f origin_visit_s
-0000d370: 7461 7475 735f 6765 745f 7261 6e64 6f6d  tatus_get_random
-0000d380: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
-0000d390: 7479 7065 3a20 7374 722c 202a 2c20 6462  type: str, *, db
-0000d3a0: 3a20 4462 2c20 6375 723d 4e6f 6e65 0a20  : Db, cur=None. 
-0000d3b0: 2020 2029 202d 3e20 4f70 7469 6f6e 616c     ) -> Optional
-0000d3c0: 5b4f 7269 6769 6e56 6973 6974 5374 6174  [OriginVisitStat
-0000d3d0: 7573 5d3a 0a20 2020 2020 2020 2072 6f77  us]:.        row
-0000d3e0: 203d 2064 622e 6f72 6967 696e 5f76 6973   = db.origin_vis
-0000d3f0: 6974 5f67 6574 5f72 616e 646f 6d28 7479  it_get_random(ty
-0000d400: 7065 2c20 6375 7229 0a20 2020 2020 2020  pe, cur).       
-0000d410: 2069 6620 726f 7720 6973 206e 6f74 204e   if row is not N
-0000d420: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000d430: 2072 6f77 5f64 203d 2064 6963 7428 7a69   row_d = dict(zi
-0000d440: 7028 6462 2e6f 7269 6769 6e5f 7669 7369  p(db.origin_visi
-0000d450: 745f 7374 6174 7573 5f63 6f6c 732c 2072  t_status_cols, r
-0000d460: 6f77 2929 0a20 2020 2020 2020 2020 2020  ow)).           
-0000d470: 2072 6574 7572 6e20 4f72 6967 696e 5669   return OriginVi
-0000d480: 7369 7453 7461 7475 7328 2a2a 726f 775f  sitStatus(**row_
-0000d490: 6429 0a20 2020 2020 2020 2072 6574 7572  d).        retur
-0000d4a0: 6e20 4e6f 6e65 0a0a 2020 2020 2323 2323  n None..    ####
-0000d4b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000d4c0: 2323 2323 2323 0a20 2020 2023 204f 7269  ######.    # Ori
-0000d4d0: 6769 6e0a 2020 2020 2323 2323 2323 2323  gin.    ########
-0000d4e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000d4f0: 2323 0a0a 2020 2020 4064 625f 7472 616e  ##..    @db_tran
-0000d500: 7361 6374 696f 6e28 7374 6174 656d 656e  saction(statemen
-0000d510: 745f 7469 6d65 6f75 743d 3130 3030 290a  t_timeout=1000).
-0000d520: 2020 2020 6465 6620 6f72 6967 696e 5f67      def origin_g
-0000d530: 6574 280a 2020 2020 2020 2020 7365 6c66  et(.        self
-0000d540: 2c20 6f72 6967 696e 733a 204c 6973 745b  , origins: List[
-0000d550: 7374 725d 2c20 2a2c 2064 623a 2044 622c  str], *, db: Db,
-0000d560: 2063 7572 3d4e 6f6e 650a 2020 2020 2920   cur=None.    ) 
-0000d570: 2d3e 2049 7465 7261 626c 655b 4f70 7469  -> Iterable[Opti
-0000d580: 6f6e 616c 5b4f 7269 6769 6e5d 5d3a 0a20  onal[Origin]]:. 
-0000d590: 2020 2020 2020 2072 6f77 7320 3d20 6462         rows = db
-0000d5a0: 2e6f 7269 6769 6e5f 6765 745f 6279 5f75  .origin_get_by_u
-0000d5b0: 726c 286f 7269 6769 6e73 2c20 6375 7229  rl(origins, cur)
-0000d5c0: 0a20 2020 2020 2020 2072 6573 756c 743a  .        result:
-0000d5d0: 204c 6973 745b 4f70 7469 6f6e 616c 5b4f   List[Optional[O
-0000d5e0: 7269 6769 6e5d 5d20 3d20 5b5d 0a20 2020  rigin]] = [].   
-0000d5f0: 2020 2020 2066 6f72 2072 6f77 2069 6e20       for row in 
-0000d600: 726f 7773 3a0a 2020 2020 2020 2020 2020  rows:.          
-0000d610: 2020 6f72 6967 696e 5f64 203d 2064 6963    origin_d = dic
-0000d620: 7428 7a69 7028 6462 2e6f 7269 6769 6e5f  t(zip(db.origin_
-0000d630: 636f 6c73 2c20 726f 7729 290a 2020 2020  cols, row)).    
-0000d640: 2020 2020 2020 2020 7572 6c20 3d20 6f72          url = or
-0000d650: 6967 696e 5f64 5b22 7572 6c22 5d0a 2020  igin_d["url"].  
-0000d660: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0000d670: 2e61 7070 656e 6428 4e6f 6e65 2069 6620  .append(None if 
-0000d680: 7572 6c20 6973 204e 6f6e 6520 656c 7365  url is None else
-0000d690: 204f 7269 6769 6e28 7572 6c3d 7572 6c29   Origin(url=url)
-0000d6a0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0000d6b0: 2072 6573 756c 740a 0a20 2020 2040 6462   result..    @db
-0000d6c0: 5f74 7261 6e73 6163 7469 6f6e 2873 7461  _transaction(sta
-0000d6d0: 7465 6d65 6e74 5f74 696d 656f 7574 3d31  tement_timeout=1
-0000d6e0: 3030 3029 0a20 2020 2064 6566 206f 7269  000).    def ori
-0000d6f0: 6769 6e5f 6765 745f 6279 5f73 6861 3128  gin_get_by_sha1(
-0000d700: 0a20 2020 2020 2020 2073 656c 662c 2073  .        self, s
-0000d710: 6861 3173 3a20 4c69 7374 5b62 7974 6573  ha1s: List[bytes
-0000d720: 5d2c 202a 2c20 6462 3a20 4462 2c20 6375  ], *, db: Db, cu
-0000d730: 723d 4e6f 6e65 0a20 2020 2029 202d 3e20  r=None.    ) -> 
-0000d740: 4c69 7374 5b4f 7074 696f 6e61 6c5b 4469  List[Optional[Di
-0000d750: 6374 5b73 7472 2c20 416e 795d 5d5d 3a0a  ct[str, Any]]]:.
-0000d760: 2020 2020 2020 2020 7265 7475 726e 205b          return [
-0000d770: 0a20 2020 2020 2020 2020 2020 2064 6963  .            dic
-0000d780: 7428 7a69 7028 6462 2e6f 7269 6769 6e5f  t(zip(db.origin_
-0000d790: 636f 6c73 2c20 726f 7729 2920 6966 2072  cols, row)) if r
-0000d7a0: 6f77 5b30 5d20 656c 7365 204e 6f6e 650a  ow[0] else None.
-0000d7b0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000d7c0: 726f 7720 696e 2064 622e 6f72 6967 696e  row in db.origin
-0000d7d0: 5f67 6574 5f62 795f 7368 6131 2873 6861  _get_by_sha1(sha
-0000d7e0: 3173 2c20 6375 7229 0a20 2020 2020 2020  1s, cur).       
-0000d7f0: 205d 0a0a 2020 2020 4064 625f 7472 616e   ]..    @db_tran
-0000d800: 7361 6374 696f 6e5f 6765 6e65 7261 746f  saction_generato
-0000d810: 7228 290a 2020 2020 6465 6620 6f72 6967  r().    def orig
-0000d820: 696e 5f67 6574 5f72 616e 6765 2873 656c  in_get_range(sel
-0000d830: 662c 206f 7269 6769 6e5f 6672 6f6d 3d31  f, origin_from=1
-0000d840: 2c20 6f72 6967 696e 5f63 6f75 6e74 3d31  , origin_count=1
-0000d850: 3030 2c20 2a2c 2064 623a 2044 622c 2063  00, *, db: Db, c
-0000d860: 7572 3d4e 6f6e 6529 3a0a 2020 2020 2020  ur=None):.      
-0000d870: 2020 666f 7220 6f72 6967 696e 2069 6e20    for origin in 
-0000d880: 6462 2e6f 7269 6769 6e5f 6765 745f 7261  db.origin_get_ra
-0000d890: 6e67 6528 6f72 6967 696e 5f66 726f 6d2c  nge(origin_from,
-0000d8a0: 206f 7269 6769 6e5f 636f 756e 742c 2063   origin_count, c
-0000d8b0: 7572 293a 0a20 2020 2020 2020 2020 2020  ur):.           
-0000d8c0: 2079 6965 6c64 2064 6963 7428 7a69 7028   yield dict(zip(
-0000d8d0: 6462 2e6f 7269 6769 6e5f 6765 745f 7261  db.origin_get_ra
-0000d8e0: 6e67 655f 636f 6c73 2c20 6f72 6967 696e  nge_cols, origin
-0000d8f0: 2929 0a0a 2020 2020 4064 625f 7472 616e  ))..    @db_tran
-0000d900: 7361 6374 696f 6e28 290a 2020 2020 6465  saction().    de
-0000d910: 6620 6f72 6967 696e 5f6c 6973 7428 0a20  f origin_list(. 
-0000d920: 2020 2020 2020 2073 656c 662c 2070 6167         self, pag
-0000d930: 655f 746f 6b65 6e3a 204f 7074 696f 6e61  e_token: Optiona
-0000d940: 6c5b 7374 725d 203d 204e 6f6e 652c 206c  l[str] = None, l
-0000d950: 696d 6974 3a20 696e 7420 3d20 3130 302c  imit: int = 100,
-0000d960: 202a 2c20 6462 3a20 4462 2c20 6375 723d   *, db: Db, cur=
-0000d970: 4e6f 6e65 0a20 2020 2029 202d 3e20 5061  None.    ) -> Pa
-0000d980: 6765 6452 6573 756c 745b 4f72 6967 696e  gedResult[Origin
-0000d990: 5d3a 0a20 2020 2020 2020 2070 6167 655f  ]:.        page_
-0000d9a0: 746f 6b65 6e20 3d20 7061 6765 5f74 6f6b  token = page_tok
-0000d9b0: 656e 206f 7220 2230 220a 2020 2020 2020  en or "0".      
-0000d9c0: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
-0000d9d0: 6e63 6528 7061 6765 5f74 6f6b 656e 2c20  nce(page_token, 
-0000d9e0: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
-0000d9f0: 2020 7261 6973 6520 5374 6f72 6167 6541    raise StorageA
-0000da00: 7267 756d 656e 7445 7863 6570 7469 6f6e  rgumentException
-0000da10: 2822 7061 6765 5f74 6f6b 656e 206d 7573  ("page_token mus
-0000da20: 7420 6265 2061 2073 7472 696e 672e 2229  t be a string.")
-0000da30: 0a20 2020 2020 2020 206f 7269 6769 6e5f  .        origin_
-0000da40: 6672 6f6d 203d 2069 6e74 2870 6167 655f  from = int(page_
-0000da50: 746f 6b65 6e29 0a20 2020 2020 2020 206e  token).        n
-0000da60: 6578 745f 7061 6765 5f74 6f6b 656e 203d  ext_page_token =
-0000da70: 204e 6f6e 650a 0a20 2020 2020 2020 206f   None..        o
-0000da80: 7269 6769 6e73 3a20 4c69 7374 5b4f 7269  rigins: List[Ori
-0000da90: 6769 6e5d 203d 205b 5d0a 2020 2020 2020  gin] = [].      
-0000daa0: 2020 2320 5461 6b65 206f 6e65 206d 6f72    # Take one mor
-0000dab0: 6520 6f72 6967 696e 2073 6f20 7765 2063  e origin so we c
-0000dac0: 616e 2072 6575 7365 2069 7420 6173 2074  an reuse it as t
-0000dad0: 6865 206e 6578 7420 7061 6765 2074 6f6b  he next page tok
-0000dae0: 656e 2069 6620 616e 790a 2020 2020 2020  en if any.      
-0000daf0: 2020 666f 7220 726f 775f 6420 696e 2073    for row_d in s
-0000db00: 656c 662e 6f72 6967 696e 5f67 6574 5f72  elf.origin_get_r
-0000db10: 616e 6765 286f 7269 6769 6e5f 6672 6f6d  ange(origin_from
-0000db20: 2c20 6c69 6d69 7420 2b20 312c 2064 623d  , limit + 1, db=
-0000db30: 6462 2c20 6375 723d 6375 7229 3a0a 2020  db, cur=cur):.  
-0000db40: 2020 2020 2020 2020 2020 6f72 6967 696e            origin
-0000db50: 732e 6170 7065 6e64 284f 7269 6769 6e28  s.append(Origin(
-0000db60: 7572 6c3d 726f 775f 645b 2275 726c 225d  url=row_d["url"]
-0000db70: 2929 0a20 2020 2020 2020 2020 2020 2023  )).            #
-0000db80: 206b 6565 7020 7468 6520 6c61 7374 5f69   keep the last_i
-0000db90: 6420 666f 7220 7468 6520 7061 6769 6e61  d for the pagina
-0000dba0: 7469 6f6e 2069 6620 6e65 6564 6564 0a20  tion if needed. 
-0000dbb0: 2020 2020 2020 2020 2020 206c 6173 745f             last_
-0000dbc0: 6964 203d 2072 6f77 5f64 5b22 6964 225d  id = row_d["id"]
-0000dbd0: 0a0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
-0000dbe0: 286f 7269 6769 6e73 2920 3e20 6c69 6d69  (origins) > limi
-0000dbf0: 743a 2020 2320 6461 7461 206c 6566 7420  t:  # data left 
-0000dc00: 666f 7220 7375 6273 6571 7565 6e74 2063  for subsequent c
-0000dc10: 616c 6c0a 2020 2020 2020 2020 2020 2020  all.            
-0000dc20: 2320 6c61 7374 206f 7269 6769 6e20 6964  # last origin id
-0000dc30: 2069 7320 7468 6520 6e65 7874 2070 6167   is the next pag
-0000dc40: 6520 746f 6b65 6e0a 2020 2020 2020 2020  e token.        
-0000dc50: 2020 2020 6e65 7874 5f70 6167 655f 746f      next_page_to
-0000dc60: 6b65 6e20 3d20 7374 7228 6c61 7374 5f69  ken = str(last_i
-0000dc70: 6429 0a20 2020 2020 2020 2020 2020 2023  d).            #
-0000dc80: 2065 7863 6c75 6469 6e67 2074 6861 7420   excluding that 
-0000dc90: 6f72 6967 696e 2066 726f 6d20 7468 6520  origin from the 
-0000dca0: 7265 7375 6c74 2074 6f20 7265 7370 6563  result to respec
-0000dcb0: 7420 7468 6520 6c69 6d69 7420 7369 7a65  t the limit size
-0000dcc0: 0a20 2020 2020 2020 2020 2020 206f 7269  .            ori
-0000dcd0: 6769 6e73 203d 206f 7269 6769 6e73 5b3a  gins = origins[:
-0000dce0: 6c69 6d69 745d 0a0a 2020 2020 2020 2020  limit]..        
-0000dcf0: 6173 7365 7274 206c 656e 286f 7269 6769  assert len(origi
-0000dd00: 6e73 2920 3c3d 206c 696d 6974 0a20 2020  ns) <= limit.   
-0000dd10: 2020 2020 2072 6574 7572 6e20 5061 6765       return Page
-0000dd20: 6452 6573 756c 7428 7265 7375 6c74 733d  dResult(results=
-0000dd30: 6f72 6967 696e 732c 206e 6578 745f 7061  origins, next_pa
-0000dd40: 6765 5f74 6f6b 656e 3d6e 6578 745f 7061  ge_token=next_pa
-0000dd50: 6765 5f74 6f6b 656e 290a 0a20 2020 2040  ge_token)..    @
-0000dd60: 6462 5f74 7261 6e73 6163 7469 6f6e 2829  db_transaction()
-0000dd70: 0a20 2020 2064 6566 206f 7269 6769 6e5f  .    def origin_
-0000dd80: 7365 6172 6368 280a 2020 2020 2020 2020  search(.        
-0000dd90: 7365 6c66 2c0a 2020 2020 2020 2020 7572  self,.        ur
-0000dda0: 6c5f 7061 7474 6572 6e3a 2073 7472 2c0a  l_pattern: str,.
-0000ddb0: 2020 2020 2020 2020 7061 6765 5f74 6f6b          page_tok
-0000ddc0: 656e 3a20 4f70 7469 6f6e 616c 5b73 7472  en: Optional[str
-0000ddd0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-0000dde0: 2020 6c69 6d69 743a 2069 6e74 203d 2035    limit: int = 5
-0000ddf0: 302c 0a20 2020 2020 2020 2072 6567 6578  0,.        regex
-0000de00: 703a 2062 6f6f 6c20 3d20 4661 6c73 652c  p: bool = False,
-0000de10: 0a20 2020 2020 2020 2077 6974 685f 7669  .        with_vi
-0000de20: 7369 743a 2062 6f6f 6c20 3d20 4661 6c73  sit: bool = Fals
-0000de30: 652c 0a20 2020 2020 2020 2076 6973 6974  e,.        visit
-0000de40: 5f74 7970 6573 3a20 4f70 7469 6f6e 616c  _types: Optional
-0000de50: 5b4c 6973 745b 7374 725d 5d20 3d20 4e6f  [List[str]] = No
-0000de60: 6e65 2c0a 2020 2020 2020 2020 2a2c 0a20  ne,.        *,. 
-0000de70: 2020 2020 2020 2064 623a 2044 622c 0a20         db: Db,. 
-0000de80: 2020 2020 2020 2063 7572 3d4e 6f6e 652c         cur=None,
-0000de90: 0a20 2020 2029 202d 3e20 5061 6765 6452  .    ) -> PagedR
-0000dea0: 6573 756c 745b 4f72 6967 696e 5d3a 0a20  esult[Origin]:. 
-0000deb0: 2020 2020 2020 206e 6578 745f 7061 6765         next_page
-0000dec0: 5f74 6f6b 656e 203d 204e 6f6e 650a 2020  _token = None.  
-0000ded0: 2020 2020 2020 6f66 6673 6574 203d 2069        offset = i
-0000dee0: 6e74 2870 6167 655f 746f 6b65 6e29 2069  nt(page_token) i
-0000def0: 6620 7061 6765 5f74 6f6b 656e 2065 6c73  f page_token els
-0000df00: 6520 300a 0a20 2020 2020 2020 206f 7269  e 0..        ori
-0000df10: 6769 6e73 203d 205b 5d0a 2020 2020 2020  gins = [].      
-0000df20: 2020 2320 5461 6b65 206f 6e65 206d 6f72    # Take one mor
-0000df30: 6520 6f72 6967 696e 2073 6f20 7765 2063  e origin so we c
-0000df40: 616e 2072 6575 7365 2069 7420 6173 2074  an reuse it as t
-0000df50: 6865 206e 6578 7420 7061 6765 2074 6f6b  he next page tok
-0000df60: 656e 2069 6620 616e 790a 2020 2020 2020  en if any.      
-0000df70: 2020 666f 7220 6f72 6967 696e 2069 6e20    for origin in 
-0000df80: 6462 2e6f 7269 6769 6e5f 7365 6172 6368  db.origin_search
-0000df90: 280a 2020 2020 2020 2020 2020 2020 7572  (.            ur
-0000dfa0: 6c5f 7061 7474 6572 6e2c 206f 6666 7365  l_pattern, offse
-0000dfb0: 742c 206c 696d 6974 202b 2031 2c20 7265  t, limit + 1, re
-0000dfc0: 6765 7870 2c20 7769 7468 5f76 6973 6974  gexp, with_visit
-0000dfd0: 2c20 7669 7369 745f 7479 7065 732c 2063  , visit_types, c
-0000dfe0: 7572 0a20 2020 2020 2020 2029 3a0a 2020  ur.        ):.  
-0000dff0: 2020 2020 2020 2020 2020 726f 775f 6420            row_d 
-0000e000: 3d20 6469 6374 287a 6970 2864 622e 6f72  = dict(zip(db.or
-0000e010: 6967 696e 5f63 6f6c 732c 206f 7269 6769  igin_cols, origi
-0000e020: 6e29 290a 2020 2020 2020 2020 2020 2020  n)).            
-0000e030: 6f72 6967 696e 732e 6170 7065 6e64 284f  origins.append(O
-0000e040: 7269 6769 6e28 7572 6c3d 726f 775f 645b  rigin(url=row_d[
-0000e050: 2275 726c 225d 2929 0a0a 2020 2020 2020  "url"]))..      
-0000e060: 2020 6966 206c 656e 286f 7269 6769 6e73    if len(origins
-0000e070: 2920 3e20 6c69 6d69 743a 0a20 2020 2020  ) > limit:.     
-0000e080: 2020 2020 2020 2023 206e 6578 7420 6f66         # next of
-0000e090: 6673 6574 0a20 2020 2020 2020 2020 2020  fset.           
-0000e0a0: 206e 6578 745f 7061 6765 5f74 6f6b 656e   next_page_token
-0000e0b0: 203d 2073 7472 286f 6666 7365 7420 2b20   = str(offset + 
-0000e0c0: 6c69 6d69 7429 0a20 2020 2020 2020 2020  limit).         
-0000e0d0: 2020 2023 2065 7863 6c75 6469 6e67 2074     # excluding t
-0000e0e0: 6861 7420 6f72 6967 696e 2066 726f 6d20  hat origin from 
-0000e0f0: 7468 6520 7265 7375 6c74 2074 6f20 7265  the result to re
-0000e100: 7370 6563 7420 7468 6520 6c69 6d69 7420  spect the limit 
-0000e110: 7369 7a65 0a20 2020 2020 2020 2020 2020  size.           
-0000e120: 206f 7269 6769 6e73 203d 206f 7269 6769   origins = origi
-0000e130: 6e73 5b3a 6c69 6d69 745d 0a0a 2020 2020  ns[:limit]..    
-0000e140: 2020 2020 6173 7365 7274 206c 656e 286f      assert len(o
-0000e150: 7269 6769 6e73 2920 3c3d 206c 696d 6974  rigins) <= limit
-0000e160: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0000e170: 2050 6167 6564 5265 7375 6c74 2872 6573   PagedResult(res
-0000e180: 756c 7473 3d6f 7269 6769 6e73 2c20 6e65  ults=origins, ne
-0000e190: 7874 5f70 6167 655f 746f 6b65 6e3d 6e65  xt_page_token=ne
-0000e1a0: 7874 5f70 6167 655f 746f 6b65 6e29 0a0a  xt_page_token)..
-0000e1b0: 2020 2020 4064 625f 7472 616e 7361 6374      @db_transact
-0000e1c0: 696f 6e28 290a 2020 2020 6465 6620 6f72  ion().    def or
-0000e1d0: 6967 696e 5f63 6f75 6e74 280a 2020 2020  igin_count(.    
-0000e1e0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0000e1f0: 2020 7572 6c5f 7061 7474 6572 6e3a 2073    url_pattern: s
-0000e200: 7472 2c0a 2020 2020 2020 2020 7265 6765  tr,.        rege
-0000e210: 7870 3a20 626f 6f6c 203d 2046 616c 7365  xp: bool = False
-0000e220: 2c0a 2020 2020 2020 2020 7769 7468 5f76  ,.        with_v
-0000e230: 6973 6974 3a20 626f 6f6c 203d 2046 616c  isit: bool = Fal
-0000e240: 7365 2c0a 2020 2020 2020 2020 2a2c 0a20  se,.        *,. 
-0000e250: 2020 2020 2020 2064 623a 2044 622c 0a20         db: Db,. 
-0000e260: 2020 2020 2020 2063 7572 3d4e 6f6e 652c         cur=None,
-0000e270: 0a20 2020 2029 202d 3e20 696e 743a 0a20  .    ) -> int:. 
-0000e280: 2020 2020 2020 2072 6574 7572 6e20 6462         return db
-0000e290: 2e6f 7269 6769 6e5f 636f 756e 7428 7572  .origin_count(ur
-0000e2a0: 6c5f 7061 7474 6572 6e2c 2072 6567 6578  l_pattern, regex
-0000e2b0: 702c 2077 6974 685f 7669 7369 742c 2063  p, with_visit, c
-0000e2c0: 7572 290a 0a20 2020 2040 6462 5f74 7261  ur)..    @db_tra
-0000e2d0: 6e73 6163 7469 6f6e 2829 0a20 2020 2064  nsaction().    d
-0000e2e0: 6566 206f 7269 6769 6e5f 736e 6170 7368  ef origin_snapsh
-0000e2f0: 6f74 5f67 6574 5f61 6c6c 280a 2020 2020  ot_get_all(.    
-0000e300: 2020 2020 7365 6c66 2c20 6f72 6967 696e      self, origin
-0000e310: 5f75 726c 3a20 7374 722c 202a 2c20 6462  _url: str, *, db
-0000e320: 3a20 4462 2c20 6375 723d 4e6f 6e65 0a20  : Db, cur=None. 
-0000e330: 2020 2029 202d 3e20 4c69 7374 5b53 6861     ) -> List[Sha
-0000e340: 3147 6974 5d3a 0a20 2020 2020 2020 2072  1Git]:.        r
-0000e350: 6574 7572 6e20 6c69 7374 2864 622e 6f72  eturn list(db.or
-0000e360: 6967 696e 5f73 6e61 7073 686f 745f 6765  igin_snapshot_ge
-0000e370: 745f 616c 6c28 6f72 6967 696e 5f75 726c  t_all(origin_url
-0000e380: 2c20 6375 7229 290a 0a20 2020 2040 6462  , cur))..    @db
-0000e390: 5f74 7261 6e73 6163 7469 6f6e 2829 0a20  _transaction(). 
-0000e3a0: 2020 2064 6566 206f 7269 6769 6e5f 6164     def origin_ad
-0000e3b0: 6428 7365 6c66 2c20 6f72 6967 696e 733a  d(self, origins:
-0000e3c0: 204c 6973 745b 4f72 6967 696e 5d2c 202a   List[Origin], *
-0000e3d0: 2c20 6462 3a20 4462 2c20 6375 723d 4e6f  , db: Db, cur=No
-0000e3e0: 6e65 2920 2d3e 2044 6963 745b 7374 722c  ne) -> Dict[str,
-0000e3f0: 2069 6e74 5d3a 0a20 2020 2020 2020 2075   int]:.        u
-0000e400: 726c 7320 3d20 5b6f 2e75 726c 2066 6f72  rls = [o.url for
-0000e410: 206f 2069 6e20 6f72 6967 696e 735d 0a20   o in origins]. 
-0000e420: 2020 2020 2020 206b 6e6f 776e 5f6f 7269         known_ori
-0000e430: 6769 6e73 203d 2073 6574 2875 726c 2066  gins = set(url f
-0000e440: 6f72 2028 7572 6c2c 2920 696e 2064 622e  or (url,) in db.
-0000e450: 6f72 6967 696e 5f67 6574 5f62 795f 7572  origin_get_by_ur
-0000e460: 6c28 7572 6c73 2c20 6375 7229 290a 2020  l(urls, cur)).  
-0000e470: 2020 2020 2020 2320 6b65 6570 206f 6e6c        # keep onl
-0000e480: 7920 6f6e 6520 6f63 6375 7272 656e 6365  y one occurrence
-0000e490: 206f 6620 6561 6368 2067 6976 656e 206f   of each given o
-0000e4a0: 7269 6769 6e20 7768 696c 6520 6b65 6570  rigin while keep
-0000e4b0: 696e 6720 7468 6520 6c69 7374 0a20 2020  ing the list.   
-0000e4c0: 2020 2020 2023 2073 6f72 7465 6420 6173       # sorted as
-0000e4d0: 206f 7269 6769 6e61 6c6c 7920 6769 7665   originally give
-0000e4e0: 6e0a 2020 2020 2020 2020 746f 5f61 6464  n.        to_add
-0000e4f0: 203d 2073 6f72 7465 6428 7365 7428 7572   = sorted(set(ur
-0000e500: 6c73 2920 2d20 6b6e 6f77 6e5f 6f72 6967  ls) - known_orig
-0000e510: 696e 732c 206b 6579 3d75 726c 732e 696e  ins, key=urls.in
-0000e520: 6465 7829 0a0a 2020 2020 2020 2020 7365  dex)..        se
-0000e530: 6c66 2e6a 6f75 726e 616c 5f77 7269 7465  lf.journal_write
-0000e540: 722e 6f72 6967 696e 5f61 6464 285b 4f72  r.origin_add([Or
-0000e550: 6967 696e 2875 726c 3d75 726c 2920 666f  igin(url=url) fo
-0000e560: 7220 7572 6c20 696e 2074 6f5f 6164 645d  r url in to_add]
-0000e570: 290a 2020 2020 2020 2020 6164 6465 6420  ).        added 
-0000e580: 3d20 300a 2020 2020 2020 2020 666f 7220  = 0.        for 
-0000e590: 7572 6c20 696e 2074 6f5f 6164 643a 0a20  url in to_add:. 
-0000e5a0: 2020 2020 2020 2020 2020 2069 6620 6462             if db
-0000e5b0: 2e6f 7269 6769 6e5f 6164 6428 7572 6c2c  .origin_add(url,
-0000e5c0: 2063 7572 293a 0a20 2020 2020 2020 2020   cur):.         
-0000e5d0: 2020 2020 2020 2061 6464 6564 202b 3d20         added += 
-0000e5e0: 310a 2020 2020 2020 2020 7265 7475 726e  1.        return
-0000e5f0: 207b 226f 7269 6769 6e3a 6164 6422 3a20   {"origin:add": 
-0000e600: 6164 6465 647d 0a0a 2020 2020 2323 2323  added}..    ####
-0000e610: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000e620: 2323 2323 2323 0a20 2020 2023 206d 6973  ######.    # mis
-0000e630: 632e 0a20 2020 2023 2323 2323 2323 2323  c..    #########
-0000e640: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000e650: 230a 0a20 2020 2040 6462 5f74 7261 6e73  #..    @db_trans
-0000e660: 6163 7469 6f6e 2873 7461 7465 6d65 6e74  action(statement
-0000e670: 5f74 696d 656f 7574 3d32 3030 3029 0a20  _timeout=2000). 
-0000e680: 2020 2064 6566 206f 626a 6563 745f 6669     def object_fi
-0000e690: 6e64 5f62 795f 7368 6131 5f67 6974 280a  nd_by_sha1_git(.
-0000e6a0: 2020 2020 2020 2020 7365 6c66 2c20 6964          self, id
-0000e6b0: 733a 204c 6973 745b 5368 6131 4769 745d  s: List[Sha1Git]
-0000e6c0: 2c20 2a2c 2064 623a 2044 622c 2063 7572  , *, db: Db, cur
-0000e6d0: 3d4e 6f6e 650a 2020 2020 2920 2d3e 2044  =None.    ) -> D
-0000e6e0: 6963 745b 5368 6131 4769 742c 204c 6973  ict[Sha1Git, Lis
-0000e6f0: 745b 4469 6374 5d5d 3a0a 2020 2020 2020  t[Dict]]:.      
-0000e700: 2020 7265 743a 2044 6963 745b 5368 6131    ret: Dict[Sha1
-0000e710: 4769 742c 204c 6973 745b 4469 6374 5d5d  Git, List[Dict]]
-0000e720: 203d 207b 6964 3a20 5b5d 2066 6f72 2069   = {id: [] for i
-0000e730: 6420 696e 2069 6473 7d0a 0a20 2020 2020  d in ids}..     
-0000e740: 2020 2066 6f72 2072 6574 7661 6c20 696e     for retval in
-0000e750: 2064 622e 6f62 6a65 6374 5f66 696e 645f   db.object_find_
-0000e760: 6279 5f73 6861 315f 6769 7428 6964 732c  by_sha1_git(ids,
-0000e770: 2063 7572 3d63 7572 293a 0a20 2020 2020   cur=cur):.     
-0000e780: 2020 2020 2020 2069 6620 7265 7476 616c         if retval
-0000e790: 5b31 5d3a 0a20 2020 2020 2020 2020 2020  [1]:.           
-0000e7a0: 2020 2020 2072 6574 5b72 6574 7661 6c5b       ret[retval[
-0000e7b0: 305d 5d2e 6170 7065 6e64 280a 2020 2020  0]].append(.    
-0000e7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e7d0: 6469 6374 287a 6970 2864 622e 6f62 6a65  dict(zip(db.obje
-0000e7e0: 6374 5f66 696e 645f 6279 5f73 6861 315f  ct_find_by_sha1_
-0000e7f0: 6769 745f 636f 6c73 2c20 7265 7476 616c  git_cols, retval
-0000e800: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-0000e810: 2020 2029 0a0a 2020 2020 2020 2020 7265     )..        re
-0000e820: 7475 726e 2072 6574 0a0a 2020 2020 4064  turn ret..    @d
-0000e830: 625f 7472 616e 7361 6374 696f 6e28 7374  b_transaction(st
-0000e840: 6174 656d 656e 745f 7469 6d65 6f75 743d  atement_timeout=
-0000e850: 3530 3029 0a20 2020 2064 6566 2073 7461  500).    def sta
-0000e860: 745f 636f 756e 7465 7273 2873 656c 662c  t_counters(self,
-0000e870: 202a 2c20 6462 3a20 4462 2c20 6375 723d   *, db: Db, cur=
-0000e880: 4e6f 6e65 293a 0a20 2020 2020 2020 2072  None):.        r
-0000e890: 6574 7572 6e20 7b6b 3a20 7620 666f 7220  eturn {k: v for 
-0000e8a0: 286b 2c20 7629 2069 6e20 6462 2e73 7461  (k, v) in db.sta
-0000e8b0: 745f 636f 756e 7465 7273 2829 7d0a 0a20  t_counters()}.. 
-0000e8c0: 2020 2040 6462 5f74 7261 6e73 6163 7469     @db_transacti
-0000e8d0: 6f6e 2829 0a20 2020 2064 6566 2072 6566  on().    def ref
-0000e8e0: 7265 7368 5f73 7461 745f 636f 756e 7465  resh_stat_counte
-0000e8f0: 7273 2873 656c 662c 202a 2c20 6462 3a20  rs(self, *, db: 
-0000e900: 4462 2c20 6375 723d 4e6f 6e65 293a 0a20  Db, cur=None):. 
-0000e910: 2020 2020 2020 206b 6579 7320 3d20 5b0a         keys = [.
-0000e920: 2020 2020 2020 2020 2020 2020 2263 6f6e              "con
-0000e930: 7465 6e74 222c 0a20 2020 2020 2020 2020  tent",.         
-0000e940: 2020 2022 6469 7265 6374 6f72 7922 2c0a     "directory",.
-0000e950: 2020 2020 2020 2020 2020 2020 2264 6972              "dir
-0000e960: 6563 746f 7279 5f65 6e74 7279 5f64 6972  ectory_entry_dir
-0000e970: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-0000e980: 6469 7265 6374 6f72 795f 656e 7472 795f  directory_entry_
-0000e990: 6669 6c65 222c 0a20 2020 2020 2020 2020  file",.         
-0000e9a0: 2020 2022 6469 7265 6374 6f72 795f 656e     "directory_en
-0000e9b0: 7472 795f 7265 7622 2c0a 2020 2020 2020  try_rev",.      
-0000e9c0: 2020 2020 2020 226f 7269 6769 6e22 2c0a        "origin",.
-0000e9d0: 2020 2020 2020 2020 2020 2020 226f 7269              "ori
-0000e9e0: 6769 6e5f 7669 7369 7422 2c0a 2020 2020  gin_visit",.    
-0000e9f0: 2020 2020 2020 2020 2270 6572 736f 6e22          "person"
-0000ea00: 2c0a 2020 2020 2020 2020 2020 2020 2272  ,.            "r
-0000ea10: 656c 6561 7365 222c 0a20 2020 2020 2020  elease",.       
-0000ea20: 2020 2020 2022 7265 7669 7369 6f6e 222c       "revision",
-0000ea30: 0a20 2020 2020 2020 2020 2020 2022 7265  .            "re
-0000ea40: 7669 7369 6f6e 5f68 6973 746f 7279 222c  vision_history",
-0000ea50: 0a20 2020 2020 2020 2020 2020 2022 736b  .            "sk
-0000ea60: 6970 7065 645f 636f 6e74 656e 7422 2c0a  ipped_content",.
-0000ea70: 2020 2020 2020 2020 2020 2020 2273 6e61              "sna
-0000ea80: 7073 686f 7422 2c0a 2020 2020 2020 2020  pshot",.        
-0000ea90: 5d0a 0a20 2020 2020 2020 2066 6f72 206b  ]..        for k
-0000eaa0: 6579 2069 6e20 6b65 7973 3a0a 2020 2020  ey in keys:.    
-0000eab0: 2020 2020 2020 2020 6375 722e 6578 6563          cur.exec
-0000eac0: 7574 6528 2273 656c 6563 7420 2a20 6672  ute("select * fr
-0000ead0: 6f6d 2073 7768 5f75 7064 6174 655f 636f  om swh_update_co
-0000eae0: 756e 7465 7228 2573 2922 2c20 286b 6579  unter(%s)", (key
-0000eaf0: 2c29 290a 0a20 2020 2023 2323 2323 2323  ,))..    #######
-0000eb00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000eb10: 2323 230a 2020 2020 2320 5261 7745 7874  ###.    # RawExt
-0000eb20: 7269 6e73 6963 4d65 7461 6461 7461 0a20  rinsicMetadata. 
-0000eb30: 2020 2023 2323 2323 2323 2323 2323 2323     #############
-0000eb40: 2323 2323 2323 2323 2323 2323 230a 0a20  #############.. 
-0000eb50: 2020 2040 6462 5f74 7261 6e73 6163 7469     @db_transacti
-0000eb60: 6f6e 2829 0a20 2020 2064 6566 2072 6177  on().    def raw
-0000eb70: 5f65 7874 7269 6e73 6963 5f6d 6574 6164  _extrinsic_metad
-0000eb80: 6174 615f 6164 6428 0a20 2020 2020 2020  ata_add(.       
-0000eb90: 2073 656c 662c 0a20 2020 2020 2020 206d   self,.        m
-0000eba0: 6574 6164 6174 613a 204c 6973 745b 5261  etadata: List[Ra
-0000ebb0: 7745 7874 7269 6e73 6963 4d65 7461 6461  wExtrinsicMetada
-0000ebc0: 7461 5d2c 0a20 2020 2020 2020 2064 622c  ta],.        db,
-0000ebd0: 0a20 2020 2020 2020 2063 7572 2c0a 2020  .        cur,.  
-0000ebe0: 2020 2920 2d3e 2044 6963 745b 7374 722c    ) -> Dict[str,
-0000ebf0: 2069 6e74 5d3a 0a20 2020 2020 2020 206d   int]:.        m
-0000ec00: 6574 6164 6174 6120 3d20 6c69 7374 286d  etadata = list(m
-0000ec10: 6574 6164 6174 6129 0a20 2020 2020 2020  etadata).       
-0000ec20: 2073 656c 662e 6a6f 7572 6e61 6c5f 7772   self.journal_wr
-0000ec30: 6974 6572 2e72 6177 5f65 7874 7269 6e73  iter.raw_extrins
-0000ec40: 6963 5f6d 6574 6164 6174 615f 6164 6428  ic_metadata_add(
-0000ec50: 6d65 7461 6461 7461 290a 2020 2020 2020  metadata).      
-0000ec60: 2020 636f 756e 7465 7220 3d20 436f 756e    counter = Coun
-0000ec70: 7465 725b 4578 7465 6e64 6564 4f62 6a65  ter[ExtendedObje
-0000ec80: 6374 5479 7065 5d28 290a 2020 2020 2020  ctType]().      
-0000ec90: 2020 666f 7220 6d65 7461 6461 7461 5f65    for metadata_e
-0000eca0: 6e74 7279 2069 6e20 6d65 7461 6461 7461  ntry in metadata
-0000ecb0: 3a0a 2020 2020 2020 2020 2020 2020 6175  :.            au
-0000ecc0: 7468 6f72 6974 795f 6964 203d 2073 656c  thority_id = sel
-0000ecd0: 662e 5f67 6574 5f61 7574 686f 7269 7479  f._get_authority
-0000ece0: 5f69 6428 6d65 7461 6461 7461 5f65 6e74  _id(metadata_ent
-0000ecf0: 7279 2e61 7574 686f 7269 7479 2c20 6462  ry.authority, db
-0000ed00: 2c20 6375 7229 0a20 2020 2020 2020 2020  , cur).         
-0000ed10: 2020 2066 6574 6368 6572 5f69 6420 3d20     fetcher_id = 
-0000ed20: 7365 6c66 2e5f 6765 745f 6665 7463 6865  self._get_fetche
-0000ed30: 725f 6964 286d 6574 6164 6174 615f 656e  r_id(metadata_en
-0000ed40: 7472 792e 6665 7463 6865 722c 2064 622c  try.fetcher, db,
-0000ed50: 2063 7572 290a 0a20 2020 2020 2020 2020   cur)..         
-0000ed60: 2020 2064 622e 7261 775f 6578 7472 696e     db.raw_extrin
-0000ed70: 7369 635f 6d65 7461 6461 7461 5f61 6464  sic_metadata_add
-0000ed80: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000ed90: 2020 6964 3d6d 6574 6164 6174 615f 656e    id=metadata_en
-0000eda0: 7472 792e 6964 2c0a 2020 2020 2020 2020  try.id,.        
-0000edb0: 2020 2020 2020 2020 7479 7065 3d6d 6574          type=met
-0000edc0: 6164 6174 615f 656e 7472 792e 7461 7267  adata_entry.targ
-0000edd0: 6574 2e6f 626a 6563 745f 7479 7065 2e6e  et.object_type.n
-0000ede0: 616d 652e 6c6f 7765 7228 292c 0a20 2020  ame.lower(),.   
-0000edf0: 2020 2020 2020 2020 2020 2020 2074 6172               tar
-0000ee00: 6765 743d 7374 7228 6d65 7461 6461 7461  get=str(metadata
-0000ee10: 5f65 6e74 7279 2e74 6172 6765 7429 2c0a  _entry.target),.
-0000ee20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee30: 6469 7363 6f76 6572 795f 6461 7465 3d6d  discovery_date=m
-0000ee40: 6574 6164 6174 615f 656e 7472 792e 6469  etadata_entry.di
-0000ee50: 7363 6f76 6572 795f 6461 7465 2c0a 2020  scovery_date,.  
-0000ee60: 2020 2020 2020 2020 2020 2020 2020 6175                au
-0000ee70: 7468 6f72 6974 795f 6964 3d61 7574 686f  thority_id=autho
-0000ee80: 7269 7479 5f69 642c 0a20 2020 2020 2020  rity_id,.       
-0000ee90: 2020 2020 2020 2020 2066 6574 6368 6572           fetcher
-0000eea0: 5f69 643d 6665 7463 6865 725f 6964 2c0a  _id=fetcher_id,.
-0000eeb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eec0: 666f 726d 6174 3d6d 6574 6164 6174 615f  format=metadata_
-0000eed0: 656e 7472 792e 666f 726d 6174 2c0a 2020  entry.format,.  
-0000eee0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-0000eef0: 7461 6461 7461 3d6d 6574 6164 6174 615f  tadata=metadata_
-0000ef00: 656e 7472 792e 6d65 7461 6461 7461 2c0a  entry.metadata,.
-0000ef10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ef20: 6f72 6967 696e 3d6d 6574 6164 6174 615f  origin=metadata_
-0000ef30: 656e 7472 792e 6f72 6967 696e 2c0a 2020  entry.origin,.  
-0000ef40: 2020 2020 2020 2020 2020 2020 2020 7669                vi
-0000ef50: 7369 743d 6d65 7461 6461 7461 5f65 6e74  sit=metadata_ent
-0000ef60: 7279 2e76 6973 6974 2c0a 2020 2020 2020  ry.visit,.      
-0000ef70: 2020 2020 2020 2020 2020 736e 6170 7368            snapsh
-0000ef80: 6f74 3d6d 6170 5f6f 7074 696f 6e61 6c28  ot=map_optional(
-0000ef90: 7374 722c 206d 6574 6164 6174 615f 656e  str, metadata_en
-0000efa0: 7472 792e 736e 6170 7368 6f74 292c 0a20  try.snapshot),. 
-0000efb0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000efc0: 656c 6561 7365 3d6d 6170 5f6f 7074 696f  elease=map_optio
-0000efd0: 6e61 6c28 7374 722c 206d 6574 6164 6174  nal(str, metadat
-0000efe0: 615f 656e 7472 792e 7265 6c65 6173 6529  a_entry.release)
-0000eff0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000f000: 2020 7265 7669 7369 6f6e 3d6d 6170 5f6f    revision=map_o
-0000f010: 7074 696f 6e61 6c28 7374 722c 206d 6574  ptional(str, met
-0000f020: 6164 6174 615f 656e 7472 792e 7265 7669  adata_entry.revi
-0000f030: 7369 6f6e 292c 0a20 2020 2020 2020 2020  sion),.         
-0000f040: 2020 2020 2020 2070 6174 683d 6d65 7461         path=meta
-0000f050: 6461 7461 5f65 6e74 7279 2e70 6174 682c  data_entry.path,
-0000f060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f070: 2064 6972 6563 746f 7279 3d6d 6170 5f6f   directory=map_o
-0000f080: 7074 696f 6e61 6c28 7374 722c 206d 6574  ptional(str, met
-0000f090: 6164 6174 615f 656e 7472 792e 6469 7265  adata_entry.dire
-0000f0a0: 6374 6f72 7929 2c0a 2020 2020 2020 2020  ctory),.        
-0000f0b0: 2020 2020 2020 2020 6375 723d 6375 722c          cur=cur,
-0000f0c0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0000f0d0: 2020 2020 2020 2020 2020 2063 6f75 6e74             count
-0000f0e0: 6572 5b6d 6574 6164 6174 615f 656e 7472  er[metadata_entr
-0000f0f0: 792e 7461 7267 6574 2e6f 626a 6563 745f  y.target.object_
-0000f100: 7479 7065 5d20 2b3d 2031 0a0a 2020 2020  type] += 1..    
-0000f110: 2020 2020 7265 7475 726e 207b 0a20 2020      return {.   
-0000f120: 2020 2020 2020 2020 2066 227b 7479 7065           f"{type
-0000f130: 2e76 616c 7565 7d5f 6d65 7461 6461 7461  .value}_metadata
-0000f140: 3a61 6464 223a 2063 6f75 6e74 2066 6f72  :add": count for
-0000f150: 2028 7479 7065 2c20 636f 756e 7429 2069   (type, count) i
-0000f160: 6e20 636f 756e 7465 722e 6974 656d 7328  n counter.items(
-0000f170: 290a 2020 2020 2020 2020 7d0a 0a20 2020  ).        }..   
-0000f180: 2040 6462 5f74 7261 6e73 6163 7469 6f6e   @db_transaction
-0000f190: 2829 0a20 2020 2064 6566 2072 6177 5f65  ().    def raw_e
-0000f1a0: 7874 7269 6e73 6963 5f6d 6574 6164 6174  xtrinsic_metadat
-0000f1b0: 615f 6765 7428 0a20 2020 2020 2020 2073  a_get(.        s
-0000f1c0: 656c 662c 0a20 2020 2020 2020 2074 6172  elf,.        tar
-0000f1d0: 6765 743a 2045 7874 656e 6465 6453 5748  get: ExtendedSWH
-0000f1e0: 4944 2c0a 2020 2020 2020 2020 6175 7468  ID,.        auth
-0000f1f0: 6f72 6974 793a 204d 6574 6164 6174 6141  ority: MetadataA
-0000f200: 7574 686f 7269 7479 2c0a 2020 2020 2020  uthority,.      
-0000f210: 2020 6166 7465 723a 204f 7074 696f 6e61    after: Optiona
-0000f220: 6c5b 6461 7465 7469 6d65 2e64 6174 6574  l[datetime.datet
-0000f230: 696d 655d 203d 204e 6f6e 652c 0a20 2020  ime] = None,.   
-0000f240: 2020 2020 2070 6167 655f 746f 6b65 6e3a       page_token:
-0000f250: 204f 7074 696f 6e61 6c5b 6279 7465 735d   Optional[bytes]
-0000f260: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0000f270: 206c 696d 6974 3a20 696e 7420 3d20 3130   limit: int = 10
-0000f280: 3030 2c0a 2020 2020 2020 2020 2a2c 0a20  00,.        *,. 
-0000f290: 2020 2020 2020 2064 623a 2044 622c 0a20         db: Db,. 
-0000f2a0: 2020 2020 2020 2063 7572 3d4e 6f6e 652c         cur=None,
-0000f2b0: 0a20 2020 2029 202d 3e20 5061 6765 6452  .    ) -> PagedR
-0000f2c0: 6573 756c 745b 5261 7745 7874 7269 6e73  esult[RawExtrins
-0000f2d0: 6963 4d65 7461 6461 7461 5d3a 0a20 2020  icMetadata]:.   
-0000f2e0: 2020 2020 2069 6620 7061 6765 5f74 6f6b       if page_tok
-0000f2f0: 656e 3a0a 2020 2020 2020 2020 2020 2020  en:.            
-0000f300: 2861 6674 6572 5f74 696d 652c 2061 6674  (after_time, aft
-0000f310: 6572 5f66 6574 6368 6572 2920 3d20 6d73  er_fetcher) = ms
-0000f320: 6770 6163 6b5f 6c6f 6164 7328 6261 7365  gpack_loads(base
-0000f330: 3634 2e62 3634 6465 636f 6465 2870 6167  64.b64decode(pag
-0000f340: 655f 746f 6b65 6e29 290a 2020 2020 2020  e_token)).      
-0000f350: 2020 2020 2020 6966 2061 6674 6572 2061        if after a
-0000f360: 6e64 2061 6674 6572 5f74 696d 6520 3c20  nd after_time < 
-0000f370: 6166 7465 723a 0a20 2020 2020 2020 2020  after:.         
-0000f380: 2020 2020 2020 2072 6169 7365 2053 746f         raise Sto
-0000f390: 7261 6765 4172 6775 6d65 6e74 4578 6365  rageArgumentExce
-0000f3a0: 7074 696f 6e28 0a20 2020 2020 2020 2020  ption(.         
-0000f3b0: 2020 2020 2020 2020 2020 2022 7061 6765             "page
-0000f3c0: 5f74 6f6b 656e 2069 7320 696e 636f 6e73  _token is incons
-0000f3d0: 6973 7465 6e74 2077 6974 6820 7468 6520  istent with the 
-0000f3e0: 7661 6c75 6520 6f66 2027 6166 7465 7227  value of 'after'
-0000f3f0: 2e22 0a20 2020 2020 2020 2020 2020 2020  .".             
-0000f400: 2020 2029 0a20 2020 2020 2020 2065 6c73     ).        els
-0000f410: 653a 0a20 2020 2020 2020 2020 2020 2061  e:.            a
-0000f420: 6674 6572 5f74 696d 6520 3d20 6166 7465  fter_time = afte
-0000f430: 720a 2020 2020 2020 2020 2020 2020 6166  r.            af
-0000f440: 7465 725f 6665 7463 6865 7220 3d20 4e6f  ter_fetcher = No
-0000f450: 6e65 0a0a 2020 2020 2020 2020 7472 793a  ne..        try:
-0000f460: 0a20 2020 2020 2020 2020 2020 2061 7574  .            aut
-0000f470: 686f 7269 7479 5f69 6420 3d20 7365 6c66  hority_id = self
-0000f480: 2e5f 6765 745f 6175 7468 6f72 6974 795f  ._get_authority_
-0000f490: 6964 2861 7574 686f 7269 7479 2c20 6462  id(authority, db
-0000f4a0: 2c20 6375 7229 0a20 2020 2020 2020 2065  , cur).        e
-0000f4b0: 7863 6570 7420 556e 6b6e 6f77 6e4d 6574  xcept UnknownMet
-0000f4c0: 6164 6174 6141 7574 686f 7269 7479 3a0a  adataAuthority:.
-0000f4d0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000f4e0: 726e 2050 6167 6564 5265 7375 6c74 280a  rn PagedResult(.
-0000f4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f500: 6e65 7874 5f70 6167 655f 746f 6b65 6e3d  next_page_token=
-0000f510: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-0000f520: 2020 2020 2020 7265 7375 6c74 733d 5b5d        results=[]
-0000f530: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-0000f540: 0a20 2020 2020 2020 2072 6f77 7320 3d20  .        rows = 
-0000f550: 6462 2e72 6177 5f65 7874 7269 6e73 6963  db.raw_extrinsic
-0000f560: 5f6d 6574 6164 6174 615f 6765 7428 0a20  _metadata_get(. 
-0000f570: 2020 2020 2020 2020 2020 2073 7472 2874             str(t
-0000f580: 6172 6765 7429 2c0a 2020 2020 2020 2020  arget),.        
-0000f590: 2020 2020 6175 7468 6f72 6974 795f 6964      authority_id
-0000f5a0: 2c0a 2020 2020 2020 2020 2020 2020 6166  ,.            af
-0000f5b0: 7465 725f 7469 6d65 2c0a 2020 2020 2020  ter_time,.      
-0000f5c0: 2020 2020 2020 6166 7465 725f 6665 7463        after_fetc
-0000f5d0: 6865 722c 0a20 2020 2020 2020 2020 2020  her,.           
-0000f5e0: 206c 696d 6974 202b 2031 2c0a 2020 2020   limit + 1,.    
-0000f5f0: 2020 2020 2020 2020 6375 722c 0a20 2020          cur,.   
-0000f600: 2020 2020 2029 0a20 2020 2020 2020 2072       ).        r
-0000f610: 6f77 7320 3d20 5b64 6963 7428 7a69 7028  ows = [dict(zip(
-0000f620: 6462 2e72 6177 5f65 7874 7269 6e73 6963  db.raw_extrinsic
-0000f630: 5f6d 6574 6164 6174 615f 6765 745f 636f  _metadata_get_co
-0000f640: 6c73 2c20 726f 7729 2920 666f 7220 726f  ls, row)) for ro
-0000f650: 7720 696e 2072 6f77 735d 0a20 2020 2020  w in rows].     
-0000f660: 2020 2072 6573 756c 7473 203d 205b 5d0a     results = [].
-0000f670: 2020 2020 2020 2020 666f 7220 726f 7720          for row 
-0000f680: 696e 2072 6f77 733a 0a20 2020 2020 2020  in rows:.       
-0000f690: 2020 2020 2061 7373 6572 7420 7374 7228       assert str(
-0000f6a0: 7461 7267 6574 2920 3d3d 2072 6f77 5b22  target) == row["
-0000f6b0: 7261 775f 6578 7472 696e 7369 635f 6d65  raw_extrinsic_me
-0000f6c0: 7461 6461 7461 2e74 6172 6765 7422 5d0a  tadata.target"].
-0000f6d0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0000f6e0: 6c74 732e 6170 7065 6e64 2863 6f6e 7665  lts.append(conve
-0000f6f0: 7274 6572 732e 6462 5f74 6f5f 7261 775f  rters.db_to_raw_
-0000f700: 6578 7472 696e 7369 635f 6d65 7461 6461  extrinsic_metada
-0000f710: 7461 2872 6f77 2929 0a0a 2020 2020 2020  ta(row))..      
-0000f720: 2020 6966 206c 656e 2872 6573 756c 7473    if len(results
-0000f730: 2920 3e20 6c69 6d69 743a 0a20 2020 2020  ) > limit:.     
-0000f740: 2020 2020 2020 2072 6573 756c 7473 2e70         results.p
-0000f750: 6f70 2829 0a20 2020 2020 2020 2020 2020  op().           
-0000f760: 2061 7373 6572 7420 6c65 6e28 7265 7375   assert len(resu
-0000f770: 6c74 7329 203d 3d20 6c69 6d69 740a 2020  lts) == limit.  
-0000f780: 2020 2020 2020 2020 2020 6c61 7374 5f72            last_r
-0000f790: 6574 7572 6e65 645f 726f 7720 3d20 726f  eturned_row = ro
-0000f7a0: 7773 5b2d 325d 2020 2320 726f 7773 5b2d  ws[-2]  # rows[-
-0000f7b0: 315d 2063 6f72 7265 7370 6f6e 6473 2074  1] corresponds t
-0000f7c0: 6f20 7468 6520 706f 7070 6564 2072 6573  o the popped res
-0000f7d0: 756c 740a 2020 2020 2020 2020 2020 2020  ult.            
-0000f7e0: 6e65 7874 5f70 6167 655f 746f 6b65 6e3a  next_page_token:
-0000f7f0: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
-0000f800: 2062 6173 6536 342e 6236 3465 6e63 6f64   base64.b64encod
-0000f810: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-0000f820: 2020 206d 7367 7061 636b 5f64 756d 7073     msgpack_dumps
-0000f830: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000f840: 2020 2020 2020 280a 2020 2020 2020 2020        (.        
-0000f850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f860: 6c61 7374 5f72 6574 7572 6e65 645f 726f  last_returned_ro
-0000f870: 775b 2264 6973 636f 7665 7279 5f64 6174  w["discovery_dat
-0000f880: 6522 5d2c 0a20 2020 2020 2020 2020 2020  e"],.           
-0000f890: 2020 2020 2020 2020 2020 2020 206c 6173               las
-0000f8a0: 745f 7265 7475 726e 6564 5f72 6f77 5b22  t_returned_row["
-0000f8b0: 6d65 7461 6461 7461 5f66 6574 6368 6572  metadata_fetcher
-0000f8c0: 2e69 6422 5d2c 0a20 2020 2020 2020 2020  .id"],.         
-0000f8d0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0000f8e0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-0000f8f0: 2020 2020 2020 2020 2020 2029 2e64 6563             ).dec
-0000f900: 6f64 6528 290a 2020 2020 2020 2020 656c  ode().        el
-0000f910: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000f920: 6e65 7874 5f70 6167 655f 746f 6b65 6e20  next_page_token 
-0000f930: 3d20 4e6f 6e65 0a0a 2020 2020 2020 2020  = None..        
-0000f940: 7265 7475 726e 2050 6167 6564 5265 7375  return PagedResu
-0000f950: 6c74 280a 2020 2020 2020 2020 2020 2020  lt(.            
-0000f960: 6e65 7874 5f70 6167 655f 746f 6b65 6e3d  next_page_token=
-0000f970: 6e65 7874 5f70 6167 655f 746f 6b65 6e2c  next_page_token,
-0000f980: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0000f990: 756c 7473 3d72 6573 756c 7473 2c0a 2020  ults=results,.  
-0000f9a0: 2020 2020 2020 290a 0a20 2020 2040 6462        )..    @db
-0000f9b0: 5f74 7261 6e73 6163 7469 6f6e 2829 0a20  _transaction(). 
-0000f9c0: 2020 2064 6566 2072 6177 5f65 7874 7269     def raw_extri
-0000f9d0: 6e73 6963 5f6d 6574 6164 6174 615f 6765  nsic_metadata_ge
-0000f9e0: 745f 6279 5f69 6473 280a 2020 2020 2020  t_by_ids(.      
-0000f9f0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0000fa00: 6964 733a 204c 6973 745b 5368 6131 4769  ids: List[Sha1Gi
-0000fa10: 745d 2c0a 2020 2020 2020 2020 2a2c 0a20  t],.        *,. 
-0000fa20: 2020 2020 2020 2064 623a 2044 622c 0a20         db: Db,. 
-0000fa30: 2020 2020 2020 2063 7572 3d4e 6f6e 652c         cur=None,
-0000fa40: 0a20 2020 2029 202d 3e20 4c69 7374 5b52  .    ) -> List[R
-0000fa50: 6177 4578 7472 696e 7369 634d 6574 6164  awExtrinsicMetad
-0000fa60: 6174 615d 3a0a 2020 2020 2020 2020 7265  ata]:.        re
-0000fa70: 7475 726e 205b 0a20 2020 2020 2020 2020  turn [.         
-0000fa80: 2020 2063 6f6e 7665 7274 6572 732e 6462     converters.db
-0000fa90: 5f74 6f5f 7261 775f 6578 7472 696e 7369  _to_raw_extrinsi
-0000faa0: 635f 6d65 7461 6461 7461 280a 2020 2020  c_metadata(.    
-0000fab0: 2020 2020 2020 2020 2020 2020 6469 6374              dict
-0000fac0: 287a 6970 2864 622e 7261 775f 6578 7472  (zip(db.raw_extr
-0000fad0: 696e 7369 635f 6d65 7461 6461 7461 5f67  insic_metadata_g
-0000fae0: 6574 5f63 6f6c 732c 2072 6f77 2929 0a20  et_cols, row)). 
-0000faf0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0000fb00: 2020 2020 2020 2020 2066 6f72 2072 6f77           for row
-0000fb10: 2069 6e20 6462 2e72 6177 5f65 7874 7269   in db.raw_extri
-0000fb20: 6e73 6963 5f6d 6574 6164 6174 615f 6765  nsic_metadata_ge
-0000fb30: 745f 6279 5f69 6473 2869 6473 290a 2020  t_by_ids(ids).  
-0000fb40: 2020 2020 2020 5d0a 0a20 2020 2023 2323        ]..    ###
-0000fb50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000fb60: 2323 2323 2323 230a 2020 2020 2320 4d65  #######.    # Me
-0000fb70: 7461 6461 7461 4665 7463 6865 7220 616e  tadataFetcher an
-0000fb80: 6420 4d65 7461 6461 7461 4175 7468 6f72  d MetadataAuthor
-0000fb90: 6974 790a 2020 2020 2323 2323 2323 2323  ity.    ########
-0000fba0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000fbb0: 2323 0a0a 2020 2020 4064 625f 7472 616e  ##..    @db_tran
-0000fbc0: 7361 6374 696f 6e28 290a 2020 2020 6465  saction().    de
-0000fbd0: 6620 6d65 7461 6461 7461 5f66 6574 6368  f metadata_fetch
-0000fbe0: 6572 5f61 6464 280a 2020 2020 2020 2020  er_add(.        
-0000fbf0: 7365 6c66 2c20 6665 7463 6865 7273 3a20  self, fetchers: 
-0000fc00: 4c69 7374 5b4d 6574 6164 6174 6146 6574  List[MetadataFet
-0000fc10: 6368 6572 5d2c 202a 2c20 6462 3a20 4462  cher], *, db: Db
-0000fc20: 2c20 6375 723d 4e6f 6e65 0a20 2020 2029  , cur=None.    )
-0000fc30: 202d 3e20 4469 6374 5b73 7472 2c20 696e   -> Dict[str, in
-0000fc40: 745d 3a0a 2020 2020 2020 2020 6665 7463  t]:.        fetc
-0000fc50: 6865 7273 203d 206c 6973 7428 6665 7463  hers = list(fetc
-0000fc60: 6865 7273 290a 2020 2020 2020 2020 7365  hers).        se
-0000fc70: 6c66 2e6a 6f75 726e 616c 5f77 7269 7465  lf.journal_write
-0000fc80: 722e 6d65 7461 6461 7461 5f66 6574 6368  r.metadata_fetch
-0000fc90: 6572 5f61 6464 2866 6574 6368 6572 7329  er_add(fetchers)
-0000fca0: 0a20 2020 2020 2020 2063 6f75 6e74 203d  .        count =
-0000fcb0: 2030 0a20 2020 2020 2020 2066 6f72 2066   0.        for f
-0000fcc0: 6574 6368 6572 2069 6e20 6665 7463 6865  etcher in fetche
-0000fcd0: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
-0000fce0: 6462 2e6d 6574 6164 6174 615f 6665 7463  db.metadata_fetc
-0000fcf0: 6865 725f 6164 6428 6665 7463 6865 722e  her_add(fetcher.
-0000fd00: 6e61 6d65 2c20 6665 7463 6865 722e 7665  name, fetcher.ve
-0000fd10: 7273 696f 6e2c 2063 7572 3d63 7572 290a  rsion, cur=cur).
-0000fd20: 2020 2020 2020 2020 2020 2020 636f 756e              coun
-0000fd30: 7420 2b3d 2031 0a20 2020 2020 2020 2072  t += 1.        r
-0000fd40: 6574 7572 6e20 7b22 6d65 7461 6461 7461  eturn {"metadata
-0000fd50: 5f66 6574 6368 6572 3a61 6464 223a 2063  _fetcher:add": c
-0000fd60: 6f75 6e74 7d0a 0a20 2020 2040 6462 5f74  ount}..    @db_t
-0000fd70: 7261 6e73 6163 7469 6f6e 2873 7461 7465  ransaction(state
-0000fd80: 6d65 6e74 5f74 696d 656f 7574 3d35 3030  ment_timeout=500
-0000fd90: 290a 2020 2020 6465 6620 6d65 7461 6461  ).    def metada
-0000fda0: 7461 5f66 6574 6368 6572 5f67 6574 280a  ta_fetcher_get(.
-0000fdb0: 2020 2020 2020 2020 7365 6c66 2c20 6e61          self, na
-0000fdc0: 6d65 3a20 7374 722c 2076 6572 7369 6f6e  me: str, version
-0000fdd0: 3a20 7374 722c 202a 2c20 6462 3a20 4462  : str, *, db: Db
-0000fde0: 2c20 6375 723d 4e6f 6e65 0a20 2020 2029  , cur=None.    )
-0000fdf0: 202d 3e20 4f70 7469 6f6e 616c 5b4d 6574   -> Optional[Met
-0000fe00: 6164 6174 6146 6574 6368 6572 5d3a 0a20  adataFetcher]:. 
-0000fe10: 2020 2020 2020 2072 6f77 203d 2064 622e         row = db.
-0000fe20: 6d65 7461 6461 7461 5f66 6574 6368 6572  metadata_fetcher
-0000fe30: 5f67 6574 286e 616d 652c 2076 6572 7369  _get(name, versi
-0000fe40: 6f6e 2c20 6375 723d 6375 7229 0a20 2020  on, cur=cur).   
-0000fe50: 2020 2020 2069 6620 6e6f 7420 726f 773a       if not row:
-0000fe60: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000fe70: 7572 6e20 4e6f 6e65 0a20 2020 2020 2020  urn None.       
-0000fe80: 2072 6574 7572 6e20 4d65 7461 6461 7461   return Metadata
-0000fe90: 4665 7463 6865 722e 6672 6f6d 5f64 6963  Fetcher.from_dic
-0000fea0: 7428 6469 6374 287a 6970 2864 622e 6d65  t(dict(zip(db.me
-0000feb0: 7461 6461 7461 5f66 6574 6368 6572 5f63  tadata_fetcher_c
-0000fec0: 6f6c 732c 2072 6f77 2929 290a 0a20 2020  ols, row)))..   
-0000fed0: 2040 6462 5f74 7261 6e73 6163 7469 6f6e   @db_transaction
-0000fee0: 2829 0a20 2020 2064 6566 2072 6177 5f65  ().    def raw_e
-0000fef0: 7874 7269 6e73 6963 5f6d 6574 6164 6174  xtrinsic_metadat
-0000ff00: 615f 6765 745f 6175 7468 6f72 6974 6965  a_get_authoritie
-0000ff10: 7328 0a20 2020 2020 2020 2073 656c 662c  s(.        self,
-0000ff20: 0a20 2020 2020 2020 2074 6172 6765 743a  .        target:
-0000ff30: 2045 7874 656e 6465 6453 5748 4944 2c0a   ExtendedSWHID,.
-0000ff40: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
-0000ff50: 2020 2064 623a 2044 622c 0a20 2020 2020     db: Db,.     
-0000ff60: 2020 2063 7572 3d4e 6f6e 652c 0a20 2020     cur=None,.   
-0000ff70: 2029 202d 3e20 4c69 7374 5b4d 6574 6164   ) -> List[Metad
-0000ff80: 6174 6141 7574 686f 7269 7479 5d3a 0a20  ataAuthority]:. 
-0000ff90: 2020 2020 2020 2072 6574 7572 6e20 5b0a         return [.
-0000ffa0: 2020 2020 2020 2020 2020 2020 4d65 7461              Meta
-0000ffb0: 6461 7461 4175 7468 6f72 6974 7928 0a20  dataAuthority(. 
-0000ffc0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000ffd0: 7970 653d 4d65 7461 6461 7461 4175 7468  ype=MetadataAuth
-0000ffe0: 6f72 6974 7954 7970 6528 6175 7468 6f72  orityType(author
-0000fff0: 6974 795f 7479 7065 292c 2075 726c 3d61  ity_type), url=a
-00010000: 7574 686f 7269 7479 5f75 726c 0a20 2020  uthority_url.   
-00010010: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00010020: 2020 2020 2020 2066 6f72 2028 0a20 2020         for (.   
-00010030: 2020 2020 2020 2020 2020 2020 2061 7574               aut
-00010040: 686f 7269 7479 5f74 7970 652c 0a20 2020  hority_type,.   
+0000ba70: 4f72 6967 696e 5669 7369 7428 0a20 2020  OriginVisit(.   
+0000ba80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba90: 206f 7269 6769 6e3d 726f 775f 645b 226f   origin=row_d["o
+0000baa0: 7269 6769 6e22 5d2c 0a20 2020 2020 2020  rigin"],.       
+0000bab0: 2020 2020 2020 2020 2020 2020 2076 6973               vis
+0000bac0: 6974 3d72 6f77 5f64 5b22 7669 7369 7422  it=row_d["visit"
+0000bad0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+0000bae0: 2020 2020 2020 2064 6174 653d 726f 775f         date=row_
+0000baf0: 645b 2264 6174 6522 5d2c 0a20 2020 2020  d["date"],.     
+0000bb00: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000bb10: 7970 653d 726f 775f 645b 2274 7970 6522  ype=row_d["type"
+0000bb20: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+0000bb30: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0000bb40: 2029 0a0a 2020 2020 2020 2020 6173 7365   )..        asse
+0000bb50: 7274 206c 656e 2876 6973 6974 7329 203c  rt len(visits) <
+0000bb60: 3d20 6578 7472 615f 6c69 6d69 740a 0a20  = extra_limit.. 
+0000bb70: 2020 2020 2020 2069 6620 6c65 6e28 7669         if len(vi
+0000bb80: 7369 7473 2920 3d3d 2065 7874 7261 5f6c  sits) == extra_l
+0000bb90: 696d 6974 3a0a 2020 2020 2020 2020 2020  imit:.          
+0000bba0: 2020 7669 7369 7473 203d 2076 6973 6974    visits = visit
+0000bbb0: 735b 3a6c 696d 6974 5d0a 2020 2020 2020  s[:limit].      
+0000bbc0: 2020 2020 2020 6e65 7874 5f70 6167 655f        next_page_
+0000bbd0: 746f 6b65 6e20 3d20 7374 7228 7669 7369  token = str(visi
+0000bbe0: 7473 5b2d 315d 2e76 6973 6974 290a 0a20  ts[-1].visit).. 
+0000bbf0: 2020 2020 2020 2072 6574 7572 6e20 5061         return Pa
+0000bc00: 6765 6452 6573 756c 7428 7265 7375 6c74  gedResult(result
+0000bc10: 733d 7669 7369 7473 2c20 6e65 7874 5f70  s=visits, next_p
+0000bc20: 6167 655f 746f 6b65 6e3d 6e65 7874 5f70  age_token=next_p
+0000bc30: 6167 655f 746f 6b65 6e29 0a0a 2020 2020  age_token)..    
+0000bc40: 4064 625f 7472 616e 7361 6374 696f 6e28  @db_transaction(
+0000bc50: 7374 6174 656d 656e 745f 7469 6d65 6f75  statement_timeou
+0000bc60: 743d 3230 3030 290a 2020 2020 6465 6620  t=2000).    def 
+0000bc70: 6f72 6967 696e 5f76 6973 6974 5f67 6574  origin_visit_get
+0000bc80: 5f77 6974 685f 7374 6174 7573 6573 280a  _with_statuses(.
+0000bc90: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+0000bca0: 2020 2020 2020 6f72 6967 696e 3a20 7374        origin: st
+0000bcb0: 722c 0a20 2020 2020 2020 2061 6c6c 6f77  r,.        allow
+0000bcc0: 6564 5f73 7461 7475 7365 733a 204f 7074  ed_statuses: Opt
+0000bcd0: 696f 6e61 6c5b 4c69 7374 5b73 7472 5d5d  ional[List[str]]
+0000bce0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0000bcf0: 2072 6571 7569 7265 5f73 6e61 7073 686f   require_snapsho
+0000bd00: 743a 2062 6f6f 6c20 3d20 4661 6c73 652c  t: bool = False,
+0000bd10: 0a20 2020 2020 2020 2070 6167 655f 746f  .        page_to
+0000bd20: 6b65 6e3a 204f 7074 696f 6e61 6c5b 7374  ken: Optional[st
+0000bd30: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
+0000bd40: 2020 206f 7264 6572 3a20 4c69 7374 4f72     order: ListOr
+0000bd50: 6465 7220 3d20 4c69 7374 4f72 6465 722e  der = ListOrder.
+0000bd60: 4153 432c 0a20 2020 2020 2020 206c 696d  ASC,.        lim
+0000bd70: 6974 3a20 696e 7420 3d20 3130 2c0a 2020  it: int = 10,.  
+0000bd80: 2020 2020 2020 2a2c 0a20 2020 2020 2020        *,.       
+0000bd90: 2064 623a 2044 622c 0a20 2020 2020 2020   db: Db,.       
+0000bda0: 2063 7572 3d4e 6f6e 652c 0a20 2020 2029   cur=None,.    )
+0000bdb0: 202d 3e20 5061 6765 6452 6573 756c 745b   -> PagedResult[
+0000bdc0: 4f72 6967 696e 5669 7369 7457 6974 6853  OriginVisitWithS
+0000bdd0: 7461 7475 7365 735d 3a0a 2020 2020 2020  tatuses]:.      
+0000bde0: 2020 7061 6765 5f74 6f6b 656e 203d 2070    page_token = p
+0000bdf0: 6167 655f 746f 6b65 6e20 6f72 2022 3022  age_token or "0"
+0000be00: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+0000be10: 6973 696e 7374 616e 6365 286f 7264 6572  isinstance(order
+0000be20: 2c20 4c69 7374 4f72 6465 7229 3a0a 2020  , ListOrder):.  
+0000be30: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0000be40: 5374 6f72 6167 6541 7267 756d 656e 7445  StorageArgumentE
+0000be50: 7863 6570 7469 6f6e 2822 6f72 6465 7220  xception("order 
+0000be60: 6d75 7374 2062 6520 6120 4c69 7374 4f72  must be a ListOr
+0000be70: 6465 7220 7661 6c75 6522 290a 2020 2020  der value").    
+0000be80: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
+0000be90: 7461 6e63 6528 7061 6765 5f74 6f6b 656e  tance(page_token
+0000bea0: 2c20 7374 7229 3a0a 2020 2020 2020 2020  , str):.        
+0000beb0: 2020 2020 7261 6973 6520 5374 6f72 6167      raise Storag
+0000bec0: 6541 7267 756d 656e 7445 7863 6570 7469  eArgumentExcepti
+0000bed0: 6f6e 2822 7061 6765 5f74 6f6b 656e 206d  on("page_token m
+0000bee0: 7573 7420 6265 2061 2073 7472 696e 672e  ust be a string.
+0000bef0: 2229 0a0a 2020 2020 2020 2020 2320 4669  ")..        # Fi
+0000bf00: 7273 7420 6765 7420 7669 7369 7473 2028  rst get visits (
+0000bf10: 706c 7573 206f 6e65 2073 6f20 7765 2063  plus one so we c
+0000bf20: 616e 2075 7365 2069 7420 6173 2074 6865  an use it as the
+0000bf30: 206e 6578 7420 7061 6765 2074 6f6b 656e   next page token
+0000bf40: 2069 6620 616e 7929 0a20 2020 2020 2020   if any).       
+0000bf50: 2076 6973 6974 735f 7061 6765 203d 2073   visits_page = s
+0000bf60: 656c 662e 6f72 6967 696e 5f76 6973 6974  elf.origin_visit
+0000bf70: 5f67 6574 280a 2020 2020 2020 2020 2020  _get(.          
+0000bf80: 2020 6f72 6967 696e 3d6f 7269 6769 6e2c    origin=origin,
+0000bf90: 0a20 2020 2020 2020 2020 2020 2070 6167  .            pag
+0000bfa0: 655f 746f 6b65 6e3d 7061 6765 5f74 6f6b  e_token=page_tok
+0000bfb0: 656e 2c0a 2020 2020 2020 2020 2020 2020  en,.            
+0000bfc0: 6f72 6465 723d 6f72 6465 722c 0a20 2020  order=order,.   
+0000bfd0: 2020 2020 2020 2020 206c 696d 6974 3d6c           limit=l
+0000bfe0: 696d 6974 2c0a 2020 2020 2020 2020 2020  imit,.          
+0000bff0: 2020 6462 3d64 622c 0a20 2020 2020 2020    db=db,.       
+0000c000: 2020 2020 2063 7572 3d63 7572 2c0a 2020       cur=cur,.  
+0000c010: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0000c020: 2076 6973 6974 7320 3d20 7669 7369 7473   visits = visits
+0000c030: 5f70 6167 652e 7265 7375 6c74 730a 2020  _page.results.  
+0000c040: 2020 2020 2020 6e65 7874 5f70 6167 655f        next_page_
+0000c050: 746f 6b65 6e20 3d20 7669 7369 7473 5f70  token = visits_p
+0000c060: 6167 652e 6e65 7874 5f70 6167 655f 746f  age.next_page_to
+0000c070: 6b65 6e0a 0a20 2020 2020 2020 2069 6620  ken..        if 
+0000c080: 7669 7369 7473 3a0a 2020 2020 2020 2020  visits:.        
+0000c090: 2020 2020 7669 7369 745f 6672 6f6d 203d      visit_from =
+0000c0a0: 206d 696e 2876 6973 6974 735b 305d 2e76   min(visits[0].v
+0000c0b0: 6973 6974 2c20 7669 7369 7473 5b2d 315d  isit, visits[-1]
+0000c0c0: 2e76 6973 6974 290a 2020 2020 2020 2020  .visit).        
+0000c0d0: 2020 2020 7669 7369 745f 746f 203d 206d      visit_to = m
+0000c0e0: 6178 2876 6973 6974 735b 305d 2e76 6973  ax(visits[0].vis
+0000c0f0: 6974 2c20 7669 7369 7473 5b2d 315d 2e76  it, visits[-1].v
+0000c100: 6973 6974 290a 0a20 2020 2020 2020 2020  isit)..         
+0000c110: 2020 2023 2054 6865 6e2c 2066 6574 6368     # Then, fetch
+0000c120: 2061 6c6c 2073 7461 7475 7365 7320 6173   all statuses as
+0000c130: 736f 6369 6174 6564 2074 6f20 7468 6573  sociated to thes
+0000c140: 6520 7669 7369 7473 0a20 2020 2020 2020  e visits.       
+0000c150: 2020 2020 2076 6973 6974 5f73 7461 7475       visit_statu
+0000c160: 7365 733a 2044 6963 745b 696e 742c 204c  ses: Dict[int, L
+0000c170: 6973 745b 4f72 6967 696e 5669 7369 7453  ist[OriginVisitS
+0000c180: 7461 7475 735d 5d20 3d20 6465 6661 756c  tatus]] = defaul
+0000c190: 7464 6963 7428 6c69 7374 290a 2020 2020  tdict(list).    
+0000c1a0: 2020 2020 2020 2020 666f 7220 726f 7720          for row 
+0000c1b0: 696e 2064 622e 6f72 6967 696e 5f76 6973  in db.origin_vis
+0000c1c0: 6974 5f73 7461 7475 735f 6765 745f 616c  it_status_get_al
+0000c1d0: 6c5f 696e 5f72 616e 6765 280a 2020 2020  l_in_range(.    
+0000c1e0: 2020 2020 2020 2020 2020 2020 6f72 6967              orig
+0000c1f0: 696e 2c0a 2020 2020 2020 2020 2020 2020  in,.            
+0000c200: 2020 2020 616c 6c6f 7765 645f 7374 6174      allowed_stat
+0000c210: 7573 6573 2c0a 2020 2020 2020 2020 2020  uses,.          
+0000c220: 2020 2020 2020 7265 7175 6972 655f 736e        require_sn
+0000c230: 6170 7368 6f74 2c0a 2020 2020 2020 2020  apshot,.        
+0000c240: 2020 2020 2020 2020 7669 7369 745f 6672          visit_fr
+0000c250: 6f6d 3d76 6973 6974 5f66 726f 6d2c 0a20  om=visit_from,. 
+0000c260: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+0000c270: 6973 6974 5f74 6f3d 7669 7369 745f 746f  isit_to=visit_to
+0000c280: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000c290: 2020 6375 723d 6375 722c 0a20 2020 2020    cur=cur,.     
+0000c2a0: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
+0000c2b0: 2020 2020 2020 2020 2020 726f 775f 6420            row_d 
+0000c2c0: 3d20 6469 6374 287a 6970 2864 622e 6f72  = dict(zip(db.or
+0000c2d0: 6967 696e 5f76 6973 6974 5f73 7461 7475  igin_visit_statu
+0000c2e0: 735f 636f 6c73 2c20 726f 7729 290a 0a20  s_cols, row)).. 
+0000c2f0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+0000c300: 6973 6974 5f73 7461 7475 7365 735b 726f  isit_statuses[ro
+0000c310: 775f 645b 2276 6973 6974 225d 5d2e 6170  w_d["visit"]].ap
+0000c320: 7065 6e64 284f 7269 6769 6e56 6973 6974  pend(OriginVisit
+0000c330: 5374 6174 7573 282a 2a72 6f77 5f64 2929  Status(**row_d))
+0000c340: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+0000c350: 7320 3d20 5b0a 2020 2020 2020 2020 2020  s = [.          
+0000c360: 2020 4f72 6967 696e 5669 7369 7457 6974    OriginVisitWit
+0000c370: 6853 7461 7475 7365 7328 7669 7369 743d  hStatuses(visit=
+0000c380: 7669 7369 742c 2073 7461 7475 7365 733d  visit, statuses=
+0000c390: 7669 7369 745f 7374 6174 7573 6573 5b76  visit_statuses[v
+0000c3a0: 6973 6974 2e76 6973 6974 5d29 0a20 2020  isit.visit]).   
+0000c3b0: 2020 2020 2020 2020 2066 6f72 2076 6973           for vis
+0000c3c0: 6974 2069 6e20 7669 7369 7473 0a20 2020  it in visits.   
+0000c3d0: 2020 2020 205d 0a0a 2020 2020 2020 2020       ]..        
+0000c3e0: 7265 7475 726e 2050 6167 6564 5265 7375  return PagedResu
+0000c3f0: 6c74 2872 6573 756c 7473 3d72 6573 756c  lt(results=resul
+0000c400: 7473 2c20 6e65 7874 5f70 6167 655f 746f  ts, next_page_to
+0000c410: 6b65 6e3d 6e65 7874 5f70 6167 655f 746f  ken=next_page_to
+0000c420: 6b65 6e29 0a0a 2020 2020 4064 625f 7472  ken)..    @db_tr
+0000c430: 616e 7361 6374 696f 6e28 7374 6174 656d  ansaction(statem
+0000c440: 656e 745f 7469 6d65 6f75 743d 3230 3030  ent_timeout=2000
+0000c450: 290a 2020 2020 6465 6620 6f72 6967 696e  ).    def origin
+0000c460: 5f76 6973 6974 5f66 696e 645f 6279 5f64  _visit_find_by_d
+0000c470: 6174 6528 0a20 2020 2020 2020 2073 656c  ate(.        sel
+0000c480: 662c 0a20 2020 2020 2020 206f 7269 6769  f,.        origi
+0000c490: 6e3a 2073 7472 2c0a 2020 2020 2020 2020  n: str,.        
+0000c4a0: 7669 7369 745f 6461 7465 3a20 6461 7465  visit_date: date
+0000c4b0: 7469 6d65 2e64 6174 6574 696d 652c 0a20  time.datetime,. 
+0000c4c0: 2020 2020 2020 2074 7970 653a 204f 7074         type: Opt
+0000c4d0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+0000c4e0: 652c 0a20 2020 2020 2020 202a 2c0a 2020  e,.        *,.  
+0000c4f0: 2020 2020 2020 6462 3a20 4462 2c0a 2020        db: Db,.  
+0000c500: 2020 2020 2020 6375 723d 4e6f 6e65 2c0a        cur=None,.
+0000c510: 2020 2020 2920 2d3e 204f 7074 696f 6e61      ) -> Optiona
+0000c520: 6c5b 4f72 6967 696e 5669 7369 745d 3a0a  l[OriginVisit]:.
+0000c530: 2020 2020 2020 2020 726f 775f 6420 3d20          row_d = 
+0000c540: 6462 2e6f 7269 6769 6e5f 7669 7369 745f  db.origin_visit_
+0000c550: 6669 6e64 5f62 795f 6461 7465 286f 7269  find_by_date(ori
+0000c560: 6769 6e2c 2076 6973 6974 5f64 6174 652c  gin, visit_date,
+0000c570: 2074 7970 653d 7479 7065 2c20 6375 723d   type=type, cur=
+0000c580: 6375 7229 0a20 2020 2020 2020 2069 6620  cur).        if 
+0000c590: 6e6f 7420 726f 775f 643a 0a20 2020 2020  not row_d:.     
+0000c5a0: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+0000c5b0: 6e65 0a20 2020 2020 2020 2072 6574 7572  ne.        retur
+0000c5c0: 6e20 4f72 6967 696e 5669 7369 7428 0a20  n OriginVisit(. 
+0000c5d0: 2020 2020 2020 2020 2020 206f 7269 6769             origi
+0000c5e0: 6e3d 726f 775f 645b 226f 7269 6769 6e22  n=row_d["origin"
+0000c5f0: 5d2c 0a20 2020 2020 2020 2020 2020 2076  ],.            v
+0000c600: 6973 6974 3d72 6f77 5f64 5b22 7669 7369  isit=row_d["visi
+0000c610: 7422 5d2c 0a20 2020 2020 2020 2020 2020  t"],.           
+0000c620: 2064 6174 653d 726f 775f 645b 2264 6174   date=row_d["dat
+0000c630: 6522 5d2c 0a20 2020 2020 2020 2020 2020  e"],.           
+0000c640: 2074 7970 653d 726f 775f 645b 2274 7970   type=row_d["typ
+0000c650: 6522 5d2c 0a20 2020 2020 2020 2029 0a0a  e"],.        )..
+0000c660: 2020 2020 4064 625f 7472 616e 7361 6374      @db_transact
+0000c670: 696f 6e28 7374 6174 656d 656e 745f 7469  ion(statement_ti
+0000c680: 6d65 6f75 743d 3530 3029 0a20 2020 2064  meout=500).    d
+0000c690: 6566 206f 7269 6769 6e5f 7669 7369 745f  ef origin_visit_
+0000c6a0: 6765 745f 6279 280a 2020 2020 2020 2020  get_by(.        
+0000c6b0: 7365 6c66 2c20 6f72 6967 696e 3a20 7374  self, origin: st
+0000c6c0: 722c 2076 6973 6974 3a20 696e 742c 202a  r, visit: int, *
+0000c6d0: 2c20 6462 3a20 4462 2c20 6375 723d 4e6f  , db: Db, cur=No
+0000c6e0: 6e65 0a20 2020 2029 202d 3e20 4f70 7469  ne.    ) -> Opti
+0000c6f0: 6f6e 616c 5b4f 7269 6769 6e56 6973 6974  onal[OriginVisit
+0000c700: 5d3a 0a20 2020 2020 2020 2072 6f77 203d  ]:.        row =
+0000c710: 2064 622e 6f72 6967 696e 5f76 6973 6974   db.origin_visit
+0000c720: 5f67 6574 286f 7269 6769 6e2c 2076 6973  _get(origin, vis
+0000c730: 6974 2c20 6375 7229 0a20 2020 2020 2020  it, cur).       
+0000c740: 2069 6620 726f 773a 0a20 2020 2020 2020   if row:.       
+0000c750: 2020 2020 2072 6f77 5f64 203d 2064 6963       row_d = dic
+0000c760: 7428 7a69 7028 6462 2e6f 7269 6769 6e5f  t(zip(db.origin_
+0000c770: 7669 7369 745f 6765 745f 636f 6c73 2c20  visit_get_cols, 
+0000c780: 726f 7729 290a 2020 2020 2020 2020 2020  row)).          
+0000c790: 2020 7265 7475 726e 204f 7269 6769 6e56    return OriginV
+0000c7a0: 6973 6974 280a 2020 2020 2020 2020 2020  isit(.          
+0000c7b0: 2020 2020 2020 6f72 6967 696e 3d72 6f77        origin=row
+0000c7c0: 5f64 5b22 6f72 6967 696e 225d 2c0a 2020  _d["origin"],.  
+0000c7d0: 2020 2020 2020 2020 2020 2020 2020 7669                vi
+0000c7e0: 7369 743d 726f 775f 645b 2276 6973 6974  sit=row_d["visit
+0000c7f0: 225d 2c0a 2020 2020 2020 2020 2020 2020  "],.            
+0000c800: 2020 2020 6461 7465 3d72 6f77 5f64 5b22      date=row_d["
+0000c810: 6461 7465 225d 2c0a 2020 2020 2020 2020  date"],.        
+0000c820: 2020 2020 2020 2020 7479 7065 3d72 6f77          type=row
+0000c830: 5f64 5b22 7479 7065 225d 2c0a 2020 2020  _d["type"],.    
+0000c840: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000c850: 2020 7265 7475 726e 204e 6f6e 650a 0a20    return None.. 
+0000c860: 2020 2040 6462 5f74 7261 6e73 6163 7469     @db_transacti
+0000c870: 6f6e 2873 7461 7465 6d65 6e74 5f74 696d  on(statement_tim
+0000c880: 656f 7574 3d34 3030 3029 0a20 2020 2064  eout=4000).    d
+0000c890: 6566 206f 7269 6769 6e5f 7669 7369 745f  ef origin_visit_
+0000c8a0: 6765 745f 6c61 7465 7374 280a 2020 2020  get_latest(.    
+0000c8b0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+0000c8c0: 2020 6f72 6967 696e 3a20 7374 722c 0a20    origin: str,. 
+0000c8d0: 2020 2020 2020 2074 7970 653a 204f 7074         type: Opt
+0000c8e0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+0000c8f0: 652c 0a20 2020 2020 2020 2061 6c6c 6f77  e,.        allow
+0000c900: 6564 5f73 7461 7475 7365 733a 204f 7074  ed_statuses: Opt
+0000c910: 696f 6e61 6c5b 4c69 7374 5b73 7472 5d5d  ional[List[str]]
+0000c920: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0000c930: 2072 6571 7569 7265 5f73 6e61 7073 686f   require_snapsho
+0000c940: 743a 2062 6f6f 6c20 3d20 4661 6c73 652c  t: bool = False,
+0000c950: 0a20 2020 2020 2020 202a 2c0a 2020 2020  .        *,.    
+0000c960: 2020 2020 6462 3a20 4462 2c0a 2020 2020      db: Db,.    
+0000c970: 2020 2020 6375 723d 4e6f 6e65 2c0a 2020      cur=None,.  
+0000c980: 2020 2920 2d3e 204f 7074 696f 6e61 6c5b    ) -> Optional[
+0000c990: 4f72 6967 696e 5669 7369 745d 3a0a 2020  OriginVisit]:.  
+0000c9a0: 2020 2020 2020 6966 2061 6c6c 6f77 6564        if allowed
+0000c9b0: 5f73 7461 7475 7365 7320 616e 6420 6e6f  _statuses and no
+0000c9c0: 7420 7365 7428 616c 6c6f 7765 645f 7374  t set(allowed_st
+0000c9d0: 6174 7573 6573 292e 696e 7465 7273 6563  atuses).intersec
+0000c9e0: 7469 6f6e 2856 4953 4954 5f53 5441 5455  tion(VISIT_STATU
+0000c9f0: 5345 5329 3a0a 2020 2020 2020 2020 2020  SES):.          
+0000ca00: 2020 7261 6973 6520 5374 6f72 6167 6541    raise StorageA
+0000ca10: 7267 756d 656e 7445 7863 6570 7469 6f6e  rgumentException
+0000ca20: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000ca30: 2020 6622 556e 6b6e 6f77 6e20 616c 6c6f    f"Unknown allo
+0000ca40: 7765 6420 7374 6174 7573 6573 207b 272c  wed statuses {',
+0000ca50: 272e 6a6f 696e 2861 6c6c 6f77 6564 5f73  '.join(allowed_s
+0000ca60: 7461 7475 7365 7329 7d2c 206f 6e6c 7920  tatuses)}, only 
+0000ca70: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000ca80: 2020 6622 7b27 2c27 2e6a 6f69 6e28 5649    f"{','.join(VI
+0000ca90: 5349 545f 5354 4154 5553 4553 297d 2061  SIT_STATUSES)} a
+0000caa0: 7574 686f 7269 7a65 6422 0a20 2020 2020  uthorized".     
+0000cab0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+0000cac0: 2020 726f 7720 3d20 6462 2e6f 7269 6769    row = db.origi
+0000cad0: 6e5f 7669 7369 745f 6765 745f 6c61 7465  n_visit_get_late
+0000cae0: 7374 280a 2020 2020 2020 2020 2020 2020  st(.            
+0000caf0: 6f72 6967 696e 2c0a 2020 2020 2020 2020  origin,.        
+0000cb00: 2020 2020 7479 7065 3d74 7970 652c 0a20      type=type,. 
+0000cb10: 2020 2020 2020 2020 2020 2061 6c6c 6f77             allow
+0000cb20: 6564 5f73 7461 7475 7365 733d 616c 6c6f  ed_statuses=allo
+0000cb30: 7765 645f 7374 6174 7573 6573 2c0a 2020  wed_statuses,.  
+0000cb40: 2020 2020 2020 2020 2020 7265 7175 6972            requir
+0000cb50: 655f 736e 6170 7368 6f74 3d72 6571 7569  e_snapshot=requi
+0000cb60: 7265 5f73 6e61 7073 686f 742c 0a20 2020  re_snapshot,.   
+0000cb70: 2020 2020 2020 2020 2063 7572 3d63 7572           cur=cur
+0000cb80: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+0000cb90: 2020 2020 6966 2072 6f77 3a0a 2020 2020      if row:.    
+0000cba0: 2020 2020 2020 2020 726f 775f 6420 3d20          row_d = 
+0000cbb0: 6469 6374 287a 6970 2864 622e 6f72 6967  dict(zip(db.orig
+0000cbc0: 696e 5f76 6973 6974 5f67 6574 5f63 6f6c  in_visit_get_col
+0000cbd0: 732c 2072 6f77 2929 0a20 2020 2020 2020  s, row)).       
+0000cbe0: 2020 2020 2061 7373 6572 7420 280a 2020       assert (.  
+0000cbf0: 2020 2020 2020 2020 2020 2020 2020 726f                ro
+0000cc00: 775f 645b 2276 6973 6974 225d 2069 7320  w_d["visit"] is 
+0000cc10: 6e6f 7420 4e6f 6e65 0a20 2020 2020 2020  not None.       
+0000cc20: 2020 2020 2029 2c20 226f 7269 6769 6e5f       ), "origin_
+0000cc30: 7669 7369 745f 7374 6174 7573 204c 4546  visit_status LEF
+0000cc40: 5420 4a4f 494e 206f 7269 6769 6e5f 7669  T JOIN origin_vi
+0000cc50: 7369 7420 7265 7475 726e 6564 204e 554c  sit returned NUL
+0000cc60: 4c22 0a20 2020 2020 2020 2020 2020 2076  L".            v
+0000cc70: 6973 6974 203d 204f 7269 6769 6e56 6973  isit = OriginVis
+0000cc80: 6974 280a 2020 2020 2020 2020 2020 2020  it(.            
+0000cc90: 2020 2020 6f72 6967 696e 3d72 6f77 5f64      origin=row_d
+0000cca0: 5b22 6f72 6967 696e 225d 2c0a 2020 2020  ["origin"],.    
+0000ccb0: 2020 2020 2020 2020 2020 2020 7669 7369              visi
+0000ccc0: 743d 726f 775f 645b 2276 6973 6974 225d  t=row_d["visit"]
+0000ccd0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000cce0: 2020 6461 7465 3d72 6f77 5f64 5b22 6461    date=row_d["da
+0000ccf0: 7465 225d 2c0a 2020 2020 2020 2020 2020  te"],.          
+0000cd00: 2020 2020 2020 7479 7065 3d72 6f77 5f64        type=row_d
+0000cd10: 5b22 7479 7065 225d 2c0a 2020 2020 2020  ["type"],.      
+0000cd20: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000cd30: 2020 2020 7265 7475 726e 2076 6973 6974      return visit
+0000cd40: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000cd50: 4e6f 6e65 0a0a 2020 2020 4064 625f 7472  None..    @db_tr
+0000cd60: 616e 7361 6374 696f 6e28 7374 6174 656d  ansaction(statem
+0000cd70: 656e 745f 7469 6d65 6f75 743d 3530 3029  ent_timeout=500)
+0000cd80: 0a20 2020 2064 6566 206f 7269 6769 6e5f  .    def origin_
+0000cd90: 7669 7369 745f 7374 6174 7573 5f67 6574  visit_status_get
+0000cda0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+0000cdb0: 2020 2020 2020 2020 6f72 6967 696e 3a20          origin: 
+0000cdc0: 7374 722c 0a20 2020 2020 2020 2076 6973  str,.        vis
+0000cdd0: 6974 3a20 696e 742c 0a20 2020 2020 2020  it: int,.       
+0000cde0: 2070 6167 655f 746f 6b65 6e3a 204f 7074   page_token: Opt
+0000cdf0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+0000ce00: 652c 0a20 2020 2020 2020 206f 7264 6572  e,.        order
+0000ce10: 3a20 4c69 7374 4f72 6465 7220 3d20 4c69  : ListOrder = Li
+0000ce20: 7374 4f72 6465 722e 4153 432c 0a20 2020  stOrder.ASC,.   
+0000ce30: 2020 2020 206c 696d 6974 3a20 696e 7420       limit: int 
+0000ce40: 3d20 3130 2c0a 2020 2020 2020 2020 2a2c  = 10,.        *,
+0000ce50: 0a20 2020 2020 2020 2064 623a 2044 622c  .        db: Db,
+0000ce60: 0a20 2020 2020 2020 2063 7572 3d4e 6f6e  .        cur=Non
+0000ce70: 652c 0a20 2020 2029 202d 3e20 5061 6765  e,.    ) -> Page
+0000ce80: 6452 6573 756c 745b 4f72 6967 696e 5669  dResult[OriginVi
+0000ce90: 7369 7453 7461 7475 735d 3a0a 2020 2020  sitStatus]:.    
+0000cea0: 2020 2020 6e65 7874 5f70 6167 655f 746f      next_page_to
+0000ceb0: 6b65 6e20 3d20 4e6f 6e65 0a20 2020 2020  ken = None.     
+0000cec0: 2020 2064 6174 655f 6672 6f6d 203d 204e     date_from = N
+0000ced0: 6f6e 650a 2020 2020 2020 2020 6966 2070  one.        if p
+0000cee0: 6167 655f 746f 6b65 6e20 6973 206e 6f74  age_token is not
+0000cef0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000cf00: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+0000cf10: 2020 2020 2020 2020 6461 7465 5f66 726f          date_fro
+0000cf20: 6d20 3d20 6461 7465 7469 6d65 2e64 6174  m = datetime.dat
+0000cf30: 6574 696d 652e 6672 6f6d 6973 6f66 6f72  etime.fromisofor
+0000cf40: 6d61 7428 7061 6765 5f74 6f6b 656e 290a  mat(page_token).
+0000cf50: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+0000cf60: 7074 2056 616c 7565 4572 726f 723a 0a20  pt ValueError:. 
+0000cf70: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000cf80: 6169 7365 2053 746f 7261 6765 4172 6775  aise StorageArgu
+0000cf90: 6d65 6e74 4578 6365 7074 696f 6e28 0a20  mentException(. 
+0000cfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cfb0: 2020 2022 496e 7661 6c69 6420 7061 6765     "Invalid page
+0000cfc0: 5f74 6f6b 656e 2061 7267 756d 656e 7420  _token argument 
+0000cfd0: 746f 206f 7269 6769 6e5f 7669 7369 745f  to origin_visit_
+0000cfe0: 7374 6174 7573 5f67 6574 2e22 0a20 2020  status_get.".   
+0000cff0: 2020 2020 2020 2020 2020 2020 2029 2066               ) f
+0000d000: 726f 6d20 4e6f 6e65 0a0a 2020 2020 2020  rom None..      
+0000d010: 2020 7669 7369 745f 7374 6174 7573 6573    visit_statuses
+0000d020: 3a20 4c69 7374 5b4f 7269 6769 6e56 6973  : List[OriginVis
+0000d030: 6974 5374 6174 7573 5d20 3d20 5b5d 0a20  itStatus] = []. 
+0000d040: 2020 2020 2020 2023 2054 616b 6520 6f6e         # Take on
+0000d050: 6520 6d6f 7265 2076 6973 6974 2073 7461  e more visit sta
+0000d060: 7475 7320 736f 2077 6520 6361 6e20 7265  tus so we can re
+0000d070: 7573 6520 6974 2061 7320 7468 6520 6e65  use it as the ne
+0000d080: 7874 2070 6167 6520 746f 6b65 6e20 6966  xt page token if
+0000d090: 2061 6e79 0a20 2020 2020 2020 2066 6f72   any.        for
+0000d0a0: 2072 6f77 2069 6e20 6462 2e6f 7269 6769   row in db.origi
+0000d0b0: 6e5f 7669 7369 745f 7374 6174 7573 5f67  n_visit_status_g
+0000d0c0: 6574 5f72 616e 6765 280a 2020 2020 2020  et_range(.      
+0000d0d0: 2020 2020 2020 6f72 6967 696e 2c0a 2020        origin,.  
+0000d0e0: 2020 2020 2020 2020 2020 7669 7369 742c            visit,
+0000d0f0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+0000d100: 655f 6672 6f6d 3d64 6174 655f 6672 6f6d  e_from=date_from
+0000d110: 2c0a 2020 2020 2020 2020 2020 2020 6f72  ,.            or
+0000d120: 6465 723d 6f72 6465 722c 0a20 2020 2020  der=order,.     
+0000d130: 2020 2020 2020 206c 696d 6974 3d6c 696d         limit=lim
+0000d140: 6974 202b 2031 2c0a 2020 2020 2020 2020  it + 1,.        
+0000d150: 2020 2020 6375 723d 6375 722c 0a20 2020      cur=cur,.   
+0000d160: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
+0000d170: 2020 2020 726f 775f 6420 3d20 6469 6374      row_d = dict
+0000d180: 287a 6970 2864 622e 6f72 6967 696e 5f76  (zip(db.origin_v
+0000d190: 6973 6974 5f73 7461 7475 735f 636f 6c73  isit_status_cols
+0000d1a0: 2c20 726f 7729 290a 2020 2020 2020 2020  , row)).        
+0000d1b0: 2020 2020 7669 7369 745f 7374 6174 7573      visit_status
+0000d1c0: 6573 2e61 7070 656e 6428 4f72 6967 696e  es.append(Origin
+0000d1d0: 5669 7369 7453 7461 7475 7328 2a2a 726f  VisitStatus(**ro
+0000d1e0: 775f 6429 290a 0a20 2020 2020 2020 2069  w_d))..        i
+0000d1f0: 6620 6c65 6e28 7669 7369 745f 7374 6174  f len(visit_stat
+0000d200: 7573 6573 2920 3e20 6c69 6d69 743a 0a20  uses) > limit:. 
+0000d210: 2020 2020 2020 2020 2020 2023 206c 6173             # las
+0000d220: 7420 7669 7369 7420 7374 6174 7573 2064  t visit status d
+0000d230: 6174 6520 6973 2074 6865 206e 6578 7420  ate is the next 
+0000d240: 7061 6765 2074 6f6b 656e 0a20 2020 2020  page token.     
+0000d250: 2020 2020 2020 206e 6578 745f 7061 6765         next_page
+0000d260: 5f74 6f6b 656e 203d 2073 7472 2876 6973  _token = str(vis
+0000d270: 6974 5f73 7461 7475 7365 735b 2d31 5d2e  it_statuses[-1].
+0000d280: 6461 7465 290a 2020 2020 2020 2020 2020  date).          
+0000d290: 2020 2320 6578 636c 7564 696e 6720 7468    # excluding th
+0000d2a0: 6174 2076 6973 6974 2073 7461 7475 7320  at visit status 
+0000d2b0: 6672 6f6d 2074 6865 2072 6573 756c 7420  from the result 
+0000d2c0: 746f 2072 6573 7065 6374 2074 6865 206c  to respect the l
+0000d2d0: 696d 6974 2073 697a 650a 2020 2020 2020  imit size.      
+0000d2e0: 2020 2020 2020 7669 7369 745f 7374 6174        visit_stat
+0000d2f0: 7573 6573 203d 2076 6973 6974 5f73 7461  uses = visit_sta
+0000d300: 7475 7365 735b 3a6c 696d 6974 5d0a 0a20  tuses[:limit].. 
+0000d310: 2020 2020 2020 2072 6574 7572 6e20 5061         return Pa
+0000d320: 6765 6452 6573 756c 7428 7265 7375 6c74  gedResult(result
+0000d330: 733d 7669 7369 745f 7374 6174 7573 6573  s=visit_statuses
+0000d340: 2c20 6e65 7874 5f70 6167 655f 746f 6b65  , next_page_toke
+0000d350: 6e3d 6e65 7874 5f70 6167 655f 746f 6b65  n=next_page_toke
+0000d360: 6e29 0a0a 2020 2020 4064 625f 7472 616e  n)..    @db_tran
+0000d370: 7361 6374 696f 6e28 290a 2020 2020 6465  saction().    de
+0000d380: 6620 6f72 6967 696e 5f76 6973 6974 5f73  f origin_visit_s
+0000d390: 7461 7475 735f 6765 745f 7261 6e64 6f6d  tatus_get_random
+0000d3a0: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
+0000d3b0: 7479 7065 3a20 7374 722c 202a 2c20 6462  type: str, *, db
+0000d3c0: 3a20 4462 2c20 6375 723d 4e6f 6e65 0a20  : Db, cur=None. 
+0000d3d0: 2020 2029 202d 3e20 4f70 7469 6f6e 616c     ) -> Optional
+0000d3e0: 5b4f 7269 6769 6e56 6973 6974 5374 6174  [OriginVisitStat
+0000d3f0: 7573 5d3a 0a20 2020 2020 2020 2072 6f77  us]:.        row
+0000d400: 203d 2064 622e 6f72 6967 696e 5f76 6973   = db.origin_vis
+0000d410: 6974 5f67 6574 5f72 616e 646f 6d28 7479  it_get_random(ty
+0000d420: 7065 2c20 6375 7229 0a20 2020 2020 2020  pe, cur).       
+0000d430: 2069 6620 726f 7720 6973 206e 6f74 204e   if row is not N
+0000d440: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000d450: 2072 6f77 5f64 203d 2064 6963 7428 7a69   row_d = dict(zi
+0000d460: 7028 6462 2e6f 7269 6769 6e5f 7669 7369  p(db.origin_visi
+0000d470: 745f 7374 6174 7573 5f63 6f6c 732c 2072  t_status_cols, r
+0000d480: 6f77 2929 0a20 2020 2020 2020 2020 2020  ow)).           
+0000d490: 2072 6574 7572 6e20 4f72 6967 696e 5669   return OriginVi
+0000d4a0: 7369 7453 7461 7475 7328 2a2a 726f 775f  sitStatus(**row_
+0000d4b0: 6429 0a20 2020 2020 2020 2072 6574 7572  d).        retur
+0000d4c0: 6e20 4e6f 6e65 0a0a 2020 2020 2323 2323  n None..    ####
+0000d4d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000d4e0: 2323 2323 2323 0a20 2020 2023 204f 7269  ######.    # Ori
+0000d4f0: 6769 6e0a 2020 2020 2323 2323 2323 2323  gin.    ########
+0000d500: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000d510: 2323 0a0a 2020 2020 4064 625f 7472 616e  ##..    @db_tran
+0000d520: 7361 6374 696f 6e28 7374 6174 656d 656e  saction(statemen
+0000d530: 745f 7469 6d65 6f75 743d 3130 3030 290a  t_timeout=1000).
+0000d540: 2020 2020 6465 6620 6f72 6967 696e 5f67      def origin_g
+0000d550: 6574 280a 2020 2020 2020 2020 7365 6c66  et(.        self
+0000d560: 2c20 6f72 6967 696e 733a 204c 6973 745b  , origins: List[
+0000d570: 7374 725d 2c20 2a2c 2064 623a 2044 622c  str], *, db: Db,
+0000d580: 2063 7572 3d4e 6f6e 650a 2020 2020 2920   cur=None.    ) 
+0000d590: 2d3e 2049 7465 7261 626c 655b 4f70 7469  -> Iterable[Opti
+0000d5a0: 6f6e 616c 5b4f 7269 6769 6e5d 5d3a 0a20  onal[Origin]]:. 
+0000d5b0: 2020 2020 2020 2072 6f77 7320 3d20 6462         rows = db
+0000d5c0: 2e6f 7269 6769 6e5f 6765 745f 6279 5f75  .origin_get_by_u
+0000d5d0: 726c 286f 7269 6769 6e73 2c20 6375 7229  rl(origins, cur)
+0000d5e0: 0a20 2020 2020 2020 2072 6573 756c 743a  .        result:
+0000d5f0: 204c 6973 745b 4f70 7469 6f6e 616c 5b4f   List[Optional[O
+0000d600: 7269 6769 6e5d 5d20 3d20 5b5d 0a20 2020  rigin]] = [].   
+0000d610: 2020 2020 2066 6f72 2072 6f77 2069 6e20       for row in 
+0000d620: 726f 7773 3a0a 2020 2020 2020 2020 2020  rows:.          
+0000d630: 2020 6f72 6967 696e 5f64 203d 2064 6963    origin_d = dic
+0000d640: 7428 7a69 7028 6462 2e6f 7269 6769 6e5f  t(zip(db.origin_
+0000d650: 636f 6c73 2c20 726f 7729 290a 2020 2020  cols, row)).    
+0000d660: 2020 2020 2020 2020 7572 6c20 3d20 6f72          url = or
+0000d670: 6967 696e 5f64 5b22 7572 6c22 5d0a 2020  igin_d["url"].  
+0000d680: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0000d690: 2e61 7070 656e 6428 4e6f 6e65 2069 6620  .append(None if 
+0000d6a0: 7572 6c20 6973 204e 6f6e 6520 656c 7365  url is None else
+0000d6b0: 204f 7269 6769 6e28 7572 6c3d 7572 6c29   Origin(url=url)
+0000d6c0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0000d6d0: 2072 6573 756c 740a 0a20 2020 2040 6462   result..    @db
+0000d6e0: 5f74 7261 6e73 6163 7469 6f6e 2873 7461  _transaction(sta
+0000d6f0: 7465 6d65 6e74 5f74 696d 656f 7574 3d31  tement_timeout=1
+0000d700: 3030 3029 0a20 2020 2064 6566 206f 7269  000).    def ori
+0000d710: 6769 6e5f 6765 745f 6279 5f73 6861 3128  gin_get_by_sha1(
+0000d720: 0a20 2020 2020 2020 2073 656c 662c 2073  .        self, s
+0000d730: 6861 3173 3a20 4c69 7374 5b62 7974 6573  ha1s: List[bytes
+0000d740: 5d2c 202a 2c20 6462 3a20 4462 2c20 6375  ], *, db: Db, cu
+0000d750: 723d 4e6f 6e65 0a20 2020 2029 202d 3e20  r=None.    ) -> 
+0000d760: 4c69 7374 5b4f 7074 696f 6e61 6c5b 4469  List[Optional[Di
+0000d770: 6374 5b73 7472 2c20 416e 795d 5d5d 3a0a  ct[str, Any]]]:.
+0000d780: 2020 2020 2020 2020 7265 7475 726e 205b          return [
+0000d790: 0a20 2020 2020 2020 2020 2020 2064 6963  .            dic
+0000d7a0: 7428 7a69 7028 6462 2e6f 7269 6769 6e5f  t(zip(db.origin_
+0000d7b0: 636f 6c73 2c20 726f 7729 2920 6966 2072  cols, row)) if r
+0000d7c0: 6f77 5b30 5d20 656c 7365 204e 6f6e 650a  ow[0] else None.
+0000d7d0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000d7e0: 726f 7720 696e 2064 622e 6f72 6967 696e  row in db.origin
+0000d7f0: 5f67 6574 5f62 795f 7368 6131 2873 6861  _get_by_sha1(sha
+0000d800: 3173 2c20 6375 7229 0a20 2020 2020 2020  1s, cur).       
+0000d810: 205d 0a0a 2020 2020 4064 625f 7472 616e   ]..    @db_tran
+0000d820: 7361 6374 696f 6e5f 6765 6e65 7261 746f  saction_generato
+0000d830: 7228 290a 2020 2020 6465 6620 6f72 6967  r().    def orig
+0000d840: 696e 5f67 6574 5f72 616e 6765 2873 656c  in_get_range(sel
+0000d850: 662c 206f 7269 6769 6e5f 6672 6f6d 3d31  f, origin_from=1
+0000d860: 2c20 6f72 6967 696e 5f63 6f75 6e74 3d31  , origin_count=1
+0000d870: 3030 2c20 2a2c 2064 623a 2044 622c 2063  00, *, db: Db, c
+0000d880: 7572 3d4e 6f6e 6529 3a0a 2020 2020 2020  ur=None):.      
+0000d890: 2020 666f 7220 6f72 6967 696e 2069 6e20    for origin in 
+0000d8a0: 6462 2e6f 7269 6769 6e5f 6765 745f 7261  db.origin_get_ra
+0000d8b0: 6e67 6528 6f72 6967 696e 5f66 726f 6d2c  nge(origin_from,
+0000d8c0: 206f 7269 6769 6e5f 636f 756e 742c 2063   origin_count, c
+0000d8d0: 7572 293a 0a20 2020 2020 2020 2020 2020  ur):.           
+0000d8e0: 2079 6965 6c64 2064 6963 7428 7a69 7028   yield dict(zip(
+0000d8f0: 6462 2e6f 7269 6769 6e5f 6765 745f 7261  db.origin_get_ra
+0000d900: 6e67 655f 636f 6c73 2c20 6f72 6967 696e  nge_cols, origin
+0000d910: 2929 0a0a 2020 2020 4064 625f 7472 616e  ))..    @db_tran
+0000d920: 7361 6374 696f 6e28 290a 2020 2020 6465  saction().    de
+0000d930: 6620 6f72 6967 696e 5f6c 6973 7428 0a20  f origin_list(. 
+0000d940: 2020 2020 2020 2073 656c 662c 2070 6167         self, pag
+0000d950: 655f 746f 6b65 6e3a 204f 7074 696f 6e61  e_token: Optiona
+0000d960: 6c5b 7374 725d 203d 204e 6f6e 652c 206c  l[str] = None, l
+0000d970: 696d 6974 3a20 696e 7420 3d20 3130 302c  imit: int = 100,
+0000d980: 202a 2c20 6462 3a20 4462 2c20 6375 723d   *, db: Db, cur=
+0000d990: 4e6f 6e65 0a20 2020 2029 202d 3e20 5061  None.    ) -> Pa
+0000d9a0: 6765 6452 6573 756c 745b 4f72 6967 696e  gedResult[Origin
+0000d9b0: 5d3a 0a20 2020 2020 2020 2070 6167 655f  ]:.        page_
+0000d9c0: 746f 6b65 6e20 3d20 7061 6765 5f74 6f6b  token = page_tok
+0000d9d0: 656e 206f 7220 2230 220a 2020 2020 2020  en or "0".      
+0000d9e0: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
+0000d9f0: 6e63 6528 7061 6765 5f74 6f6b 656e 2c20  nce(page_token, 
+0000da00: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
+0000da10: 2020 7261 6973 6520 5374 6f72 6167 6541    raise StorageA
+0000da20: 7267 756d 656e 7445 7863 6570 7469 6f6e  rgumentException
+0000da30: 2822 7061 6765 5f74 6f6b 656e 206d 7573  ("page_token mus
+0000da40: 7420 6265 2061 2073 7472 696e 672e 2229  t be a string.")
+0000da50: 0a20 2020 2020 2020 206f 7269 6769 6e5f  .        origin_
+0000da60: 6672 6f6d 203d 2069 6e74 2870 6167 655f  from = int(page_
+0000da70: 746f 6b65 6e29 0a20 2020 2020 2020 206e  token).        n
+0000da80: 6578 745f 7061 6765 5f74 6f6b 656e 203d  ext_page_token =
+0000da90: 204e 6f6e 650a 0a20 2020 2020 2020 206f   None..        o
+0000daa0: 7269 6769 6e73 3a20 4c69 7374 5b4f 7269  rigins: List[Ori
+0000dab0: 6769 6e5d 203d 205b 5d0a 2020 2020 2020  gin] = [].      
+0000dac0: 2020 2320 5461 6b65 206f 6e65 206d 6f72    # Take one mor
+0000dad0: 6520 6f72 6967 696e 2073 6f20 7765 2063  e origin so we c
+0000dae0: 616e 2072 6575 7365 2069 7420 6173 2074  an reuse it as t
+0000daf0: 6865 206e 6578 7420 7061 6765 2074 6f6b  he next page tok
+0000db00: 656e 2069 6620 616e 790a 2020 2020 2020  en if any.      
+0000db10: 2020 666f 7220 726f 775f 6420 696e 2073    for row_d in s
+0000db20: 656c 662e 6f72 6967 696e 5f67 6574 5f72  elf.origin_get_r
+0000db30: 616e 6765 286f 7269 6769 6e5f 6672 6f6d  ange(origin_from
+0000db40: 2c20 6c69 6d69 7420 2b20 312c 2064 623d  , limit + 1, db=
+0000db50: 6462 2c20 6375 723d 6375 7229 3a0a 2020  db, cur=cur):.  
+0000db60: 2020 2020 2020 2020 2020 6f72 6967 696e            origin
+0000db70: 732e 6170 7065 6e64 284f 7269 6769 6e28  s.append(Origin(
+0000db80: 7572 6c3d 726f 775f 645b 2275 726c 225d  url=row_d["url"]
+0000db90: 2929 0a20 2020 2020 2020 2020 2020 2023  )).            #
+0000dba0: 206b 6565 7020 7468 6520 6c61 7374 5f69   keep the last_i
+0000dbb0: 6420 666f 7220 7468 6520 7061 6769 6e61  d for the pagina
+0000dbc0: 7469 6f6e 2069 6620 6e65 6564 6564 0a20  tion if needed. 
+0000dbd0: 2020 2020 2020 2020 2020 206c 6173 745f             last_
+0000dbe0: 6964 203d 2072 6f77 5f64 5b22 6964 225d  id = row_d["id"]
+0000dbf0: 0a0a 2020 2020 2020 2020 6966 206c 656e  ..        if len
+0000dc00: 286f 7269 6769 6e73 2920 3e20 6c69 6d69  (origins) > limi
+0000dc10: 743a 2020 2320 6461 7461 206c 6566 7420  t:  # data left 
+0000dc20: 666f 7220 7375 6273 6571 7565 6e74 2063  for subsequent c
+0000dc30: 616c 6c0a 2020 2020 2020 2020 2020 2020  all.            
+0000dc40: 2320 6c61 7374 206f 7269 6769 6e20 6964  # last origin id
+0000dc50: 2069 7320 7468 6520 6e65 7874 2070 6167   is the next pag
+0000dc60: 6520 746f 6b65 6e0a 2020 2020 2020 2020  e token.        
+0000dc70: 2020 2020 6e65 7874 5f70 6167 655f 746f      next_page_to
+0000dc80: 6b65 6e20 3d20 7374 7228 6c61 7374 5f69  ken = str(last_i
+0000dc90: 6429 0a20 2020 2020 2020 2020 2020 2023  d).            #
+0000dca0: 2065 7863 6c75 6469 6e67 2074 6861 7420   excluding that 
+0000dcb0: 6f72 6967 696e 2066 726f 6d20 7468 6520  origin from the 
+0000dcc0: 7265 7375 6c74 2074 6f20 7265 7370 6563  result to respec
+0000dcd0: 7420 7468 6520 6c69 6d69 7420 7369 7a65  t the limit size
+0000dce0: 0a20 2020 2020 2020 2020 2020 206f 7269  .            ori
+0000dcf0: 6769 6e73 203d 206f 7269 6769 6e73 5b3a  gins = origins[:
+0000dd00: 6c69 6d69 745d 0a0a 2020 2020 2020 2020  limit]..        
+0000dd10: 6173 7365 7274 206c 656e 286f 7269 6769  assert len(origi
+0000dd20: 6e73 2920 3c3d 206c 696d 6974 0a20 2020  ns) <= limit.   
+0000dd30: 2020 2020 2072 6574 7572 6e20 5061 6765       return Page
+0000dd40: 6452 6573 756c 7428 7265 7375 6c74 733d  dResult(results=
+0000dd50: 6f72 6967 696e 732c 206e 6578 745f 7061  origins, next_pa
+0000dd60: 6765 5f74 6f6b 656e 3d6e 6578 745f 7061  ge_token=next_pa
+0000dd70: 6765 5f74 6f6b 656e 290a 0a20 2020 2040  ge_token)..    @
+0000dd80: 6462 5f74 7261 6e73 6163 7469 6f6e 2829  db_transaction()
+0000dd90: 0a20 2020 2064 6566 206f 7269 6769 6e5f  .    def origin_
+0000dda0: 7365 6172 6368 280a 2020 2020 2020 2020  search(.        
+0000ddb0: 7365 6c66 2c0a 2020 2020 2020 2020 7572  self,.        ur
+0000ddc0: 6c5f 7061 7474 6572 6e3a 2073 7472 2c0a  l_pattern: str,.
+0000ddd0: 2020 2020 2020 2020 7061 6765 5f74 6f6b          page_tok
+0000dde0: 656e 3a20 4f70 7469 6f6e 616c 5b73 7472  en: Optional[str
+0000ddf0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+0000de00: 2020 6c69 6d69 743a 2069 6e74 203d 2035    limit: int = 5
+0000de10: 302c 0a20 2020 2020 2020 2072 6567 6578  0,.        regex
+0000de20: 703a 2062 6f6f 6c20 3d20 4661 6c73 652c  p: bool = False,
+0000de30: 0a20 2020 2020 2020 2077 6974 685f 7669  .        with_vi
+0000de40: 7369 743a 2062 6f6f 6c20 3d20 4661 6c73  sit: bool = Fals
+0000de50: 652c 0a20 2020 2020 2020 2076 6973 6974  e,.        visit
+0000de60: 5f74 7970 6573 3a20 4f70 7469 6f6e 616c  _types: Optional
+0000de70: 5b4c 6973 745b 7374 725d 5d20 3d20 4e6f  [List[str]] = No
+0000de80: 6e65 2c0a 2020 2020 2020 2020 2a2c 0a20  ne,.        *,. 
+0000de90: 2020 2020 2020 2064 623a 2044 622c 0a20         db: Db,. 
+0000dea0: 2020 2020 2020 2063 7572 3d4e 6f6e 652c         cur=None,
+0000deb0: 0a20 2020 2029 202d 3e20 5061 6765 6452  .    ) -> PagedR
+0000dec0: 6573 756c 745b 4f72 6967 696e 5d3a 0a20  esult[Origin]:. 
+0000ded0: 2020 2020 2020 206e 6578 745f 7061 6765         next_page
+0000dee0: 5f74 6f6b 656e 203d 204e 6f6e 650a 2020  _token = None.  
+0000def0: 2020 2020 2020 6f66 6673 6574 203d 2069        offset = i
+0000df00: 6e74 2870 6167 655f 746f 6b65 6e29 2069  nt(page_token) i
+0000df10: 6620 7061 6765 5f74 6f6b 656e 2065 6c73  f page_token els
+0000df20: 6520 300a 0a20 2020 2020 2020 206f 7269  e 0..        ori
+0000df30: 6769 6e73 203d 205b 5d0a 2020 2020 2020  gins = [].      
+0000df40: 2020 2320 5461 6b65 206f 6e65 206d 6f72    # Take one mor
+0000df50: 6520 6f72 6967 696e 2073 6f20 7765 2063  e origin so we c
+0000df60: 616e 2072 6575 7365 2069 7420 6173 2074  an reuse it as t
+0000df70: 6865 206e 6578 7420 7061 6765 2074 6f6b  he next page tok
+0000df80: 656e 2069 6620 616e 790a 2020 2020 2020  en if any.      
+0000df90: 2020 666f 7220 6f72 6967 696e 2069 6e20    for origin in 
+0000dfa0: 6462 2e6f 7269 6769 6e5f 7365 6172 6368  db.origin_search
+0000dfb0: 280a 2020 2020 2020 2020 2020 2020 7572  (.            ur
+0000dfc0: 6c5f 7061 7474 6572 6e2c 206f 6666 7365  l_pattern, offse
+0000dfd0: 742c 206c 696d 6974 202b 2031 2c20 7265  t, limit + 1, re
+0000dfe0: 6765 7870 2c20 7769 7468 5f76 6973 6974  gexp, with_visit
+0000dff0: 2c20 7669 7369 745f 7479 7065 732c 2063  , visit_types, c
+0000e000: 7572 0a20 2020 2020 2020 2029 3a0a 2020  ur.        ):.  
+0000e010: 2020 2020 2020 2020 2020 726f 775f 6420            row_d 
+0000e020: 3d20 6469 6374 287a 6970 2864 622e 6f72  = dict(zip(db.or
+0000e030: 6967 696e 5f63 6f6c 732c 206f 7269 6769  igin_cols, origi
+0000e040: 6e29 290a 2020 2020 2020 2020 2020 2020  n)).            
+0000e050: 6f72 6967 696e 732e 6170 7065 6e64 284f  origins.append(O
+0000e060: 7269 6769 6e28 7572 6c3d 726f 775f 645b  rigin(url=row_d[
+0000e070: 2275 726c 225d 2929 0a0a 2020 2020 2020  "url"]))..      
+0000e080: 2020 6966 206c 656e 286f 7269 6769 6e73    if len(origins
+0000e090: 2920 3e20 6c69 6d69 743a 0a20 2020 2020  ) > limit:.     
+0000e0a0: 2020 2020 2020 2023 206e 6578 7420 6f66         # next of
+0000e0b0: 6673 6574 0a20 2020 2020 2020 2020 2020  fset.           
+0000e0c0: 206e 6578 745f 7061 6765 5f74 6f6b 656e   next_page_token
+0000e0d0: 203d 2073 7472 286f 6666 7365 7420 2b20   = str(offset + 
+0000e0e0: 6c69 6d69 7429 0a20 2020 2020 2020 2020  limit).         
+0000e0f0: 2020 2023 2065 7863 6c75 6469 6e67 2074     # excluding t
+0000e100: 6861 7420 6f72 6967 696e 2066 726f 6d20  hat origin from 
+0000e110: 7468 6520 7265 7375 6c74 2074 6f20 7265  the result to re
+0000e120: 7370 6563 7420 7468 6520 6c69 6d69 7420  spect the limit 
+0000e130: 7369 7a65 0a20 2020 2020 2020 2020 2020  size.           
+0000e140: 206f 7269 6769 6e73 203d 206f 7269 6769   origins = origi
+0000e150: 6e73 5b3a 6c69 6d69 745d 0a0a 2020 2020  ns[:limit]..    
+0000e160: 2020 2020 6173 7365 7274 206c 656e 286f      assert len(o
+0000e170: 7269 6769 6e73 2920 3c3d 206c 696d 6974  rigins) <= limit
+0000e180: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0000e190: 2050 6167 6564 5265 7375 6c74 2872 6573   PagedResult(res
+0000e1a0: 756c 7473 3d6f 7269 6769 6e73 2c20 6e65  ults=origins, ne
+0000e1b0: 7874 5f70 6167 655f 746f 6b65 6e3d 6e65  xt_page_token=ne
+0000e1c0: 7874 5f70 6167 655f 746f 6b65 6e29 0a0a  xt_page_token)..
+0000e1d0: 2020 2020 4064 625f 7472 616e 7361 6374      @db_transact
+0000e1e0: 696f 6e28 290a 2020 2020 6465 6620 6f72  ion().    def or
+0000e1f0: 6967 696e 5f63 6f75 6e74 280a 2020 2020  igin_count(.    
+0000e200: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+0000e210: 2020 7572 6c5f 7061 7474 6572 6e3a 2073    url_pattern: s
+0000e220: 7472 2c0a 2020 2020 2020 2020 7265 6765  tr,.        rege
+0000e230: 7870 3a20 626f 6f6c 203d 2046 616c 7365  xp: bool = False
+0000e240: 2c0a 2020 2020 2020 2020 7769 7468 5f76  ,.        with_v
+0000e250: 6973 6974 3a20 626f 6f6c 203d 2046 616c  isit: bool = Fal
+0000e260: 7365 2c0a 2020 2020 2020 2020 2a2c 0a20  se,.        *,. 
+0000e270: 2020 2020 2020 2064 623a 2044 622c 0a20         db: Db,. 
+0000e280: 2020 2020 2020 2063 7572 3d4e 6f6e 652c         cur=None,
+0000e290: 0a20 2020 2029 202d 3e20 696e 743a 0a20  .    ) -> int:. 
+0000e2a0: 2020 2020 2020 2072 6574 7572 6e20 6462         return db
+0000e2b0: 2e6f 7269 6769 6e5f 636f 756e 7428 7572  .origin_count(ur
+0000e2c0: 6c5f 7061 7474 6572 6e2c 2072 6567 6578  l_pattern, regex
+0000e2d0: 702c 2077 6974 685f 7669 7369 742c 2063  p, with_visit, c
+0000e2e0: 7572 290a 0a20 2020 2040 6462 5f74 7261  ur)..    @db_tra
+0000e2f0: 6e73 6163 7469 6f6e 2829 0a20 2020 2064  nsaction().    d
+0000e300: 6566 206f 7269 6769 6e5f 736e 6170 7368  ef origin_snapsh
+0000e310: 6f74 5f67 6574 5f61 6c6c 280a 2020 2020  ot_get_all(.    
+0000e320: 2020 2020 7365 6c66 2c20 6f72 6967 696e      self, origin
+0000e330: 5f75 726c 3a20 7374 722c 202a 2c20 6462  _url: str, *, db
+0000e340: 3a20 4462 2c20 6375 723d 4e6f 6e65 0a20  : Db, cur=None. 
+0000e350: 2020 2029 202d 3e20 4c69 7374 5b53 6861     ) -> List[Sha
+0000e360: 3147 6974 5d3a 0a20 2020 2020 2020 2072  1Git]:.        r
+0000e370: 6574 7572 6e20 6c69 7374 2864 622e 6f72  eturn list(db.or
+0000e380: 6967 696e 5f73 6e61 7073 686f 745f 6765  igin_snapshot_ge
+0000e390: 745f 616c 6c28 6f72 6967 696e 5f75 726c  t_all(origin_url
+0000e3a0: 2c20 6375 7229 290a 0a20 2020 2040 6462  , cur))..    @db
+0000e3b0: 5f74 7261 6e73 6163 7469 6f6e 2829 0a20  _transaction(). 
+0000e3c0: 2020 2064 6566 206f 7269 6769 6e5f 6164     def origin_ad
+0000e3d0: 6428 7365 6c66 2c20 6f72 6967 696e 733a  d(self, origins:
+0000e3e0: 204c 6973 745b 4f72 6967 696e 5d2c 202a   List[Origin], *
+0000e3f0: 2c20 6462 3a20 4462 2c20 6375 723d 4e6f  , db: Db, cur=No
+0000e400: 6e65 2920 2d3e 2044 6963 745b 7374 722c  ne) -> Dict[str,
+0000e410: 2069 6e74 5d3a 0a20 2020 2020 2020 2075   int]:.        u
+0000e420: 726c 7320 3d20 5b6f 2e75 726c 2066 6f72  rls = [o.url for
+0000e430: 206f 2069 6e20 6f72 6967 696e 735d 0a20   o in origins]. 
+0000e440: 2020 2020 2020 206b 6e6f 776e 5f6f 7269         known_ori
+0000e450: 6769 6e73 203d 2073 6574 2875 726c 2066  gins = set(url f
+0000e460: 6f72 2028 7572 6c2c 2920 696e 2064 622e  or (url,) in db.
+0000e470: 6f72 6967 696e 5f67 6574 5f62 795f 7572  origin_get_by_ur
+0000e480: 6c28 7572 6c73 2c20 6375 7229 290a 2020  l(urls, cur)).  
+0000e490: 2020 2020 2020 2320 6b65 6570 206f 6e6c        # keep onl
+0000e4a0: 7920 6f6e 6520 6f63 6375 7272 656e 6365  y one occurrence
+0000e4b0: 206f 6620 6561 6368 2067 6976 656e 206f   of each given o
+0000e4c0: 7269 6769 6e20 7768 696c 6520 6b65 6570  rigin while keep
+0000e4d0: 696e 6720 7468 6520 6c69 7374 0a20 2020  ing the list.   
+0000e4e0: 2020 2020 2023 2073 6f72 7465 6420 6173       # sorted as
+0000e4f0: 206f 7269 6769 6e61 6c6c 7920 6769 7665   originally give
+0000e500: 6e0a 2020 2020 2020 2020 746f 5f61 6464  n.        to_add
+0000e510: 203d 2073 6f72 7465 6428 7365 7428 7572   = sorted(set(ur
+0000e520: 6c73 2920 2d20 6b6e 6f77 6e5f 6f72 6967  ls) - known_orig
+0000e530: 696e 732c 206b 6579 3d75 726c 732e 696e  ins, key=urls.in
+0000e540: 6465 7829 0a0a 2020 2020 2020 2020 7365  dex)..        se
+0000e550: 6c66 2e6a 6f75 726e 616c 5f77 7269 7465  lf.journal_write
+0000e560: 722e 6f72 6967 696e 5f61 6464 285b 4f72  r.origin_add([Or
+0000e570: 6967 696e 2875 726c 3d75 726c 2920 666f  igin(url=url) fo
+0000e580: 7220 7572 6c20 696e 2074 6f5f 6164 645d  r url in to_add]
+0000e590: 290a 2020 2020 2020 2020 6164 6465 6420  ).        added 
+0000e5a0: 3d20 300a 2020 2020 2020 2020 666f 7220  = 0.        for 
+0000e5b0: 7572 6c20 696e 2074 6f5f 6164 643a 0a20  url in to_add:. 
+0000e5c0: 2020 2020 2020 2020 2020 2069 6620 6462             if db
+0000e5d0: 2e6f 7269 6769 6e5f 6164 6428 7572 6c2c  .origin_add(url,
+0000e5e0: 2063 7572 293a 0a20 2020 2020 2020 2020   cur):.         
+0000e5f0: 2020 2020 2020 2061 6464 6564 202b 3d20         added += 
+0000e600: 310a 2020 2020 2020 2020 7265 7475 726e  1.        return
+0000e610: 207b 226f 7269 6769 6e3a 6164 6422 3a20   {"origin:add": 
+0000e620: 6164 6465 647d 0a0a 2020 2020 2323 2323  added}..    ####
+0000e630: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000e640: 2323 2323 2323 0a20 2020 2023 206d 6973  ######.    # mis
+0000e650: 632e 0a20 2020 2023 2323 2323 2323 2323  c..    #########
+0000e660: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000e670: 230a 0a20 2020 2040 6462 5f74 7261 6e73  #..    @db_trans
+0000e680: 6163 7469 6f6e 2873 7461 7465 6d65 6e74  action(statement
+0000e690: 5f74 696d 656f 7574 3d32 3030 3029 0a20  _timeout=2000). 
+0000e6a0: 2020 2064 6566 206f 626a 6563 745f 6669     def object_fi
+0000e6b0: 6e64 5f62 795f 7368 6131 5f67 6974 280a  nd_by_sha1_git(.
+0000e6c0: 2020 2020 2020 2020 7365 6c66 2c20 6964          self, id
+0000e6d0: 733a 204c 6973 745b 5368 6131 4769 745d  s: List[Sha1Git]
+0000e6e0: 2c20 2a2c 2064 623a 2044 622c 2063 7572  , *, db: Db, cur
+0000e6f0: 3d4e 6f6e 650a 2020 2020 2920 2d3e 2044  =None.    ) -> D
+0000e700: 6963 745b 5368 6131 4769 742c 204c 6973  ict[Sha1Git, Lis
+0000e710: 745b 4469 6374 5d5d 3a0a 2020 2020 2020  t[Dict]]:.      
+0000e720: 2020 7265 743a 2044 6963 745b 5368 6131    ret: Dict[Sha1
+0000e730: 4769 742c 204c 6973 745b 4469 6374 5d5d  Git, List[Dict]]
+0000e740: 203d 207b 6964 3a20 5b5d 2066 6f72 2069   = {id: [] for i
+0000e750: 6420 696e 2069 6473 7d0a 0a20 2020 2020  d in ids}..     
+0000e760: 2020 2066 6f72 2072 6574 7661 6c20 696e     for retval in
+0000e770: 2064 622e 6f62 6a65 6374 5f66 696e 645f   db.object_find_
+0000e780: 6279 5f73 6861 315f 6769 7428 6964 732c  by_sha1_git(ids,
+0000e790: 2063 7572 3d63 7572 293a 0a20 2020 2020   cur=cur):.     
+0000e7a0: 2020 2020 2020 2069 6620 7265 7476 616c         if retval
+0000e7b0: 5b31 5d3a 0a20 2020 2020 2020 2020 2020  [1]:.           
+0000e7c0: 2020 2020 2072 6574 5b72 6574 7661 6c5b       ret[retval[
+0000e7d0: 305d 5d2e 6170 7065 6e64 280a 2020 2020  0]].append(.    
+0000e7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e7f0: 6469 6374 287a 6970 2864 622e 6f62 6a65  dict(zip(db.obje
+0000e800: 6374 5f66 696e 645f 6279 5f73 6861 315f  ct_find_by_sha1_
+0000e810: 6769 745f 636f 6c73 2c20 7265 7476 616c  git_cols, retval
+0000e820: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+0000e830: 2020 2029 0a0a 2020 2020 2020 2020 7265     )..        re
+0000e840: 7475 726e 2072 6574 0a0a 2020 2020 4064  turn ret..    @d
+0000e850: 625f 7472 616e 7361 6374 696f 6e28 7374  b_transaction(st
+0000e860: 6174 656d 656e 745f 7469 6d65 6f75 743d  atement_timeout=
+0000e870: 3530 3029 0a20 2020 2064 6566 2073 7461  500).    def sta
+0000e880: 745f 636f 756e 7465 7273 2873 656c 662c  t_counters(self,
+0000e890: 202a 2c20 6462 3a20 4462 2c20 6375 723d   *, db: Db, cur=
+0000e8a0: 4e6f 6e65 293a 0a20 2020 2020 2020 2072  None):.        r
+0000e8b0: 6574 7572 6e20 7b6b 3a20 7620 666f 7220  eturn {k: v for 
+0000e8c0: 286b 2c20 7629 2069 6e20 6462 2e73 7461  (k, v) in db.sta
+0000e8d0: 745f 636f 756e 7465 7273 2829 7d0a 0a20  t_counters()}.. 
+0000e8e0: 2020 2040 6462 5f74 7261 6e73 6163 7469     @db_transacti
+0000e8f0: 6f6e 2829 0a20 2020 2064 6566 2072 6566  on().    def ref
+0000e900: 7265 7368 5f73 7461 745f 636f 756e 7465  resh_stat_counte
+0000e910: 7273 2873 656c 662c 202a 2c20 6462 3a20  rs(self, *, db: 
+0000e920: 4462 2c20 6375 723d 4e6f 6e65 293a 0a20  Db, cur=None):. 
+0000e930: 2020 2020 2020 206b 6579 7320 3d20 5b0a         keys = [.
+0000e940: 2020 2020 2020 2020 2020 2020 2263 6f6e              "con
+0000e950: 7465 6e74 222c 0a20 2020 2020 2020 2020  tent",.         
+0000e960: 2020 2022 6469 7265 6374 6f72 7922 2c0a     "directory",.
+0000e970: 2020 2020 2020 2020 2020 2020 2264 6972              "dir
+0000e980: 6563 746f 7279 5f65 6e74 7279 5f64 6972  ectory_entry_dir
+0000e990: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+0000e9a0: 6469 7265 6374 6f72 795f 656e 7472 795f  directory_entry_
+0000e9b0: 6669 6c65 222c 0a20 2020 2020 2020 2020  file",.         
+0000e9c0: 2020 2022 6469 7265 6374 6f72 795f 656e     "directory_en
+0000e9d0: 7472 795f 7265 7622 2c0a 2020 2020 2020  try_rev",.      
+0000e9e0: 2020 2020 2020 226f 7269 6769 6e22 2c0a        "origin",.
+0000e9f0: 2020 2020 2020 2020 2020 2020 226f 7269              "ori
+0000ea00: 6769 6e5f 7669 7369 7422 2c0a 2020 2020  gin_visit",.    
+0000ea10: 2020 2020 2020 2020 2270 6572 736f 6e22          "person"
+0000ea20: 2c0a 2020 2020 2020 2020 2020 2020 2272  ,.            "r
+0000ea30: 656c 6561 7365 222c 0a20 2020 2020 2020  elease",.       
+0000ea40: 2020 2020 2022 7265 7669 7369 6f6e 222c       "revision",
+0000ea50: 0a20 2020 2020 2020 2020 2020 2022 7265  .            "re
+0000ea60: 7669 7369 6f6e 5f68 6973 746f 7279 222c  vision_history",
+0000ea70: 0a20 2020 2020 2020 2020 2020 2022 736b  .            "sk
+0000ea80: 6970 7065 645f 636f 6e74 656e 7422 2c0a  ipped_content",.
+0000ea90: 2020 2020 2020 2020 2020 2020 2273 6e61              "sna
+0000eaa0: 7073 686f 7422 2c0a 2020 2020 2020 2020  pshot",.        
+0000eab0: 5d0a 0a20 2020 2020 2020 2066 6f72 206b  ]..        for k
+0000eac0: 6579 2069 6e20 6b65 7973 3a0a 2020 2020  ey in keys:.    
+0000ead0: 2020 2020 2020 2020 6375 722e 6578 6563          cur.exec
+0000eae0: 7574 6528 2273 656c 6563 7420 2a20 6672  ute("select * fr
+0000eaf0: 6f6d 2073 7768 5f75 7064 6174 655f 636f  om swh_update_co
+0000eb00: 756e 7465 7228 2573 2922 2c20 286b 6579  unter(%s)", (key
+0000eb10: 2c29 290a 0a20 2020 2023 2323 2323 2323  ,))..    #######
+0000eb20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000eb30: 2323 230a 2020 2020 2320 5261 7745 7874  ###.    # RawExt
+0000eb40: 7269 6e73 6963 4d65 7461 6461 7461 0a20  rinsicMetadata. 
+0000eb50: 2020 2023 2323 2323 2323 2323 2323 2323     #############
+0000eb60: 2323 2323 2323 2323 2323 2323 230a 0a20  #############.. 
+0000eb70: 2020 2040 6462 5f74 7261 6e73 6163 7469     @db_transacti
+0000eb80: 6f6e 2829 0a20 2020 2064 6566 2072 6177  on().    def raw
+0000eb90: 5f65 7874 7269 6e73 6963 5f6d 6574 6164  _extrinsic_metad
+0000eba0: 6174 615f 6164 6428 0a20 2020 2020 2020  ata_add(.       
+0000ebb0: 2073 656c 662c 0a20 2020 2020 2020 206d   self,.        m
+0000ebc0: 6574 6164 6174 613a 204c 6973 745b 5261  etadata: List[Ra
+0000ebd0: 7745 7874 7269 6e73 6963 4d65 7461 6461  wExtrinsicMetada
+0000ebe0: 7461 5d2c 0a20 2020 2020 2020 2064 622c  ta],.        db,
+0000ebf0: 0a20 2020 2020 2020 2063 7572 2c0a 2020  .        cur,.  
+0000ec00: 2020 2920 2d3e 2044 6963 745b 7374 722c    ) -> Dict[str,
+0000ec10: 2069 6e74 5d3a 0a20 2020 2020 2020 206d   int]:.        m
+0000ec20: 6574 6164 6174 6120 3d20 6c69 7374 286d  etadata = list(m
+0000ec30: 6574 6164 6174 6129 0a20 2020 2020 2020  etadata).       
+0000ec40: 2073 656c 662e 6a6f 7572 6e61 6c5f 7772   self.journal_wr
+0000ec50: 6974 6572 2e72 6177 5f65 7874 7269 6e73  iter.raw_extrins
+0000ec60: 6963 5f6d 6574 6164 6174 615f 6164 6428  ic_metadata_add(
+0000ec70: 6d65 7461 6461 7461 290a 2020 2020 2020  metadata).      
+0000ec80: 2020 636f 756e 7465 7220 3d20 436f 756e    counter = Coun
+0000ec90: 7465 725b 4578 7465 6e64 6564 4f62 6a65  ter[ExtendedObje
+0000eca0: 6374 5479 7065 5d28 290a 2020 2020 2020  ctType]().      
+0000ecb0: 2020 666f 7220 6d65 7461 6461 7461 5f65    for metadata_e
+0000ecc0: 6e74 7279 2069 6e20 6d65 7461 6461 7461  ntry in metadata
+0000ecd0: 3a0a 2020 2020 2020 2020 2020 2020 6175  :.            au
+0000ece0: 7468 6f72 6974 795f 6964 203d 2073 656c  thority_id = sel
+0000ecf0: 662e 5f67 6574 5f61 7574 686f 7269 7479  f._get_authority
+0000ed00: 5f69 6428 6d65 7461 6461 7461 5f65 6e74  _id(metadata_ent
+0000ed10: 7279 2e61 7574 686f 7269 7479 2c20 6462  ry.authority, db
+0000ed20: 2c20 6375 7229 0a20 2020 2020 2020 2020  , cur).         
+0000ed30: 2020 2066 6574 6368 6572 5f69 6420 3d20     fetcher_id = 
+0000ed40: 7365 6c66 2e5f 6765 745f 6665 7463 6865  self._get_fetche
+0000ed50: 725f 6964 286d 6574 6164 6174 615f 656e  r_id(metadata_en
+0000ed60: 7472 792e 6665 7463 6865 722c 2064 622c  try.fetcher, db,
+0000ed70: 2063 7572 290a 0a20 2020 2020 2020 2020   cur)..         
+0000ed80: 2020 2064 622e 7261 775f 6578 7472 696e     db.raw_extrin
+0000ed90: 7369 635f 6d65 7461 6461 7461 5f61 6464  sic_metadata_add
+0000eda0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000edb0: 2020 6964 3d6d 6574 6164 6174 615f 656e    id=metadata_en
+0000edc0: 7472 792e 6964 2c0a 2020 2020 2020 2020  try.id,.        
+0000edd0: 2020 2020 2020 2020 7479 7065 3d6d 6574          type=met
+0000ede0: 6164 6174 615f 656e 7472 792e 7461 7267  adata_entry.targ
+0000edf0: 6574 2e6f 626a 6563 745f 7479 7065 2e6e  et.object_type.n
+0000ee00: 616d 652e 6c6f 7765 7228 292c 0a20 2020  ame.lower(),.   
+0000ee10: 2020 2020 2020 2020 2020 2020 2074 6172               tar
+0000ee20: 6765 743d 7374 7228 6d65 7461 6461 7461  get=str(metadata
+0000ee30: 5f65 6e74 7279 2e74 6172 6765 7429 2c0a  _entry.target),.
+0000ee40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee50: 6469 7363 6f76 6572 795f 6461 7465 3d6d  discovery_date=m
+0000ee60: 6574 6164 6174 615f 656e 7472 792e 6469  etadata_entry.di
+0000ee70: 7363 6f76 6572 795f 6461 7465 2c0a 2020  scovery_date,.  
+0000ee80: 2020 2020 2020 2020 2020 2020 2020 6175                au
+0000ee90: 7468 6f72 6974 795f 6964 3d61 7574 686f  thority_id=autho
+0000eea0: 7269 7479 5f69 642c 0a20 2020 2020 2020  rity_id,.       
+0000eeb0: 2020 2020 2020 2020 2066 6574 6368 6572           fetcher
+0000eec0: 5f69 643d 6665 7463 6865 725f 6964 2c0a  _id=fetcher_id,.
+0000eed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eee0: 666f 726d 6174 3d6d 6574 6164 6174 615f  format=metadata_
+0000eef0: 656e 7472 792e 666f 726d 6174 2c0a 2020  entry.format,.  
+0000ef00: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+0000ef10: 7461 6461 7461 3d6d 6574 6164 6174 615f  tadata=metadata_
+0000ef20: 656e 7472 792e 6d65 7461 6461 7461 2c0a  entry.metadata,.
+0000ef30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ef40: 6f72 6967 696e 3d6d 6574 6164 6174 615f  origin=metadata_
+0000ef50: 656e 7472 792e 6f72 6967 696e 2c0a 2020  entry.origin,.  
+0000ef60: 2020 2020 2020 2020 2020 2020 2020 7669                vi
+0000ef70: 7369 743d 6d65 7461 6461 7461 5f65 6e74  sit=metadata_ent
+0000ef80: 7279 2e76 6973 6974 2c0a 2020 2020 2020  ry.visit,.      
+0000ef90: 2020 2020 2020 2020 2020 736e 6170 7368            snapsh
+0000efa0: 6f74 3d6d 6170 5f6f 7074 696f 6e61 6c28  ot=map_optional(
+0000efb0: 7374 722c 206d 6574 6164 6174 615f 656e  str, metadata_en
+0000efc0: 7472 792e 736e 6170 7368 6f74 292c 0a20  try.snapshot),. 
+0000efd0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000efe0: 656c 6561 7365 3d6d 6170 5f6f 7074 696f  elease=map_optio
+0000eff0: 6e61 6c28 7374 722c 206d 6574 6164 6174  nal(str, metadat
+0000f000: 615f 656e 7472 792e 7265 6c65 6173 6529  a_entry.release)
+0000f010: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000f020: 2020 7265 7669 7369 6f6e 3d6d 6170 5f6f    revision=map_o
+0000f030: 7074 696f 6e61 6c28 7374 722c 206d 6574  ptional(str, met
+0000f040: 6164 6174 615f 656e 7472 792e 7265 7669  adata_entry.revi
+0000f050: 7369 6f6e 292c 0a20 2020 2020 2020 2020  sion),.         
+0000f060: 2020 2020 2020 2070 6174 683d 6d65 7461         path=meta
+0000f070: 6461 7461 5f65 6e74 7279 2e70 6174 682c  data_entry.path,
+0000f080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f090: 2064 6972 6563 746f 7279 3d6d 6170 5f6f   directory=map_o
+0000f0a0: 7074 696f 6e61 6c28 7374 722c 206d 6574  ptional(str, met
+0000f0b0: 6164 6174 615f 656e 7472 792e 6469 7265  adata_entry.dire
+0000f0c0: 6374 6f72 7929 2c0a 2020 2020 2020 2020  ctory),.        
+0000f0d0: 2020 2020 2020 2020 6375 723d 6375 722c          cur=cur,
+0000f0e0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+0000f0f0: 2020 2020 2020 2020 2020 2063 6f75 6e74             count
+0000f100: 6572 5b6d 6574 6164 6174 615f 656e 7472  er[metadata_entr
+0000f110: 792e 7461 7267 6574 2e6f 626a 6563 745f  y.target.object_
+0000f120: 7479 7065 5d20 2b3d 2031 0a0a 2020 2020  type] += 1..    
+0000f130: 2020 2020 7265 7475 726e 207b 0a20 2020      return {.   
+0000f140: 2020 2020 2020 2020 2066 227b 7479 7065           f"{type
+0000f150: 2e76 616c 7565 7d5f 6d65 7461 6461 7461  .value}_metadata
+0000f160: 3a61 6464 223a 2063 6f75 6e74 2066 6f72  :add": count for
+0000f170: 2028 7479 7065 2c20 636f 756e 7429 2069   (type, count) i
+0000f180: 6e20 636f 756e 7465 722e 6974 656d 7328  n counter.items(
+0000f190: 290a 2020 2020 2020 2020 7d0a 0a20 2020  ).        }..   
+0000f1a0: 2040 6462 5f74 7261 6e73 6163 7469 6f6e   @db_transaction
+0000f1b0: 2829 0a20 2020 2064 6566 2072 6177 5f65  ().    def raw_e
+0000f1c0: 7874 7269 6e73 6963 5f6d 6574 6164 6174  xtrinsic_metadat
+0000f1d0: 615f 6765 7428 0a20 2020 2020 2020 2073  a_get(.        s
+0000f1e0: 656c 662c 0a20 2020 2020 2020 2074 6172  elf,.        tar
+0000f1f0: 6765 743a 2045 7874 656e 6465 6453 5748  get: ExtendedSWH
+0000f200: 4944 2c0a 2020 2020 2020 2020 6175 7468  ID,.        auth
+0000f210: 6f72 6974 793a 204d 6574 6164 6174 6141  ority: MetadataA
+0000f220: 7574 686f 7269 7479 2c0a 2020 2020 2020  uthority,.      
+0000f230: 2020 6166 7465 723a 204f 7074 696f 6e61    after: Optiona
+0000f240: 6c5b 6461 7465 7469 6d65 2e64 6174 6574  l[datetime.datet
+0000f250: 696d 655d 203d 204e 6f6e 652c 0a20 2020  ime] = None,.   
+0000f260: 2020 2020 2070 6167 655f 746f 6b65 6e3a       page_token:
+0000f270: 204f 7074 696f 6e61 6c5b 6279 7465 735d   Optional[bytes]
+0000f280: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0000f290: 206c 696d 6974 3a20 696e 7420 3d20 3130   limit: int = 10
+0000f2a0: 3030 2c0a 2020 2020 2020 2020 2a2c 0a20  00,.        *,. 
+0000f2b0: 2020 2020 2020 2064 623a 2044 622c 0a20         db: Db,. 
+0000f2c0: 2020 2020 2020 2063 7572 3d4e 6f6e 652c         cur=None,
+0000f2d0: 0a20 2020 2029 202d 3e20 5061 6765 6452  .    ) -> PagedR
+0000f2e0: 6573 756c 745b 5261 7745 7874 7269 6e73  esult[RawExtrins
+0000f2f0: 6963 4d65 7461 6461 7461 5d3a 0a20 2020  icMetadata]:.   
+0000f300: 2020 2020 2069 6620 7061 6765 5f74 6f6b       if page_tok
+0000f310: 656e 3a0a 2020 2020 2020 2020 2020 2020  en:.            
+0000f320: 2861 6674 6572 5f74 696d 652c 2061 6674  (after_time, aft
+0000f330: 6572 5f66 6574 6368 6572 2920 3d20 6d73  er_fetcher) = ms
+0000f340: 6770 6163 6b5f 6c6f 6164 7328 6261 7365  gpack_loads(base
+0000f350: 3634 2e62 3634 6465 636f 6465 2870 6167  64.b64decode(pag
+0000f360: 655f 746f 6b65 6e29 290a 2020 2020 2020  e_token)).      
+0000f370: 2020 2020 2020 6966 2061 6674 6572 2061        if after a
+0000f380: 6e64 2061 6674 6572 5f74 696d 6520 3c20  nd after_time < 
+0000f390: 6166 7465 723a 0a20 2020 2020 2020 2020  after:.         
+0000f3a0: 2020 2020 2020 2072 6169 7365 2053 746f         raise Sto
+0000f3b0: 7261 6765 4172 6775 6d65 6e74 4578 6365  rageArgumentExce
+0000f3c0: 7074 696f 6e28 0a20 2020 2020 2020 2020  ption(.         
+0000f3d0: 2020 2020 2020 2020 2020 2022 7061 6765             "page
+0000f3e0: 5f74 6f6b 656e 2069 7320 696e 636f 6e73  _token is incons
+0000f3f0: 6973 7465 6e74 2077 6974 6820 7468 6520  istent with the 
+0000f400: 7661 6c75 6520 6f66 2027 6166 7465 7227  value of 'after'
+0000f410: 2e22 0a20 2020 2020 2020 2020 2020 2020  .".             
+0000f420: 2020 2029 0a20 2020 2020 2020 2065 6c73     ).        els
+0000f430: 653a 0a20 2020 2020 2020 2020 2020 2061  e:.            a
+0000f440: 6674 6572 5f74 696d 6520 3d20 6166 7465  fter_time = afte
+0000f450: 720a 2020 2020 2020 2020 2020 2020 6166  r.            af
+0000f460: 7465 725f 6665 7463 6865 7220 3d20 4e6f  ter_fetcher = No
+0000f470: 6e65 0a0a 2020 2020 2020 2020 7472 793a  ne..        try:
+0000f480: 0a20 2020 2020 2020 2020 2020 2061 7574  .            aut
+0000f490: 686f 7269 7479 5f69 6420 3d20 7365 6c66  hority_id = self
+0000f4a0: 2e5f 6765 745f 6175 7468 6f72 6974 795f  ._get_authority_
+0000f4b0: 6964 2861 7574 686f 7269 7479 2c20 6462  id(authority, db
+0000f4c0: 2c20 6375 7229 0a20 2020 2020 2020 2065  , cur).        e
+0000f4d0: 7863 6570 7420 556e 6b6e 6f77 6e4d 6574  xcept UnknownMet
+0000f4e0: 6164 6174 6141 7574 686f 7269 7479 3a0a  adataAuthority:.
+0000f4f0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000f500: 726e 2050 6167 6564 5265 7375 6c74 280a  rn PagedResult(.
+0000f510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f520: 6e65 7874 5f70 6167 655f 746f 6b65 6e3d  next_page_token=
+0000f530: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+0000f540: 2020 2020 2020 7265 7375 6c74 733d 5b5d        results=[]
+0000f550: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+0000f560: 0a20 2020 2020 2020 2072 6f77 7320 3d20  .        rows = 
+0000f570: 6462 2e72 6177 5f65 7874 7269 6e73 6963  db.raw_extrinsic
+0000f580: 5f6d 6574 6164 6174 615f 6765 7428 0a20  _metadata_get(. 
+0000f590: 2020 2020 2020 2020 2020 2073 7472 2874             str(t
+0000f5a0: 6172 6765 7429 2c0a 2020 2020 2020 2020  arget),.        
+0000f5b0: 2020 2020 6175 7468 6f72 6974 795f 6964      authority_id
+0000f5c0: 2c0a 2020 2020 2020 2020 2020 2020 6166  ,.            af
+0000f5d0: 7465 725f 7469 6d65 2c0a 2020 2020 2020  ter_time,.      
+0000f5e0: 2020 2020 2020 6166 7465 725f 6665 7463        after_fetc
+0000f5f0: 6865 722c 0a20 2020 2020 2020 2020 2020  her,.           
+0000f600: 206c 696d 6974 202b 2031 2c0a 2020 2020   limit + 1,.    
+0000f610: 2020 2020 2020 2020 6375 722c 0a20 2020          cur,.   
+0000f620: 2020 2020 2029 0a20 2020 2020 2020 2072       ).        r
+0000f630: 6f77 7320 3d20 5b64 6963 7428 7a69 7028  ows = [dict(zip(
+0000f640: 6462 2e72 6177 5f65 7874 7269 6e73 6963  db.raw_extrinsic
+0000f650: 5f6d 6574 6164 6174 615f 6765 745f 636f  _metadata_get_co
+0000f660: 6c73 2c20 726f 7729 2920 666f 7220 726f  ls, row)) for ro
+0000f670: 7720 696e 2072 6f77 735d 0a20 2020 2020  w in rows].     
+0000f680: 2020 2072 6573 756c 7473 203d 205b 5d0a     results = [].
+0000f690: 2020 2020 2020 2020 666f 7220 726f 7720          for row 
+0000f6a0: 696e 2072 6f77 733a 0a20 2020 2020 2020  in rows:.       
+0000f6b0: 2020 2020 2061 7373 6572 7420 7374 7228       assert str(
+0000f6c0: 7461 7267 6574 2920 3d3d 2072 6f77 5b22  target) == row["
+0000f6d0: 7261 775f 6578 7472 696e 7369 635f 6d65  raw_extrinsic_me
+0000f6e0: 7461 6461 7461 2e74 6172 6765 7422 5d0a  tadata.target"].
+0000f6f0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0000f700: 6c74 732e 6170 7065 6e64 2863 6f6e 7665  lts.append(conve
+0000f710: 7274 6572 732e 6462 5f74 6f5f 7261 775f  rters.db_to_raw_
+0000f720: 6578 7472 696e 7369 635f 6d65 7461 6461  extrinsic_metada
+0000f730: 7461 2872 6f77 2929 0a0a 2020 2020 2020  ta(row))..      
+0000f740: 2020 6966 206c 656e 2872 6573 756c 7473    if len(results
+0000f750: 2920 3e20 6c69 6d69 743a 0a20 2020 2020  ) > limit:.     
+0000f760: 2020 2020 2020 2072 6573 756c 7473 2e70         results.p
+0000f770: 6f70 2829 0a20 2020 2020 2020 2020 2020  op().           
+0000f780: 2061 7373 6572 7420 6c65 6e28 7265 7375   assert len(resu
+0000f790: 6c74 7329 203d 3d20 6c69 6d69 740a 2020  lts) == limit.  
+0000f7a0: 2020 2020 2020 2020 2020 6c61 7374 5f72            last_r
+0000f7b0: 6574 7572 6e65 645f 726f 7720 3d20 726f  eturned_row = ro
+0000f7c0: 7773 5b2d 325d 2020 2320 726f 7773 5b2d  ws[-2]  # rows[-
+0000f7d0: 315d 2063 6f72 7265 7370 6f6e 6473 2074  1] corresponds t
+0000f7e0: 6f20 7468 6520 706f 7070 6564 2072 6573  o the popped res
+0000f7f0: 756c 740a 2020 2020 2020 2020 2020 2020  ult.            
+0000f800: 6e65 7874 5f70 6167 655f 746f 6b65 6e3a  next_page_token:
+0000f810: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+0000f820: 2062 6173 6536 342e 6236 3465 6e63 6f64   base64.b64encod
+0000f830: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
+0000f840: 2020 206d 7367 7061 636b 5f64 756d 7073     msgpack_dumps
+0000f850: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000f860: 2020 2020 2020 280a 2020 2020 2020 2020        (.        
+0000f870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f880: 6c61 7374 5f72 6574 7572 6e65 645f 726f  last_returned_ro
+0000f890: 775b 2264 6973 636f 7665 7279 5f64 6174  w["discovery_dat
+0000f8a0: 6522 5d2c 0a20 2020 2020 2020 2020 2020  e"],.           
+0000f8b0: 2020 2020 2020 2020 2020 2020 206c 6173               las
+0000f8c0: 745f 7265 7475 726e 6564 5f72 6f77 5b22  t_returned_row["
+0000f8d0: 6d65 7461 6461 7461 5f66 6574 6368 6572  metadata_fetcher
+0000f8e0: 2e69 6422 5d2c 0a20 2020 2020 2020 2020  .id"],.         
+0000f8f0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000f900: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+0000f910: 2020 2020 2020 2020 2020 2029 2e64 6563             ).dec
+0000f920: 6f64 6528 290a 2020 2020 2020 2020 656c  ode().        el
+0000f930: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000f940: 6e65 7874 5f70 6167 655f 746f 6b65 6e20  next_page_token 
+0000f950: 3d20 4e6f 6e65 0a0a 2020 2020 2020 2020  = None..        
+0000f960: 7265 7475 726e 2050 6167 6564 5265 7375  return PagedResu
+0000f970: 6c74 280a 2020 2020 2020 2020 2020 2020  lt(.            
+0000f980: 6e65 7874 5f70 6167 655f 746f 6b65 6e3d  next_page_token=
+0000f990: 6e65 7874 5f70 6167 655f 746f 6b65 6e2c  next_page_token,
+0000f9a0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0000f9b0: 756c 7473 3d72 6573 756c 7473 2c0a 2020  ults=results,.  
+0000f9c0: 2020 2020 2020 290a 0a20 2020 2040 6462        )..    @db
+0000f9d0: 5f74 7261 6e73 6163 7469 6f6e 2829 0a20  _transaction(). 
+0000f9e0: 2020 2064 6566 2072 6177 5f65 7874 7269     def raw_extri
+0000f9f0: 6e73 6963 5f6d 6574 6164 6174 615f 6765  nsic_metadata_ge
+0000fa00: 745f 6279 5f69 6473 280a 2020 2020 2020  t_by_ids(.      
+0000fa10: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+0000fa20: 6964 733a 204c 6973 745b 5368 6131 4769  ids: List[Sha1Gi
+0000fa30: 745d 2c0a 2020 2020 2020 2020 2a2c 0a20  t],.        *,. 
+0000fa40: 2020 2020 2020 2064 623a 2044 622c 0a20         db: Db,. 
+0000fa50: 2020 2020 2020 2063 7572 3d4e 6f6e 652c         cur=None,
+0000fa60: 0a20 2020 2029 202d 3e20 4c69 7374 5b52  .    ) -> List[R
+0000fa70: 6177 4578 7472 696e 7369 634d 6574 6164  awExtrinsicMetad
+0000fa80: 6174 615d 3a0a 2020 2020 2020 2020 7265  ata]:.        re
+0000fa90: 7475 726e 205b 0a20 2020 2020 2020 2020  turn [.         
+0000faa0: 2020 2063 6f6e 7665 7274 6572 732e 6462     converters.db
+0000fab0: 5f74 6f5f 7261 775f 6578 7472 696e 7369  _to_raw_extrinsi
+0000fac0: 635f 6d65 7461 6461 7461 280a 2020 2020  c_metadata(.    
+0000fad0: 2020 2020 2020 2020 2020 2020 6469 6374              dict
+0000fae0: 287a 6970 2864 622e 7261 775f 6578 7472  (zip(db.raw_extr
+0000faf0: 696e 7369 635f 6d65 7461 6461 7461 5f67  insic_metadata_g
+0000fb00: 6574 5f63 6f6c 732c 2072 6f77 2929 0a20  et_cols, row)). 
+0000fb10: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000fb20: 2020 2020 2020 2020 2066 6f72 2072 6f77           for row
+0000fb30: 2069 6e20 6462 2e72 6177 5f65 7874 7269   in db.raw_extri
+0000fb40: 6e73 6963 5f6d 6574 6164 6174 615f 6765  nsic_metadata_ge
+0000fb50: 745f 6279 5f69 6473 2869 6473 290a 2020  t_by_ids(ids).  
+0000fb60: 2020 2020 2020 5d0a 0a20 2020 2023 2323        ]..    ###
+0000fb70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000fb80: 2323 2323 2323 230a 2020 2020 2320 4d65  #######.    # Me
+0000fb90: 7461 6461 7461 4665 7463 6865 7220 616e  tadataFetcher an
+0000fba0: 6420 4d65 7461 6461 7461 4175 7468 6f72  d MetadataAuthor
+0000fbb0: 6974 790a 2020 2020 2323 2323 2323 2323  ity.    ########
+0000fbc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000fbd0: 2323 0a0a 2020 2020 4064 625f 7472 616e  ##..    @db_tran
+0000fbe0: 7361 6374 696f 6e28 290a 2020 2020 6465  saction().    de
+0000fbf0: 6620 6d65 7461 6461 7461 5f66 6574 6368  f metadata_fetch
+0000fc00: 6572 5f61 6464 280a 2020 2020 2020 2020  er_add(.        
+0000fc10: 7365 6c66 2c20 6665 7463 6865 7273 3a20  self, fetchers: 
+0000fc20: 4c69 7374 5b4d 6574 6164 6174 6146 6574  List[MetadataFet
+0000fc30: 6368 6572 5d2c 202a 2c20 6462 3a20 4462  cher], *, db: Db
+0000fc40: 2c20 6375 723d 4e6f 6e65 0a20 2020 2029  , cur=None.    )
+0000fc50: 202d 3e20 4469 6374 5b73 7472 2c20 696e   -> Dict[str, in
+0000fc60: 745d 3a0a 2020 2020 2020 2020 6665 7463  t]:.        fetc
+0000fc70: 6865 7273 203d 206c 6973 7428 6665 7463  hers = list(fetc
+0000fc80: 6865 7273 290a 2020 2020 2020 2020 7365  hers).        se
+0000fc90: 6c66 2e6a 6f75 726e 616c 5f77 7269 7465  lf.journal_write
+0000fca0: 722e 6d65 7461 6461 7461 5f66 6574 6368  r.metadata_fetch
+0000fcb0: 6572 5f61 6464 2866 6574 6368 6572 7329  er_add(fetchers)
+0000fcc0: 0a20 2020 2020 2020 2063 6f75 6e74 203d  .        count =
+0000fcd0: 2030 0a20 2020 2020 2020 2066 6f72 2066   0.        for f
+0000fce0: 6574 6368 6572 2069 6e20 6665 7463 6865  etcher in fetche
+0000fcf0: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
+0000fd00: 6462 2e6d 6574 6164 6174 615f 6665 7463  db.metadata_fetc
+0000fd10: 6865 725f 6164 6428 6665 7463 6865 722e  her_add(fetcher.
+0000fd20: 6e61 6d65 2c20 6665 7463 6865 722e 7665  name, fetcher.ve
+0000fd30: 7273 696f 6e2c 2063 7572 3d63 7572 290a  rsion, cur=cur).
+0000fd40: 2020 2020 2020 2020 2020 2020 636f 756e              coun
+0000fd50: 7420 2b3d 2031 0a20 2020 2020 2020 2072  t += 1.        r
+0000fd60: 6574 7572 6e20 7b22 6d65 7461 6461 7461  eturn {"metadata
+0000fd70: 5f66 6574 6368 6572 3a61 6464 223a 2063  _fetcher:add": c
+0000fd80: 6f75 6e74 7d0a 0a20 2020 2040 6462 5f74  ount}..    @db_t
+0000fd90: 7261 6e73 6163 7469 6f6e 2873 7461 7465  ransaction(state
+0000fda0: 6d65 6e74 5f74 696d 656f 7574 3d35 3030  ment_timeout=500
+0000fdb0: 290a 2020 2020 6465 6620 6d65 7461 6461  ).    def metada
+0000fdc0: 7461 5f66 6574 6368 6572 5f67 6574 280a  ta_fetcher_get(.
+0000fdd0: 2020 2020 2020 2020 7365 6c66 2c20 6e61          self, na
+0000fde0: 6d65 3a20 7374 722c 2076 6572 7369 6f6e  me: str, version
+0000fdf0: 3a20 7374 722c 202a 2c20 6462 3a20 4462  : str, *, db: Db
+0000fe00: 2c20 6375 723d 4e6f 6e65 0a20 2020 2029  , cur=None.    )
+0000fe10: 202d 3e20 4f70 7469 6f6e 616c 5b4d 6574   -> Optional[Met
+0000fe20: 6164 6174 6146 6574 6368 6572 5d3a 0a20  adataFetcher]:. 
+0000fe30: 2020 2020 2020 2072 6f77 203d 2064 622e         row = db.
+0000fe40: 6d65 7461 6461 7461 5f66 6574 6368 6572  metadata_fetcher
+0000fe50: 5f67 6574 286e 616d 652c 2076 6572 7369  _get(name, versi
+0000fe60: 6f6e 2c20 6375 723d 6375 7229 0a20 2020  on, cur=cur).   
+0000fe70: 2020 2020 2069 6620 6e6f 7420 726f 773a       if not row:
+0000fe80: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000fe90: 7572 6e20 4e6f 6e65 0a20 2020 2020 2020  urn None.       
+0000fea0: 2072 6574 7572 6e20 4d65 7461 6461 7461   return Metadata
+0000feb0: 4665 7463 6865 722e 6672 6f6d 5f64 6963  Fetcher.from_dic
+0000fec0: 7428 6469 6374 287a 6970 2864 622e 6d65  t(dict(zip(db.me
+0000fed0: 7461 6461 7461 5f66 6574 6368 6572 5f63  tadata_fetcher_c
+0000fee0: 6f6c 732c 2072 6f77 2929 290a 0a20 2020  ols, row)))..   
+0000fef0: 2040 6462 5f74 7261 6e73 6163 7469 6f6e   @db_transaction
+0000ff00: 2829 0a20 2020 2064 6566 2072 6177 5f65  ().    def raw_e
+0000ff10: 7874 7269 6e73 6963 5f6d 6574 6164 6174  xtrinsic_metadat
+0000ff20: 615f 6765 745f 6175 7468 6f72 6974 6965  a_get_authoritie
+0000ff30: 7328 0a20 2020 2020 2020 2073 656c 662c  s(.        self,
+0000ff40: 0a20 2020 2020 2020 2074 6172 6765 743a  .        target:
+0000ff50: 2045 7874 656e 6465 6453 5748 4944 2c0a   ExtendedSWHID,.
+0000ff60: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
+0000ff70: 2020 2064 623a 2044 622c 0a20 2020 2020     db: Db,.     
+0000ff80: 2020 2063 7572 3d4e 6f6e 652c 0a20 2020     cur=None,.   
+0000ff90: 2029 202d 3e20 4c69 7374 5b4d 6574 6164   ) -> List[Metad
+0000ffa0: 6174 6141 7574 686f 7269 7479 5d3a 0a20  ataAuthority]:. 
+0000ffb0: 2020 2020 2020 2072 6574 7572 6e20 5b0a         return [.
+0000ffc0: 2020 2020 2020 2020 2020 2020 4d65 7461              Meta
+0000ffd0: 6461 7461 4175 7468 6f72 6974 7928 0a20  dataAuthority(. 
+0000ffe0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000fff0: 7970 653d 4d65 7461 6461 7461 4175 7468  ype=MetadataAuth
+00010000: 6f72 6974 7954 7970 6528 6175 7468 6f72  orityType(author
+00010010: 6974 795f 7479 7065 292c 2075 726c 3d61  ity_type), url=a
+00010020: 7574 686f 7269 7479 5f75 726c 0a20 2020  uthority_url.   
+00010030: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00010040: 2020 2020 2020 2066 6f72 2028 0a20 2020         for (.   
 00010050: 2020 2020 2020 2020 2020 2020 2061 7574               aut
-00010060: 686f 7269 7479 5f75 726c 2c0a 2020 2020  hority_url,.    
-00010070: 2020 2020 2020 2020 2920 696e 2064 622e          ) in db.
-00010080: 7261 775f 6578 7472 696e 7369 635f 6d65  raw_extrinsic_me
-00010090: 7461 6461 7461 5f67 6574 5f61 7574 686f  tadata_get_autho
-000100a0: 7269 7469 6573 2873 7472 2874 6172 6765  rities(str(targe
-000100b0: 7429 2c20 6375 7229 0a20 2020 2020 2020  t), cur).       
-000100c0: 205d 0a0a 2020 2020 4064 625f 7472 616e   ]..    @db_tran
-000100d0: 7361 6374 696f 6e28 290a 2020 2020 6465  saction().    de
-000100e0: 6620 6d65 7461 6461 7461 5f61 7574 686f  f metadata_autho
-000100f0: 7269 7479 5f61 6464 280a 2020 2020 2020  rity_add(.      
-00010100: 2020 7365 6c66 2c20 6175 7468 6f72 6974    self, authorit
-00010110: 6965 733a 204c 6973 745b 4d65 7461 6461  ies: List[Metada
-00010120: 7461 4175 7468 6f72 6974 795d 2c20 2a2c  taAuthority], *,
-00010130: 2064 623a 2044 622c 2063 7572 3d4e 6f6e   db: Db, cur=Non
-00010140: 650a 2020 2020 2920 2d3e 2044 6963 745b  e.    ) -> Dict[
-00010150: 7374 722c 2069 6e74 5d3a 0a20 2020 2020  str, int]:.     
-00010160: 2020 2061 7574 686f 7269 7469 6573 203d     authorities =
-00010170: 206c 6973 7428 6175 7468 6f72 6974 6965   list(authoritie
-00010180: 7329 0a20 2020 2020 2020 2073 656c 662e  s).        self.
-00010190: 6a6f 7572 6e61 6c5f 7772 6974 6572 2e6d  journal_writer.m
-000101a0: 6574 6164 6174 615f 6175 7468 6f72 6974  etadata_authorit
-000101b0: 795f 6164 6428 6175 7468 6f72 6974 6965  y_add(authoritie
-000101c0: 7329 0a20 2020 2020 2020 2063 6f75 6e74  s).        count
-000101d0: 203d 2030 0a20 2020 2020 2020 2066 6f72   = 0.        for
-000101e0: 2061 7574 686f 7269 7479 2069 6e20 6175   authority in au
-000101f0: 7468 6f72 6974 6965 733a 0a20 2020 2020  thorities:.     
-00010200: 2020 2020 2020 2064 622e 6d65 7461 6461         db.metada
-00010210: 7461 5f61 7574 686f 7269 7479 5f61 6464  ta_authority_add
-00010220: 2861 7574 686f 7269 7479 2e74 7970 652e  (authority.type.
-00010230: 7661 6c75 652c 2061 7574 686f 7269 7479  value, authority
-00010240: 2e75 726c 2c20 6375 723d 6375 7229 0a20  .url, cur=cur). 
-00010250: 2020 2020 2020 2020 2020 2063 6f75 6e74             count
-00010260: 202b 3d20 310a 2020 2020 2020 2020 7265   += 1.        re
-00010270: 7475 726e 207b 226d 6574 6164 6174 615f  turn {"metadata_
-00010280: 6175 7468 6f72 6974 793a 6164 6422 3a20  authority:add": 
-00010290: 636f 756e 747d 0a0a 2020 2020 4064 625f  count}..    @db_
-000102a0: 7472 616e 7361 6374 696f 6e28 290a 2020  transaction().  
-000102b0: 2020 6465 6620 6d65 7461 6461 7461 5f61    def metadata_a
-000102c0: 7574 686f 7269 7479 5f67 6574 280a 2020  uthority_get(.  
-000102d0: 2020 2020 2020 7365 6c66 2c20 7479 7065        self, type
-000102e0: 3a20 4d65 7461 6461 7461 4175 7468 6f72  : MetadataAuthor
-000102f0: 6974 7954 7970 652c 2075 726c 3a20 7374  ityType, url: st
-00010300: 722c 202a 2c20 6462 3a20 4462 2c20 6375  r, *, db: Db, cu
-00010310: 723d 4e6f 6e65 0a20 2020 2029 202d 3e20  r=None.    ) -> 
-00010320: 4f70 7469 6f6e 616c 5b4d 6574 6164 6174  Optional[Metadat
-00010330: 6141 7574 686f 7269 7479 5d3a 0a20 2020  aAuthority]:.   
-00010340: 2020 2020 2072 6f77 203d 2064 622e 6d65       row = db.me
-00010350: 7461 6461 7461 5f61 7574 686f 7269 7479  tadata_authority
-00010360: 5f67 6574 2874 7970 652e 7661 6c75 652c  _get(type.value,
-00010370: 2075 726c 2c20 6375 723d 6375 7229 0a20   url, cur=cur). 
-00010380: 2020 2020 2020 2069 6620 6e6f 7420 726f         if not ro
-00010390: 773a 0a20 2020 2020 2020 2020 2020 2072  w:.            r
-000103a0: 6574 7572 6e20 4e6f 6e65 0a20 2020 2020  eturn None.     
-000103b0: 2020 2072 6574 7572 6e20 4d65 7461 6461     return Metada
-000103c0: 7461 4175 7468 6f72 6974 792e 6672 6f6d  taAuthority.from
-000103d0: 5f64 6963 7428 6469 6374 287a 6970 2864  _dict(dict(zip(d
-000103e0: 622e 6d65 7461 6461 7461 5f61 7574 686f  b.metadata_autho
-000103f0: 7269 7479 5f63 6f6c 732c 2072 6f77 2929  rity_cols, row))
-00010400: 290a 0a20 2020 2023 2323 2323 2323 2323  )..    #########
-00010410: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00010420: 0a20 2020 2023 2027 6f62 6a65 6374 5f72  .    # 'object_r
-00010430: 6566 6572 656e 6365 7327 2074 6162 6c65  eferences' table
-00010440: 0a20 2020 2023 2323 2323 2323 2323 2323  .    ###########
-00010450: 2323 2323 2323 2323 2323 2323 2323 0a0a  ##############..
-00010460: 2020 2020 4064 625f 7472 616e 7361 6374      @db_transact
-00010470: 696f 6e28 290a 2020 2020 6465 6620 6f62  ion().    def ob
-00010480: 6a65 6374 5f66 696e 645f 7265 6365 6e74  ject_find_recent
-00010490: 5f72 6566 6572 656e 6365 7328 0a20 2020  _references(.   
-000104a0: 2020 2020 2073 656c 662c 2074 6172 6765       self, targe
-000104b0: 745f 7377 6869 643a 2045 7874 656e 6465  t_swhid: Extende
-000104c0: 6453 5748 4944 2c20 6c69 6d69 743a 2069  dSWHID, limit: i
-000104d0: 6e74 2c20 2a2c 2064 623a 2044 622c 2063  nt, *, db: Db, c
-000104e0: 7572 3d4e 6f6e 650a 2020 2020 2920 2d3e  ur=None.    ) ->
-000104f0: 204c 6973 745b 4578 7465 6e64 6564 5357   List[ExtendedSW
-00010500: 4849 445d 3a0a 2020 2020 2020 2020 7265  HID]:.        re
-00010510: 7475 726e 205b 0a20 2020 2020 2020 2020  turn [.         
-00010520: 2020 2063 6f6e 7665 7274 6572 732e 6462     converters.db
-00010530: 5f74 6f5f 6f62 6a65 6374 5f72 6566 6572  _to_object_refer
-00010540: 656e 6365 5f73 6f75 7263 6528 726f 7729  ence_source(row)
-00010550: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00010560: 2072 6f77 2069 6e20 6462 2e6f 626a 6563   row in db.objec
-00010570: 745f 7265 6665 7265 6e63 6573 5f67 6574  t_references_get
-00010580: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00010590: 2020 7461 7267 6574 5f74 7970 653d 7461    target_type=ta
-000105a0: 7267 6574 5f73 7768 6964 2e6f 626a 6563  rget_swhid.objec
-000105b0: 745f 7479 7065 2e6e 616d 652e 6c6f 7765  t_type.name.lowe
-000105c0: 7228 292c 0a20 2020 2020 2020 2020 2020  r(),.           
-000105d0: 2020 2020 2074 6172 6765 743d 7461 7267       target=targ
-000105e0: 6574 5f73 7768 6964 2e6f 626a 6563 745f  et_swhid.object_
-000105f0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
-00010600: 2020 2020 6c69 6d69 743d 6c69 6d69 742c      limit=limit,
-00010610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010620: 2063 7572 3d63 7572 2c0a 2020 2020 2020   cur=cur,.      
-00010630: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00010640: 5d0a 0a20 2020 2040 6462 5f74 7261 6e73  ]..    @db_trans
-00010650: 6163 7469 6f6e 2829 0a20 2020 2064 6566  action().    def
-00010660: 206f 626a 6563 745f 7265 6665 7265 6e63   object_referenc
-00010670: 6573 5f61 6464 280a 2020 2020 2020 2020  es_add(.        
-00010680: 7365 6c66 2c20 7265 6665 7265 6e63 6573  self, references
-00010690: 3a20 4c69 7374 5b4f 626a 6563 7452 6566  : List[ObjectRef
-000106a0: 6572 656e 6365 5d2c 202a 2c20 6462 3a20  erence], *, db: 
-000106b0: 4462 2c20 6375 723d 4e6f 6e65 0a20 2020  Db, cur=None.   
-000106c0: 2029 202d 3e20 4469 6374 5b73 7472 2c20   ) -> Dict[str, 
-000106d0: 696e 745d 3a0a 2020 2020 2020 2020 746f  int]:.        to
-000106e0: 5f61 6464 203d 206c 6973 7428 7b63 6f6e  _add = list({con
-000106f0: 7665 7274 6572 732e 6f62 6a65 6374 5f72  verters.object_r
-00010700: 6566 6572 656e 6365 5f74 6f5f 6462 2872  eference_to_db(r
-00010710: 6566 2920 666f 7220 7265 6620 696e 2072  ef) for ref in r
-00010720: 6566 6572 656e 6365 737d 290a 2020 2020  eferences}).    
-00010730: 2020 2020 6462 2e6f 626a 6563 745f 7265      db.object_re
-00010740: 6665 7265 6e63 6573 5f61 6464 280a 2020  ferences_add(.  
-00010750: 2020 2020 2020 2020 2020 746f 5f61 6464            to_add
-00010760: 2c0a 2020 2020 2020 2020 2020 2020 6375  ,.            cu
-00010770: 723d 6375 722c 0a20 2020 2020 2020 2029  r=cur,.        )
-00010780: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00010790: 207b 226f 626a 6563 745f 7265 6665 7265   {"object_refere
-000107a0: 6e63 653a 6164 6422 3a20 6c65 6e28 746f  nce:add": len(to
-000107b0: 5f61 6464 297d 0a0a 2020 2020 6465 6620  _add)}..    def 
-000107c0: 636c 6561 725f 6275 6666 6572 7328 7365  clear_buffers(se
-000107d0: 6c66 2c20 6f62 6a65 6374 5f74 7970 6573  lf, object_types
-000107e0: 3a20 5365 7175 656e 6365 5b73 7472 5d20  : Sequence[str] 
-000107f0: 3d20 2829 2920 2d3e 204e 6f6e 653a 0a20  = ()) -> None:. 
-00010800: 2020 2020 2020 2022 2222 446f 206e 6f74         """Do not
-00010810: 6869 6e67 2222 220a 2020 2020 2020 2020  hing""".        
-00010820: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
-00010830: 2064 6566 2066 6c75 7368 2873 656c 662c   def flush(self,
-00010840: 206f 626a 6563 745f 7479 7065 733a 2053   object_types: S
-00010850: 6571 7565 6e63 655b 7374 725d 203d 2028  equence[str] = (
-00010860: 2929 202d 3e20 4469 6374 5b73 7472 2c20  )) -> Dict[str, 
-00010870: 696e 745d 3a0a 2020 2020 2020 2020 7265  int]:.        re
-00010880: 7475 726e 207b 7d0a 0a20 2020 2064 6566  turn {}..    def
-00010890: 205f 6765 745f 6175 7468 6f72 6974 795f   _get_authority_
-000108a0: 6964 2873 656c 662c 2061 7574 686f 7269  id(self, authori
-000108b0: 7479 3a20 4d65 7461 6461 7461 4175 7468  ty: MetadataAuth
-000108c0: 6f72 6974 792c 2064 622c 2063 7572 293a  ority, db, cur):
-000108d0: 0a20 2020 2020 2020 2061 7574 686f 7269  .        authori
-000108e0: 7479 5f69 6420 3d20 6462 2e6d 6574 6164  ty_id = db.metad
-000108f0: 6174 615f 6175 7468 6f72 6974 795f 6765  ata_authority_ge
-00010900: 745f 6964 280a 2020 2020 2020 2020 2020  t_id(.          
-00010910: 2020 6175 7468 6f72 6974 792e 7479 7065    authority.type
-00010920: 2e76 616c 7565 2c20 6175 7468 6f72 6974  .value, authorit
-00010930: 792e 7572 6c2c 2063 7572 0a20 2020 2020  y.url, cur.     
-00010940: 2020 2029 0a20 2020 2020 2020 2069 6620     ).        if 
-00010950: 6e6f 7420 6175 7468 6f72 6974 795f 6964  not authority_id
-00010960: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00010970: 6973 6520 556e 6b6e 6f77 6e4d 6574 6164  ise UnknownMetad
-00010980: 6174 6141 7574 686f 7269 7479 2873 7472  ataAuthority(str
-00010990: 2861 7574 686f 7269 7479 2929 0a20 2020  (authority)).   
-000109a0: 2020 2020 2072 6574 7572 6e20 6175 7468       return auth
-000109b0: 6f72 6974 795f 6964 0a0a 2020 2020 6465  ority_id..    de
-000109c0: 6620 5f67 6574 5f66 6574 6368 6572 5f69  f _get_fetcher_i
-000109d0: 6428 7365 6c66 2c20 6665 7463 6865 723a  d(self, fetcher:
-000109e0: 204d 6574 6164 6174 6146 6574 6368 6572   MetadataFetcher
-000109f0: 2c20 6462 2c20 6375 7229 3a0a 2020 2020  , db, cur):.    
-00010a00: 2020 2020 6665 7463 6865 725f 6964 203d      fetcher_id =
-00010a10: 2064 622e 6d65 7461 6461 7461 5f66 6574   db.metadata_fet
-00010a20: 6368 6572 5f67 6574 5f69 6428 6665 7463  cher_get_id(fetc
-00010a30: 6865 722e 6e61 6d65 2c20 6665 7463 6865  her.name, fetche
-00010a40: 722e 7665 7273 696f 6e2c 2063 7572 290a  r.version, cur).
-00010a50: 2020 2020 2020 2020 6966 206e 6f74 2066          if not f
-00010a60: 6574 6368 6572 5f69 643a 0a20 2020 2020  etcher_id:.     
-00010a70: 2020 2020 2020 2072 6169 7365 2055 6e6b         raise Unk
-00010a80: 6e6f 776e 4d65 7461 6461 7461 4665 7463  nownMetadataFetc
-00010a90: 6865 7228 7374 7228 6665 7463 6865 7229  her(str(fetcher)
-00010aa0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00010ab0: 2066 6574 6368 6572 5f69 640a 0a20 2020   fetcher_id..   
-00010ac0: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
-00010ad0: 2323 2323 2323 2323 2323 0a20 2020 2023  ##########.    #
-00010ae0: 204f 626a 6563 7444 656c 6574 696f 6e49   ObjectDeletionI
-00010af0: 6e74 6572 6661 6365 0a20 2020 2023 2323  nterface.    ###
-00010b00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00010b10: 2323 2323 2323 0a0a 2020 2020 4064 625f  ######..    @db_
-00010b20: 7472 616e 7361 6374 696f 6e28 290a 2020  transaction().  
-00010b30: 2020 6465 6620 6f62 6a65 6374 5f64 656c    def object_del
-00010b40: 6574 6528 0a20 2020 2020 2020 2073 656c  ete(.        sel
-00010b50: 662c 2073 7768 6964 733a 204c 6973 745b  f, swhids: List[
-00010b60: 4578 7465 6e64 6564 5357 4849 445d 2c20  ExtendedSWHID], 
-00010b70: 2a2c 2064 623a 2044 622c 2063 7572 3d4e  *, db: Db, cur=N
-00010b80: 6f6e 650a 2020 2020 2920 2d3e 2044 6963  one.    ) -> Dic
-00010b90: 745b 7374 722c 2069 6e74 5d3a 0a20 2020  t[str, int]:.   
-00010ba0: 2020 2020 2022 2222 4465 6c65 7465 206f       """Delete o
-00010bb0: 626a 6563 7473 2066 726f 6d20 7468 6520  bjects from the 
-00010bc0: 7374 6f72 6167 650a 0a20 2020 2020 2020  storage..       
-00010bd0: 2041 6c6c 2073 6b69 7070 6564 2063 6f6e   All skipped con
-00010be0: 7465 6e74 206f 626a 6563 7473 206d 6174  tent objects mat
-00010bf0: 6368 696e 6720 7468 6520 6769 7665 6e20  ching the given 
-00010c00: 5357 4849 4420 7769 6c6c 2062 6520 7265  SWHID will be re
-00010c10: 6d6f 7665 642c 0a20 2020 2020 2020 2069  moved,.        i
-00010c20: 6e63 6c75 6469 6e67 2074 686f 7365 2077  ncluding those w
-00010c30: 686f 2068 6176 6520 7468 6520 7361 6d65  ho have the same
-00010c40: 2053 5748 4944 2064 7565 2074 6f20 6861   SWHID due to ha
-00010c50: 7368 2063 6f6c 6c69 7369 6f6e 732e 0a0a  sh collisions...
-00010c60: 2020 2020 2020 2020 4f72 6967 696e 206f          Origin o
-00010c70: 626a 6563 7473 2061 7265 2072 656d 6f76  bjects are remov
-00010c80: 6564 2061 6c6f 6e67 7369 6465 2074 6865  ed alongside the
-00010c90: 6972 2061 7373 6f63 6961 7465 6420 6f72  ir associated or
-00010ca0: 6967 696e 2076 6973 6974 2061 6e64 0a20  igin visit and. 
-00010cb0: 2020 2020 2020 206f 7269 6769 6e20 7669         origin vi
-00010cc0: 7369 7420 7374 6174 7573 206f 626a 6563  sit status objec
-00010cd0: 7473 2e0a 0a20 2020 2020 2020 2041 7267  ts...        Arg
-00010ce0: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
-00010cf0: 7768 6964 733a 206c 6973 7420 6f66 2053  whids: list of S
-00010d00: 5748 4944 206f 6620 7468 6520 6f62 6a65  WHID of the obje
-00010d10: 6374 7320 746f 2072 656d 6f76 650a 0a20  cts to remove.. 
-00010d20: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-00010d30: 2020 2020 2020 2020 2020 2020 5375 6d6d              Summ
-00010d40: 6172 7920 6469 6374 2077 6974 6820 7468  ary dict with th
-00010d50: 6520 666f 6c6c 6f77 696e 6720 6b65 7973  e following keys
-00010d60: 2061 6e64 2061 7373 6f63 6961 7465 6420   and associated 
-00010d70: 7661 6c75 6573 3a0a 0a20 2020 2020 2020  values:..       
-00010d80: 2020 2020 2020 2020 2063 6f6e 7465 6e74           content
-00010d90: 3a64 656c 6574 653a 204e 756d 6265 7220  :delete: Number 
-00010da0: 6f66 2063 6f6e 7465 6e74 206f 626a 6563  of content objec
-00010db0: 7473 2072 656d 6f76 6564 0a20 2020 2020  ts removed.     
-00010dc0: 2020 2020 2020 2020 2020 2063 6f6e 7465             conte
-00010dd0: 6e74 3a64 656c 6574 653a 6279 7465 733a  nt:delete:bytes:
-00010de0: 2053 756d 206f 6620 7468 6520 7265 6d6f   Sum of the remo
-00010df0: 7665 6420 636f 6e74 656e 7473 e280 9920  ved contents... 
-00010e00: 6461 7461 206c 656e 6774 680a 2020 2020  data length.    
-00010e10: 2020 2020 2020 2020 2020 2020 736b 6970              skip
-00010e20: 7065 645f 636f 6e74 656e 743a 6465 6c65  ped_content:dele
-00010e30: 7465 3a20 4e75 6d62 6572 206f 6620 736b  te: Number of sk
-00010e40: 6970 7065 6420 636f 6e74 656e 7420 6f62  ipped content ob
-00010e50: 6a65 6374 7320 7265 6d6f 7665 640a 2020  jects removed.  
-00010e60: 2020 2020 2020 2020 2020 2020 2020 6469                di
-00010e70: 7265 6374 6f72 793a 6465 6c65 7465 3a20  rectory:delete: 
-00010e80: 4e75 6d62 6572 206f 6620 6469 7265 6374  Number of direct
-00010e90: 6f72 7920 6f62 6a65 6374 7320 7265 6d6f  ory objects remo
-00010ea0: 7665 640a 2020 2020 2020 2020 2020 2020  ved.            
-00010eb0: 2020 2020 7265 7669 7369 6f6e 3a64 656c      revision:del
-00010ec0: 6574 653a 204e 756d 6265 7220 6f66 2072  ete: Number of r
-00010ed0: 6576 6973 696f 6e20 6f62 6a65 6374 7320  evision objects 
-00010ee0: 7265 6d6f 7665 640a 2020 2020 2020 2020  removed.        
-00010ef0: 2020 2020 2020 2020 7265 6c65 6173 653a          release:
-00010f00: 6465 6c65 7465 3a20 4e75 6d62 6572 206f  delete: Number o
-00010f10: 6620 7265 6c65 6173 6520 6f62 6a65 6374  f release object
-00010f20: 7320 7265 6d6f 7665 640a 2020 2020 2020  s removed.      
-00010f30: 2020 2020 2020 2020 2020 736e 6170 7368            snapsh
-00010f40: 6f74 3a64 656c 6574 653a 204e 756d 6265  ot:delete: Numbe
-00010f50: 7220 6f66 2073 6e61 7073 686f 7420 6f62  r of snapshot ob
-00010f60: 6a65 6374 7320 7265 6d6f 7665 640a 2020  jects removed.  
-00010f70: 2020 2020 2020 2020 2020 2020 2020 6f72                or
-00010f80: 6967 696e 3a64 656c 6574 653a 204e 756d  igin:delete: Num
-00010f90: 6265 7220 6f66 206f 7269 6769 6e20 6f62  ber of origin ob
-00010fa0: 6a65 6374 7320 7265 6d6f 7665 640a 2020  jects removed.  
-00010fb0: 2020 2020 2020 2020 2020 2020 2020 6f72                or
-00010fc0: 6967 696e 5f76 6973 6974 3a64 656c 6574  igin_visit:delet
-00010fd0: 653a 204e 756d 6265 7220 6f66 206f 7269  e: Number of ori
-00010fe0: 6769 6e20 7669 7369 7420 6f62 6a65 6374  gin visit object
-00010ff0: 7320 7265 6d6f 7665 640a 2020 2020 2020  s removed.      
-00011000: 2020 2020 2020 2020 2020 6f72 6967 696e            origin
-00011010: 5f76 6973 6974 5f73 7461 7475 733a 6465  _visit_status:de
-00011020: 6c65 7465 3a20 4e75 6d62 6572 206f 6620  lete: Number of 
-00011030: 6f72 6967 696e 2076 6973 6974 2073 7461  origin visit sta
-00011040: 7475 7320 6f62 6a65 6374 7320 7265 6d6f  tus objects remo
-00011050: 7665 640a 2020 2020 2020 2020 2222 220a  ved.        """.
-00011060: 2020 2020 2020 2020 6f62 6a65 6374 5f72          object_r
-00011070: 6f77 7320 3d20 5b0a 2020 2020 2020 2020  ows = [.        
-00011080: 2020 2020 2873 7768 6964 2e6f 626a 6563      (swhid.objec
-00011090: 745f 7479 7065 2e6e 616d 652e 6c6f 7765  t_type.name.lowe
-000110a0: 7228 292c 2073 7768 6964 2e6f 626a 6563  r(), swhid.objec
-000110b0: 745f 6964 2920 666f 7220 7377 6869 6420  t_id) for swhid 
-000110c0: 696e 2073 7768 6964 730a 2020 2020 2020  in swhids.      
-000110d0: 2020 5d0a 2020 2020 2020 2020 7265 7475    ].        retu
-000110e0: 726e 2064 622e 6f62 6a65 6374 5f64 656c  rn db.object_del
-000110f0: 6574 6528 6f62 6a65 6374 5f72 6f77 7329  ete(object_rows)
-00011100: 0a                                       .
+00010060: 686f 7269 7479 5f74 7970 652c 0a20 2020  hority_type,.   
+00010070: 2020 2020 2020 2020 2020 2020 2061 7574               aut
+00010080: 686f 7269 7479 5f75 726c 2c0a 2020 2020  hority_url,.    
+00010090: 2020 2020 2020 2020 2920 696e 2064 622e          ) in db.
+000100a0: 7261 775f 6578 7472 696e 7369 635f 6d65  raw_extrinsic_me
+000100b0: 7461 6461 7461 5f67 6574 5f61 7574 686f  tadata_get_autho
+000100c0: 7269 7469 6573 2873 7472 2874 6172 6765  rities(str(targe
+000100d0: 7429 2c20 6375 7229 0a20 2020 2020 2020  t), cur).       
+000100e0: 205d 0a0a 2020 2020 4064 625f 7472 616e   ]..    @db_tran
+000100f0: 7361 6374 696f 6e28 290a 2020 2020 6465  saction().    de
+00010100: 6620 6d65 7461 6461 7461 5f61 7574 686f  f metadata_autho
+00010110: 7269 7479 5f61 6464 280a 2020 2020 2020  rity_add(.      
+00010120: 2020 7365 6c66 2c20 6175 7468 6f72 6974    self, authorit
+00010130: 6965 733a 204c 6973 745b 4d65 7461 6461  ies: List[Metada
+00010140: 7461 4175 7468 6f72 6974 795d 2c20 2a2c  taAuthority], *,
+00010150: 2064 623a 2044 622c 2063 7572 3d4e 6f6e   db: Db, cur=Non
+00010160: 650a 2020 2020 2920 2d3e 2044 6963 745b  e.    ) -> Dict[
+00010170: 7374 722c 2069 6e74 5d3a 0a20 2020 2020  str, int]:.     
+00010180: 2020 2061 7574 686f 7269 7469 6573 203d     authorities =
+00010190: 206c 6973 7428 6175 7468 6f72 6974 6965   list(authoritie
+000101a0: 7329 0a20 2020 2020 2020 2073 656c 662e  s).        self.
+000101b0: 6a6f 7572 6e61 6c5f 7772 6974 6572 2e6d  journal_writer.m
+000101c0: 6574 6164 6174 615f 6175 7468 6f72 6974  etadata_authorit
+000101d0: 795f 6164 6428 6175 7468 6f72 6974 6965  y_add(authoritie
+000101e0: 7329 0a20 2020 2020 2020 2063 6f75 6e74  s).        count
+000101f0: 203d 2030 0a20 2020 2020 2020 2066 6f72   = 0.        for
+00010200: 2061 7574 686f 7269 7479 2069 6e20 6175   authority in au
+00010210: 7468 6f72 6974 6965 733a 0a20 2020 2020  thorities:.     
+00010220: 2020 2020 2020 2064 622e 6d65 7461 6461         db.metada
+00010230: 7461 5f61 7574 686f 7269 7479 5f61 6464  ta_authority_add
+00010240: 2861 7574 686f 7269 7479 2e74 7970 652e  (authority.type.
+00010250: 7661 6c75 652c 2061 7574 686f 7269 7479  value, authority
+00010260: 2e75 726c 2c20 6375 723d 6375 7229 0a20  .url, cur=cur). 
+00010270: 2020 2020 2020 2020 2020 2063 6f75 6e74             count
+00010280: 202b 3d20 310a 2020 2020 2020 2020 7265   += 1.        re
+00010290: 7475 726e 207b 226d 6574 6164 6174 615f  turn {"metadata_
+000102a0: 6175 7468 6f72 6974 793a 6164 6422 3a20  authority:add": 
+000102b0: 636f 756e 747d 0a0a 2020 2020 4064 625f  count}..    @db_
+000102c0: 7472 616e 7361 6374 696f 6e28 290a 2020  transaction().  
+000102d0: 2020 6465 6620 6d65 7461 6461 7461 5f61    def metadata_a
+000102e0: 7574 686f 7269 7479 5f67 6574 280a 2020  uthority_get(.  
+000102f0: 2020 2020 2020 7365 6c66 2c20 7479 7065        self, type
+00010300: 3a20 4d65 7461 6461 7461 4175 7468 6f72  : MetadataAuthor
+00010310: 6974 7954 7970 652c 2075 726c 3a20 7374  ityType, url: st
+00010320: 722c 202a 2c20 6462 3a20 4462 2c20 6375  r, *, db: Db, cu
+00010330: 723d 4e6f 6e65 0a20 2020 2029 202d 3e20  r=None.    ) -> 
+00010340: 4f70 7469 6f6e 616c 5b4d 6574 6164 6174  Optional[Metadat
+00010350: 6141 7574 686f 7269 7479 5d3a 0a20 2020  aAuthority]:.   
+00010360: 2020 2020 2072 6f77 203d 2064 622e 6d65       row = db.me
+00010370: 7461 6461 7461 5f61 7574 686f 7269 7479  tadata_authority
+00010380: 5f67 6574 2874 7970 652e 7661 6c75 652c  _get(type.value,
+00010390: 2075 726c 2c20 6375 723d 6375 7229 0a20   url, cur=cur). 
+000103a0: 2020 2020 2020 2069 6620 6e6f 7420 726f         if not ro
+000103b0: 773a 0a20 2020 2020 2020 2020 2020 2072  w:.            r
+000103c0: 6574 7572 6e20 4e6f 6e65 0a20 2020 2020  eturn None.     
+000103d0: 2020 2072 6574 7572 6e20 4d65 7461 6461     return Metada
+000103e0: 7461 4175 7468 6f72 6974 792e 6672 6f6d  taAuthority.from
+000103f0: 5f64 6963 7428 6469 6374 287a 6970 2864  _dict(dict(zip(d
+00010400: 622e 6d65 7461 6461 7461 5f61 7574 686f  b.metadata_autho
+00010410: 7269 7479 5f63 6f6c 732c 2072 6f77 2929  rity_cols, row))
+00010420: 290a 0a20 2020 2023 2323 2323 2323 2323  )..    #########
+00010430: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00010440: 0a20 2020 2023 2027 6f62 6a65 6374 5f72  .    # 'object_r
+00010450: 6566 6572 656e 6365 7327 2074 6162 6c65  eferences' table
+00010460: 0a20 2020 2023 2323 2323 2323 2323 2323  .    ###########
+00010470: 2323 2323 2323 2323 2323 2323 2323 0a0a  ##############..
+00010480: 2020 2020 4064 625f 7472 616e 7361 6374      @db_transact
+00010490: 696f 6e28 290a 2020 2020 6465 6620 6f62  ion().    def ob
+000104a0: 6a65 6374 5f66 696e 645f 7265 6365 6e74  ject_find_recent
+000104b0: 5f72 6566 6572 656e 6365 7328 0a20 2020  _references(.   
+000104c0: 2020 2020 2073 656c 662c 2074 6172 6765       self, targe
+000104d0: 745f 7377 6869 643a 2045 7874 656e 6465  t_swhid: Extende
+000104e0: 6453 5748 4944 2c20 6c69 6d69 743a 2069  dSWHID, limit: i
+000104f0: 6e74 2c20 2a2c 2064 623a 2044 622c 2063  nt, *, db: Db, c
+00010500: 7572 3d4e 6f6e 650a 2020 2020 2920 2d3e  ur=None.    ) ->
+00010510: 204c 6973 745b 4578 7465 6e64 6564 5357   List[ExtendedSW
+00010520: 4849 445d 3a0a 2020 2020 2020 2020 7265  HID]:.        re
+00010530: 7475 726e 205b 0a20 2020 2020 2020 2020  turn [.         
+00010540: 2020 2063 6f6e 7665 7274 6572 732e 6462     converters.db
+00010550: 5f74 6f5f 6f62 6a65 6374 5f72 6566 6572  _to_object_refer
+00010560: 656e 6365 5f73 6f75 7263 6528 726f 7729  ence_source(row)
+00010570: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00010580: 2072 6f77 2069 6e20 6462 2e6f 626a 6563   row in db.objec
+00010590: 745f 7265 6665 7265 6e63 6573 5f67 6574  t_references_get
+000105a0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000105b0: 2020 7461 7267 6574 5f74 7970 653d 7461    target_type=ta
+000105c0: 7267 6574 5f73 7768 6964 2e6f 626a 6563  rget_swhid.objec
+000105d0: 745f 7479 7065 2e6e 616d 652e 6c6f 7765  t_type.name.lowe
+000105e0: 7228 292c 0a20 2020 2020 2020 2020 2020  r(),.           
+000105f0: 2020 2020 2074 6172 6765 743d 7461 7267       target=targ
+00010600: 6574 5f73 7768 6964 2e6f 626a 6563 745f  et_swhid.object_
+00010610: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+00010620: 2020 2020 6c69 6d69 743d 6c69 6d69 742c      limit=limit,
+00010630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010640: 2063 7572 3d63 7572 2c0a 2020 2020 2020   cur=cur,.      
+00010650: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00010660: 5d0a 0a20 2020 2040 6462 5f74 7261 6e73  ]..    @db_trans
+00010670: 6163 7469 6f6e 2829 0a20 2020 2064 6566  action().    def
+00010680: 206f 626a 6563 745f 7265 6665 7265 6e63   object_referenc
+00010690: 6573 5f61 6464 280a 2020 2020 2020 2020  es_add(.        
+000106a0: 7365 6c66 2c20 7265 6665 7265 6e63 6573  self, references
+000106b0: 3a20 4c69 7374 5b4f 626a 6563 7452 6566  : List[ObjectRef
+000106c0: 6572 656e 6365 5d2c 202a 2c20 6462 3a20  erence], *, db: 
+000106d0: 4462 2c20 6375 723d 4e6f 6e65 0a20 2020  Db, cur=None.   
+000106e0: 2029 202d 3e20 4469 6374 5b73 7472 2c20   ) -> Dict[str, 
+000106f0: 696e 745d 3a0a 2020 2020 2020 2020 746f  int]:.        to
+00010700: 5f61 6464 203d 206c 6973 7428 7b63 6f6e  _add = list({con
+00010710: 7665 7274 6572 732e 6f62 6a65 6374 5f72  verters.object_r
+00010720: 6566 6572 656e 6365 5f74 6f5f 6462 2872  eference_to_db(r
+00010730: 6566 2920 666f 7220 7265 6620 696e 2072  ef) for ref in r
+00010740: 6566 6572 656e 6365 737d 290a 2020 2020  eferences}).    
+00010750: 2020 2020 6462 2e6f 626a 6563 745f 7265      db.object_re
+00010760: 6665 7265 6e63 6573 5f61 6464 280a 2020  ferences_add(.  
+00010770: 2020 2020 2020 2020 2020 746f 5f61 6464            to_add
+00010780: 2c0a 2020 2020 2020 2020 2020 2020 6375  ,.            cu
+00010790: 723d 6375 722c 0a20 2020 2020 2020 2029  r=cur,.        )
+000107a0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+000107b0: 207b 226f 626a 6563 745f 7265 6665 7265   {"object_refere
+000107c0: 6e63 653a 6164 6422 3a20 6c65 6e28 746f  nce:add": len(to
+000107d0: 5f61 6464 297d 0a0a 2020 2020 6465 6620  _add)}..    def 
+000107e0: 636c 6561 725f 6275 6666 6572 7328 7365  clear_buffers(se
+000107f0: 6c66 2c20 6f62 6a65 6374 5f74 7970 6573  lf, object_types
+00010800: 3a20 5365 7175 656e 6365 5b73 7472 5d20  : Sequence[str] 
+00010810: 3d20 2829 2920 2d3e 204e 6f6e 653a 0a20  = ()) -> None:. 
+00010820: 2020 2020 2020 2022 2222 446f 206e 6f74         """Do not
+00010830: 6869 6e67 2222 220a 2020 2020 2020 2020  hing""".        
+00010840: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
+00010850: 2064 6566 2066 6c75 7368 2873 656c 662c   def flush(self,
+00010860: 206f 626a 6563 745f 7479 7065 733a 2053   object_types: S
+00010870: 6571 7565 6e63 655b 7374 725d 203d 2028  equence[str] = (
+00010880: 2929 202d 3e20 4469 6374 5b73 7472 2c20  )) -> Dict[str, 
+00010890: 696e 745d 3a0a 2020 2020 2020 2020 7265  int]:.        re
+000108a0: 7475 726e 207b 7d0a 0a20 2020 2064 6566  turn {}..    def
+000108b0: 205f 6765 745f 6175 7468 6f72 6974 795f   _get_authority_
+000108c0: 6964 2873 656c 662c 2061 7574 686f 7269  id(self, authori
+000108d0: 7479 3a20 4d65 7461 6461 7461 4175 7468  ty: MetadataAuth
+000108e0: 6f72 6974 792c 2064 622c 2063 7572 293a  ority, db, cur):
+000108f0: 0a20 2020 2020 2020 2061 7574 686f 7269  .        authori
+00010900: 7479 5f69 6420 3d20 6462 2e6d 6574 6164  ty_id = db.metad
+00010910: 6174 615f 6175 7468 6f72 6974 795f 6765  ata_authority_ge
+00010920: 745f 6964 280a 2020 2020 2020 2020 2020  t_id(.          
+00010930: 2020 6175 7468 6f72 6974 792e 7479 7065    authority.type
+00010940: 2e76 616c 7565 2c20 6175 7468 6f72 6974  .value, authorit
+00010950: 792e 7572 6c2c 2063 7572 0a20 2020 2020  y.url, cur.     
+00010960: 2020 2029 0a20 2020 2020 2020 2069 6620     ).        if 
+00010970: 6e6f 7420 6175 7468 6f72 6974 795f 6964  not authority_id
+00010980: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00010990: 6973 6520 556e 6b6e 6f77 6e4d 6574 6164  ise UnknownMetad
+000109a0: 6174 6141 7574 686f 7269 7479 2873 7472  ataAuthority(str
+000109b0: 2861 7574 686f 7269 7479 2929 0a20 2020  (authority)).   
+000109c0: 2020 2020 2072 6574 7572 6e20 6175 7468       return auth
+000109d0: 6f72 6974 795f 6964 0a0a 2020 2020 6465  ority_id..    de
+000109e0: 6620 5f67 6574 5f66 6574 6368 6572 5f69  f _get_fetcher_i
+000109f0: 6428 7365 6c66 2c20 6665 7463 6865 723a  d(self, fetcher:
+00010a00: 204d 6574 6164 6174 6146 6574 6368 6572   MetadataFetcher
+00010a10: 2c20 6462 2c20 6375 7229 3a0a 2020 2020  , db, cur):.    
+00010a20: 2020 2020 6665 7463 6865 725f 6964 203d      fetcher_id =
+00010a30: 2064 622e 6d65 7461 6461 7461 5f66 6574   db.metadata_fet
+00010a40: 6368 6572 5f67 6574 5f69 6428 6665 7463  cher_get_id(fetc
+00010a50: 6865 722e 6e61 6d65 2c20 6665 7463 6865  her.name, fetche
+00010a60: 722e 7665 7273 696f 6e2c 2063 7572 290a  r.version, cur).
+00010a70: 2020 2020 2020 2020 6966 206e 6f74 2066          if not f
+00010a80: 6574 6368 6572 5f69 643a 0a20 2020 2020  etcher_id:.     
+00010a90: 2020 2020 2020 2072 6169 7365 2055 6e6b         raise Unk
+00010aa0: 6e6f 776e 4d65 7461 6461 7461 4665 7463  nownMetadataFetc
+00010ab0: 6865 7228 7374 7228 6665 7463 6865 7229  her(str(fetcher)
+00010ac0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00010ad0: 2066 6574 6368 6572 5f69 640a 0a20 2020   fetcher_id..   
+00010ae0: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
+00010af0: 2323 2323 2323 2323 2323 0a20 2020 2023  ##########.    #
+00010b00: 204f 626a 6563 7444 656c 6574 696f 6e49   ObjectDeletionI
+00010b10: 6e74 6572 6661 6365 0a20 2020 2023 2323  nterface.    ###
+00010b20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00010b30: 2323 2323 2323 0a0a 2020 2020 4064 625f  ######..    @db_
+00010b40: 7472 616e 7361 6374 696f 6e28 290a 2020  transaction().  
+00010b50: 2020 6465 6620 6f62 6a65 6374 5f64 656c    def object_del
+00010b60: 6574 6528 0a20 2020 2020 2020 2073 656c  ete(.        sel
+00010b70: 662c 2073 7768 6964 733a 204c 6973 745b  f, swhids: List[
+00010b80: 4578 7465 6e64 6564 5357 4849 445d 2c20  ExtendedSWHID], 
+00010b90: 2a2c 2064 623a 2044 622c 2063 7572 3d4e  *, db: Db, cur=N
+00010ba0: 6f6e 650a 2020 2020 2920 2d3e 2044 6963  one.    ) -> Dic
+00010bb0: 745b 7374 722c 2069 6e74 5d3a 0a20 2020  t[str, int]:.   
+00010bc0: 2020 2020 2022 2222 4465 6c65 7465 206f       """Delete o
+00010bd0: 626a 6563 7473 2066 726f 6d20 7468 6520  bjects from the 
+00010be0: 7374 6f72 6167 650a 0a20 2020 2020 2020  storage..       
+00010bf0: 2041 6c6c 2073 6b69 7070 6564 2063 6f6e   All skipped con
+00010c00: 7465 6e74 206f 626a 6563 7473 206d 6174  tent objects mat
+00010c10: 6368 696e 6720 7468 6520 6769 7665 6e20  ching the given 
+00010c20: 5357 4849 4420 7769 6c6c 2062 6520 7265  SWHID will be re
+00010c30: 6d6f 7665 642c 0a20 2020 2020 2020 2069  moved,.        i
+00010c40: 6e63 6c75 6469 6e67 2074 686f 7365 2077  ncluding those w
+00010c50: 686f 2068 6176 6520 7468 6520 7361 6d65  ho have the same
+00010c60: 2053 5748 4944 2064 7565 2074 6f20 6861   SWHID due to ha
+00010c70: 7368 2063 6f6c 6c69 7369 6f6e 732e 0a0a  sh collisions...
+00010c80: 2020 2020 2020 2020 4f72 6967 696e 206f          Origin o
+00010c90: 626a 6563 7473 2061 7265 2072 656d 6f76  bjects are remov
+00010ca0: 6564 2061 6c6f 6e67 7369 6465 2074 6865  ed alongside the
+00010cb0: 6972 2061 7373 6f63 6961 7465 6420 6f72  ir associated or
+00010cc0: 6967 696e 2076 6973 6974 2061 6e64 0a20  igin visit and. 
+00010cd0: 2020 2020 2020 206f 7269 6769 6e20 7669         origin vi
+00010ce0: 7369 7420 7374 6174 7573 206f 626a 6563  sit status objec
+00010cf0: 7473 2e0a 0a20 2020 2020 2020 2041 7267  ts...        Arg
+00010d00: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
+00010d10: 7768 6964 733a 206c 6973 7420 6f66 2053  whids: list of S
+00010d20: 5748 4944 206f 6620 7468 6520 6f62 6a65  WHID of the obje
+00010d30: 6374 7320 746f 2072 656d 6f76 650a 0a20  cts to remove.. 
+00010d40: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+00010d50: 2020 2020 2020 2020 2020 2020 5375 6d6d              Summ
+00010d60: 6172 7920 6469 6374 2077 6974 6820 7468  ary dict with th
+00010d70: 6520 666f 6c6c 6f77 696e 6720 6b65 7973  e following keys
+00010d80: 2061 6e64 2061 7373 6f63 6961 7465 6420   and associated 
+00010d90: 7661 6c75 6573 3a0a 0a20 2020 2020 2020  values:..       
+00010da0: 2020 2020 2020 2020 2063 6f6e 7465 6e74           content
+00010db0: 3a64 656c 6574 653a 204e 756d 6265 7220  :delete: Number 
+00010dc0: 6f66 2063 6f6e 7465 6e74 206f 626a 6563  of content objec
+00010dd0: 7473 2072 656d 6f76 6564 0a20 2020 2020  ts removed.     
+00010de0: 2020 2020 2020 2020 2020 2063 6f6e 7465             conte
+00010df0: 6e74 3a64 656c 6574 653a 6279 7465 733a  nt:delete:bytes:
+00010e00: 2053 756d 206f 6620 7468 6520 7265 6d6f   Sum of the remo
+00010e10: 7665 6420 636f 6e74 656e 7473 e280 9920  ved contents... 
+00010e20: 6461 7461 206c 656e 6774 680a 2020 2020  data length.    
+00010e30: 2020 2020 2020 2020 2020 2020 736b 6970              skip
+00010e40: 7065 645f 636f 6e74 656e 743a 6465 6c65  ped_content:dele
+00010e50: 7465 3a20 4e75 6d62 6572 206f 6620 736b  te: Number of sk
+00010e60: 6970 7065 6420 636f 6e74 656e 7420 6f62  ipped content ob
+00010e70: 6a65 6374 7320 7265 6d6f 7665 640a 2020  jects removed.  
+00010e80: 2020 2020 2020 2020 2020 2020 2020 6469                di
+00010e90: 7265 6374 6f72 793a 6465 6c65 7465 3a20  rectory:delete: 
+00010ea0: 4e75 6d62 6572 206f 6620 6469 7265 6374  Number of direct
+00010eb0: 6f72 7920 6f62 6a65 6374 7320 7265 6d6f  ory objects remo
+00010ec0: 7665 640a 2020 2020 2020 2020 2020 2020  ved.            
+00010ed0: 2020 2020 7265 7669 7369 6f6e 3a64 656c      revision:del
+00010ee0: 6574 653a 204e 756d 6265 7220 6f66 2072  ete: Number of r
+00010ef0: 6576 6973 696f 6e20 6f62 6a65 6374 7320  evision objects 
+00010f00: 7265 6d6f 7665 640a 2020 2020 2020 2020  removed.        
+00010f10: 2020 2020 2020 2020 7265 6c65 6173 653a          release:
+00010f20: 6465 6c65 7465 3a20 4e75 6d62 6572 206f  delete: Number o
+00010f30: 6620 7265 6c65 6173 6520 6f62 6a65 6374  f release object
+00010f40: 7320 7265 6d6f 7665 640a 2020 2020 2020  s removed.      
+00010f50: 2020 2020 2020 2020 2020 736e 6170 7368            snapsh
+00010f60: 6f74 3a64 656c 6574 653a 204e 756d 6265  ot:delete: Numbe
+00010f70: 7220 6f66 2073 6e61 7073 686f 7420 6f62  r of snapshot ob
+00010f80: 6a65 6374 7320 7265 6d6f 7665 640a 2020  jects removed.  
+00010f90: 2020 2020 2020 2020 2020 2020 2020 6f72                or
+00010fa0: 6967 696e 3a64 656c 6574 653a 204e 756d  igin:delete: Num
+00010fb0: 6265 7220 6f66 206f 7269 6769 6e20 6f62  ber of origin ob
+00010fc0: 6a65 6374 7320 7265 6d6f 7665 640a 2020  jects removed.  
+00010fd0: 2020 2020 2020 2020 2020 2020 2020 6f72                or
+00010fe0: 6967 696e 5f76 6973 6974 3a64 656c 6574  igin_visit:delet
+00010ff0: 653a 204e 756d 6265 7220 6f66 206f 7269  e: Number of ori
+00011000: 6769 6e20 7669 7369 7420 6f62 6a65 6374  gin visit object
+00011010: 7320 7265 6d6f 7665 640a 2020 2020 2020  s removed.      
+00011020: 2020 2020 2020 2020 2020 6f72 6967 696e            origin
+00011030: 5f76 6973 6974 5f73 7461 7475 733a 6465  _visit_status:de
+00011040: 6c65 7465 3a20 4e75 6d62 6572 206f 6620  lete: Number of 
+00011050: 6f72 6967 696e 2076 6973 6974 2073 7461  origin visit sta
+00011060: 7475 7320 6f62 6a65 6374 7320 7265 6d6f  tus objects remo
+00011070: 7665 640a 2020 2020 2020 2020 2222 220a  ved.        """.
+00011080: 2020 2020 2020 2020 6f62 6a65 6374 5f72          object_r
+00011090: 6f77 7320 3d20 5b0a 2020 2020 2020 2020  ows = [.        
+000110a0: 2020 2020 2873 7768 6964 2e6f 626a 6563      (swhid.objec
+000110b0: 745f 7479 7065 2e6e 616d 652e 6c6f 7765  t_type.name.lowe
+000110c0: 7228 292c 2073 7768 6964 2e6f 626a 6563  r(), swhid.objec
+000110d0: 745f 6964 2920 666f 7220 7377 6869 6420  t_id) for swhid 
+000110e0: 696e 2073 7768 6964 730a 2020 2020 2020  in swhids.      
+000110f0: 2020 5d0a 2020 2020 2020 2020 7265 7475    ].        retu
+00011100: 726e 2064 622e 6f62 6a65 6374 5f64 656c  rn db.object_del
+00011110: 6574 6528 6f62 6a65 6374 5f72 6f77 7329  ete(object_rows)
+00011120: 0a                                       .
```

### Comparing `swh_storage-2.3.1/swh/storage/proxies/buffer.py` & `swh_storage-2.4.0/swh/storage/proxies/buffer.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/proxies/counter.py` & `swh_storage-2.4.0/swh/storage/proxies/counter.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/proxies/filter.py` & `swh_storage-2.4.0/swh/storage/proxies/filter.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/proxies/masking/__init__.py` & `swh_storage-2.4.0/swh/storage/proxies/masking/__init__.py`

 * *Files identical despite different names*

```diff
@@ -108,15 +108,15 @@
                 swhid, ExtendedSWHID
             ), f"{method_name} returned object with unexpected swhid() method return type"
             return [swhid]
 
         if result_type:
             if result_type == "extid":
                 return [result.target.to_extended()]
-            if result_type.startswith("origin_visit"):
+            if result_type.value.startswith("origin_visit"):
                 return [Origin(url=result.origin).swhid()]
 
         if (
             object_type := method_name.removesuffix("_get_random").removesuffix(
                 "_get_id_partition"
             )
         ) != method_name:
```

### Comparing `swh_storage-2.3.1/swh/storage/proxies/masking/cli.py` & `swh_storage-2.4.0/swh/storage/proxies/masking/cli.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/proxies/masking/db.py` & `swh_storage-2.4.0/swh/storage/proxies/masking/db.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/proxies/masking/sql/30-schema.sql` & `swh_storage-2.4.0/swh/storage/proxies/masking/sql/30-schema.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/proxies/record_references.py` & `swh_storage-2.4.0/swh/storage/proxies/record_references.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/proxies/retry.py` & `swh_storage-2.4.0/swh/storage/proxies/retry.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/proxies/tenacious.py` & `swh_storage-2.4.0/swh/storage/proxies/tenacious.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/pytest_plugin.py` & `swh_storage-2.4.0/swh/storage/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/replay.py` & `swh_storage-2.4.0/swh/storage/replay.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,17 +177,17 @@
                 else:
                     oid = f"{object_type}:uuid:{uuid4()}"
             elif hasattr(obj, "swhid"):
                 swhid = obj.swhid()
                 oid = str(swhid)
             elif isinstance(obj, HashableObject):
                 uid = obj.compute_hash()
-                oid = f"{obj.object_type}:{uid.hex()}"  # type: ignore[attr-defined]
+                oid = f"{obj.object_type}:{uid.hex()}"
             else:
-                oid = f"{obj.object_type}:uuid:{uuid4()}"  # type: ignore[attr-defined]
+                oid = f"{obj.object_type}:uuid:{uuid4()}"
 
             self.reporter(oid, msg)
 
 
 def process_replay_objects(
     all_objects: Dict[str, List[BaseModel]], *, storage: StorageInterface
 ) -> None:
```

### Comparing `swh_storage-2.3.1/swh/storage/sql/10-superuser-init.sql` & `swh_storage-2.4.0/swh/storage/sql/10-superuser-init.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/15-flavor.sql` & `swh_storage-2.4.0/swh/storage/sql/15-flavor.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/20-enums.sql` & `swh_storage-2.4.0/swh/storage/sql/20-enums.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/30-schema.sql` & `swh_storage-2.4.0/swh/storage/sql/30-schema.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/40-funcs.sql` & `swh_storage-2.4.0/swh/storage/sql/40-funcs.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/60-indexes.sql` & `swh_storage-2.4.0/swh/storage/sql/60-indexes.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/logical_replication/replication_source.sql` & `swh_storage-2.4.0/swh/storage/sql/logical_replication/replication_source.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/015.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/015.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/016.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/016.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/017.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/017.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/018.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/018.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/019.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/019.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/020.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/020.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/021.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/021.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/022.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/022.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/023.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/023.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/024.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/024.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/025.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/025.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/026.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/026.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/027.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/027.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/028.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/028.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/029.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/029.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/030.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/030.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/032.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/032.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/033.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/033.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/034.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/034.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/035.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/035.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/036.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/036.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/037.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/037.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/038.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/038.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/039.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/039.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/040.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/040.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/041.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/041.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/042.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/042.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/043.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/043.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/044.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/044.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/046.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/046.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/047.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/047.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/048.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/048.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/049.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/049.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/050.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/050.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/051.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/051.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/052.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/052.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/053.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/053.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/054.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/054.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/055.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/055.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/056.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/056.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/057.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/057.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/058.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/058.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/059.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/059.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/060.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/060.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/061.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/061.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/062.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/062.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/063.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/063.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/064.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/064.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/065.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/065.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/067.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/067.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/068.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/068.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/069.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/069.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/071.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/071.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/072.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/072.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/073.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/073.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/074.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/074.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/075.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/075.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/076.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/076.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/077.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/077.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/078.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/078.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/079.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/079.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/080.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/080.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/081.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/081.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/082.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/082.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/083.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/083.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/084.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/084.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/085.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/085.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/086.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/086.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/087.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/087.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/088.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/088.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/089.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/089.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/090.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/090.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/091.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/091.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/092.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/092.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/093.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/093.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/094.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/094.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/095.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/095.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/096.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/096.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/097.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/097.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/099.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/099.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/100.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/100.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/101.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/101.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/102.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/102.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/103.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/103.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/104.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/104.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/105.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/105.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/106.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/106.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/107.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/107.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/108.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/108.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/109.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/109.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/110.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/110.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/111.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/111.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/112.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/112.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/113.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/113.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/114.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/114.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/115.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/115.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/117.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/117.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/118.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/118.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/119.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/119.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/120.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/120.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/123.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/123.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/124.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/124.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/125.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/125.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/127.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/127.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/128.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/128.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/129.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/129.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/130.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/130.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/134.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/134.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/136.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/136.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/137.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/137.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/138.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/138.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/139.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/139.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/143.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/143.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/146.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/146.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/147.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/147.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/148.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/148.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/149.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/149.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/150.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/150.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/154.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/154.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/155.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/155.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/156.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/156.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/157.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/157.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/158.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/158.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/159.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/159.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/160.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/160.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/161.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/161.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/162.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/162.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/163.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/163.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/167.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/167.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/168.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/168.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/169.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/169.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/170.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/170.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/171.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/171.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/172.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/172.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/173.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/173.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/175.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/175.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/176.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/176.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/179.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/179.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/180.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/180.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/181.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/181.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/182.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/182.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/183.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/183.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/184.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/184.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/185.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/185.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/187.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/187.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/188.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/188.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/189.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/189.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/190.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/190.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/191.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/191.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/sql/upgrades/193.sql` & `swh_storage-2.4.0/swh/storage/sql/upgrades/193.sql`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/algos/test_diff.py` & `swh_storage-2.4.0/swh/storage/tests/algos/test_diff.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/algos/test_dir_iterator.py` & `swh_storage-2.4.0/swh/storage/tests/algos/test_dir_iterator.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/algos/test_directory.py` & `swh_storage-2.4.0/swh/storage/tests/algos/test_directory.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/algos/test_discovery.py` & `swh_storage-2.4.0/swh/storage/tests/algos/test_discovery.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/algos/test_origin.py` & `swh_storage-2.4.0/swh/storage/tests/algos/test_origin.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/algos/test_revisions_walker.py` & `swh_storage-2.4.0/swh/storage/tests/algos/test_revisions_walker.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/algos/test_snapshot.py` & `swh_storage-2.4.0/swh/storage/tests/algos/test_snapshot.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 from hypothesis import HealthCheck, given, settings
 import pytest
 
-from swh.model.hypothesis_strategies import branch_names, branch_targets, snapshots
+from swh.model.hypothesis_strategies import branch_names, snapshot_targets, snapshots
 from swh.model.model import (
     OriginVisit,
     OriginVisitStatus,
     Snapshot,
     SnapshotBranch,
-    TargetType,
+    SnapshotTargetType,
 )
 from swh.storage.algos.snapshot import (
     snapshot_get_all_branches,
     snapshot_get_latest,
     snapshot_id_get_from_revision,
     snapshot_resolve_alias,
     visits_and_snapshots_get_from_revision,
@@ -44,18 +44,18 @@
     swh_storage.snapshot_add([snapshot])
 
     returned_snapshot = snapshot_get_all_branches(swh_storage, snapshot.id)
     assert snapshot == returned_snapshot
 
 
 @settings(suppress_health_check=disabled_health_checks, deadline=None)
-@given(branch_name=branch_names(), branch_target=branch_targets(only_objects=True))
-def test_snapshot_large(swh_storage, branch_name, branch_target):  # noqa
+@given(branch_name=branch_names(), snapshot_target=snapshot_targets(only_objects=True))
+def test_snapshot_large(swh_storage, branch_name, snapshot_target):  # noqa
     snapshot = Snapshot(
-        branches={b"%s%05d" % (branch_name, i): branch_target for i in range(10000)},
+        branches={b"%s%05d" % (branch_name, i): snapshot_target for i in range(10000)},
     )
 
     swh_storage.snapshot_add([snapshot])
 
     returned_snapshot = snapshot_get_all_branches(swh_storage, snapshot.id)
     assert snapshot == returned_snapshot
 
@@ -314,32 +314,32 @@
     rel_branch_name = b"release_branch"
     rev_alias1_name = b"rev_alias1"
     rev_alias2_name = b"rev_alias2"
     rev_alias3_name = b"rev_alias3"
     rel_alias_name = b"rel_alias"
     rev_branch_info = SnapshotBranch(
         target=sample_data.revisions[0].id,
-        target_type=TargetType.REVISION,
+        target_type=SnapshotTargetType.REVISION,
     )
     rel_branch_info = SnapshotBranch(
         target=sample_data.releases[0].id,
-        target_type=TargetType.RELEASE,
+        target_type=SnapshotTargetType.RELEASE,
     )
     rev_alias1_branch_info = SnapshotBranch(
-        target=rev_branch_name, target_type=TargetType.ALIAS
+        target=rev_branch_name, target_type=SnapshotTargetType.ALIAS
     )
     rev_alias2_branch_info = SnapshotBranch(
-        target=rev_alias1_name, target_type=TargetType.ALIAS
+        target=rev_alias1_name, target_type=SnapshotTargetType.ALIAS
     )
 
     rev_alias3_branch_info = SnapshotBranch(
-        target=rev_alias2_name, target_type=TargetType.ALIAS
+        target=rev_alias2_name, target_type=SnapshotTargetType.ALIAS
     )
     rel_alias_branch_info = SnapshotBranch(
-        target=rel_branch_name, target_type=TargetType.ALIAS
+        target=rel_branch_name, target_type=SnapshotTargetType.ALIAS
     )
 
     snapshot = Snapshot(
         branches={
             rev_branch_name: rev_branch_info,
             rel_branch_name: rel_branch_info,
             rev_alias1_name: rev_alias1_branch_info,
@@ -369,15 +369,15 @@
 
 
 def test_snapshot_resolve_alias_dangling_branch(swh_storage):
     dangling_branch_name = b"dangling_branch"
     alias_name = b"rev_alias"
 
     alias_branch = SnapshotBranch(
-        target=dangling_branch_name, target_type=TargetType.ALIAS
+        target=dangling_branch_name, target_type=SnapshotTargetType.ALIAS
     )
 
     snapshot = Snapshot(
         branches={
             dangling_branch_name: None,
             alias_name: alias_branch,
         }
@@ -388,15 +388,15 @@
 
 
 def test_snapshot_resolve_alias_missing_branch(swh_storage):
     missing_branch_name = b"missing_branch"
     alias_name = b"rev_alias"
 
     alias_branch = SnapshotBranch(
-        target=missing_branch_name, target_type=TargetType.ALIAS
+        target=missing_branch_name, target_type=SnapshotTargetType.ALIAS
     )
 
     snapshot = Snapshot(
         id=b"42" * 10,
         branches={
             alias_name: alias_branch,
         },
@@ -409,24 +409,24 @@
 def test_snapshot_resolve_alias_cycle_found(swh_storage):
     alias1_name = b"alias_1"
     alias2_name = b"alias_2"
     alias3_name = b"alias_3"
     alias4_name = b"alias_4"
 
     alias1_branch_info = SnapshotBranch(
-        target=alias2_name, target_type=TargetType.ALIAS
+        target=alias2_name, target_type=SnapshotTargetType.ALIAS
     )
     alias2_branch_info = SnapshotBranch(
-        target=alias3_name, target_type=TargetType.ALIAS
+        target=alias3_name, target_type=SnapshotTargetType.ALIAS
     )
     alias3_branch_info = SnapshotBranch(
-        target=alias4_name, target_type=TargetType.ALIAS
+        target=alias4_name, target_type=SnapshotTargetType.ALIAS
     )
     alias4_branch_info = SnapshotBranch(
-        target=alias2_name, target_type=TargetType.ALIAS
+        target=alias2_name, target_type=SnapshotTargetType.ALIAS
     )
 
     snapshot = Snapshot(
         branches={
             alias1_name: alias1_branch_info,
             alias2_name: alias2_branch_info,
             alias3_name: alias3_branch_info,
```

### Comparing `swh_storage-2.3.1/swh/storage/tests/conftest.py` & `swh_storage-2.4.0/swh/storage/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/masking/conftest.py` & `swh_storage-2.4.0/swh/storage/tests/masking/conftest.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/masking/test_cli.py` & `swh_storage-2.4.0/swh/storage/tests/masking/test_cli.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/masking/test_db.py` & `swh_storage-2.4.0/swh/storage/tests/masking/test_db.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/masking/test_proxy.py` & `swh_storage-2.4.0/swh/storage/tests/masking/test_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,25 +7,27 @@
 from typing import Iterable, cast
 
 import attr
 import pytest
 
 from swh.core.api.classes import stream_results
 from swh.model.model import (
+    Directory,
+    DirectoryEntry,
+    ExtID,
     OriginVisit,
     OriginVisitStatus,
     Release,
+    ReleaseTargetType,
     Revision,
     RevisionType,
     Snapshot,
     SnapshotBranch,
-    TargetType,
+    SnapshotTargetType,
 )
-from swh.model.model import Directory, DirectoryEntry, ExtID
-from swh.model.model import ObjectType as ModelObjectType
 from swh.model.swhids import CoreSWHID, ExtendedObjectType, ExtendedSWHID, ObjectType
 from swh.storage.exc import MaskedObjectException
 from swh.storage.interface import HashDict
 from swh.storage.proxies.masking import MaskingProxyStorage
 from swh.storage.proxies.masking.db import MaskedState
 from swh.storage.tests.storage_data import StorageData
 
@@ -507,19 +509,19 @@
     # Should this mask extids if the target is masked?
     pass
 
 
 def test_release_get(swh_storage, set_object_visibility):
     # release.target = revision
     assert StorageData.release.target == StorageData.revision.id
-    assert StorageData.release.target_type == ModelObjectType.REVISION
+    assert StorageData.release.target_type == ReleaseTargetType.REVISION
 
     # release2.target = revision2
     assert StorageData.release2.target == StorageData.revision2.id
-    assert StorageData.release2.target_type == ModelObjectType.REVISION
+    assert StorageData.release2.target_type == ReleaseTargetType.REVISION
 
     # Ensure that object masking doesn't prevent insertion
     set_object_visibility(
         [StorageData.release.swhid().to_extended()], MaskedState.DECISION_PENDING
     )
 
     swh_storage.release_add([StorageData.release, StorageData.release2])
@@ -546,15 +548,15 @@
     releases = [
         Release(
             name=f"release{i}".encode(),
             message=f"hello{i}".encode(),
             author=None,
             date=None,
             target=b"\x00" * 20,
-            target_type=ModelObjectType.REVISION,
+            target_type=ReleaseTargetType.REVISION,
             synthetic=True,
         )
         for i in range(100)
     ]
     swh_storage.release_add(releases)
 
     nb_partitions = 4
@@ -591,15 +593,15 @@
 
     assert (
         swh_storage.snapshot_get(StorageData.complete_snapshot.id)
         == complete_snapshot_dict
     )
     # Check that masking branch targets doesn't affect snapshot visibility
     for branch in StorageData.complete_snapshot.branches.values():
-        if not branch or branch.target_type == TargetType.ALIAS:
+        if not branch or branch.target_type == SnapshotTargetType.ALIAS:
             continue
 
         set_object_visibility(
             [branch.swhid().to_extended()], MaskedState.DECISION_PENDING
         )
         assert (
             swh_storage.snapshot_get(StorageData.complete_snapshot.id)
@@ -638,15 +640,15 @@
 
     assert (
         swh_storage.snapshot_get_branches(StorageData.complete_snapshot.id)
         == get_branches_result
     )
     # Check that masking branch targets doesn't affect snapshot visibility
     for branch in StorageData.complete_snapshot.branches.values():
-        if not branch or branch.target_type == TargetType.ALIAS:
+        if not branch or branch.target_type == SnapshotTargetType.ALIAS:
             continue
 
         set_object_visibility(
             [branch.swhid().to_extended()], MaskedState.DECISION_PENDING
         )
         assert (
             swh_storage.snapshot_get_branches(StorageData.complete_snapshot.id)
@@ -669,15 +671,15 @@
 
     assert swh_storage.snapshot_branch_get_by_name(
         StorageData.complete_snapshot.id, branch_name=b"content"
     ).branch_found
 
     # Check that masking branch targets doesn't affect snapshot visibility
     for name, branch in StorageData.complete_snapshot.branches.items():
-        if branch and branch.target_type != TargetType.ALIAS:
+        if branch and branch.target_type != SnapshotTargetType.ALIAS:
             set_object_visibility(
                 [branch.swhid().to_extended()], MaskedState.DECISION_PENDING
             )
 
         found = swh_storage.snapshot_branch_get_by_name(
             StorageData.complete_snapshot.id, branch_name=name, follow_alias_chain=False
         )
@@ -696,15 +698,15 @@
 
 def test_snapshot_get_id_partition(swh_storage, set_object_visibility):
     snapshots = [
         Snapshot(
             branches={
                 f"branch{i}".encode(): SnapshotBranch(
                     target=b"\x00" * 20,
-                    target_type=TargetType.REVISION,
+                    target_type=SnapshotTargetType.REVISION,
                 ),
             },
         )
         for i in range(100)
     ]
     swh_storage.snapshot_add(snapshots)
```

### Comparing `swh_storage-2.3.1/swh/storage/tests/masking/test_proxy_masking.py` & `swh_storage-2.4.0/swh/storage/tests/masking/test_proxy_masking.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/masking/test_proxy_no_masking.py` & `swh_storage-2.4.0/swh/storage/tests/masking/test_proxy_no_masking.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/migrate_extrinsic_metadata/test_cran.py` & `swh_storage-2.4.0/swh/storage/tests/migrate_extrinsic_metadata/test_cran.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/migrate_extrinsic_metadata/test_debian.py` & `swh_storage-2.4.0/swh/storage/tests/migrate_extrinsic_metadata/test_debian.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     OriginVisitStatus,
     Person,
     RawExtrinsicMetadata,
     Revision,
     RevisionType,
     Snapshot,
     SnapshotBranch,
-    TargetType,
+    SnapshotTargetType,
     Timestamp,
     TimestampWithTimezone,
 )
 from swh.model.swhids import CoreSWHID, ExtendedObjectType, ExtendedSWHID
 from swh.storage import get_storage
 from swh.storage.interface import ListOrder, PagedResult
 from swh.storage.migrate_extrinsic_metadata import debian_origins_from_row, handle_row
@@ -113,15 +113,15 @@
 
     snapshot = Snapshot(
         id=b"\xafD\x15\x98){\xd4$\xdeI\x1f\xbe\x95lh`x\x14\xce\xc4",
         branches={
             # ...
             b"releases/unstable/main/4:19.12.1-1": SnapshotBranch(
                 target=b"\x00\x00\x03l1\x1e\xf3:(\x1b\x05h\x8fn\xad\xcf\xc0\x94:\xee",
-                target_type=TargetType.REVISION,
+                target_type=SnapshotTargetType.REVISION,
             ),
         },
     )
 
     revision_row = {
         "id": b"\x00\x00\x03l1\x1e\xf3:(\x1b\x05h\x8fn\xad\xcf\xc0\x94:\xee",
         "directory": DIRECTORY_ID,
@@ -222,15 +222,15 @@
     # "remove" the snapshot again
     storage = copy.deepcopy(storage_before_snapshot)
 
     snapshot = attr.evolve(
         snapshot,
         branches={
             b"foo": SnapshotBranch(
-                target_type=TargetType.REVISION,
+                target_type=SnapshotTargetType.REVISION,
                 target=revision_id,
             )
         },
     )
     storage.snapshot_add([snapshot])
 
     # branch points to unknown revision
@@ -311,15 +311,15 @@
     )
     storage.snapshot_add(
         [
             Snapshot(
                 id=b"42" * 10,
                 branches={
                     b"foo": SnapshotBranch(
-                        target_type=TargetType.REVISION, target=revision_id
+                        target_type=SnapshotTargetType.REVISION, target=revision_id
                     )
                 },
             )
         ]
     )
 
     storage_before_revision = copy.deepcopy(storage)
```

### Comparing `swh_storage-2.3.1/swh/storage/tests/migrate_extrinsic_metadata/test_deposit.py` & `swh_storage-2.4.0/swh/storage/tests/migrate_extrinsic_metadata/test_deposit.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/migrate_extrinsic_metadata/test_gnu.py` & `swh_storage-2.4.0/swh/storage/tests/migrate_extrinsic_metadata/test_gnu.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/migrate_extrinsic_metadata/test_nixguix.py` & `swh_storage-2.4.0/swh/storage/tests/migrate_extrinsic_metadata/test_nixguix.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/migrate_extrinsic_metadata/test_npm.py` & `swh_storage-2.4.0/swh/storage/tests/migrate_extrinsic_metadata/test_npm.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/migrate_extrinsic_metadata/test_pypi.py` & `swh_storage-2.4.0/swh/storage/tests/migrate_extrinsic_metadata/test_pypi.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     MetadataFetcher,
     Origin,
     OriginVisit,
     OriginVisitStatus,
     RawExtrinsicMetadata,
     Snapshot,
     SnapshotBranch,
-    TargetType,
+    SnapshotTargetType,
 )
 from swh.model.swhids import CoreSWHID, ExtendedObjectType, ExtendedSWHID
 from swh.storage import get_storage
 from swh.storage.interface import PagedResult
 from swh.storage.migrate_extrinsic_metadata import (
     handle_row,
     pypi_origin_from_filename,
@@ -173,15 +173,15 @@
     )
     storage.snapshot_add(
         [
             Snapshot(
                 id=snapshot_id,
                 branches={
                     b"foo": SnapshotBranch(
-                        target_type=TargetType.REVISION,
+                        target_type=SnapshotTargetType.REVISION,
                         target=revision_id,
                     )
                 },
             )
         ]
     )
 
@@ -662,15 +662,15 @@
     )
     storage.snapshot_add(
         [
             Snapshot(
                 id=snapshot_id,
                 branches={
                     b"foo": SnapshotBranch(
-                        target_type=TargetType.REVISION,
+                        target_type=SnapshotTargetType.REVISION,
                         target=revision_id,
                     )
                 },
             )
         ]
     )
     storage.metadata_authority_add(
```

### Comparing `swh_storage-2.3.1/swh/storage/tests/storage_data.py` & `swh_storage-2.4.0/swh/storage/tests/storage_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     RawExtrinsicMetadata,
     Release,
     Revision,
     RevisionType,
     SkippedContent,
     Snapshot,
     SnapshotBranch,
-    TargetType,
+    SnapshotTargetType,
     Timestamp,
     TimestampWithTimezone,
 )
 from swh.model.swhids import CoreSWHID, ExtendedObjectType, ExtendedSWHID
 from swh.model.swhids import ObjectType as SwhidObjectType
 
 
@@ -692,52 +692,52 @@
     releases: Tuple[Release, ...] = (release, release2, release3)
 
     snapshot = Snapshot(
         id=hash_to_bytes("9b922e6d8d5b803c1582aabe5525b7b91150788e"),
         branches={
             b"master": SnapshotBranch(
                 target=revision.id,
-                target_type=TargetType.REVISION,
+                target_type=SnapshotTargetType.REVISION,
             ),
         },
     )
     empty_snapshot = Snapshot(
         id=hash_to_bytes("1a8893e6a86f444e8be8e7bda6cb34fb1735a00e"),
         branches={},
     )
     complete_snapshot = Snapshot(
         id=hash_to_bytes("db99fda25b43dc5cd90625ee4b0744751799c917"),
         branches={
             b"directory": SnapshotBranch(
                 target=directory.id,
-                target_type=TargetType.DIRECTORY,
+                target_type=SnapshotTargetType.DIRECTORY,
             ),
             b"directory2": SnapshotBranch(
                 target=directory2.id,
-                target_type=TargetType.DIRECTORY,
+                target_type=SnapshotTargetType.DIRECTORY,
             ),
             b"content": SnapshotBranch(
                 target=content.sha1_git,
-                target_type=TargetType.CONTENT,
+                target_type=SnapshotTargetType.CONTENT,
             ),
             b"alias": SnapshotBranch(
                 target=b"revision",
-                target_type=TargetType.ALIAS,
+                target_type=SnapshotTargetType.ALIAS,
             ),
             b"revision": SnapshotBranch(
                 target=revision.id,
-                target_type=TargetType.REVISION,
+                target_type=SnapshotTargetType.REVISION,
             ),
             b"release": SnapshotBranch(
                 target=release.id,
-                target_type=TargetType.RELEASE,
+                target_type=SnapshotTargetType.RELEASE,
             ),
             b"snapshot": SnapshotBranch(
                 target=empty_snapshot.id,
-                target_type=TargetType.SNAPSHOT,
+                target_type=SnapshotTargetType.SNAPSHOT,
             ),
             b"dangling": None,
         },
     )
 
     snapshots: Tuple[Snapshot, ...] = (snapshot, empty_snapshot, complete_snapshot)
```

### Comparing `swh_storage-2.3.1/swh/storage/tests/storage_tests.py` & `swh_storage-2.4.0/swh/storage/tests/storage_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,31 +20,33 @@
 import pytest
 
 from swh.core.api import RemoteException
 from swh.core.api.classes import stream_results
 from swh.model import from_disk, hypothesis_strategies
 from swh.model.hashutil import DEFAULT_ALGORITHMS, MultiHash, hash_to_bytes
 from swh.model.model import (
+    Directory,
+    DirectoryEntry,
+    ExtID,
     Origin,
     OriginVisit,
     OriginVisitStatus,
     Person,
     RawExtrinsicMetadata,
     Release,
+    ReleaseTargetType,
     Revision,
     RevisionType,
     SkippedContent,
     Snapshot,
     SnapshotBranch,
-    TargetType,
+    SnapshotTargetType,
     Timestamp,
     TimestampWithTimezone,
 )
-from swh.model.model import Content, Directory, DirectoryEntry, ExtID
-from swh.model.model import ObjectType as ModelObjectType
 from swh.model.swhids import CoreSWHID, ExtendedSWHID, ObjectType
 from swh.storage.cassandra.storage import CassandraStorage
 from swh.storage.common import origin_url_to_sha1 as sha1
 from swh.storage.exc import (
     HashCollision,
     QueryTimeout,
     StorageArgumentException,
@@ -128,19 +130,14 @@
 
 
 def filter_dict(d):
     "Filter None value from a dict"
     return {k: v for k, v in d.items() if v is not None}
 
 
-class LazyContent(Content):
-    def with_data(self):
-        return Content.from_dict({**self.to_dict(), "data": b"42\n"})
-
-
 class TestStorage:
     """Main class for Storage testing.
 
     This class is used as-is to test local storage (see TestLocalStorage
     below) and remote storage (see TestRemoteStorage in
     test_remote_storage.py.
 
@@ -285,15 +282,15 @@
             swh_storage, CassandraStorage
         ):
             swh_storage.refresh_stat_counters()
             assert swh_storage.stat_counters()["content"] == 1
 
     def test_content_add_from_lazy_content(self, swh_storage, sample_data):
         cont = sample_data.content
-        lazy_content = LazyContent.from_dict(cont.to_dict())
+        lazy_content = cont.evolve(data=None, get_data=lambda: cont.data)
 
         insertion_start_time = now()
 
         actual_result = swh_storage.content_add([lazy_content])
 
         insertion_end_time = now()
 
@@ -302,25 +299,25 @@
             "content:add:bytes": cont.length,
         }
 
         # the fact that we retrieve the content object from the storage with
         # the correct 'data' field ensures it has been 'called'
         assert swh_storage.content_get_data({"sha1": cont.sha1}) == cont.data
 
-        expected_cont = attr.evolve(lazy_content, data=None, ctime=None)
+        expected_cont = cont.evolve(data=None, ctime=None, get_data=None)
         contents = [
             obj
             for (obj_type, obj) in swh_storage.journal_writer.journal.objects
             if obj_type == "content"
         ]
         assert len(contents) == 1
         for obj in contents:
             assert insertion_start_time <= obj.ctime
             assert obj.ctime <= insertion_end_time
-            assert attr.evolve(obj, ctime=None).to_dict() == expected_cont.to_dict()
+            assert obj.evolve(ctime=None).to_dict() == expected_cont.to_dict()
 
         if isinstance(swh_storage, InMemoryStorage) or not isinstance(
             swh_storage, CassandraStorage
         ):
             swh_storage.refresh_stat_counters()
             assert swh_storage.stat_counters()["content"] == 1
 
@@ -2230,15 +2227,15 @@
         releases = list(sample_data.releases) + [
             Release(
                 name=f"release{i}".encode(),
                 message=f"hello{i}".encode(),
                 author=None,
                 date=None,
                 target=b"\x00" * 20,
-                target_type=ModelObjectType.REVISION,
+                target_type=ReleaseTargetType.REVISION,
                 synthetic=True,
             )
             for i in range(100)
         ]
         swh_storage.release_add(releases)
 
         # nb_partitions = smallest power of 2 such that at least one of
@@ -4573,27 +4570,27 @@
     def test_snapshot_add_count_branches_with_filtering_edge_cases(
         self, swh_storage, sample_data
     ):
         snapshot = Snapshot(
             branches={
                 b"\xaa\xff": SnapshotBranch(
                     target=sample_data.revision.id,
-                    target_type=TargetType.REVISION,
+                    target_type=SnapshotTargetType.REVISION,
                 ),
                 b"\xaa\xff\x00": SnapshotBranch(
                     target=sample_data.revision.id,
-                    target_type=TargetType.REVISION,
+                    target_type=SnapshotTargetType.REVISION,
                 ),
                 b"\xff\xff": SnapshotBranch(
                     target=sample_data.release.id,
-                    target_type=TargetType.RELEASE,
+                    target_type=SnapshotTargetType.RELEASE,
                 ),
                 b"\xff\xff\x00": SnapshotBranch(
                     target=sample_data.release.id,
-                    target_type=TargetType.RELEASE,
+                    target_type=SnapshotTargetType.RELEASE,
                 ),
                 b"dangling": None,
             },
         )
 
         swh_storage.snapshot_add([snapshot])
 
@@ -4688,29 +4685,31 @@
         )
 
         expected_snapshot = {
             "id": snp_id,
             "branches": {
                 name: tgt
                 for name, tgt in branches.items()
-                if tgt and tgt.target_type in [TargetType.RELEASE, TargetType.REVISION]
+                if tgt
+                and tgt.target_type
+                in [SnapshotTargetType.RELEASE, SnapshotTargetType.REVISION]
             },
             "next_branch": None,
         }
 
         assert snapshot == expected_snapshot
 
         snapshot = swh_storage.snapshot_get_branches(snp_id, target_types=["alias"])
 
         expected_snapshot = {
             "id": snp_id,
             "branches": {
                 name: tgt
                 for name, tgt in branches.items()
-                if tgt and tgt.target_type == TargetType.ALIAS
+                if tgt and tgt.target_type == SnapshotTargetType.ALIAS
             },
             "next_branch": None,
         }
 
         assert snapshot == expected_snapshot
 
     def test_snapshot_add_get_filtered_and_paginated(self, swh_storage, sample_data):
@@ -4817,44 +4816,44 @@
         assert alias1 in branches
 
     def test_snapshot_add_get_by_branches_name_pattern(self, swh_storage, sample_data):
         snapshot = Snapshot(
             branches={
                 b"refs/heads/master": SnapshotBranch(
                     target=sample_data.revision.id,
-                    target_type=TargetType.REVISION,
+                    target_type=SnapshotTargetType.REVISION,
                 ),
                 b"refs/heads/incoming": SnapshotBranch(
                     target=sample_data.revision.id,
-                    target_type=TargetType.REVISION,
+                    target_type=SnapshotTargetType.REVISION,
                 ),
                 b"refs/pull/1": SnapshotBranch(
                     target=sample_data.revision.id,
-                    target_type=TargetType.REVISION,
+                    target_type=SnapshotTargetType.REVISION,
                 ),
                 b"refs/pull/2": SnapshotBranch(
                     target=sample_data.revision.id,
-                    target_type=TargetType.REVISION,
+                    target_type=SnapshotTargetType.REVISION,
                 ),
                 b"dangling": None,
                 b"\xaa\xff": SnapshotBranch(
                     target=sample_data.revision.id,
-                    target_type=TargetType.REVISION,
+                    target_type=SnapshotTargetType.REVISION,
                 ),
                 b"\xaa\xff\x00": SnapshotBranch(
                     target=sample_data.revision.id,
-                    target_type=TargetType.REVISION,
+                    target_type=SnapshotTargetType.REVISION,
                 ),
                 b"\xff\xff": SnapshotBranch(
                     target=sample_data.revision.id,
-                    target_type=TargetType.REVISION,
+                    target_type=SnapshotTargetType.REVISION,
                 ),
                 b"\xff\xff\x00": SnapshotBranch(
                     target=sample_data.revision.id,
-                    target_type=TargetType.REVISION,
+                    target_type=SnapshotTargetType.REVISION,
                 ),
             },
         )
         swh_storage.snapshot_add([snapshot])
 
         for include_pattern, exclude_prefix, nb_results in (
             (b"pull", None, 2),
@@ -4888,37 +4887,37 @@
     ):
         pattern = b"foo"
         nb_branches_by_target_type = 10
         branches = {}
         for i in range(nb_branches_by_target_type):
             branches[f"branch/directory/bar{i}".encode()] = SnapshotBranch(
                 target=sample_data.directory.id,
-                target_type=TargetType.DIRECTORY,
+                target_type=SnapshotTargetType.DIRECTORY,
             )
             branches[f"branch/revision/bar{i}".encode()] = SnapshotBranch(
                 target=sample_data.revision.id,
-                target_type=TargetType.REVISION,
+                target_type=SnapshotTargetType.REVISION,
             )
             branches[f"branch/directory/{pattern}{i}".encode()] = SnapshotBranch(
                 target=sample_data.directory.id,
-                target_type=TargetType.DIRECTORY,
+                target_type=SnapshotTargetType.DIRECTORY,
             )
             branches[f"branch/revision/{pattern}{i}".encode()] = SnapshotBranch(
                 target=sample_data.revision.id,
-                target_type=TargetType.REVISION,
+                target_type=SnapshotTargetType.REVISION,
             )
 
         snapshot = Snapshot(branches=branches)
         swh_storage.snapshot_add([snapshot])
 
         branches_count = nb_branches_by_target_type // 2
 
         for target_type in (
-            TargetType.DIRECTORY,
-            TargetType.REVISION,
+            SnapshotTargetType.DIRECTORY,
+            SnapshotTargetType.REVISION,
         ):
             target_type_str = target_type.value
             partial_branches = swh_storage.snapshot_get_branches(
                 snapshot.id,
                 branch_name_include_substring=pattern,
                 target_types=[target_type_str],
                 branches_count=branches_count,
@@ -4955,15 +4954,15 @@
             assert partial_branches["next_branch"] is None
 
     def test_snapshot_get_branches_from_no_result(self, swh_storage, sample_data):
         snapshot = Snapshot(
             branches={
                 b"refs/heads/master": SnapshotBranch(
                     target=sample_data.revision.id,
-                    target_type=TargetType.REVISION,
+                    target_type=SnapshotTargetType.REVISION,
                 ),
             },
         )
         swh_storage.snapshot_add([snapshot])
 
         partial_branches = swh_storage.snapshot_get_branches(
             snapshot.id,
@@ -4975,56 +4974,56 @@
 
     def test_snapshot_get_branches_correct_branch_count(self, swh_storage, sample_data):
         n = 20
         branches = {}
         for i in range(n):
             branches[f"refs/heads/head{i:02d}".encode()] = SnapshotBranch(
                 target=sample_data.revision.id,
-                target_type=TargetType.REVISION,
+                target_type=SnapshotTargetType.REVISION,
             )
             branches[f"refs/tags/tag{i:02d}".encode()] = SnapshotBranch(
                 target=sample_data.release.id,
-                target_type=TargetType.RELEASE,
+                target_type=SnapshotTargetType.RELEASE,
             )
         for i in range(n):
             branches[f"refs/tags/tag{n+i:02d}".encode()] = SnapshotBranch(
                 target=sample_data.release.id,
-                target_type=TargetType.RELEASE,
+                target_type=SnapshotTargetType.RELEASE,
             )
 
         snapshot = Snapshot(branches=branches)
         swh_storage.snapshot_add([snapshot])
 
         partial_branches = swh_storage.snapshot_get_branches(
             snapshot.id, target_types=["release"], branches_count=n
         )
 
         assert len(partial_branches["branches"]) == n
         assert all(
-            branch.target_type == TargetType.RELEASE
+            branch.target_type == SnapshotTargetType.RELEASE
             for branch in partial_branches["branches"].values()
         )
         assert partial_branches["next_branch"] == b"refs/tags/tag20"
 
     def test_snapshot_get_branches_from_after_exclude_prefix(
         self, swh_storage, sample_data
     ):
         snapshot = Snapshot(
             branches={
                 b"refs/pulls/pull0": SnapshotBranch(
                     target=sample_data.revision.id,
-                    target_type=TargetType.REVISION,
+                    target_type=SnapshotTargetType.REVISION,
                 ),
                 b"refs/tags/tag00": SnapshotBranch(
                     target=sample_data.release.id,
-                    target_type=TargetType.RELEASE,
+                    target_type=SnapshotTargetType.RELEASE,
                 ),
                 b"refs/tags/tag01": SnapshotBranch(
                     target=sample_data.release.id,
-                    target_type=TargetType.RELEASE,
+                    target_type=SnapshotTargetType.RELEASE,
                 ),
             }
         )
         swh_storage.snapshot_add([snapshot])
 
         branches_from = b"refs/tags/tag01"
         partial_branches = swh_storage.snapshot_get_branches(
@@ -5088,15 +5087,15 @@
 
     def test_snapshot_get_id_partition(self, swh_storage, sample_data):
         snapshots = list(sample_data.snapshots) + [
             Snapshot(
                 branches={
                     f"branch{i}".encode(): SnapshotBranch(
                         target=b"\x00" * 20,
-                        target_type=TargetType.REVISION,
+                        target_type=SnapshotTargetType.REVISION,
                     ),
                 },
             )
             for i in range(100)
         ]
         swh_storage.snapshot_add(snapshots)
 
@@ -5214,19 +5213,19 @@
 
     def test_snapshot_branch_get_by_name_alias_chain_cycles(self, swh_storage):
         snapshot = Snapshot(
             id=hash_to_bytes("428893e6a864344e8be8e7bda6cb34fb1735a00e"),
             branches={
                 b"HEAD1": SnapshotBranch(
                     target=b"HEAD2",
-                    target_type=TargetType.ALIAS,
+                    target_type=SnapshotTargetType.ALIAS,
                 ),
                 b"HEAD2": SnapshotBranch(
                     target=b"HEAD1",
-                    target_type=TargetType.ALIAS,
+                    target_type=SnapshotTargetType.ALIAS,
                 ),
             },
         )
         swh_storage.snapshot_add([snapshot])
         branch = swh_storage.snapshot_branch_get_by_name(
             snapshot_id=snapshot.id, branch_name=b"HEAD1"
         )
@@ -5238,27 +5237,27 @@
 
     def test_snapshot_branch_get_by_name_alias_chain_too_long(self, swh_storage):
         snapshot = Snapshot(
             id=hash_to_bytes("873893e6a864344e8be8e7bda6cb34fb1735a00e"),
             branches={
                 b"first": SnapshotBranch(
                     target=b"second",
-                    target_type=TargetType.ALIAS,
+                    target_type=SnapshotTargetType.ALIAS,
                 ),
                 b"second": SnapshotBranch(
                     target=b"third",
-                    target_type=TargetType.ALIAS,
+                    target_type=SnapshotTargetType.ALIAS,
                 ),
                 b"third": SnapshotBranch(
                     target=b"forth",
-                    target_type=TargetType.ALIAS,
+                    target_type=SnapshotTargetType.ALIAS,
                 ),
                 b"forth": SnapshotBranch(
                     target=b"revision",
-                    target_type=TargetType.ALIAS,
+                    target_type=SnapshotTargetType.ALIAS,
                 ),
             },
         )
         swh_storage.snapshot_add([snapshot])
         branch = swh_storage.snapshot_branch_get_by_name(
             snapshot_id=snapshot.id, branch_name=b"first", max_alias_chain_length=3
         )
```

### Comparing `swh_storage-2.3.1/swh/storage/tests/test_api_client.py` & `swh_storage-2.4.0/swh/storage/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/test_backfill.py` & `swh_storage-2.4.0/swh/storage/tests/test_backfill.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/test_buffer.py` & `swh_storage-2.4.0/swh/storage/tests/test_buffer.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/test_cassandra.py` & `swh_storage-2.4.0/swh/storage/tests/test_cassandra.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/test_cassandra_converters.py` & `swh_storage-2.4.0/swh/storage/tests/test_cassandra_converters.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/test_cassandra_migration.py` & `swh_storage-2.4.0/swh/storage/tests/test_cassandra_migration.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/test_cli.py` & `swh_storage-2.4.0/swh/storage/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from click.testing import CliRunner
 from confluent_kafka import Producer
 import pytest
 import yaml
 
 from swh.journal.serializers import key_to_kafka, value_to_kafka
-from swh.model.model import Origin, Snapshot, SnapshotBranch, TargetType
+from swh.model.model import Origin, Snapshot, SnapshotBranch, SnapshotTargetType
 from swh.storage import get_storage
 from swh.storage.cli import storage as cli
 from swh.storage.replay import OBJECT_CONVERTERS
 
 logger = logging.getLogger(__name__)
 
 
@@ -107,15 +107,15 @@
             "acks": "all",
         }
     )
 
     snapshot = Snapshot(
         branches={
             b"HEAD": SnapshotBranch(
-                target_type=TargetType.REVISION,
+                target_type=SnapshotTargetType.REVISION,
                 target=b"\x01" * 20,
             )
         },
     )
     snapshot_dict = snapshot.to_dict()
 
     producer.produce(
@@ -164,15 +164,15 @@
             "acks": "all",
         }
     )
 
     snapshot = Snapshot(
         branches={
             b"HEAD": SnapshotBranch(
-                target_type=TargetType.REVISION,
+                target_type=SnapshotTargetType.REVISION,
                 target=b"\x01" * 20,
             )
         },
     )
     snapshot_dict = snapshot.to_dict()
     producer.produce(
         topic=kafka_prefix + ".snapshot",
```

### Comparing `swh_storage-2.3.1/swh/storage/tests/test_counter.py` & `swh_storage-2.4.0/swh/storage/tests/test_counter.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/test_exception.py` & `swh_storage-2.4.0/swh/storage/tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/test_filter.py` & `swh_storage-2.4.0/swh/storage/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/test_in_memory.py` & `swh_storage-2.4.0/swh/storage/tests/test_in_memory.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/test_init.py` & `swh_storage-2.4.0/swh/storage/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/test_kafka_writer.py` & `swh_storage-2.4.0/swh/storage/tests/test_kafka_writer.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/test_metrics.py` & `swh_storage-2.4.0/swh/storage/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/test_postgresql.py` & `swh_storage-2.4.0/swh/storage/tests/test_postgresql.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/test_postgresql_converters.py` & `swh_storage-2.4.0/swh/storage/tests/test_postgresql_converters.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/test_postgresql_flavor_mirror.py` & `swh_storage-2.4.0/swh/storage/tests/test_postgresql_flavor_mirror.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/test_postgresql_flavor_readreplica.py` & `swh_storage-2.4.0/swh/storage/tests/test_postgresql_flavor_readreplica.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/test_pytest_plugin.py` & `swh_storage-2.4.0/swh/storage/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/test_record_references.py` & `swh_storage-2.4.0/swh/storage/tests/test_record_references.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/test_replay.py` & `swh_storage-2.4.0/swh/storage/tests/test_replay.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/test_retry.py` & `swh_storage-2.4.0/swh/storage/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/test_revision_bw_compat.py` & `swh_storage-2.4.0/swh/storage/tests/test_revision_bw_compat.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/test_serializers.py` & `swh_storage-2.4.0/swh/storage/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/test_server.py` & `swh_storage-2.4.0/swh/storage/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/test_storage_data.py` & `swh_storage-2.4.0/swh/storage/tests/test_storage_data.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/test_tenacious.py` & `swh_storage-2.4.0/swh/storage/tests/test_tenacious.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/test_utils.py` & `swh_storage-2.4.0/swh/storage/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/tests/test_validate.py` & `swh_storage-2.4.0/swh/storage/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/utils.py` & `swh_storage-2.4.0/swh/storage/utils.py`

 * *Files identical despite different names*

### Comparing `swh_storage-2.3.1/swh/storage/writer.py` & `swh_storage-2.4.0/swh/storage/writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # Copyright (C) 2020 The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 from typing import Any, Dict, Iterable
 
-from attr import evolve
-
 from swh.model.model import (
     Content,
     Directory,
     ExtID,
     MetadataAuthority,
     MetadataFetcher,
     Origin,
@@ -64,15 +62,15 @@
 
     def write_additions(self, object_type, values) -> None:
         if self.journal:
             self.journal.write_additions(object_type, values)
 
     def content_add(self, contents: Iterable[Content]) -> None:
         """Add contents to the journal. Drop the data field if provided."""
-        contents = [evolve(item, data=None) for item in contents]
+        contents = [item.evolve(data=None, get_data=None) for item in contents]
         self.write_additions("content", contents)
 
     def content_update(self, contents: Iterable[Dict[str, Any]]) -> None:
         if self.journal:
             raise NotImplementedError("content_update is not supported by the journal.")
 
     def content_add_metadata(self, contents: Iterable[Content]) -> None:
```

### Comparing `swh_storage-2.3.1/swh.storage.egg-info/PKG-INFO` & `swh_storage-2.4.0/swh.storage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.storage
-Version: 2.3.1
+Version: 2.4.0
 Summary: Software Heritage storage manager
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-storage
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-storage/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-storage/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-storage.git
@@ -25,22 +25,22 @@
 Requires-Dist: mypy_extensions
 Requires-Dist: psycopg2
 Requires-Dist: redis
 Requires-Dist: tenacity!=8.2.0,>=6.2
 Requires-Dist: typing-extensions
 Requires-Dist: swh.core[db,http]>=3.0.0
 Requires-Dist: swh.counters>=v0.8.0
-Requires-Dist: swh.model>=6.11.0
+Requires-Dist: swh.model>=6.13.0
 Requires-Dist: swh.objstorage>=2.2.0
 Provides-Extra: testing
 Requires-Dist: hypothesis>=3.11.0; extra == "testing"
 Requires-Dist: pytest>=8.1; extra == "testing"
 Requires-Dist: pytest-mock; extra == "testing"
 Requires-Dist: swh.core[testing]>=3.0.0; extra == "testing"
-Requires-Dist: swh.model[testing]>=0.0.50; extra == "testing"
+Requires-Dist: swh.model[testing]>=6.13.0; extra == "testing"
 Requires-Dist: pytz; extra == "testing"
 Requires-Dist: pytest-redis; extra == "testing"
 Requires-Dist: pytest-xdist; extra == "testing"
 Requires-Dist: types-python-dateutil; extra == "testing"
 Requires-Dist: types-pytz; extra == "testing"
 Requires-Dist: types-pyyaml; extra == "testing"
 Requires-Dist: types-redis; extra == "testing"
```

### Comparing `swh_storage-2.3.1/swh.storage.egg-info/SOURCES.txt` & `swh_storage-2.4.0/swh.storage.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -102,14 +102,20 @@
 swh/storage/proxies/buffer.py
 swh/storage/proxies/counter.py
 swh/storage/proxies/filter.py
 swh/storage/proxies/record_references.py
 swh/storage/proxies/retry.py
 swh/storage/proxies/tenacious.py
 swh/storage/proxies/validate.py
+swh/storage/proxies/blocking/__init__.py
+swh/storage/proxies/blocking/cli.py
+swh/storage/proxies/blocking/db.py
+swh/storage/proxies/blocking/sql/10-superuser-init.sql
+swh/storage/proxies/blocking/sql/30-schema.sql
+swh/storage/proxies/blocking/sql/60-indexes.sql
 swh/storage/proxies/masking/__init__.py
 swh/storage/proxies/masking/cli.py
 swh/storage/proxies/masking/db.py
 swh/storage/proxies/masking/sql/10-superuser-init.sql
 swh/storage/proxies/masking/sql/20-types.sql
 swh/storage/proxies/masking/sql/30-schema.sql
 swh/storage/proxies/masking/sql/60-indexes.sql
@@ -336,14 +342,21 @@
 swh/storage/tests/algos/test_diff.py
 swh/storage/tests/algos/test_dir_iterator.py
 swh/storage/tests/algos/test_directory.py
 swh/storage/tests/algos/test_discovery.py
 swh/storage/tests/algos/test_origin.py
 swh/storage/tests/algos/test_revisions_walker.py
 swh/storage/tests/algos/test_snapshot.py
+swh/storage/tests/blocking/__init__.py
+swh/storage/tests/blocking/conftest.py
+swh/storage/tests/blocking/test_cli.py
+swh/storage/tests/blocking/test_db.py
+swh/storage/tests/blocking/test_proxy.py
+swh/storage/tests/blocking/test_proxy_blocking.py
+swh/storage/tests/blocking/test_proxy_no_blocking.py
 swh/storage/tests/data/storage.yml
 swh/storage/tests/masking/__init__.py
 swh/storage/tests/masking/conftest.py
 swh/storage/tests/masking/test_cli.py
 swh/storage/tests/masking/test_db.py
 swh/storage/tests/masking/test_proxy.py
 swh/storage/tests/masking/test_proxy_masking.py
```

### Comparing `swh_storage-2.3.1/swh.storage.egg-info/entry_points.txt` & `swh_storage-2.4.0/swh.storage.egg-info/entry_points.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 [swh.cli.subcommands]
 swh.storage = swh.storage.cli
+swh.storage.proxies.blocking = swh.storage.proxies.blocking.cli
 swh.storage.proxies.masking = swh.storage.proxies.masking.cli
 
 [swh.storage.classes]
+blocking = swh.storage.proxies.blocking:BlockingProxyStorage
 buffer = swh.storage.proxies.buffer:BufferingProxyStorage
 cassandra = swh.storage.cassandra:CassandraStorage
 counter = swh.storage.proxies.counter:CountingProxyStorage
 filter = swh.storage.proxies.filter:FilteringProxyStorage
 local = swh.storage.postgresql.storage:Storage
 masking = swh.storage.proxies.masking:MaskingProxyStorage
 memory = swh.storage.in_memory:InMemoryStorage
```

### Comparing `swh_storage-2.3.1/tox.ini` & `swh_storage-2.4.0/tox.ini`

 * *Files identical despite different names*

