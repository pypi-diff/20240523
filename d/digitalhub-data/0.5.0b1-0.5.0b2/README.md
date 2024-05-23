# Comparing `tmp/digitalhub_data-0.5.0b1.tar.gz` & `tmp/digitalhub_data-0.5.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalhub_data-0.5.0b1.tar", last modified: Tue May 21 15:54:06 2024, max compression
+gzip compressed data, was "digitalhub_data-0.5.0b2.tar", last modified: Thu May 23 14:03:28 2024, max compression
```

## Comparing `digitalhub_data-0.5.0b1.tar` & `digitalhub_data-0.5.0b2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:54:06.158311 digitalhub_data-0.5.0b1/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)     1024 2024-05-21 15:54:06.158311 digitalhub_data-0.5.0b1/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      468 2024-04-23 09:36:04.000000 digitalhub_data-0.5.0b1/README.md
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:54:06.150311 digitalhub_data-0.5.0b1/digitalhub_data/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      329 2024-05-21 13:14:46.000000 digitalhub_data-0.5.0b1/digitalhub_data/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:54:06.150311 digitalhub_data-0.5.0b1/digitalhub_data/datastores/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 09:37:15.000000 digitalhub_data-0.5.0b1/digitalhub_data/datastores/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3283 2024-05-21 13:54:52.000000 digitalhub_data-0.5.0b1/digitalhub_data/datastores/builder.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:54:06.154312 digitalhub_data-0.5.0b1/digitalhub_data/datastores/objects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 09:37:57.000000 digitalhub_data-0.5.0b1/digitalhub_data/datastores/objects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3442 2024-05-21 14:03:19.000000 digitalhub_data-0.5.0b1/digitalhub_data/datastores/objects/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1507 2024-05-21 13:34:40.000000 digitalhub_data-0.5.0b1/digitalhub_data/datastores/objects/local.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      826 2024-05-21 13:34:45.000000 digitalhub_data-0.5.0b1/digitalhub_data/datastores/objects/remote.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1353 2024-05-21 13:34:51.000000 digitalhub_data-0.5.0b1/digitalhub_data/datastores/objects/s3.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2016 2024-05-21 13:34:58.000000 digitalhub_data-0.5.0b1/digitalhub_data/datastores/objects/sql.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:54:06.154312 digitalhub_data-0.5.0b1/digitalhub_data/entities/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:56.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:54:06.154312 digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:45.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3322 2024-05-21 13:14:46.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/builder.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6484 2024-05-21 13:14:46.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/crud.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:54:06.158311 digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/entity/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-03-04 14:42:21.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/entity/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6975 2024-05-21 13:14:46.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/entity/_base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      180 2024-03-15 13:13:54.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/entity/dataitem.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      142 2024-03-04 15:16:25.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/entity/iceberg.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2972 2024-05-21 13:35:17.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/entity/table.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      582 2024-04-23 09:36:04.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1093 2024-04-08 13:12:06.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1418 2024-04-08 13:12:04.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      863 2024-03-15 12:04:24.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/status.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      415 2024-05-06 11:22:14.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/entity_types.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:54:06.158311 digitalhub_data-0.5.0b1/digitalhub_data/entities/projects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-31 10:03:33.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/projects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6053 2024-05-21 13:14:46.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/projects/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6000 2024-05-21 13:14:46.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/projects/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      950 2024-02-15 10:15:41.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/projects/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      773 2024-05-06 11:19:40.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/registries.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:54:06.158311 digitalhub_data-0.5.0b1/digitalhub_data/entities/runs/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-22 14:51:32.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/runs/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-03-07 13:39:55.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/runs/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      407 2024-03-08 13:54:39.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/runs/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      351 2024-03-14 13:46:16.000000 digitalhub_data-0.5.0b1/digitalhub_data/entities/runs/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:54:06.158311 digitalhub_data-0.5.0b1/digitalhub_data/readers/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 09:54:41.000000 digitalhub_data-0.5.0b1/digitalhub_data/readers/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1148 2024-05-21 12:30:09.000000 digitalhub_data-0.5.0b1/digitalhub_data/readers/builder.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:54:06.158311 digitalhub_data-0.5.0b1/digitalhub_data/readers/objects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 10:51:19.000000 digitalhub_data-0.5.0b1/digitalhub_data/readers/objects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      667 2024-05-21 13:09:30.000000 digitalhub_data-0.5.0b1/digitalhub_data/readers/objects/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1902 2024-05-21 13:14:39.000000 digitalhub_data-0.5.0b1/digitalhub_data/readers/objects/pandas.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      278 2024-05-21 12:28:44.000000 digitalhub_data-0.5.0b1/digitalhub_data/readers/registry.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:54:06.158311 digitalhub_data-0.5.0b1/digitalhub_data/utils/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-29 10:07:05.000000 digitalhub_data-0.5.0b1/digitalhub_data/utils/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2440 2024-02-05 09:25:21.000000 digitalhub_data-0.5.0b1/digitalhub_data/utils/data_utils.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 15:54:06.158311 digitalhub_data-0.5.0b1/digitalhub_data.egg-info/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)     1024 2024-05-21 15:54:06.000000 digitalhub_data-0.5.0b1/digitalhub_data.egg-info/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1918 2024-05-21 15:54:06.000000 digitalhub_data-0.5.0b1/digitalhub_data.egg-info/SOURCES.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-21 15:54:06.000000 digitalhub_data-0.5.0b1/digitalhub_data.egg-info/dependency_links.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       52 2024-05-21 15:54:06.000000 digitalhub_data-0.5.0b1/digitalhub_data.egg-info/requires.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-05-21 15:54:06.000000 digitalhub_data-0.5.0b1/digitalhub_data.egg-info/top_level.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1130 2024-05-21 15:33:27.000000 digitalhub_data-0.5.0b1/pyproject.toml
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-21 15:54:06.158311 digitalhub_data-0.5.0b1/setup.cfg
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 14:03:28.993155 digitalhub_data-0.5.0b2/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)     1024 2024-05-23 14:03:28.993155 digitalhub_data-0.5.0b2/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      468 2024-04-23 09:36:04.000000 digitalhub_data-0.5.0b2/README.md
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 14:03:28.985155 digitalhub_data-0.5.0b2/digitalhub_data/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      329 2024-05-23 09:43:32.000000 digitalhub_data-0.5.0b2/digitalhub_data/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 14:03:28.985155 digitalhub_data-0.5.0b2/digitalhub_data/datastores/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 09:37:15.000000 digitalhub_data-0.5.0b2/digitalhub_data/datastores/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3209 2024-05-23 09:43:05.000000 digitalhub_data-0.5.0b2/digitalhub_data/datastores/builder.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 14:03:28.985155 digitalhub_data-0.5.0b2/digitalhub_data/datastores/objects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 09:37:57.000000 digitalhub_data-0.5.0b2/digitalhub_data/datastores/objects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3443 2024-05-22 13:22:43.000000 digitalhub_data-0.5.0b2/digitalhub_data/datastores/objects/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1350 2024-05-23 09:43:30.000000 digitalhub_data-0.5.0b2/digitalhub_data/datastores/objects/local.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      667 2024-05-23 09:43:30.000000 digitalhub_data-0.5.0b2/digitalhub_data/datastores/objects/remote.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1202 2024-05-23 09:43:30.000000 digitalhub_data-0.5.0b2/digitalhub_data/datastores/objects/s3.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1863 2024-05-23 09:43:30.000000 digitalhub_data-0.5.0b2/digitalhub_data/datastores/objects/sql.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 14:03:28.985155 digitalhub_data-0.5.0b2/digitalhub_data/entities/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:56.000000 digitalhub_data-0.5.0b2/digitalhub_data/entities/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 14:03:28.989155 digitalhub_data-0.5.0b2/digitalhub_data/entities/dataitems/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:45.000000 digitalhub_data-0.5.0b2/digitalhub_data/entities/dataitems/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3322 2024-05-23 09:43:32.000000 digitalhub_data-0.5.0b2/digitalhub_data/entities/dataitems/builder.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6484 2024-05-23 09:43:32.000000 digitalhub_data-0.5.0b2/digitalhub_data/entities/dataitems/crud.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 14:03:28.989155 digitalhub_data-0.5.0b2/digitalhub_data/entities/dataitems/entity/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-03-04 14:42:21.000000 digitalhub_data-0.5.0b2/digitalhub_data/entities/dataitems/entity/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6975 2024-05-23 09:43:32.000000 digitalhub_data-0.5.0b2/digitalhub_data/entities/dataitems/entity/_base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      180 2024-03-15 13:13:54.000000 digitalhub_data-0.5.0b2/digitalhub_data/entities/dataitems/entity/dataitem.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      142 2024-03-04 15:16:25.000000 digitalhub_data-0.5.0b2/digitalhub_data/entities/dataitems/entity/iceberg.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2958 2024-05-23 09:43:32.000000 digitalhub_data-0.5.0b2/digitalhub_data/entities/dataitems/entity/table.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      582 2024-04-23 09:36:04.000000 digitalhub_data-0.5.0b2/digitalhub_data/entities/dataitems/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1093 2024-04-08 13:12:06.000000 digitalhub_data-0.5.0b2/digitalhub_data/entities/dataitems/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1418 2024-04-08 13:12:04.000000 digitalhub_data-0.5.0b2/digitalhub_data/entities/dataitems/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      863 2024-03-15 12:04:24.000000 digitalhub_data-0.5.0b2/digitalhub_data/entities/dataitems/status.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      415 2024-05-06 11:22:14.000000 digitalhub_data-0.5.0b2/digitalhub_data/entities/entity_types.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 14:03:28.989155 digitalhub_data-0.5.0b2/digitalhub_data/entities/projects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-31 10:03:33.000000 digitalhub_data-0.5.0b2/digitalhub_data/entities/projects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6053 2024-05-23 09:43:32.000000 digitalhub_data-0.5.0b2/digitalhub_data/entities/projects/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6000 2024-05-23 09:43:32.000000 digitalhub_data-0.5.0b2/digitalhub_data/entities/projects/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      950 2024-02-15 10:15:41.000000 digitalhub_data-0.5.0b2/digitalhub_data/entities/projects/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      773 2024-05-06 11:19:40.000000 digitalhub_data-0.5.0b2/digitalhub_data/entities/registries.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 14:03:28.989155 digitalhub_data-0.5.0b2/digitalhub_data/entities/runs/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-22 14:51:32.000000 digitalhub_data-0.5.0b2/digitalhub_data/entities/runs/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-03-07 13:39:55.000000 digitalhub_data-0.5.0b2/digitalhub_data/entities/runs/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      407 2024-03-08 13:54:39.000000 digitalhub_data-0.5.0b2/digitalhub_data/entities/runs/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      351 2024-03-14 13:46:16.000000 digitalhub_data-0.5.0b2/digitalhub_data/entities/runs/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 14:03:28.989155 digitalhub_data-0.5.0b2/digitalhub_data/readers/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 09:54:41.000000 digitalhub_data-0.5.0b2/digitalhub_data/readers/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1148 2024-05-21 12:30:09.000000 digitalhub_data-0.5.0b2/digitalhub_data/readers/builder.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 14:03:28.989155 digitalhub_data-0.5.0b2/digitalhub_data/readers/objects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 10:51:19.000000 digitalhub_data-0.5.0b2/digitalhub_data/readers/objects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      667 2024-05-21 13:09:30.000000 digitalhub_data-0.5.0b2/digitalhub_data/readers/objects/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1902 2024-05-21 13:14:39.000000 digitalhub_data-0.5.0b2/digitalhub_data/readers/objects/pandas.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      358 2024-05-23 13:24:44.000000 digitalhub_data-0.5.0b2/digitalhub_data/readers/registry.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 14:03:28.989155 digitalhub_data-0.5.0b2/digitalhub_data/utils/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-29 10:07:05.000000 digitalhub_data-0.5.0b2/digitalhub_data/utils/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2440 2024-02-05 09:25:21.000000 digitalhub_data-0.5.0b2/digitalhub_data/utils/data_utils.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-23 14:03:28.989155 digitalhub_data-0.5.0b2/digitalhub_data.egg-info/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)     1024 2024-05-23 14:03:28.000000 digitalhub_data-0.5.0b2/digitalhub_data.egg-info/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1918 2024-05-23 14:03:28.000000 digitalhub_data-0.5.0b2/digitalhub_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-23 14:03:28.000000 digitalhub_data-0.5.0b2/digitalhub_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       52 2024-05-23 14:03:28.000000 digitalhub_data-0.5.0b2/digitalhub_data.egg-info/requires.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-05-23 14:03:28.000000 digitalhub_data-0.5.0b2/digitalhub_data.egg-info/top_level.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1130 2024-05-23 13:58:10.000000 digitalhub_data-0.5.0b2/pyproject.toml
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-23 14:03:28.993155 digitalhub_data-0.5.0b2/setup.cfg
```

### Comparing `digitalhub_data-0.5.0b1/PKG-INFO` & `digitalhub_data-0.5.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: digitalhub-data
-Version: 0.5.0b1
+Version: 0.5.0b2
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 Keywords: data,dataops,kubernetes
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: digitalhub-core==0.5.0b1
+Requires-Dist: digitalhub-core==0.5.0b2
 Provides-Extra: pandas
 Requires-Dist: pandas<2.2,>=1.2; extra == "pandas"
 
 # Digitalhub-data Library
 
 The Digitalhub-data SDK library is used to manage entities and executions in Digitalhub from Python.
 The Digitalhub-data layer is the second layer of the Digitalhub Data platform, focused on operations on data.
```

### Comparing `digitalhub_data-0.5.0b1/digitalhub_data/datastores/builder.py` & `digitalhub_data-0.5.0b2/digitalhub_data/datastores/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 from __future__ import annotations
 
 import typing
-from digitalhub_core.stores.builder import get_store, get_default_store
+
+from digitalhub_core.stores.builder import get_default_store, get_store
+from digitalhub_core.utils.uri_utils import map_uri_scheme
 from digitalhub_data.datastores.objects.local import LocalDatastore
 from digitalhub_data.datastores.objects.remote import RemoteDatastore
 from digitalhub_data.datastores.objects.s3 import S3Datastore
 from digitalhub_data.datastores.objects.sql import SqlDatastore
-from digitalhub_core.utils.exceptions import StoreError
-from digitalhub_core.utils.uri_utils import map_uri_scheme
-
 
 if typing.TYPE_CHECKING:
-    from digitalhub_data.datastores.objects.base import Datastore
     from digitalhub_core.stores.objects.base import Store
+    from digitalhub_data.datastores.objects.base import Datastore
 
 
-REGISTRY_DATASTORES = {
-    "local": LocalDatastore,
-    "remote": RemoteDatastore,
-    "s3": S3Datastore,
-    "sql": SqlDatastore
-}
+REGISTRY_DATASTORES = {"local": LocalDatastore, "remote": RemoteDatastore, "s3": S3Datastore, "sql": SqlDatastore}
+
 
 class DatastoreBuilder:
     """
     Datastore builder class.
     """
 
     def __init__(self) -> None:
@@ -126,15 +121,14 @@
     -------
     Datastore
         The datastore instance.
     """
     return builder.get(uri)
 
 
-
 def get_default_datastore() -> Datastore:
     """
     Get the default datastore instance.
 
     Returns
     -------
     Datastore
```

### Comparing `digitalhub_data-0.5.0b1/digitalhub_data/datastores/objects/base.py` & `digitalhub_data-0.5.0b2/digitalhub_data/datastores/objects/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     from digitalhub_core.stores.objects.base import Store
 
 
 class Datastore(metaclass=ABCMeta):
     """
     Datastore abstract class.
     """
+
     def __init__(self, store: Store, **kwargs) -> None:
         """
         Constructor.
         """
         self.store = store
 
     ############################
```

### Comparing `digitalhub_data-0.5.0b1/digitalhub_data/datastores/objects/local.py` & `digitalhub_data-0.5.0b2/digitalhub_data/datastores/objects/local.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 """
 Local datastore module.
 """
 from __future__ import annotations
 
-import typing
 from pathlib import Path
 from typing import Any
 
-from digitalhub_core.stores.builder import get_store
 from digitalhub_core.utils.generic_utils import build_uuid
 from digitalhub_data.datastores.objects.base import Datastore
 from digitalhub_data.readers.builder import get_reader_by_object
 
-if typing.TYPE_CHECKING:
-    from digitalhub_core.stores.objects.local import LocalStore
-
 
 class LocalDatastore(Datastore):
     """
     Local Datastore class.
     """
 
     def write_df(self, df: Any, dst: str | None = None, **kwargs) -> str:
```

### Comparing `digitalhub_data-0.5.0b1/digitalhub_data/datastores/objects/remote.py` & `digitalhub_data-0.5.0b2/digitalhub_data/datastores/objects/remote.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 """
 Remote datastore module.
 """
 from __future__ import annotations
 
-import typing
 from typing import Any
 
-from digitalhub_core.stores.builder import get_store
 from digitalhub_data.datastores.objects.base import Datastore
 
-if typing.TYPE_CHECKING:
-    from digitalhub_core.stores.objects.remote import RemoteStore
-
 
 class RemoteDatastore(Datastore):
     """
     Remote Datastore class.
     """
 
     def write_df(self, df: Any, dst: str | None = None, **kwargs) -> str:
```

### Comparing `digitalhub_data-0.5.0b1/digitalhub_data/datastores/objects/s3.py` & `digitalhub_data-0.5.0b2/digitalhub_data/datastores/objects/s3.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 """
 S3 datastore module.
 """
 from __future__ import annotations
 
-import typing
 from io import BytesIO
 from typing import Any
 
-from digitalhub_core.stores.builder import get_store
 from digitalhub_core.utils.exceptions import StoreError
 from digitalhub_data.datastores.objects.base import Datastore
 from digitalhub_data.readers.builder import get_reader_by_object
 
-if typing.TYPE_CHECKING:
-    from digitalhub_core.stores.objects.s3 import S3Store
-
 
 class S3Datastore(Datastore):
     """
     S3 Datastore class.
     """
 
     def write_df(self, df: Any, dst: str | None = None, **kwargs) -> str:
```

### Comparing `digitalhub_data-0.5.0b1/digitalhub_data/datastores/objects/sql.py` & `digitalhub_data-0.5.0b2/digitalhub_data/datastores/objects/sql.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 """
 Sql datastore module.
 """
 from __future__ import annotations
 
-import typing
 from typing import Any
 
 import pandas as pd
-from digitalhub_core.stores.builder import get_store
 from digitalhub_core.utils.generic_utils import build_uuid
 from digitalhub_data.datastores.objects.base import Datastore
 from digitalhub_data.readers.builder import get_reader_by_object
 
-if typing.TYPE_CHECKING:
-    from digitalhub_core.stores.objects.sql import SqlStore
-
 
 class SqlDatastore(Datastore):
     """
     Sql Datastore class.
     """
 
     def write_df(self, df: Any, dst: str | None = None, **kwargs) -> str:
```

### Comparing `digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/builder.py` & `digitalhub_data-0.5.0b2/digitalhub_data/entities/dataitems/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/crud.py` & `digitalhub_data-0.5.0b2/digitalhub_data/entities/dataitems/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/entity/_base.py` & `digitalhub_data-0.5.0b2/digitalhub_data/entities/dataitems/entity/_base.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/entity/table.py` & `digitalhub_data-0.5.0b2/digitalhub_data/entities/dataitems/entity/table.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 import shutil
-import typing
 from pathlib import Path
 from typing import Any
 
-from digitalhub_data.datastores.builder import get_default_datastore, get_datastore
+from digitalhub_data.datastores.builder import get_datastore, get_default_datastore
 from digitalhub_data.entities.dataitems.entity._base import Dataitem
 
 
 class DataitemTable(Dataitem):
 
     """
     Table dataitem.
```

### Comparing `digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/metadata.py` & `digitalhub_data-0.5.0b2/digitalhub_data/entities/dataitems/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/models.py` & `digitalhub_data-0.5.0b2/digitalhub_data/entities/dataitems/models.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/spec.py` & `digitalhub_data-0.5.0b2/digitalhub_data/entities/dataitems/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b1/digitalhub_data/entities/dataitems/status.py` & `digitalhub_data-0.5.0b2/digitalhub_data/entities/dataitems/status.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b1/digitalhub_data/entities/projects/crud.py` & `digitalhub_data-0.5.0b2/digitalhub_data/entities/projects/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b1/digitalhub_data/entities/projects/entity.py` & `digitalhub_data-0.5.0b2/digitalhub_data/entities/projects/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b1/digitalhub_data/entities/projects/spec.py` & `digitalhub_data-0.5.0b2/digitalhub_data/entities/projects/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b1/digitalhub_data/entities/registries.py` & `digitalhub_data-0.5.0b2/digitalhub_data/entities/registries.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b1/digitalhub_data/readers/builder.py` & `digitalhub_data-0.5.0b2/digitalhub_data/readers/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b1/digitalhub_data/readers/objects/base.py` & `digitalhub_data-0.5.0b2/digitalhub_data/readers/objects/base.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b1/digitalhub_data/readers/objects/pandas.py` & `digitalhub_data-0.5.0b2/digitalhub_data/readers/objects/pandas.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b1/digitalhub_data/utils/data_utils.py` & `digitalhub_data-0.5.0b2/digitalhub_data/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b1/digitalhub_data.egg-info/PKG-INFO` & `digitalhub_data-0.5.0b2/digitalhub_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: digitalhub-data
-Version: 0.5.0b1
+Version: 0.5.0b2
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 Keywords: data,dataops,kubernetes
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: digitalhub-core==0.5.0b1
+Requires-Dist: digitalhub-core==0.5.0b2
 Provides-Extra: pandas
 Requires-Dist: pandas<2.2,>=1.2; extra == "pandas"
 
 # Digitalhub-data Library
 
 The Digitalhub-data SDK library is used to manage entities and executions in Digitalhub from Python.
 The Digitalhub-data layer is the second layer of the Digitalhub Data platform, focused on operations on data.
```

### Comparing `digitalhub_data-0.5.0b1/digitalhub_data.egg-info/SOURCES.txt` & `digitalhub_data-0.5.0b2/digitalhub_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b1/pyproject.toml` & `digitalhub_data-0.5.0b2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digitalhub-data"
-version = "0.5.0b1"
+version = "0.5.0b2"
 description = "Python SDK for DHCore"
 readme = "README.md"
 authors = [
     { name = "Fondazione Bruno Kessler", email = "dslab@fbk.eu" },
     { name = "Matteo Martini", email = "mmartini@fbk.eu" }
 ]
 license = { file = "LICENSE.txt" }
@@ -16,26 +16,26 @@
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10"
 ]
 keywords = ["data", "dataops", "kubernetes"]
 requires-python = ">=3.9"
 dependencies = [
-    "digitalhub-core==0.5.0b1",
+    "digitalhub-core==0.5.0b2",
 ]
 [project.optional-dependencies]
 pandas = [
     "pandas>=1.2, <2.2",
 ]
 
 [tool.setuptools.packages.find]
 exclude = ["modules*"]
 
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
