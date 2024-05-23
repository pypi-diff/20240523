# Comparing `tmp/digitalhub_core-0.5.0b1.tar.gz` & `tmp/digitalhub_core-0.5.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalhub_core-0.5.0b1.tar", last modified: Tue May 21 15:53:29 2024, max compression
+gzip compressed data, was "digitalhub_core-0.5.0b2.tar", last modified: Thu May 23 14:02:52 2024, max compression
```

## Comparing `digitalhub_core-0.5.0b1.tar` & `digitalhub_core-0.5.0b2.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.509397 digitalhub_core-0.5.0b1/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    11585 2023-08-23 08:29:57.000000 digitalhub_core-0.5.0b1/LICENSE.txt
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14995 2024-05-21 15:53:29.509397 digitalhub_core-0.5.0b1/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      499 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/README.md
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.485396 digitalhub_core-0.5.0b1/digitalhub_core/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1259 2024-05-21 13:14:45.000000 digitalhub_core-0.5.0b1/digitalhub_core/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.485396 digitalhub_core-0.5.0b1/digitalhub_core/client/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b1/digitalhub_core/client/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2352 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/client/builder.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.489396 digitalhub_core-0.5.0b1/digitalhub_core/client/objects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-10-10 11:19:53.000000 digitalhub_core-0.5.0b1/digitalhub_core/client/objects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1166 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/client/objects/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8892 2024-05-02 13:03:59.000000 digitalhub_core-0.5.0b1/digitalhub_core/client/objects/dhcore.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    16292 2024-05-13 12:38:37.000000 digitalhub_core-0.5.0b1/digitalhub_core/client/objects/local.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.489396 digitalhub_core-0.5.0b1/digitalhub_core/context/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b1/digitalhub_core/context/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3098 2024-03-12 14:22:03.000000 digitalhub_core-0.5.0b1/digitalhub_core/context/builder.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2926 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/context/context.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.489396 digitalhub_core-0.5.0b1/digitalhub_core/entities/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.493396 digitalhub_core-0.5.0b1/digitalhub_core/entities/_base/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/_base/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1521 2024-02-05 10:28:22.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/_base/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3172 2024-05-02 12:54:20.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/_base/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2485 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/_base/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1024 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/_base/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1567 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/_base/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.493396 digitalhub_core-0.5.0b1/digitalhub_core/entities/_builders/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-09-27 11:31:31.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/_builders/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1794 2024-05-06 11:10:34.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/_builders/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1435 2024-05-06 11:10:34.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/_builders/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1748 2024-05-06 11:10:34.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/_builders/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.493396 digitalhub_core-0.5.0b1/digitalhub_core/entities/artifacts/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/artifacts/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6641 2024-05-21 13:14:45.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/artifacts/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    14010 2024-05-21 13:14:46.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/artifacts/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      339 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/artifacts/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1876 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/artifacts/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      322 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/artifacts/status.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      318 2024-05-06 11:13:11.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/entity_types.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.497396 digitalhub_core-0.5.0b1/digitalhub_core/entities/functions/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/functions/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6298 2024-05-21 13:14:45.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/functions/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    16737 2024-05-21 13:14:45.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/functions/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      227 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/functions/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1699 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/functions/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-22 07:49:08.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/functions/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.497396 digitalhub_core-0.5.0b1/digitalhub_core/entities/projects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/projects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8705 2024-05-21 13:14:45.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/projects/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    22032 2024-05-21 13:14:46.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/projects/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      224 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/projects/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1467 2024-02-29 07:59:41.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/projects/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-02-15 09:23:23.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/projects/status.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      927 2024-05-06 11:13:11.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/registries.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.497396 digitalhub_core-0.5.0b1/digitalhub_core/entities/runs/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/runs/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4897 2024-05-21 13:14:45.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/runs/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    14326 2024-05-21 13:14:46.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/runs/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      212 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/runs/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3532 2024-05-09 11:08:45.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/runs/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2620 2024-05-13 12:22:42.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/runs/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.501397 digitalhub_core-0.5.0b1/digitalhub_core/entities/secrets/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-06 10:39:09.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/secrets/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6160 2024-05-21 13:14:45.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/secrets/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8742 2024-05-21 13:14:45.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/secrets/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      221 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/secrets/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      746 2024-02-15 09:49:55.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/secrets/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      212 2024-02-15 09:23:29.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/secrets/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.501397 digitalhub_core-0.5.0b1/digitalhub_core/entities/tasks/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/tasks/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5550 2024-05-21 13:14:45.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/tasks/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    10643 2024-05-21 13:14:45.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/tasks/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/tasks/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5151 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/tasks/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      431 2024-03-19 10:12:26.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/tasks/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      206 2023-11-17 12:02:01.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/tasks/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.501397 digitalhub_core-0.5.0b1/digitalhub_core/entities/workflows/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/workflows/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6358 2024-05-21 13:14:45.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/workflows/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    16023 2024-05-21 13:14:46.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/workflows/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      227 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/workflows/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      295 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/workflows/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-15 09:23:47.000000 digitalhub_core-0.5.0b1/digitalhub_core/entities/workflows/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.501397 digitalhub_core-0.5.0b1/digitalhub_core/registry/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/registry/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1468 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/registry/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1866 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/registry/registry.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3714 2024-05-06 11:10:35.000000 digitalhub_core-0.5.0b1/digitalhub_core/registry/utils.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.505396 digitalhub_core-0.5.0b1/digitalhub_core/runtimes/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-09-05 11:37:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/runtimes/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3931 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/runtimes/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1005 2024-05-06 11:10:34.000000 digitalhub_core-0.5.0b1/digitalhub_core/runtimes/builder.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.505396 digitalhub_core-0.5.0b1/digitalhub_core/stores/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b1/digitalhub_core/stores/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6767 2024-05-21 13:14:45.000000 digitalhub_core-0.5.0b1/digitalhub_core/stores/builder.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.505396 digitalhub_core-0.5.0b1/digitalhub_core/stores/objects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b1/digitalhub_core/stores/objects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3635 2024-05-21 14:15:02.000000 digitalhub_core-0.5.0b1/digitalhub_core/stores/objects/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3623 2024-05-21 14:15:34.000000 digitalhub_core-0.5.0b1/digitalhub_core/stores/objects/local.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4548 2024-05-21 14:15:53.000000 digitalhub_core-0.5.0b1/digitalhub_core/stores/objects/remote.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     7995 2024-05-21 14:16:16.000000 digitalhub_core-0.5.0b1/digitalhub_core/stores/objects/s3.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     9035 2024-05-21 15:25:40.000000 digitalhub_core-0.5.0b1/digitalhub_core/stores/objects/sql.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.505396 digitalhub_core-0.5.0b1/digitalhub_core/utils/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b1/digitalhub_core/utils/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3646 2024-03-12 14:23:02.000000 digitalhub_core-0.5.0b1/digitalhub_core/utils/api.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2215 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/utils/env_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      346 2023-12-11 08:31:30.000000 digitalhub_core-0.5.0b1/digitalhub_core/utils/exceptions.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1332 2024-04-08 14:07:02.000000 digitalhub_core-0.5.0b1/digitalhub_core/utils/file_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4237 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/utils/generic_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3054 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/utils/git_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1794 2024-02-01 10:08:51.000000 digitalhub_core-0.5.0b1/digitalhub_core/utils/io_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      460 2023-11-21 13:33:17.000000 digitalhub_core-0.5.0b1/digitalhub_core/utils/logger.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      805 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b1/digitalhub_core/utils/uri_utils.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:53:29.505396 digitalhub_core-0.5.0b1/digitalhub_core.egg-info/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14995 2024-05-21 15:53:29.000000 digitalhub_core-0.5.0b1/digitalhub_core.egg-info/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3901 2024-05-21 15:53:29.000000 digitalhub_core-0.5.0b1/digitalhub_core.egg-info/SOURCES.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-21 15:53:29.000000 digitalhub_core-0.5.0b1/digitalhub_core.egg-info/dependency_links.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      221 2024-05-21 15:53:29.000000 digitalhub_core-0.5.0b1/digitalhub_core.egg-info/requires.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-05-21 15:53:29.000000 digitalhub_core-0.5.0b1/digitalhub_core.egg-info/top_level.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1687 2024-05-21 15:31:37.000000 digitalhub_core-0.5.0b1/pyproject.toml
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-21 15:53:29.509397 digitalhub_core-0.5.0b1/setup.cfg
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 14:02:52.340801 digitalhub_core-0.5.0b2/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    11585 2023-08-23 08:29:57.000000 digitalhub_core-0.5.0b2/LICENSE.txt
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14995 2024-05-23 14:02:52.340801 digitalhub_core-0.5.0b2/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      499 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b2/README.md
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 14:02:52.320801 digitalhub_core-0.5.0b2/digitalhub_core/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1259 2024-05-23 09:43:31.000000 digitalhub_core-0.5.0b2/digitalhub_core/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 14:02:52.324801 digitalhub_core-0.5.0b2/digitalhub_core/client/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b2/digitalhub_core/client/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2352 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b2/digitalhub_core/client/builder.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 14:02:52.324801 digitalhub_core-0.5.0b2/digitalhub_core/client/objects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-10-10 11:19:53.000000 digitalhub_core-0.5.0b2/digitalhub_core/client/objects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1166 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b2/digitalhub_core/client/objects/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8892 2024-05-02 13:03:59.000000 digitalhub_core-0.5.0b2/digitalhub_core/client/objects/dhcore.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    16292 2024-05-13 12:38:37.000000 digitalhub_core-0.5.0b2/digitalhub_core/client/objects/local.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 14:02:52.324801 digitalhub_core-0.5.0b2/digitalhub_core/context/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b2/digitalhub_core/context/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3098 2024-03-12 14:22:03.000000 digitalhub_core-0.5.0b2/digitalhub_core/context/builder.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2926 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b2/digitalhub_core/context/context.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 14:02:52.324801 digitalhub_core-0.5.0b2/digitalhub_core/entities/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 14:02:52.324801 digitalhub_core-0.5.0b2/digitalhub_core/entities/_base/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/_base/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1521 2024-02-05 10:28:22.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/_base/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3172 2024-05-02 12:54:20.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/_base/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2485 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/_base/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1024 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/_base/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1567 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/_base/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 14:02:52.328801 digitalhub_core-0.5.0b2/digitalhub_core/entities/_builders/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-09-27 11:31:31.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/_builders/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1794 2024-05-06 11:10:34.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/_builders/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1435 2024-05-06 11:10:34.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/_builders/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1748 2024-05-06 11:10:34.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/_builders/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 14:02:52.328801 digitalhub_core-0.5.0b2/digitalhub_core/entities/artifacts/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/artifacts/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6641 2024-05-23 09:43:31.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/artifacts/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    14010 2024-05-23 09:43:32.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/artifacts/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      339 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/artifacts/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1876 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/artifacts/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      322 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/artifacts/status.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      318 2024-05-06 11:13:11.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/entity_types.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 14:02:52.328801 digitalhub_core-0.5.0b2/digitalhub_core/entities/functions/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/functions/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6298 2024-05-23 09:43:31.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/functions/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    16737 2024-05-23 09:43:32.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/functions/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      227 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/functions/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1699 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/functions/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-22 07:49:08.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/functions/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 14:02:52.328801 digitalhub_core-0.5.0b2/digitalhub_core/entities/projects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/projects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8705 2024-05-23 09:43:31.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/projects/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    22032 2024-05-23 09:43:32.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/projects/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      224 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/projects/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1467 2024-02-29 07:59:41.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/projects/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-02-15 09:23:23.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/projects/status.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      927 2024-05-06 11:13:11.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/registries.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 14:02:52.332801 digitalhub_core-0.5.0b2/digitalhub_core/entities/runs/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/runs/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4897 2024-05-23 09:43:31.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/runs/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    14326 2024-05-23 09:43:32.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/runs/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      212 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/runs/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3532 2024-05-09 11:08:45.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/runs/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2674 2024-05-23 13:52:47.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/runs/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 14:02:52.332801 digitalhub_core-0.5.0b2/digitalhub_core/entities/secrets/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-06 10:39:09.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/secrets/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6160 2024-05-23 09:43:31.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/secrets/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8742 2024-05-23 09:43:32.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/secrets/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      221 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/secrets/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      746 2024-02-15 09:49:55.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/secrets/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      212 2024-02-15 09:23:29.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/secrets/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 14:02:52.332801 digitalhub_core-0.5.0b2/digitalhub_core/entities/tasks/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/tasks/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5550 2024-05-23 09:43:31.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/tasks/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    10643 2024-05-23 09:43:32.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/tasks/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/tasks/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5151 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/tasks/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      431 2024-03-19 10:12:26.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/tasks/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      206 2023-11-17 12:02:01.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/tasks/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 14:02:52.332801 digitalhub_core-0.5.0b2/digitalhub_core/entities/workflows/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/workflows/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6358 2024-05-23 09:43:32.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/workflows/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    16023 2024-05-23 09:43:32.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/workflows/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      227 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/workflows/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      295 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/workflows/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-15 09:23:47.000000 digitalhub_core-0.5.0b2/digitalhub_core/entities/workflows/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 14:02:52.332801 digitalhub_core-0.5.0b2/digitalhub_core/registry/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b2/digitalhub_core/registry/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1468 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b2/digitalhub_core/registry/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1866 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b2/digitalhub_core/registry/registry.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3714 2024-05-06 11:10:35.000000 digitalhub_core-0.5.0b2/digitalhub_core/registry/utils.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 14:02:52.336801 digitalhub_core-0.5.0b2/digitalhub_core/runtimes/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-09-05 11:37:04.000000 digitalhub_core-0.5.0b2/digitalhub_core/runtimes/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3931 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b2/digitalhub_core/runtimes/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1005 2024-05-06 11:10:34.000000 digitalhub_core-0.5.0b2/digitalhub_core/runtimes/builder.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 14:02:52.336801 digitalhub_core-0.5.0b2/digitalhub_core/stores/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b2/digitalhub_core/stores/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6767 2024-05-23 09:43:32.000000 digitalhub_core-0.5.0b2/digitalhub_core/stores/builder.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 14:02:52.336801 digitalhub_core-0.5.0b2/digitalhub_core/stores/objects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b2/digitalhub_core/stores/objects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3635 2024-05-21 14:15:02.000000 digitalhub_core-0.5.0b2/digitalhub_core/stores/objects/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3608 2024-05-23 09:43:05.000000 digitalhub_core-0.5.0b2/digitalhub_core/stores/objects/local.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4534 2024-05-23 09:43:05.000000 digitalhub_core-0.5.0b2/digitalhub_core/stores/objects/remote.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     7980 2024-05-23 09:43:05.000000 digitalhub_core-0.5.0b2/digitalhub_core/stores/objects/s3.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     9012 2024-05-23 09:43:05.000000 digitalhub_core-0.5.0b2/digitalhub_core/stores/objects/sql.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 14:02:52.336801 digitalhub_core-0.5.0b2/digitalhub_core/utils/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b2/digitalhub_core/utils/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3646 2024-03-12 14:23:02.000000 digitalhub_core-0.5.0b2/digitalhub_core/utils/api.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2215 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b2/digitalhub_core/utils/env_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      346 2023-12-11 08:31:30.000000 digitalhub_core-0.5.0b2/digitalhub_core/utils/exceptions.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1332 2024-04-08 14:07:02.000000 digitalhub_core-0.5.0b2/digitalhub_core/utils/file_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4237 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b2/digitalhub_core/utils/generic_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3054 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b2/digitalhub_core/utils/git_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1794 2024-02-01 10:08:51.000000 digitalhub_core-0.5.0b2/digitalhub_core/utils/io_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      460 2023-11-21 13:33:17.000000 digitalhub_core-0.5.0b2/digitalhub_core/utils/logger.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      805 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b2/digitalhub_core/utils/uri_utils.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 14:02:52.336801 digitalhub_core-0.5.0b2/digitalhub_core.egg-info/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14995 2024-05-23 14:02:52.000000 digitalhub_core-0.5.0b2/digitalhub_core.egg-info/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3901 2024-05-23 14:02:52.000000 digitalhub_core-0.5.0b2/digitalhub_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-23 14:02:52.000000 digitalhub_core-0.5.0b2/digitalhub_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      221 2024-05-23 14:02:52.000000 digitalhub_core-0.5.0b2/digitalhub_core.egg-info/requires.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-05-23 14:02:52.000000 digitalhub_core-0.5.0b2/digitalhub_core.egg-info/top_level.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1687 2024-05-23 13:58:10.000000 digitalhub_core-0.5.0b2/pyproject.toml
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-23 14:02:52.340801 digitalhub_core-0.5.0b2/setup.cfg
```

### Comparing `digitalhub_core-0.5.0b1/LICENSE.txt` & `digitalhub_core-0.5.0b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/PKG-INFO` & `digitalhub_core-0.5.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-core
-Version: 0.5.0b1
+Version: 0.5.0b2
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 License:                               Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/__init__.py` & `digitalhub_core-0.5.0b2/digitalhub_core/__init__.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/client/builder.py` & `digitalhub_core-0.5.0b2/digitalhub_core/client/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/client/objects/base.py` & `digitalhub_core-0.5.0b2/digitalhub_core/client/objects/base.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/client/objects/dhcore.py` & `digitalhub_core-0.5.0b2/digitalhub_core/client/objects/dhcore.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/client/objects/local.py` & `digitalhub_core-0.5.0b2/digitalhub_core/client/objects/local.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/context/builder.py` & `digitalhub_core-0.5.0b2/digitalhub_core/context/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/context/context.py` & `digitalhub_core-0.5.0b2/digitalhub_core/context/context.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/entities/_base/base.py` & `digitalhub_core-0.5.0b2/digitalhub_core/entities/_base/base.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/entities/_base/entity.py` & `digitalhub_core-0.5.0b2/digitalhub_core/entities/_base/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/entities/_base/metadata.py` & `digitalhub_core-0.5.0b2/digitalhub_core/entities/_base/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/entities/_base/spec.py` & `digitalhub_core-0.5.0b2/digitalhub_core/entities/_base/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/entities/_base/status.py` & `digitalhub_core-0.5.0b2/digitalhub_core/entities/_base/status.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/entities/_builders/metadata.py` & `digitalhub_core-0.5.0b2/digitalhub_core/entities/_builders/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/entities/_builders/spec.py` & `digitalhub_core-0.5.0b2/digitalhub_core/entities/_builders/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/entities/_builders/status.py` & `digitalhub_core-0.5.0b2/digitalhub_core/entities/_builders/status.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/entities/artifacts/crud.py` & `digitalhub_core-0.5.0b2/digitalhub_core/entities/artifacts/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/entities/artifacts/entity.py` & `digitalhub_core-0.5.0b2/digitalhub_core/entities/artifacts/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/entities/artifacts/spec.py` & `digitalhub_core-0.5.0b2/digitalhub_core/entities/artifacts/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/entities/functions/crud.py` & `digitalhub_core-0.5.0b2/digitalhub_core/entities/functions/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/entities/functions/entity.py` & `digitalhub_core-0.5.0b2/digitalhub_core/entities/functions/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/entities/functions/spec.py` & `digitalhub_core-0.5.0b2/digitalhub_core/entities/functions/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/entities/projects/crud.py` & `digitalhub_core-0.5.0b2/digitalhub_core/entities/projects/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/entities/projects/entity.py` & `digitalhub_core-0.5.0b2/digitalhub_core/entities/projects/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/entities/projects/spec.py` & `digitalhub_core-0.5.0b2/digitalhub_core/entities/projects/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/entities/registries.py` & `digitalhub_core-0.5.0b2/digitalhub_core/entities/registries.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/entities/runs/crud.py` & `digitalhub_core-0.5.0b2/digitalhub_core/entities/runs/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/entities/runs/entity.py` & `digitalhub_core-0.5.0b2/digitalhub_core/entities/runs/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/entities/runs/spec.py` & `digitalhub_core-0.5.0b2/digitalhub_core/entities/runs/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/entities/runs/status.py` & `digitalhub_core-0.5.0b2/digitalhub_core/entities/runs/status.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,22 +24,25 @@
 
     def __init__(
         self,
         state: str,
         message: str | None = None,
         outputs: list | None = None,
         results: dict | None = None,
+        **kwargs,
     ) -> None:
         """
         Constructor.
         """
         super().__init__(state, message)
         self.outputs = outputs
         self.results = results
 
+        self._any_setter(**kwargs)
+
     def get_results(self) -> dict:
         """
         Get results.
 
         Returns
         -------
         dict
```

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/entities/secrets/crud.py` & `digitalhub_core-0.5.0b2/digitalhub_core/entities/secrets/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/entities/secrets/entity.py` & `digitalhub_core-0.5.0b2/digitalhub_core/entities/secrets/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/entities/secrets/spec.py` & `digitalhub_core-0.5.0b2/digitalhub_core/entities/secrets/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/entities/tasks/crud.py` & `digitalhub_core-0.5.0b2/digitalhub_core/entities/tasks/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/entities/tasks/entity.py` & `digitalhub_core-0.5.0b2/digitalhub_core/entities/tasks/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/entities/tasks/models.py` & `digitalhub_core-0.5.0b2/digitalhub_core/entities/tasks/models.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/entities/workflows/crud.py` & `digitalhub_core-0.5.0b2/digitalhub_core/entities/workflows/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/entities/workflows/entity.py` & `digitalhub_core-0.5.0b2/digitalhub_core/entities/workflows/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/registry/models.py` & `digitalhub_core-0.5.0b2/digitalhub_core/registry/models.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/registry/registry.py` & `digitalhub_core-0.5.0b2/digitalhub_core/registry/registry.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/registry/utils.py` & `digitalhub_core-0.5.0b2/digitalhub_core/registry/utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/runtimes/base.py` & `digitalhub_core-0.5.0b2/digitalhub_core/runtimes/base.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/runtimes/builder.py` & `digitalhub_core-0.5.0b2/digitalhub_core/runtimes/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/stores/builder.py` & `digitalhub_core-0.5.0b2/digitalhub_core/stores/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/stores/objects/base.py` & `digitalhub_core-0.5.0b2/digitalhub_core/stores/objects/base.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/stores/objects/local.py` & `digitalhub_core-0.5.0b2/digitalhub_core/stores/objects/local.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 """
 Local store module.
 """
 from __future__ import annotations
 
 import shutil
-import typing
 from pathlib import Path
 
 from digitalhub_core.stores.objects.base import Store, StoreConfig
 
 
-
 class LocalStoreConfig(StoreConfig):
     """
     Local store configuration class.
     """
 
     path: str
     """Local path."""
```

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/stores/objects/remote.py` & `digitalhub_core-0.5.0b2/digitalhub_core/stores/objects/remote.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Remote store module.
 """
 from __future__ import annotations
 
-import typing
 from pathlib import Path
 
 import requests
 from digitalhub_core.stores.objects.base import Store, StoreConfig
 
 
 class RemoteStoreConfig(StoreConfig):
```

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/stores/objects/s3.py` & `digitalhub_core-0.5.0b2/digitalhub_core/stores/objects/s3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 """
 S3Store module.
 """
 from __future__ import annotations
 
-import typing
 from io import BytesIO
 from typing import Type
 from urllib.parse import urlparse
 
 import boto3
 import botocore.client  # pylint: disable=unused-import
 from botocore.exceptions import ClientError
 from digitalhub_core.stores.objects.base import Store, StoreConfig
 from digitalhub_core.utils.exceptions import StoreError
 
-
 # Type aliases
 S3Client = Type["botocore.client.S3"]
 
 
 class S3StoreConfig(StoreConfig):
     """
     S3 store configuration class.
```

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/stores/objects/sql.py` & `digitalhub_core-0.5.0b2/digitalhub_core/stores/objects/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """
 SQLStore module.
 """
 from __future__ import annotations
 
 from pathlib import Path
-from typing import Any
 
 import pyarrow as pa
 import pyarrow.parquet as pq
 from digitalhub_core.stores.objects.base import Store, StoreConfig
 from digitalhub_core.utils.exceptions import StoreError
-from sqlalchemy import create_engine, Table, MetaData
+from sqlalchemy import MetaData, Table, create_engine
 from sqlalchemy.engine import Engine
-from sqlalchemy.exc import SQLAlchemyError
 from sqlalchemy.engine.row import LegacyRow
+from sqlalchemy.exc import SQLAlchemyError
 
 
 class SQLStoreConfig(StoreConfig):
     """
     SQL store configuration class.
     """
```

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/utils/api.py` & `digitalhub_core-0.5.0b2/digitalhub_core/utils/api.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/utils/env_utils.py` & `digitalhub_core-0.5.0b2/digitalhub_core/utils/env_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/utils/file_utils.py` & `digitalhub_core-0.5.0b2/digitalhub_core/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/utils/generic_utils.py` & `digitalhub_core-0.5.0b2/digitalhub_core/utils/generic_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/utils/git_utils.py` & `digitalhub_core-0.5.0b2/digitalhub_core/utils/git_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/utils/io_utils.py` & `digitalhub_core-0.5.0b2/digitalhub_core/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core/utils/uri_utils.py` & `digitalhub_core-0.5.0b2/digitalhub_core/utils/uri_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core.egg-info/PKG-INFO` & `digitalhub_core-0.5.0b2/digitalhub_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-core
-Version: 0.5.0b1
+Version: 0.5.0b2
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 License:                               Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `digitalhub_core-0.5.0b1/digitalhub_core.egg-info/SOURCES.txt` & `digitalhub_core-0.5.0b2/digitalhub_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.5.0b1/pyproject.toml` & `digitalhub_core-0.5.0b2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digitalhub-core"
-version = "0.5.0b1"
+version = "0.5.0b2"
 description = "Python SDK for DHCore"
 readme = "README.md"
 authors = [
     { name = "Fondazione Bruno Kessler", email = "dslab@fbk.eu" },
     { name = "Matteo Martini", email = "mmartini@fbk.eu" }
 ]
 license = { file = "LICENSE.txt" }
@@ -59,15 +59,15 @@
 [tool.ruff.extend-per-file-ignores]
 "__init__.py" = ["F401"]
 
 [tool.ruff.pydocstyle]
 convention = "numpy"
 
 [tool.bumpver]
-current_version = "0.5.0b1"
+current_version = "0.5.0b2"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = false
 tag             = false
 push            = false
 
 [tool.bumpver.file_patterns]
```

