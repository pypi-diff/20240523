# Comparing `tmp/meerschaum-2.2.0rc1.tar.gz` & `tmp/meerschaum-2.2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meerschaum-2.2.0rc1.tar", last modified: Thu May 16 05:35:41 2024, max compression
+gzip compressed data, was "meerschaum-2.2.0rc2.tar", last modified: Wed May 22 22:01:38 2024, max compression
```

## Comparing `meerschaum-2.2.0rc1.tar` & `meerschaum-2.2.0rc2.tar`

### file list

```diff
@@ -1,300 +1,301 @@
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.637744 meerschaum-2.2.0rc1/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11359 2021-12-27 13:50:47.000000 meerschaum-2.2.0rc1/LICENSE
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      114 2021-12-27 13:50:47.000000 meerschaum-2.2.0rc1/NOTICE
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23441 2024-05-16 05:35:41.637744 meerschaum-2.2.0rc1/PKG-INFO
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9183 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc1/README.md
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.588744 meerschaum-2.2.0rc1/meerschaum/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1487 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc1/meerschaum/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2763 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc1/meerschaum/__main__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.589744 meerschaum-2.2.0rc1/meerschaum/_internal/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      169 2022-04-23 01:15:00.000000 meerschaum-2.2.0rc1/meerschaum/_internal/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.589744 meerschaum-2.2.0rc1/meerschaum/_internal/arguments/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      519 2022-10-22 06:25:53.000000 meerschaum-2.2.0rc1/meerschaum/_internal/arguments/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10249 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/_internal/arguments/_parse_arguments.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13719 2024-05-07 20:25:34.000000 meerschaum-2.2.0rc1/meerschaum/_internal/arguments/_parser.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.589744 meerschaum-2.2.0rc1/meerschaum/_internal/docs/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      126 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/_internal/docs/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7076 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc1/meerschaum/_internal/docs/index.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4806 2024-05-15 15:21:26.000000 meerschaum-2.2.0rc1/meerschaum/_internal/entry.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.589744 meerschaum-2.2.0rc1/meerschaum/_internal/gui/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1313 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/_internal/gui/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.590744 meerschaum-2.2.0rc1/meerschaum/_internal/gui/app/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1565 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc1/meerschaum/_internal/gui/app/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2632 2022-10-18 06:13:35.000000 meerschaum-2.2.0rc1/meerschaum/_internal/gui/app/_windows.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      935 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/_internal/gui/app/actions.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1596 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/_internal/gui/app/pipes.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.590744 meerschaum-2.2.0rc1/meerschaum/_internal/shell/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    32826 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc1/meerschaum/_internal/shell/Shell.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3114 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc1/meerschaum/_internal/shell/ShellCompleter.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1280 2022-10-26 04:20:20.000000 meerschaum-2.2.0rc1/meerschaum/_internal/shell/ValidAutoSuggest.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      281 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc1/meerschaum/_internal/shell/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.590744 meerschaum-2.2.0rc1/meerschaum/_internal/shell/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc1/meerschaum/_internal/shell/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.591745 meerschaum-2.2.0rc1/meerschaum/_internal/term/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      520 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc1/meerschaum/_internal/term/TermPageHandler.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1594 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc1/meerschaum/_internal/term/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      716 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/_internal/term/tools.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.594744 meerschaum-2.2.0rc1/meerschaum/actions/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11360 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc1/meerschaum/actions/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12756 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc1/meerschaum/actions/api.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13396 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc1/meerschaum/actions/bootstrap.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4851 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/actions/clear.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6213 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/actions/copy.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1167 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/actions/deduplicate.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15528 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc1/meerschaum/actions/delete.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2453 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/actions/drop.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9487 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/actions/edit.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7431 2024-05-07 20:26:48.000000 meerschaum-2.2.0rc1/meerschaum/actions/install.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4206 2023-09-21 17:52:19.000000 meerschaum-2.2.0rc1/meerschaum/actions/login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2251 2022-08-29 21:54:10.000000 meerschaum-2.2.0rc1/meerschaum/actions/os.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3909 2023-11-13 21:37:33.000000 meerschaum-2.2.0rc1/meerschaum/actions/pause.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2395 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc1/meerschaum/actions/python.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11326 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc1/meerschaum/actions/register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      508 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc1/meerschaum/actions/reload.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3205 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/actions/setup.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2026 2022-08-29 21:54:10.000000 meerschaum-2.2.0rc1/meerschaum/actions/sh.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    28057 2024-05-16 03:38:37.000000 meerschaum-2.2.0rc1/meerschaum/actions/show.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4311 2023-10-27 06:03:46.000000 meerschaum-2.2.0rc1/meerschaum/actions/sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5886 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc1/meerschaum/actions/stack.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18384 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc1/meerschaum/actions/start.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4311 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/actions/stop.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    17518 2024-03-26 19:47:08.000000 meerschaum-2.2.0rc1/meerschaum/actions/sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3053 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc1/meerschaum/actions/tag.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6068 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/actions/uninstall.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6302 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/actions/upgrade.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4885 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/actions/verify.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.594744 meerschaum-2.2.0rc1/meerschaum/api/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7694 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc1/meerschaum/api/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      875 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc1/meerschaum/api/_chain.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1603 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/api/_events.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      961 2023-08-24 00:13:16.000000 meerschaum-2.2.0rc1/meerschaum/api/_oauth2.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1609 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc1/meerschaum/api/_websockets.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.595744 meerschaum-2.2.0rc1/meerschaum/api/dash/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2252 2024-03-20 22:38:46.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9418 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/actions.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.596744 meerschaum-2.2.0rc1/meerschaum/api/dash/assets/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/assets/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21923 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/assets/ansi_up.js
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)   338636 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/assets/banner_1920x320.png
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/assets/favicon.ico
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10218 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/assets/logo_48x48.png
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    67702 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/assets/logo_500x500.png
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.597744 meerschaum-2.2.0rc1/meerschaum/api/dash/callbacks/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      325 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/callbacks/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    32346 2024-05-10 18:44:59.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/callbacks/dashboard.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7689 2024-05-10 01:45:18.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/callbacks/jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2613 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/callbacks/login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2777 2022-07-26 06:45:25.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/callbacks/plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3600 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/callbacks/register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6364 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/components.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      843 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/connectors.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2046 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/graphs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7529 2024-05-10 02:30:25.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12591 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/keys.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.597744 meerschaum-2.2.0rc1/meerschaum/api/dash/pages/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      273 2023-07-21 01:07:38.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/pages/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3930 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/pages/dashboard.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      595 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/pages/error.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4600 2023-10-04 04:03:08.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/pages/login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1549 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/pages/plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2364 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/pages/register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18496 2024-05-10 18:08:18.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3115 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      504 2022-07-26 06:45:25.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2362 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      924 2022-10-31 13:18:31.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/websockets.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3298 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc1/meerschaum/api/dash/webterm.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.598744 meerschaum-2.2.0rc1/meerschaum/api/models/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      276 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/models/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      263 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/models/_interfaces.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      304 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/models/_locations.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      295 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/models/_metrics.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      463 2021-11-20 21:54:59.000000 meerschaum-2.2.0rc1/meerschaum/api/models/_pipes.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.598744 meerschaum-2.2.0rc1/meerschaum/api/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      115 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.598744 meerschaum-2.2.0rc1/meerschaum/api/resources/static/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/static/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.599744 meerschaum-2.2.0rc1/meerschaum/api/resources/static/css/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/static/css/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)   180286 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/static/css/bootstrap.min.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1714 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/static/css/dash.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6087 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/static/css/dbc_dark.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       81 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/static/css/styles.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5383 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/static/css/xterm.css
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.599744 meerschaum-2.2.0rc1/meerschaum/api/resources/static/ico/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/static/ico/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/static/ico/logo.ico
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.599744 meerschaum-2.2.0rc1/meerschaum/api/resources/static/js/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/static/js/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      540 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/static/js/action_button.js
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/static/js/main.js
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1729 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/static/js/terminado.js
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)   289441 2024-04-05 14:30:27.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/static/js/xterm.js
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.600744 meerschaum-2.2.0rc1/meerschaum/api/resources/static/png/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/static/png/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.600744 meerschaum-2.2.0rc1/meerschaum/api/resources/templates/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/templates/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1019 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/templates/index.html
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1711 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/templates/old_index.html
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      141 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/templates/secret.html
--rwxr-xr-x   0 bmeares   (1000) bmeares   (1000)     4443 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc1/meerschaum/api/resources/templates/termpage.html
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.601744 meerschaum-2.2.0rc1/meerschaum/api/routes/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      564 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/api/routes/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2022-06-27 01:07:31.000000 meerschaum-2.2.0rc1/meerschaum/api/routes/_actions.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1849 2023-10-04 04:03:08.000000 meerschaum-2.2.0rc1/meerschaum/api/routes/_connectors.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      578 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc1/meerschaum/api/routes/_index.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1935 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc1/meerschaum/api/routes/_login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2469 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/api/routes/_misc.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21677 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc1/meerschaum/api/routes/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6151 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/api/routes/_plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7204 2023-08-24 00:13:16.000000 meerschaum-2.2.0rc1/meerschaum/api/routes/_users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      825 2022-06-27 01:07:31.000000 meerschaum-2.2.0rc1/meerschaum/api/routes/_version.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3909 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc1/meerschaum/api/routes/_webterm.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.601744 meerschaum-2.2.0rc1/meerschaum/api/tables/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      482 2023-10-26 06:22:59.000000 meerschaum-2.2.0rc1/meerschaum/api/tables/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.603744 meerschaum-2.2.0rc1/meerschaum/config/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11517 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc1/meerschaum/config/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5184 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc1/meerschaum/config/_default.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8218 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc1/meerschaum/config/_edit.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4419 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc1/meerschaum/config/_environment.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6635 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc1/meerschaum/config/_formatting.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1073 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/config/_jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1526 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc1/meerschaum/config/_patch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7983 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc1/meerschaum/config/_paths.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1220 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc1/meerschaum/config/_preprocess.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14720 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/config/_read_config.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3551 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc1/meerschaum/config/_shell.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4120 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc1/meerschaum/config/_sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       74 2024-05-15 19:44:53.000000 meerschaum-2.2.0rc1/meerschaum/config/_version.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.603744 meerschaum-2.2.0rc1/meerschaum/config/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/config/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.603744 meerschaum-2.2.0rc1/meerschaum/config/stack/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9012 2024-05-10 20:46:41.000000 meerschaum-2.2.0rc1/meerschaum/config/stack/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.603744 meerschaum-2.2.0rc1/meerschaum/config/stack/grafana/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2010 2022-11-01 03:52:40.000000 meerschaum-2.2.0rc1/meerschaum/config/stack/grafana/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.603744 meerschaum-2.2.0rc1/meerschaum/config/stack/mosquitto/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      186 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/config/stack/mosquitto/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.603744 meerschaum-2.2.0rc1/meerschaum/config/stack/mosquitto/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/config/stack/mosquitto/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.603744 meerschaum-2.2.0rc1/meerschaum/config/stack/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/config/stack/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.603744 meerschaum-2.2.0rc1/meerschaum/config/static/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4361 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc1/meerschaum/config/static/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.604744 meerschaum-2.2.0rc1/meerschaum/connectors/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6381 2023-04-25 23:57:31.000000 meerschaum-2.2.0rc1/meerschaum/connectors/Connector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12023 2023-10-04 04:03:08.000000 meerschaum-2.2.0rc1/meerschaum/connectors/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.605744 meerschaum-2.2.0rc1/meerschaum/connectors/api/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4355 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc1/meerschaum/connectors/api/APIConnector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      205 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/connectors/api/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2755 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc1/meerschaum/connectors/api/_actions.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2072 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/connectors/api/_fetch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2050 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc1/meerschaum/connectors/api/_login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1093 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc1/meerschaum/connectors/api/_misc.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    20962 2023-11-10 05:44:22.000000 meerschaum-2.2.0rc1/meerschaum/connectors/api/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5217 2024-05-07 20:27:04.000000 meerschaum-2.2.0rc1/meerschaum/connectors/api/_plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6922 2023-10-04 04:03:08.000000 meerschaum-2.2.0rc1/meerschaum/connectors/api/_request.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1489 2022-07-25 06:37:48.000000 meerschaum-2.2.0rc1/meerschaum/connectors/api/_uri.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5275 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc1/meerschaum/connectors/api/_users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4044 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc1/meerschaum/connectors/parse.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.605744 meerschaum-2.2.0rc1/meerschaum/connectors/plugin/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2084 2022-10-25 06:38:00.000000 meerschaum-2.2.0rc1/meerschaum/connectors/plugin/PluginConnector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      198 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/connectors/plugin/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7363 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/connectors/poll.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.606744 meerschaum-2.2.0rc1/meerschaum/connectors/sql/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11522 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc1/meerschaum/connectors/sql/SQLConnector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      175 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc1/meerschaum/connectors/sql/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4123 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc1/meerschaum/connectors/sql/_cli.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10375 2024-03-26 20:20:31.000000 meerschaum-2.2.0rc1/meerschaum/connectors/sql/_create_engine.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13086 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc1/meerschaum/connectors/sql/_fetch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6447 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc1/meerschaum/connectors/sql/_instance.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)   100925 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc1/meerschaum/connectors/sql/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8323 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/connectors/sql/_plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34262 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc1/meerschaum/connectors/sql/_sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3460 2023-10-26 06:22:59.000000 meerschaum-2.2.0rc1/meerschaum/connectors/sql/_uri.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10100 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc1/meerschaum/connectors/sql/_users.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.606744 meerschaum-2.2.0rc1/meerschaum/connectors/sql/tables/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9001 2023-12-04 02:32:59.000000 meerschaum-2.2.0rc1/meerschaum/connectors/sql/tables/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1573 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc1/meerschaum/connectors/sql/tables/types.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      187 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc1/meerschaum/connectors/sql/tools.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.606744 meerschaum-2.2.0rc1/meerschaum/core/
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.608744 meerschaum-2.2.0rc1/meerschaum/core/Pipe/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    16230 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc1/meerschaum/core/Pipe/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13202 2023-04-26 08:12:59.000000 meerschaum-2.2.0rc1/meerschaum/core/Pipe/_attributes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7613 2023-04-25 23:57:31.000000 meerschaum-2.2.0rc1/meerschaum/core/Pipe/_bootstrap.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2261 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/core/Pipe/_clear.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    20880 2023-12-04 02:32:59.000000 meerschaum-2.2.0rc1/meerschaum/core/Pipe/_data.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10267 2023-11-13 06:20:00.000000 meerschaum-2.2.0rc1/meerschaum/core/Pipe/_deduplicate.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2118 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc1/meerschaum/core/Pipe/_delete.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1052 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/core/Pipe/_drop.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3694 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc1/meerschaum/core/Pipe/_dtypes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8471 2022-12-05 04:26:42.000000 meerschaum-2.2.0rc1/meerschaum/core/Pipe/_edit.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5234 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc1/meerschaum/core/Pipe/_fetch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2023-01-16 21:21:28.000000 meerschaum-2.2.0rc1/meerschaum/core/Pipe/_register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1352 2023-04-25 23:57:31.000000 meerschaum-2.2.0rc1/meerschaum/core/Pipe/_show.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    28038 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc1/meerschaum/core/Pipe/_sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14262 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc1/meerschaum/core/Pipe/_verify.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.608744 meerschaum-2.2.0rc1/meerschaum/core/Plugin/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      137 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc1/meerschaum/core/Plugin/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.608744 meerschaum-2.2.0rc1/meerschaum/core/User/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2448 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc1/meerschaum/core/User/_User.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      161 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc1/meerschaum/core/User/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      251 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc1/meerschaum/core/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.608744 meerschaum-2.2.0rc1/meerschaum/plugins/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34013 2024-05-07 20:28:41.000000 meerschaum-2.2.0rc1/meerschaum/plugins/_Plugin.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    20760 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc1/meerschaum/plugins/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.610744 meerschaum-2.2.0rc1/meerschaum/utils/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      612 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc1/meerschaum/utils/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11460 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc1/meerschaum/utils/_get_pipes.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.611744 meerschaum-2.2.0rc1/meerschaum/utils/daemon/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    33047 2024-05-16 05:26:37.000000 meerschaum-2.2.0rc1/meerschaum/utils/daemon/Daemon.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1813 2024-05-16 05:29:15.000000 meerschaum-2.2.0rc1/meerschaum/utils/daemon/FileDescriptorInterceptor.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    22775 2024-05-16 05:30:05.000000 meerschaum-2.2.0rc1/meerschaum/utils/daemon/RotatingFile.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8174 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc1/meerschaum/utils/daemon/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4330 2023-09-26 04:28:45.000000 meerschaum-2.2.0rc1/meerschaum/utils/daemon/_names.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    31955 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc1/meerschaum/utils/dataframe.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3690 2023-01-09 09:23:24.000000 meerschaum-2.2.0rc1/meerschaum/utils/debug.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.611744 meerschaum-2.2.0rc1/meerschaum/utils/dtypes/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6261 2024-03-26 20:33:15.000000 meerschaum-2.2.0rc1/meerschaum/utils/dtypes/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14638 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc1/meerschaum/utils/dtypes/sql.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.611744 meerschaum-2.2.0rc1/meerschaum/utils/formatting/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13778 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc1/meerschaum/utils/formatting/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3294 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/utils/formatting/_jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    19492 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc1/meerschaum/utils/formatting/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3096 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/utils/formatting/_pprint.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3677 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/utils/formatting/_shell.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3196 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc1/meerschaum/utils/interactive.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    43296 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc1/meerschaum/utils/misc.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1006 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc1/meerschaum/utils/networking.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.612744 meerschaum-2.2.0rc1/meerschaum/utils/packages/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    57032 2024-05-15 15:40:39.000000 meerschaum-2.2.0rc1/meerschaum/utils/packages/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7968 2024-05-16 05:34:17.000000 meerschaum-2.2.0rc1/meerschaum/utils/packages/_packages.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2540 2022-07-25 06:37:48.000000 meerschaum-2.2.0rc1/meerschaum/utils/packages/lazy_loader.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2655 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc1/meerschaum/utils/pool.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7098 2023-10-04 03:17:38.000000 meerschaum-2.2.0rc1/meerschaum/utils/process.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    16490 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/utils/prompt.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10020 2024-05-16 04:42:13.000000 meerschaum-2.2.0rc1/meerschaum/utils/schedule.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    46656 2023-12-04 02:32:59.000000 meerschaum-2.2.0rc1/meerschaum/utils/sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2472 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/meerschaum/utils/threading.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2807 2024-03-20 22:41:20.000000 meerschaum-2.2.0rc1/meerschaum/utils/typing.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.612744 meerschaum-2.2.0rc1/meerschaum/utils/venv/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3553 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc1/meerschaum/utils/venv/_Venv.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23183 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc1/meerschaum/utils/venv/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6535 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc1/meerschaum/utils/warnings.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3162 2023-01-09 09:23:24.000000 meerschaum-2.2.0rc1/meerschaum/utils/yaml.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.613744 meerschaum-2.2.0rc1/meerschaum.egg-info/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23441 2024-05-16 05:35:41.000000 meerschaum-2.2.0rc1/meerschaum.egg-info/PKG-INFO
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8458 2024-05-16 05:35:41.000000 meerschaum-2.2.0rc1/meerschaum.egg-info/SOURCES.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2024-05-16 05:35:41.000000 meerschaum-2.2.0rc1/meerschaum.egg-info/dependency_links.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       88 2024-05-16 05:35:41.000000 meerschaum-2.2.0rc1/meerschaum.egg-info/entry_points.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4726 2024-05-16 05:35:41.000000 meerschaum-2.2.0rc1/meerschaum.egg-info/requires.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       11 2024-05-16 05:35:41.000000 meerschaum-2.2.0rc1/meerschaum.egg-info/top_level.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2024-05-16 05:35:41.000000 meerschaum-2.2.0rc1/meerschaum.egg-info/zip-safe
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       38 2024-05-16 05:35:41.637744 meerschaum-2.2.0rc1/setup.cfg
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3254 2024-05-15 14:36:58.000000 meerschaum-2.2.0rc1/setup.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-16 05:35:41.613744 meerschaum-2.2.0rc1/tests/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3139 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc1/tests/test_deduplicate.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15351 2023-11-13 21:37:33.000000 meerschaum-2.2.0rc1/tests/test_pipes_dtypes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3646 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/tests/test_sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21818 2024-05-10 21:08:07.000000 meerschaum-2.2.0rc1/tests/test_sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      744 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/tests/test_users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3090 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc1/tests/test_verify.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.944576 meerschaum-2.2.0rc2/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11359 2021-12-27 13:50:47.000000 meerschaum-2.2.0rc2/LICENSE
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      114 2021-12-27 13:50:47.000000 meerschaum-2.2.0rc2/NOTICE
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23441 2024-05-22 22:01:38.944576 meerschaum-2.2.0rc2/PKG-INFO
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9183 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc2/README.md
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.887577 meerschaum-2.2.0rc2/meerschaum/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1487 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc2/meerschaum/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2763 2024-05-17 16:18:37.000000 meerschaum-2.2.0rc2/meerschaum/__main__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.888577 meerschaum-2.2.0rc2/meerschaum/_internal/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      169 2022-04-23 01:15:00.000000 meerschaum-2.2.0rc2/meerschaum/_internal/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.888577 meerschaum-2.2.0rc2/meerschaum/_internal/arguments/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      519 2022-10-22 06:25:53.000000 meerschaum-2.2.0rc2/meerschaum/_internal/arguments/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10249 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/_internal/arguments/_parse_arguments.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13719 2024-05-07 20:25:34.000000 meerschaum-2.2.0rc2/meerschaum/_internal/arguments/_parser.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.889577 meerschaum-2.2.0rc2/meerschaum/_internal/docs/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      126 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/_internal/docs/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7076 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc2/meerschaum/_internal/docs/index.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4806 2024-05-15 15:21:26.000000 meerschaum-2.2.0rc2/meerschaum/_internal/entry.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.889577 meerschaum-2.2.0rc2/meerschaum/_internal/gui/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1313 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc2/meerschaum/_internal/gui/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.889577 meerschaum-2.2.0rc2/meerschaum/_internal/gui/app/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1565 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc2/meerschaum/_internal/gui/app/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2632 2022-10-18 06:13:35.000000 meerschaum-2.2.0rc2/meerschaum/_internal/gui/app/_windows.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      935 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc2/meerschaum/_internal/gui/app/actions.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1596 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc2/meerschaum/_internal/gui/app/pipes.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.890576 meerschaum-2.2.0rc2/meerschaum/_internal/shell/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    32826 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc2/meerschaum/_internal/shell/Shell.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3114 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc2/meerschaum/_internal/shell/ShellCompleter.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1280 2022-10-26 04:20:20.000000 meerschaum-2.2.0rc2/meerschaum/_internal/shell/ValidAutoSuggest.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      281 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc2/meerschaum/_internal/shell/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.890576 meerschaum-2.2.0rc2/meerschaum/_internal/shell/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc2/meerschaum/_internal/shell/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.891577 meerschaum-2.2.0rc2/meerschaum/_internal/term/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      520 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc2/meerschaum/_internal/term/TermPageHandler.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1594 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc2/meerschaum/_internal/term/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      716 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc2/meerschaum/_internal/term/tools.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.894577 meerschaum-2.2.0rc2/meerschaum/actions/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11360 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc2/meerschaum/actions/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12756 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc2/meerschaum/actions/api.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13396 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc2/meerschaum/actions/bootstrap.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4851 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/actions/clear.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6213 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/actions/copy.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1167 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/actions/deduplicate.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15528 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc2/meerschaum/actions/delete.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2453 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/actions/drop.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9487 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/actions/edit.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7431 2024-05-07 20:26:48.000000 meerschaum-2.2.0rc2/meerschaum/actions/install.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4206 2023-09-21 17:52:19.000000 meerschaum-2.2.0rc2/meerschaum/actions/login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2251 2022-08-29 21:54:10.000000 meerschaum-2.2.0rc2/meerschaum/actions/os.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3909 2023-11-13 21:37:33.000000 meerschaum-2.2.0rc2/meerschaum/actions/pause.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2395 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc2/meerschaum/actions/python.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11326 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc2/meerschaum/actions/register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      508 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc2/meerschaum/actions/reload.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3205 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/actions/setup.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2026 2022-08-29 21:54:10.000000 meerschaum-2.2.0rc2/meerschaum/actions/sh.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    29016 2024-05-22 21:36:42.000000 meerschaum-2.2.0rc2/meerschaum/actions/show.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4311 2023-10-27 06:03:46.000000 meerschaum-2.2.0rc2/meerschaum/actions/sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5886 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc2/meerschaum/actions/stack.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18384 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc2/meerschaum/actions/start.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4311 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/actions/stop.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    17518 2024-03-26 19:47:08.000000 meerschaum-2.2.0rc2/meerschaum/actions/sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3053 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc2/meerschaum/actions/tag.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6068 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/actions/uninstall.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6302 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/actions/upgrade.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4885 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/actions/verify.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.895577 meerschaum-2.2.0rc2/meerschaum/api/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7694 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc2/meerschaum/api/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      875 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc2/meerschaum/api/_chain.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1603 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc2/meerschaum/api/_events.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      961 2023-08-24 00:13:16.000000 meerschaum-2.2.0rc2/meerschaum/api/_oauth2.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1609 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc2/meerschaum/api/_websockets.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.897576 meerschaum-2.2.0rc2/meerschaum/api/dash/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2252 2024-03-20 22:38:46.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9418 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/actions.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.898577 meerschaum-2.2.0rc2/meerschaum/api/dash/assets/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/assets/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21923 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/assets/ansi_up.js
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)   338636 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/assets/banner_1920x320.png
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/assets/favicon.ico
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10218 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/assets/logo_48x48.png
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    67702 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/assets/logo_500x500.png
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.899577 meerschaum-2.2.0rc2/meerschaum/api/dash/callbacks/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      325 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/callbacks/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    32283 2024-05-22 21:31:12.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/callbacks/dashboard.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7689 2024-05-10 01:45:18.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/callbacks/jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2613 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/callbacks/login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2777 2022-07-26 06:45:25.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/callbacks/plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3600 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/callbacks/register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6364 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/components.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      843 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/connectors.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2046 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/graphs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7529 2024-05-10 02:30:25.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12591 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/keys.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.899577 meerschaum-2.2.0rc2/meerschaum/api/dash/pages/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      273 2023-07-21 01:07:38.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/pages/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3930 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/pages/dashboard.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      595 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/pages/error.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4600 2023-10-04 04:03:08.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/pages/login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1549 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/pages/plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2364 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/pages/register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    19233 2024-05-17 02:49:16.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3662 2024-05-16 15:25:17.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      504 2022-07-26 06:45:25.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2362 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      924 2022-10-31 13:18:31.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/websockets.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3298 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc2/meerschaum/api/dash/webterm.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.900576 meerschaum-2.2.0rc2/meerschaum/api/models/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      276 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/models/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      263 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/models/_interfaces.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      304 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/models/_locations.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      295 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/models/_metrics.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      463 2021-11-20 21:54:59.000000 meerschaum-2.2.0rc2/meerschaum/api/models/_pipes.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.900576 meerschaum-2.2.0rc2/meerschaum/api/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      115 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.900576 meerschaum-2.2.0rc2/meerschaum/api/resources/static/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/static/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.901576 meerschaum-2.2.0rc2/meerschaum/api/resources/static/css/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/static/css/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)   180286 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/static/css/bootstrap.min.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1714 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/static/css/dash.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6087 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/static/css/dbc_dark.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       81 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/static/css/styles.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5383 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/static/css/xterm.css
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.901576 meerschaum-2.2.0rc2/meerschaum/api/resources/static/ico/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/static/ico/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/static/ico/logo.ico
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.902577 meerschaum-2.2.0rc2/meerschaum/api/resources/static/js/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/static/js/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      540 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/static/js/action_button.js
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/static/js/main.js
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1729 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/static/js/terminado.js
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)   289441 2024-04-05 14:30:27.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/static/js/xterm.js
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.902577 meerschaum-2.2.0rc2/meerschaum/api/resources/static/png/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/static/png/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.903576 meerschaum-2.2.0rc2/meerschaum/api/resources/templates/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/templates/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1019 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/templates/index.html
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1711 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/templates/old_index.html
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      141 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/templates/secret.html
+-rwxr-xr-x   0 bmeares   (1000) bmeares   (1000)     4527 2024-05-22 21:27:22.000000 meerschaum-2.2.0rc2/meerschaum/api/resources/templates/termpage.html
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.904576 meerschaum-2.2.0rc2/meerschaum/api/routes/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      564 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc2/meerschaum/api/routes/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2022-06-27 01:07:31.000000 meerschaum-2.2.0rc2/meerschaum/api/routes/_actions.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1849 2023-10-04 04:03:08.000000 meerschaum-2.2.0rc2/meerschaum/api/routes/_connectors.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      578 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc2/meerschaum/api/routes/_index.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1933 2024-05-22 19:54:14.000000 meerschaum-2.2.0rc2/meerschaum/api/routes/_login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2469 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc2/meerschaum/api/routes/_misc.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21677 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc2/meerschaum/api/routes/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6216 2024-05-16 15:09:58.000000 meerschaum-2.2.0rc2/meerschaum/api/routes/_plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7204 2023-08-24 00:13:16.000000 meerschaum-2.2.0rc2/meerschaum/api/routes/_users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      825 2022-06-27 01:07:31.000000 meerschaum-2.2.0rc2/meerschaum/api/routes/_version.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3909 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc2/meerschaum/api/routes/_webterm.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.904576 meerschaum-2.2.0rc2/meerschaum/api/tables/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      482 2023-10-26 06:22:59.000000 meerschaum-2.2.0rc2/meerschaum/api/tables/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.906576 meerschaum-2.2.0rc2/meerschaum/config/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11517 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc2/meerschaum/config/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      187 2024-05-16 15:33:56.000000 meerschaum-2.2.0rc2/meerschaum/config/_dash.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5251 2024-05-16 15:31:32.000000 meerschaum-2.2.0rc2/meerschaum/config/_default.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8218 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc2/meerschaum/config/_edit.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4419 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc2/meerschaum/config/_environment.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6635 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc2/meerschaum/config/_formatting.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1228 2024-05-17 21:01:54.000000 meerschaum-2.2.0rc2/meerschaum/config/_jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1526 2023-11-06 21:03:03.000000 meerschaum-2.2.0rc2/meerschaum/config/_patch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8064 2024-05-22 16:51:21.000000 meerschaum-2.2.0rc2/meerschaum/config/_paths.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1220 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc2/meerschaum/config/_preprocess.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14720 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/config/_read_config.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3551 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc2/meerschaum/config/_shell.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4155 2024-05-22 20:00:09.000000 meerschaum-2.2.0rc2/meerschaum/config/_sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       74 2024-05-22 16:51:34.000000 meerschaum-2.2.0rc2/meerschaum/config/_version.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.906576 meerschaum-2.2.0rc2/meerschaum/config/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/config/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.906576 meerschaum-2.2.0rc2/meerschaum/config/stack/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9007 2024-05-22 20:05:40.000000 meerschaum-2.2.0rc2/meerschaum/config/stack/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.906576 meerschaum-2.2.0rc2/meerschaum/config/stack/grafana/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2010 2024-05-22 20:11:13.000000 meerschaum-2.2.0rc2/meerschaum/config/stack/grafana/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.906576 meerschaum-2.2.0rc2/meerschaum/config/stack/mosquitto/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      186 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/config/stack/mosquitto/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.907576 meerschaum-2.2.0rc2/meerschaum/config/stack/mosquitto/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/config/stack/mosquitto/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.907576 meerschaum-2.2.0rc2/meerschaum/config/stack/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/config/stack/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.907576 meerschaum-2.2.0rc2/meerschaum/config/static/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4435 2024-05-22 19:41:39.000000 meerschaum-2.2.0rc2/meerschaum/config/static/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.907576 meerschaum-2.2.0rc2/meerschaum/connectors/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6381 2023-04-25 23:57:31.000000 meerschaum-2.2.0rc2/meerschaum/connectors/Connector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12023 2023-10-04 04:03:08.000000 meerschaum-2.2.0rc2/meerschaum/connectors/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.909577 meerschaum-2.2.0rc2/meerschaum/connectors/api/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4355 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc2/meerschaum/connectors/api/APIConnector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      205 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/connectors/api/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2755 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc2/meerschaum/connectors/api/_actions.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2072 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/connectors/api/_fetch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2050 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc2/meerschaum/connectors/api/_login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1093 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc2/meerschaum/connectors/api/_misc.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    20962 2023-11-10 05:44:22.000000 meerschaum-2.2.0rc2/meerschaum/connectors/api/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5217 2024-05-07 20:27:04.000000 meerschaum-2.2.0rc2/meerschaum/connectors/api/_plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6922 2023-10-04 04:03:08.000000 meerschaum-2.2.0rc2/meerschaum/connectors/api/_request.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1489 2022-07-25 06:37:48.000000 meerschaum-2.2.0rc2/meerschaum/connectors/api/_uri.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5275 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc2/meerschaum/connectors/api/_users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4044 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc2/meerschaum/connectors/parse.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.909577 meerschaum-2.2.0rc2/meerschaum/connectors/plugin/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2084 2022-10-25 06:38:00.000000 meerschaum-2.2.0rc2/meerschaum/connectors/plugin/PluginConnector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      198 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/connectors/plugin/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7363 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc2/meerschaum/connectors/poll.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.911576 meerschaum-2.2.0rc2/meerschaum/connectors/sql/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11522 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc2/meerschaum/connectors/sql/SQLConnector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      175 2021-11-08 16:07:48.000000 meerschaum-2.2.0rc2/meerschaum/connectors/sql/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4123 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc2/meerschaum/connectors/sql/_cli.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10375 2024-03-26 20:20:31.000000 meerschaum-2.2.0rc2/meerschaum/connectors/sql/_create_engine.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13086 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc2/meerschaum/connectors/sql/_fetch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6447 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc2/meerschaum/connectors/sql/_instance.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)   100925 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc2/meerschaum/connectors/sql/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8321 2024-05-16 15:18:16.000000 meerschaum-2.2.0rc2/meerschaum/connectors/sql/_plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34262 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc2/meerschaum/connectors/sql/_sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3460 2023-10-26 06:22:59.000000 meerschaum-2.2.0rc2/meerschaum/connectors/sql/_uri.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10100 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc2/meerschaum/connectors/sql/_users.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.911576 meerschaum-2.2.0rc2/meerschaum/connectors/sql/tables/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9001 2023-12-04 02:32:59.000000 meerschaum-2.2.0rc2/meerschaum/connectors/sql/tables/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1573 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc2/meerschaum/connectors/sql/tables/types.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      187 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc2/meerschaum/connectors/sql/tools.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.911576 meerschaum-2.2.0rc2/meerschaum/core/
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.913576 meerschaum-2.2.0rc2/meerschaum/core/Pipe/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    16230 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc2/meerschaum/core/Pipe/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13202 2023-04-26 08:12:59.000000 meerschaum-2.2.0rc2/meerschaum/core/Pipe/_attributes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7613 2023-04-25 23:57:31.000000 meerschaum-2.2.0rc2/meerschaum/core/Pipe/_bootstrap.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2261 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/core/Pipe/_clear.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    20880 2023-12-04 02:32:59.000000 meerschaum-2.2.0rc2/meerschaum/core/Pipe/_data.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10267 2023-11-13 06:20:00.000000 meerschaum-2.2.0rc2/meerschaum/core/Pipe/_deduplicate.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2118 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc2/meerschaum/core/Pipe/_delete.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1052 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/core/Pipe/_drop.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3694 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc2/meerschaum/core/Pipe/_dtypes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8471 2022-12-05 04:26:42.000000 meerschaum-2.2.0rc2/meerschaum/core/Pipe/_edit.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5234 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc2/meerschaum/core/Pipe/_fetch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2023-01-16 21:21:28.000000 meerschaum-2.2.0rc2/meerschaum/core/Pipe/_register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1352 2023-04-25 23:57:31.000000 meerschaum-2.2.0rc2/meerschaum/core/Pipe/_show.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    28038 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc2/meerschaum/core/Pipe/_sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14262 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc2/meerschaum/core/Pipe/_verify.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.913576 meerschaum-2.2.0rc2/meerschaum/core/Plugin/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      137 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc2/meerschaum/core/Plugin/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.914576 meerschaum-2.2.0rc2/meerschaum/core/User/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6456 2024-05-22 21:15:28.000000 meerschaum-2.2.0rc2/meerschaum/core/User/_User.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      193 2024-05-22 19:53:09.000000 meerschaum-2.2.0rc2/meerschaum/core/User/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      251 2022-04-24 10:29:36.000000 meerschaum-2.2.0rc2/meerschaum/core/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.914576 meerschaum-2.2.0rc2/meerschaum/plugins/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34039 2024-05-16 15:06:05.000000 meerschaum-2.2.0rc2/meerschaum/plugins/_Plugin.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    20760 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc2/meerschaum/plugins/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.916576 meerschaum-2.2.0rc2/meerschaum/utils/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      612 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc2/meerschaum/utils/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11460 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc2/meerschaum/utils/_get_pipes.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.917576 meerschaum-2.2.0rc2/meerschaum/utils/daemon/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    33728 2024-05-22 21:57:49.000000 meerschaum-2.2.0rc2/meerschaum/utils/daemon/Daemon.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3180 2024-05-22 17:22:17.000000 meerschaum-2.2.0rc2/meerschaum/utils/daemon/FileDescriptorInterceptor.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23376 2024-05-22 21:47:46.000000 meerschaum-2.2.0rc2/meerschaum/utils/daemon/RotatingFile.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8262 2024-05-16 15:03:42.000000 meerschaum-2.2.0rc2/meerschaum/utils/daemon/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4330 2023-09-26 04:28:45.000000 meerschaum-2.2.0rc2/meerschaum/utils/daemon/_names.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    31955 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc2/meerschaum/utils/dataframe.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3690 2023-01-09 09:23:24.000000 meerschaum-2.2.0rc2/meerschaum/utils/debug.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.917576 meerschaum-2.2.0rc2/meerschaum/utils/dtypes/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6261 2024-03-26 20:33:15.000000 meerschaum-2.2.0rc2/meerschaum/utils/dtypes/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14638 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc2/meerschaum/utils/dtypes/sql.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.918576 meerschaum-2.2.0rc2/meerschaum/utils/formatting/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13778 2023-11-26 03:23:44.000000 meerschaum-2.2.0rc2/meerschaum/utils/formatting/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3294 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/utils/formatting/_jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    19492 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc2/meerschaum/utils/formatting/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3096 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/utils/formatting/_pprint.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3677 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc2/meerschaum/utils/formatting/_shell.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3196 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc2/meerschaum/utils/interactive.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    43296 2024-01-08 03:48:33.000000 meerschaum-2.2.0rc2/meerschaum/utils/misc.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1006 2022-02-28 20:55:01.000000 meerschaum-2.2.0rc2/meerschaum/utils/networking.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.918576 meerschaum-2.2.0rc2/meerschaum/utils/packages/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    57032 2024-05-15 15:40:39.000000 meerschaum-2.2.0rc2/meerschaum/utils/packages/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7968 2024-05-16 05:34:17.000000 meerschaum-2.2.0rc2/meerschaum/utils/packages/_packages.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2540 2022-07-25 06:37:48.000000 meerschaum-2.2.0rc2/meerschaum/utils/packages/lazy_loader.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2655 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc2/meerschaum/utils/pool.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7098 2023-10-04 03:17:38.000000 meerschaum-2.2.0rc2/meerschaum/utils/process.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    16490 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/meerschaum/utils/prompt.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10020 2024-05-16 04:42:13.000000 meerschaum-2.2.0rc2/meerschaum/utils/schedule.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    46656 2023-12-04 02:32:59.000000 meerschaum-2.2.0rc2/meerschaum/utils/sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2489 2024-05-17 21:02:01.000000 meerschaum-2.2.0rc2/meerschaum/utils/threading.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2807 2024-03-20 22:41:20.000000 meerschaum-2.2.0rc2/meerschaum/utils/typing.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.918576 meerschaum-2.2.0rc2/meerschaum/utils/venv/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3553 2023-08-28 22:18:25.000000 meerschaum-2.2.0rc2/meerschaum/utils/venv/_Venv.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23183 2023-12-01 07:12:21.000000 meerschaum-2.2.0rc2/meerschaum/utils/venv/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6535 2023-08-24 14:21:38.000000 meerschaum-2.2.0rc2/meerschaum/utils/warnings.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3162 2023-01-09 09:23:24.000000 meerschaum-2.2.0rc2/meerschaum/utils/yaml.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.920576 meerschaum-2.2.0rc2/meerschaum.egg-info/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23441 2024-05-22 22:01:38.000000 meerschaum-2.2.0rc2/meerschaum.egg-info/PKG-INFO
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8485 2024-05-22 22:01:38.000000 meerschaum-2.2.0rc2/meerschaum.egg-info/SOURCES.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2024-05-22 22:01:38.000000 meerschaum-2.2.0rc2/meerschaum.egg-info/dependency_links.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       88 2024-05-22 22:01:38.000000 meerschaum-2.2.0rc2/meerschaum.egg-info/entry_points.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4726 2024-05-22 22:01:38.000000 meerschaum-2.2.0rc2/meerschaum.egg-info/requires.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       11 2024-05-22 22:01:38.000000 meerschaum-2.2.0rc2/meerschaum.egg-info/top_level.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2024-05-22 22:01:38.000000 meerschaum-2.2.0rc2/meerschaum.egg-info/zip-safe
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       38 2024-05-22 22:01:38.944576 meerschaum-2.2.0rc2/setup.cfg
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3254 2024-05-15 14:36:58.000000 meerschaum-2.2.0rc2/setup.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2024-05-22 22:01:38.920576 meerschaum-2.2.0rc2/tests/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3139 2023-11-13 16:31:14.000000 meerschaum-2.2.0rc2/tests/test_deduplicate.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15351 2023-11-13 21:37:33.000000 meerschaum-2.2.0rc2/tests/test_pipes_dtypes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3646 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/tests/test_sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21818 2024-05-10 21:08:07.000000 meerschaum-2.2.0rc2/tests/test_sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      744 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/tests/test_users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3090 2023-09-25 20:34:26.000000 meerschaum-2.2.0rc2/tests/test_verify.py
```

### Comparing `meerschaum-2.2.0rc1/LICENSE` & `meerschaum-2.2.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/PKG-INFO` & `meerschaum-2.2.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meerschaum
-Version: 2.2.0rc1
+Version: 2.2.0rc2
 Summary: Sync Time-Series Pipes with Meerschaum
 Home-page: https://meerschaum.io
 Author: Bennett Meares
 Author-email: bennett.meares@gmail.com
 Maintainer-email: bennett.meares@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://docs.meerschaum.io
```

### Comparing `meerschaum-2.2.0rc1/README.md` & `meerschaum-2.2.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/__init__.py` & `meerschaum-2.2.0rc2/meerschaum/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/__main__.py` & `meerschaum-2.2.0rc2/meerschaum/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! /usr/bin/env python
 # PYTHON_ARGCOMPLETE_OK
 # -*- coding: utf-8 -*-
 # vim:fenc=utf-8
 
 """
-Copyright 2021 Bennett Meares
+Copyright 2024 Bennett Meares
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `meerschaum-2.2.0rc1/meerschaum/_internal/arguments/__init__.py` & `meerschaum-2.2.0rc2/meerschaum/_internal/arguments/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/_internal/arguments/_parse_arguments.py` & `meerschaum-2.2.0rc2/meerschaum/_internal/arguments/_parse_arguments.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/_internal/arguments/_parser.py` & `meerschaum-2.2.0rc2/meerschaum/_internal/arguments/_parser.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/_internal/docs/index.py` & `meerschaum-2.2.0rc2/meerschaum/_internal/docs/index.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/_internal/entry.py` & `meerschaum-2.2.0rc2/meerschaum/_internal/entry.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/_internal/gui/__init__.py` & `meerschaum-2.2.0rc2/meerschaum/_internal/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/_internal/gui/app/__init__.py` & `meerschaum-2.2.0rc2/meerschaum/_internal/gui/app/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/_internal/gui/app/_windows.py` & `meerschaum-2.2.0rc2/meerschaum/_internal/gui/app/_windows.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/_internal/gui/app/actions.py` & `meerschaum-2.2.0rc2/meerschaum/_internal/gui/app/actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/_internal/gui/app/pipes.py` & `meerschaum-2.2.0rc2/meerschaum/_internal/gui/app/pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/_internal/shell/Shell.py` & `meerschaum-2.2.0rc2/meerschaum/_internal/shell/Shell.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/_internal/shell/ShellCompleter.py` & `meerschaum-2.2.0rc2/meerschaum/_internal/shell/ShellCompleter.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/_internal/shell/ValidAutoSuggest.py` & `meerschaum-2.2.0rc2/meerschaum/_internal/shell/ValidAutoSuggest.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/_internal/term/TermPageHandler.py` & `meerschaum-2.2.0rc2/meerschaum/_internal/term/TermPageHandler.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/_internal/term/__init__.py` & `meerschaum-2.2.0rc2/meerschaum/_internal/term/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/_internal/term/tools.py` & `meerschaum-2.2.0rc2/meerschaum/_internal/term/tools.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/actions/__init__.py` & `meerschaum-2.2.0rc2/meerschaum/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/actions/api.py` & `meerschaum-2.2.0rc2/meerschaum/actions/api.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/actions/bootstrap.py` & `meerschaum-2.2.0rc2/meerschaum/actions/bootstrap.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/actions/clear.py` & `meerschaum-2.2.0rc2/meerschaum/actions/clear.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/actions/copy.py` & `meerschaum-2.2.0rc2/meerschaum/actions/copy.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/actions/deduplicate.py` & `meerschaum-2.2.0rc2/meerschaum/actions/deduplicate.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/actions/delete.py` & `meerschaum-2.2.0rc2/meerschaum/actions/delete.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/actions/drop.py` & `meerschaum-2.2.0rc2/meerschaum/actions/drop.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/actions/edit.py` & `meerschaum-2.2.0rc2/meerschaum/actions/edit.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/actions/install.py` & `meerschaum-2.2.0rc2/meerschaum/actions/install.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/actions/login.py` & `meerschaum-2.2.0rc2/meerschaum/actions/login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/actions/os.py` & `meerschaum-2.2.0rc2/meerschaum/actions/os.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/actions/pause.py` & `meerschaum-2.2.0rc2/meerschaum/actions/pause.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/actions/python.py` & `meerschaum-2.2.0rc2/meerschaum/actions/python.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/actions/register.py` & `meerschaum-2.2.0rc2/meerschaum/actions/register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/actions/setup.py` & `meerschaum-2.2.0rc2/meerschaum/actions/setup.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/actions/sh.py` & `meerschaum-2.2.0rc2/meerschaum/actions/sh.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/actions/show.py` & `meerschaum-2.2.0rc2/meerschaum/actions/show.py`

 * *Files 3% similar despite different names*

```diff
@@ -574,100 +574,125 @@
     
     Usage:
         `show logs`
         `show logs --nopretty`
         `show logs myjob myotherjob`
     """
     import os, pathlib, random, asyncio
-    from datetime import datetime
+    from datetime import datetime, timezone
     from meerschaum.utils.packages import attempt_import, import_rich
     from meerschaum.utils.daemon import get_filtered_daemons, Daemon
     from meerschaum.utils.warnings import warn, info
     from meerschaum.utils.formatting import get_console, ANSI, UNICODE
     from meerschaum.utils.misc import tail
     from meerschaum.config._paths import LOGS_RESOURCES_PATH
     from meerschaum.config import get_config
     if not ANSI:
         info = print
     colors = get_config('jobs', 'logs', 'colors')
+    timestamp_format = get_config('jobs', 'logs', 'timestamp_format')
+    follow_timestamp_format = get_config('jobs', 'logs', 'follow_timestamp_format')
     daemons = get_filtered_daemons(action)
-
-    def _build_buffer_spaces(daemons) -> Dict[str, str]:
-        _max_len_id = max([len(d.daemon_id) for d in daemons]) if daemons else 0
-        _buffer_len = max(get_config('jobs', 'logs', 'min_buffer_len'), _max_len_id + 2)
+    now = datetime.now(timezone.utc)
+    now_str = now.strftime(timestamp_format)
+    now_follow_str = now.strftime(follow_timestamp_format)
+
+    def build_buffer_spaces(daemons) -> Dict[str, str]:
+        max_len_id = max(len(d.daemon_id) for d in daemons) if daemons else 0
+        buffer_len = max(
+            get_config('jobs', 'logs', 'min_buffer_len'),
+            max_len_id 
+        )
         return {
-            d.daemon_id: ''.join([' ' for i in range(_buffer_len - len(d.daemon_id))])
+            d.daemon_id: ''.join([' ' for i in range(buffer_len - len(d.daemon_id))])
             for d in daemons
         }
 
-    def _build_job_colors(daemons, _old_job_colors = None) -> Dict[str, str]:
+    def build_job_colors(daemons, _old_job_colors = None) -> Dict[str, str]:
         return {d.daemon_id: colors[i % len(colors)] for i, d in enumerate(daemons)}
 
-    _buffer_spaces = _build_buffer_spaces(daemons)
-    _job_colors = _build_job_colors(daemons)
+    buffer_spaces = build_buffer_spaces(daemons)
+    job_colors = build_job_colors(daemons)
 
-    def _get_buffer_spaces(daemon_id):
-        nonlocal _buffer_spaces, daemons
-        if daemon_id not in _buffer_spaces:
+    def get_buffer_spaces(daemon_id):
+        nonlocal buffer_spaces, daemons
+        if daemon_id not in buffer_spaces:
             d = Daemon(daemon_id=daemon_id)
             if d not in daemons:
                 daemons = get_filtered_daemons(action)
-            _buffer_spaces = _build_buffer_spaces(daemons)
-        return _buffer_spaces[daemon_id]
+            buffer_spaces = build_buffer_spaces(daemons)
+        return buffer_spaces[daemon_id] or ' '
 
-    def _get_job_colors(daemon_id):
-        nonlocal _job_colors, daemons
-        if daemon_id not in _job_colors:
+    def get_job_colors(daemon_id):
+        nonlocal job_colors, daemons
+        if daemon_id not in job_colors:
             d = Daemon(daemon_id=daemon_id)
             if d not in daemons:
                 daemons = get_filtered_daemons(action)
-            _job_colors = _build_job_colors(daemons)
-        return _job_colors[daemon_id]
+            job_colors = build_job_colors(daemons)
+        return job_colors[daemon_id]
 
-    def _follow_pretty_print():
+    def follow_pretty_print():
         watchfiles = attempt_import('watchfiles')
         rich = import_rich()
         rich_text = attempt_import('rich.text')
-        _watch_daemon_ids = {d.daemon_id: d for d in daemons}
+        watch_daemon_ids = {d.daemon_id: d for d in daemons}
         info("Watching log files...")
 
-        def _print_job_line(daemon, line):
-            date_prefix_str = line[:len('YYYY-MM-DD HH:mm')]
+        previous_line_timestamp = None
+        def print_job_line(daemon, line):
+            nonlocal previous_line_timestamp
+            date_prefix_str = line[:len(now_str)]
             try:
-                line_timestamp = datetime.fromisoformat(date_prefix_str)
+                line_timestamp = datetime.strptime(date_prefix_str, timestamp_format)
+                previous_line_timestamp = line_timestamp
             except Exception as e:
                 line_timestamp = None
             if line_timestamp:
-                line = line[len('YYYY-MM-DD HH:mm | '):]
-            if len(line) == 0:
+                line = line[(len(now_str) + 3):]
+            else:
+                line_timestamp = previous_line_timestamp
+
+            if len(line) == 0 or line == '\n':
                 return
+
             text = rich_text.Text(daemon.daemon_id)
-            text.append(
-                _get_buffer_spaces(daemon.daemon_id) + '| '
-                + (line[:-1] if line[-1] == '\n' else line)
+            line_prefix = (
+                get_buffer_spaces(daemon.daemon_id)
+                + (line_timestamp.strftime(follow_timestamp_format) if line_timestamp else '')
+                + ' | '
             )
+            text.append(line_prefix + (line[:-1] if line[-1] == '\n' else line))
             if ANSI:
                 text.stylize(
-                    _get_job_colors(daemon.daemon_id),
+                    get_job_colors(daemon.daemon_id),
                     0,
-                    len(daemon.daemon_id) + len(_get_buffer_spaces(daemon.daemon_id)) + 1
+                    len(daemon.daemon_id) + len(line_prefix)
                 )
             get_console().print(text)
 
 
-        def _print_log_lines(daemon):
+        def print_log_lines(daemon):
             for line in daemon.readlines():
-                _print_job_line(daemon, line)
+                print_job_line(daemon, line)
 
-        def _seek_back_offset(d) -> bool:
+        def seek_back_offset(d) -> bool:
             if d.log_offset_path.exists():
                 d.log_offset_path.unlink()
 
             latest_subfile_path = d.rotating_log.get_latest_subfile_path()
             latest_subfile_index = d.rotating_log.get_latest_subfile_index()
+
+            ### Sometimes the latest file is empty.
+            if os.stat(latest_subfile_path).st_size == 0 and latest_subfile_index > 0:
+                latest_subfile_index -= 1
+                latest_subfile_path = d.rotating_log.get_subfile_path_from_index(
+                    latest_subfile_index
+                )
+
             with open(latest_subfile_path, 'r', encoding='utf-8') as f:
                 latest_lines = f.readlines()
 
             lines_to_show = get_config('jobs', 'logs', 'lines_to_show')
             positions_to_rewind = len(''.join(latest_lines[(-1 * lines_to_show):]))
             backup_index = len(''.join(latest_lines)) - positions_to_rewind
 
@@ -679,54 +704,54 @@
             return True
 
         daemons_being_watched = {
             d.daemon_id: d
             for d in daemons
         }
         for d in daemons:
-            _seek_back_offset(d)
-            _print_log_lines(d)
+            seek_back_offset(d)
+            print_log_lines(d)
 
         _quit = False
-        def _watch_logs():
+        def watch_logs():
             for changes in watchfiles.watch(LOGS_RESOURCES_PATH):
                 if _quit:
                     return
                 for change in changes:
                     file_path_str = change[1]
                     if '.log' not in file_path_str or '.log.offset' in file_path_str:
                         continue
                     file_path = pathlib.Path(file_path_str)
                     if not file_path.exists():
                         continue
                     daemon_id = file_path.name.split('.log')[0]
-                    if daemon_id not in _watch_daemon_ids and action:
+                    if daemon_id not in watch_daemon_ids and action:
                         continue
                     try:
                         daemon = Daemon(daemon_id=daemon_id)
                     except Exception as e:
                         daemon = None
                         warn(f"Seeing new logs for non-existent job '{daemon_id}'.", stack=False)
 
                     if daemon is not None:
-                        _print_log_lines(daemon)
+                        print_log_lines(daemon)
 
         try:
-            _watch_logs()
+            watch_logs()
         except KeyboardInterrupt as ki:
             _quit = True
 
-    def _print_nopretty_log_text():
+    def print_nopretty_log_text():
         for d in daemons:
             log_text = d.log_text
             print(d.daemon_id)
             print(log_text)
 
-    _print_log_text = _follow_pretty_print if not nopretty else _print_nopretty_log_text
-    _print_log_text()
+    print_log_text = follow_pretty_print if not nopretty else print_nopretty_log_text
+    print_log_text()
 
     return True, "Success"
 
 
 def _show_environment(
         nopretty: bool = False,
         **kw
```

### Comparing `meerschaum-2.2.0rc1/meerschaum/actions/sql.py` & `meerschaum-2.2.0rc2/meerschaum/actions/sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/actions/stack.py` & `meerschaum-2.2.0rc2/meerschaum/actions/stack.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/actions/start.py` & `meerschaum-2.2.0rc2/meerschaum/actions/start.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/actions/stop.py` & `meerschaum-2.2.0rc2/meerschaum/actions/stop.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/actions/sync.py` & `meerschaum-2.2.0rc2/meerschaum/actions/sync.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/actions/tag.py` & `meerschaum-2.2.0rc2/meerschaum/actions/tag.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/actions/uninstall.py` & `meerschaum-2.2.0rc2/meerschaum/actions/uninstall.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/actions/upgrade.py` & `meerschaum-2.2.0rc2/meerschaum/actions/upgrade.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/actions/verify.py` & `meerschaum-2.2.0rc2/meerschaum/actions/verify.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/__init__.py` & `meerschaum-2.2.0rc2/meerschaum/api/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/_chain.py` & `meerschaum-2.2.0rc2/meerschaum/api/_chain.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/_events.py` & `meerschaum-2.2.0rc2/meerschaum/api/_events.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/_oauth2.py` & `meerschaum-2.2.0rc2/meerschaum/api/_oauth2.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/_websockets.py` & `meerschaum-2.2.0rc2/meerschaum/api/_websockets.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/dash/__init__.py` & `meerschaum-2.2.0rc2/meerschaum/api/dash/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/dash/actions.py` & `meerschaum-2.2.0rc2/meerschaum/api/dash/actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/dash/assets/ansi_up.js` & `meerschaum-2.2.0rc2/meerschaum/api/dash/assets/ansi_up.js`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/dash/assets/banner_1920x320.png` & `meerschaum-2.2.0rc2/meerschaum/api/dash/assets/banner_1920x320.png`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/dash/assets/favicon.ico` & `meerschaum-2.2.0rc2/meerschaum/api/dash/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/dash/assets/logo_48x48.png` & `meerschaum-2.2.0rc2/meerschaum/api/dash/assets/logo_48x48.png`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/dash/assets/logo_500x500.png` & `meerschaum-2.2.0rc2/meerschaum/api/dash/assets/logo_500x500.png`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/dash/callbacks/dashboard.py` & `meerschaum-2.2.0rc2/meerschaum/api/dash/callbacks/dashboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -436,26 +436,21 @@
         ]
         return dbc.Row(
             row_children,
             id = {'type': 'input-flags-row', 'index': index},
             className = 'input-text',
         )
 
+    remove_index = trigger_dict['index'] if trigger_type == 'input-flags-remove-button' else None
     rows = [
         build_row(i, val, val_text)
         for i, (val, val_text) in enumerate(zip(input_flags_dropdown_values, input_flags_texts))
+        if i != remove_index
     ]
 
-    if trigger_type == 'input-flags-remove-button':
-        remove_index = trigger_dict['index']
-        try:
-            del rows[remove_index]
-        except IndexError:
-            pass
-
     if not rows or input_flags_dropdown_values[-1]:
         rows.append(build_row(len(rows), None, None))
 
     return rows, build_flags_options()
 
 
 @dash_app.callback(
```

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/dash/callbacks/jobs.py` & `meerschaum-2.2.0rc2/meerschaum/api/dash/callbacks/jobs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/dash/callbacks/login.py` & `meerschaum-2.2.0rc2/meerschaum/api/dash/callbacks/login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/dash/callbacks/plugins.py` & `meerschaum-2.2.0rc2/meerschaum/api/dash/callbacks/plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/dash/callbacks/register.py` & `meerschaum-2.2.0rc2/meerschaum/api/dash/callbacks/register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/dash/components.py` & `meerschaum-2.2.0rc2/meerschaum/api/dash/components.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/dash/connectors.py` & `meerschaum-2.2.0rc2/meerschaum/api/dash/connectors.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/dash/graphs.py` & `meerschaum-2.2.0rc2/meerschaum/api/dash/graphs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/dash/jobs.py` & `meerschaum-2.2.0rc2/meerschaum/api/dash/jobs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/dash/keys.py` & `meerschaum-2.2.0rc2/meerschaum/api/dash/keys.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/dash/pages/dashboard.py` & `meerschaum-2.2.0rc2/meerschaum/api/dash/pages/dashboard.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/dash/pages/error.py` & `meerschaum-2.2.0rc2/meerschaum/api/dash/pages/error.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/dash/pages/login.py` & `meerschaum-2.2.0rc2/meerschaum/api/dash/pages/login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/dash/pages/plugins.py` & `meerschaum-2.2.0rc2/meerschaum/api/dash/pages/plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/dash/pages/register.py` & `meerschaum-2.2.0rc2/meerschaum/api/dash/pages/register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/dash/pipes.py` & `meerschaum-2.2.0rc2/meerschaum/api/dash/pipes.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from meerschaum.api import endpoints, CHECK_UPDATE
 from meerschaum.api.dash import (
     dash_app, debug, _get_pipes
 )
 from meerschaum.api.dash.connectors import get_web_connector
 from meerschaum.api.dash.components import alert_from_success_tuple
 from meerschaum.api.dash.users import is_session_authenticated
+from meerschaum.config import get_config
 import meerschaum as mrsm
 dbc = attempt_import('dash_bootstrap_components', lazy=False, check_update=CHECK_UPDATE)
 dash_ace = attempt_import('dash_ace', lazy=False, check_update=CHECK_UPDATE)
 html, dcc = import_html(check_update=CHECK_UPDATE), import_dcc(check_update=CHECK_UPDATE)
 humanfriendly = attempt_import('humanfriendly', check_update=CHECK_UPDATE)
 pd = import_pandas()
 
@@ -106,20 +107,24 @@
         - pipes as a list of cards
         - alert list
     """
     cards = []
     session_id = (session_data or {}).get('session-id', None)
     authenticated = is_session_authenticated(str(session_id))
 
-    _pipes = pipes_from_state(*keys, as_list=True)
-    alerts = [alert_from_success_tuple(_pipes)]
-    if not isinstance(_pipes, list):
-        _pipes = []
-    for p in _pipes:
-        meta_str = json.dumps(p.meta)
+    pipes = pipes_from_state(*keys, as_list=True)
+    alerts = [alert_from_success_tuple(pipes)]
+    if not isinstance(pipes, list):
+        pipes = []
+
+    max_num_pipes_cards = get_config('dash', 'max_num_pipes_cards')
+    overflow_pipes = pipes[max_num_pipes_cards:]
+
+    for pipe in pipes[:max_num_pipes_cards]:
+        meta_str = json.dumps(pipe.meta)
         footer_children = dbc.Row(
             [
                 dbc.Col(
                     (
                         dbc.DropdownMenu(
                             label = "Manage",
                             children = [
@@ -184,34 +189,53 @@
                     width = 4,
                 ),
             ],
             justify = 'start',
         )
         card_body_children = [
             html.H5(
-                html.B(str(p)),
+                html.B(str(pipe)),
                 className = 'card-title',
                 style = {'font-family': ['monospace']}
             ),
             html.Div(
                 dbc.Accordion(
-                    accordion_items_from_pipe(p, authenticated=authenticated),
+                    accordion_items_from_pipe(pipe, authenticated=authenticated),
                     flush = True,
                     start_collapsed = True,
                     id = {'type': 'pipe-accordion', 'index': meta_str},
                 )
             )
 
         ]
         cards.append(
-            dbc.Card(children=[
+            dbc.Card([
                 dbc.CardBody(children=card_body_children),
                 dbc.CardFooter(children=footer_children),
             ])
         )
+
+    if overflow_pipes:
+        cards.append(
+            dbc.Card([
+                dbc.CardBody(
+                    html.Ul(
+                        [
+                            html.Li(html.H5(
+                                html.B(str(pipe)),
+                                className = 'card-title',
+                                style = {'font-family': ['monospace']}
+                            ))
+                            for pipe in overflow_pipes
+                        ]
+                    )
+                )
+            ])
+        )
+
     return cards, alerts
 
 
 def accordion_items_from_pipe(
         pipe: mrsm.Pipe,
         active_items: Optional[List[str]] = None,
         authenticated: bool = False,
```

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/dash/plugins.py` & `meerschaum-2.2.0rc2/meerschaum/api/dash/plugins.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,41 +28,57 @@
     if session_data is None:
         session_data = {}
     for plugin_name in sorted(get_api_connector().get_plugins(search_term=search_term)):
         plugin = Plugin(plugin_name)
         desc = get_api_connector().get_plugin_attributes(plugin).get(
             'description', 'No description provided.'
         )
-        desc_textarea_kw = dict(
-            value=desc, readOnly=True, debounce=False, className='plugin-description',
-            draggable=False, wrap='overflow',
-            id={'type': 'description-textarea', 'index': plugin_name},
-        )
+        desc_textarea_kw = {
+            'value': desc,
+            'readOnly': True,
+            'debounce': False,
+            'className': 'plugin-description',
+            'draggable': False,
+            'wrap': 'overflow',
+            'placeholder': "Edit the plugin's description",
+            'id': {'type': 'description-textarea', 'index': plugin_name},
+        }
 
         card_body_children = [html.H4(plugin_name)]
 
         if is_plugin_owner(plugin_name, session_data):
             desc_textarea_kw['readOnly'] = False
-        card_body_children += [dbc.Textarea(**desc_textarea_kw)]
+        card_body_children.append(dbc.Textarea(**desc_textarea_kw))
         if not desc_textarea_kw['readOnly']:
             card_body_children += [
                 dbc.Button(
                     'Update description',
                     size="sm",
                     color="link",
                     id={'type': 'edit-button', 'index': plugin_name},
                 ),
                 html.Div(id={'type': 'edit-alert-div', 'index': plugin_name}),
             ]
-        _plugin_username = get_api_connector().get_plugin_username(plugin, debug=debug)
+        plugin_username = get_api_connector().get_plugin_username(plugin, debug=debug)
+        plugin_version = get_api_connector().get_plugin_version(plugin, debug=debug) or ' '
         card_children = [
-            dbc.CardHeader([html.A('👤 ' + str(_plugin_username), href='#')]),
+            dbc.CardHeader(
+                [
+                    dbc.Row(
+                        [
+                            dbc.Col(html.A('👤 ' + str(plugin_username), href='#')),
+                            dbc.Col(html.Pre(str(plugin_version), style={'text-align': 'right'})),
+                        ],
+                        justify = 'between',
+                    ),
+                ],
+            ),
             dbc.CardBody(card_body_children),
             dbc.CardFooter([
-                html.A('⬇️ Download source', href=(endpoints['plugins'] + '/' + plugin_name))
+                html.A('⬇️ Download', href=(endpoints['plugins'] + '/' + plugin_name))
             ]),
         ]
         cards.append(
             dbc.Card(card_children, id=plugin_name + '_card', className='plugin-card')
         )
     return cards, alerts
```

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/dash/users.py` & `meerschaum-2.2.0rc2/meerschaum/api/dash/users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/dash/websockets.py` & `meerschaum-2.2.0rc2/meerschaum/api/dash/websockets.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/dash/webterm.py` & `meerschaum-2.2.0rc2/meerschaum/api/dash/webterm.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/resources/static/css/bootstrap.min.css` & `meerschaum-2.2.0rc2/meerschaum/api/resources/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/resources/static/css/dash.css` & `meerschaum-2.2.0rc2/meerschaum/api/resources/static/css/dash.css`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/resources/static/css/dbc_dark.css` & `meerschaum-2.2.0rc2/meerschaum/api/resources/static/css/dbc_dark.css`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/resources/static/css/xterm.css` & `meerschaum-2.2.0rc2/meerschaum/api/resources/static/css/xterm.css`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/resources/static/ico/logo.ico` & `meerschaum-2.2.0rc2/meerschaum/api/resources/static/ico/logo.ico`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/resources/static/js/action_button.js` & `meerschaum-2.2.0rc2/meerschaum/api/resources/static/js/action_button.js`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/resources/static/js/terminado.js` & `meerschaum-2.2.0rc2/meerschaum/api/resources/static/js/terminado.js`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/resources/static/js/xterm.js` & `meerschaum-2.2.0rc2/meerschaum/api/resources/static/js/xterm.js`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/resources/templates/index.html` & `meerschaum-2.2.0rc2/meerschaum/api/resources/templates/index.html`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/resources/templates/old_index.html` & `meerschaum-2.2.0rc2/meerschaum/api/resources/templates/old_index.html`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/resources/templates/termpage.html` & `meerschaum-2.2.0rc2/meerschaum/api/resources/templates/termpage.html`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,17 @@
     }
     // NOTE: Input flags are not quoted to allow for multiple arguments.
     input_flags = event.data['input_flags'] ? event.data['input_flags'] : [];
     for (const [index, fl] of input_flags.entries()){
         if (!fl){ continue; }
         fl_val = event.data['input_flags_texts'][index];
         if (!fl_val){ continue; }
+        if (fl_val.includes(' ')){
+          fl_val = "'" + fl_val + "'";
+        }
         flags_str += " " + fl + " " + fl_val;
     }
 
     line = (
       "\x03"
       + action_str
       + connector_keys_str
```

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/routes/__init__.py` & `meerschaum-2.2.0rc2/meerschaum/api/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/routes/_actions.py` & `meerschaum-2.2.0rc2/meerschaum/api/routes/_actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/routes/_connectors.py` & `meerschaum-2.2.0rc2/meerschaum/api/routes/_connectors.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/routes/_index.py` & `meerschaum-2.2.0rc2/meerschaum/api/routes/_index.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/routes/_login.py` & `meerschaum-2.2.0rc2/meerschaum/api/routes/_login.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,27 +35,28 @@
     Login and set the session token.
     """
     username, password = (
         (data['username'], data['password']) if isinstance(data, dict)
         else (data.username, data.password)
     ) if not no_auth else ('no-auth', 'no-auth')
 
-    from meerschaum.core.User._User import get_pwd_context
+    from meerschaum.core.User._User import verify_password
     user = User(username, password)
-    correct_password = no_auth or get_pwd_context().verify(
-        password, get_api_connector().get_user_password_hash(user, debug=debug)
+    correct_password = no_auth or verify_password(
+        password,
+        get_api_connector().get_user_password_hash(user, debug=debug)
     )
     if not correct_password:
         raise InvalidCredentialsException
 
     expires_minutes = STATIC_CONFIG['api']['oauth']['token_expires_minutes']
     expires_delta = timedelta(minutes=expires_minutes)
     expires_dt = datetime.now(timezone.utc).replace(tzinfo=None) + expires_delta
     access_token = manager.create_access_token(
-        data = dict(sub=username),
+        data = {'sub': username},
         expires = expires_delta
     )
     return {
         'access_token': access_token,
         'token_type': 'bearer',
         'expires' : expires_dt,
     }
```

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/routes/_misc.py` & `meerschaum-2.2.0rc2/meerschaum/api/routes/_misc.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/routes/_pipes.py` & `meerschaum-2.2.0rc2/meerschaum/api/routes/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/routes/_plugins.py` & `meerschaum-2.2.0rc2/meerschaum/api/routes/_plugins.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,26 +86,29 @@
     if isinstance(attributes, str) and attributes[0] == '{':
         try:
             attributes = json.loads(attributes)
         except Exception as e:
             pass
 
     plugin = Plugin(name, version=version, attributes=attributes)
+    if curr_user is None:
+        return (
+            False,
+            "Cannot register a plugin without logging in (are you running with `--insecure`)?"
+        )
+
     if curr_user is not None:
         plugin_user_id = get_api_connector().get_plugin_user_id(plugin)
         curr_user_id = get_api_connector().get_user_id(curr_user) if curr_user is not None else -1
         if plugin_user_id is not None and plugin_user_id != curr_user_id:
             return False, f"User '{curr_user.username}' cannot edit plugin '{plugin}'."
         plugin.user_id = curr_user_id
-    else:
-        plugin.user_id = -1
 
     success, msg = get_api_connector().register_plugin(plugin, make_archive=False, debug=debug)
 
-    ### TODO delete and install new version of plugin on success
     if success:
         archive_path = plugin.archive_path
         temp_archive_path = pathlib.Path(str(archive_path) + '.tmp')
         with temp_archive_path.open('wb') as buff:
             shutil.copyfileobj(archive.file, buff)
         temp_archive_path.chmod(0o775)
         os.rename(temp_archive_path, archive_path)
```

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/routes/_users.py` & `meerschaum-2.2.0rc2/meerschaum/api/routes/_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/routes/_version.py` & `meerschaum-2.2.0rc2/meerschaum/api/routes/_version.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/api/routes/_webterm.py` & `meerschaum-2.2.0rc2/meerschaum/api/routes/_webterm.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/config/__init__.py` & `meerschaum-2.2.0rc2/meerschaum/config/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/config/_default.py` & `meerschaum-2.2.0rc2/meerschaum/config/_default.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,15 @@
             'default': connector_attributes['api']['default'],
             'main': {
                 'host': 'localhost',
                 'port': 8000,
             },
             'local': {
                 'host': 'localhost',
+                'port': 8000,
             },
             'mrsm': {
                 'host': 'api.mrsm.io',
                 'port': 443,
                 'protocol': 'https',
             },
         },
@@ -147,23 +148,24 @@
 default_config['formatting'] = default_formatting_config
 from meerschaum.config._shell import default_shell_config
 default_config['shell'] = default_shell_config
 default_config['pipes'] = default_pipes_config
 default_config['plugins'] = default_plugins_config
 from meerschaum.config._jobs import default_jobs_config
 default_config['jobs'] = default_jobs_config
-#  default_config['experimental'] = default_experimental_config
 ### add configs from other packages
 try:
     import meerschaum.config.stack
 except ImportError as e:
     pass
 finally:
     from meerschaum.config.stack import default_stack_config
 default_config['stack'] = default_stack_config
+from meerschaum.config._dash import default_dash_config
+default_config['dash'] = default_dash_config
 
 default_header_comment = """
 #####################################################################
 #                                                                   #
 #  Edit or add credentials for connectors.                          #
 #  You can read more about connectors at https://meerschaum.io.     #
 #                                                                   #
```

### Comparing `meerschaum-2.2.0rc1/meerschaum/config/_edit.py` & `meerschaum-2.2.0rc2/meerschaum/config/_edit.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/config/_environment.py` & `meerschaum-2.2.0rc2/meerschaum/config/_environment.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/config/_formatting.py` & `meerschaum-2.2.0rc2/meerschaum/config/_formatting.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/config/_jobs.py` & `meerschaum-2.2.0rc2/meerschaum/config/_jobs.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,21 +5,27 @@
 """
 Default configuration for jobs.
 """
 
 default_jobs_config = {
     'timeout_seconds': 8,
     'check_timeout_interval_seconds': 0.1,
-    'logs' : {
+    'terminal': {
+        'lines': 40,
+        'columns': 70,
+    },
+    'logs': {
         'num_files_to_keep': 5,
         'max_file_size': 100_000,
         'lines_to_show': 30,
-        'refresh_files_seconds': 5.0,
-        'min_buffer_len': 15,
-        'colors' : [
+        'refresh_files_seconds': 5,
+        'min_buffer_len': 10,
+        'timestamp_format': '%Y-%m-%d %H:%M',
+        'follow_timestamp_format': '%H:%M',
+        'colors': [
             'cyan',
             'magenta',
             'orange3',
             'green',
             'blue',
             'red',
             'spring_green3',
```

### Comparing `meerschaum-2.2.0rc1/meerschaum/config/_patch.py` & `meerschaum-2.2.0rc2/meerschaum/config/_patch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/config/_paths.py` & `meerschaum-2.2.0rc2/meerschaum/config/_paths.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,14 +149,15 @@
     'MOSQUITTO_RESOURCES_PATH'       : ('{STACK_RESOURCES_PATH}', 'mosquitto', 'resources'),
     'MOSQUITTO_CONFIG_PATH'          : ('{MOSQUITTO_RESOURCES_PATH}', 'mosquitto.conf'),
 
     'PORTABLE_CHECK_READLINE_PATH'   : ('{SHELL_RESOURCES_PATH}', '.readline_attempted_install'),
 
     'DAEMON_RESOURCES_PATH'          : ('{ROOT_DIR_PATH}', 'jobs'),
     'LOGS_RESOURCES_PATH'            : ('{ROOT_DIR_PATH}', 'logs'),
+    'DAEMON_ERROR_LOG_PATH'          : ('{ROOT_DIR_PATH}', 'daemon_errors.log'),
 }
 
 def set_root(root: Union[Path, str]):
     """Modify the value of `ROOT_DIR_PATH`."""
     paths['ROOT_DIR_PATH'] = Path(root).resolve()
     for path_name, path_parts in paths.items():
         if isinstance(path_parts, tuple) and path_parts[0] == '{ROOT_DIR_PATH}':
```

### Comparing `meerschaum-2.2.0rc1/meerschaum/config/_preprocess.py` & `meerschaum-2.2.0rc2/meerschaum/config/_preprocess.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/config/_read_config.py` & `meerschaum-2.2.0rc2/meerschaum/config/_read_config.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/config/_shell.py` & `meerschaum-2.2.0rc2/meerschaum/config/_shell.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/config/_sync.py` & `meerschaum-2.2.0rc2/meerschaum/config/_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     from meerschaum.config._read_config import search_and_substitute_config, get_keyfile_path
 
     def _read_yaml_config(path):
         """Read YAML file with header comment."""
         if not path.exists():
             return "", {}
         header_comment = ""
-        with open(path, 'r') as f:
+        with open(path, 'r', encoding='utf-8') as f:
             if _yaml is not None:
                 config = yaml.load(f)
             else:
                 print("PyYAML not installed!")
                 sys.exit(1)
             f.seek(0)
             for line in f:
@@ -80,15 +80,15 @@
     if replace_tuples:
         for replace_tuple in replace_tuples:
             new_config_text = new_config_text.replace(replace_tuple[0], replace_tuple[1])
     new_header = sub_header
     new_path = sub_path
 
     ### write changes
-    with open(new_path, 'w+') as f:
+    with open(new_path, 'w+', encoding='utf-8') as f:
         f.write(new_header)
         f.write(new_config_text)
     if permissions is not None:
         os.chmod(new_path, permissions)
 
 def sync_files(keys: Optional[List[str]] = None):
     if keys is None:
@@ -129,8 +129,7 @@
         'stack': _stack,
     }
     if keys is None:
         keys = list(key_functions.keys())
     for k in keys:
         if k in key_functions:
             key_functions[k]()
-
```

### Comparing `meerschaum-2.2.0rc1/meerschaum/config/stack/__init__.py` & `meerschaum-2.2.0rc2/meerschaum/config/stack/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 db_hostname = "db"
 db_host = 'MRSM{stack:' + str(STACK_COMPOSE_FILENAME) + ':services:db:hostname}'
 api_port = "MRSM{meerschaum:connectors:api:main:port}"
 api_host = "api"
 
 env_dict = {
     'COMPOSE_PROJECT_NAME' : 'mrsm',
-    'TIMESCALEDB_VERSION' : 'latest-pg15-oss',
+    'TIMESCALEDB_VERSION' : 'latest-pg16-oss',
     'POSTGRES_USER' : f'{db_user}',
     'POSTGRES_PASSWORD' : f'{db_pass}',
     'POSTGRES_DB' : f'{db_base}',
     'MEERSCHAUM_API_HOSTNAME' : f'{api_host}',
     'ALLOW_IP_RANGE' : '0.0.0.0/0',
     'MEERSCHAUM_API_CONFIG_RESOURCES' : '/meerschaum',
 }
@@ -228,34 +228,34 @@
         substitute = True,
     )
 
 NECESSARY_FILES = [STACK_COMPOSE_PATH, GRAFANA_DATASOURCE_PATH, GRAFANA_DASHBOARD_PATH]
 def get_necessary_files():
     from meerschaum.config import get_config
     return {
-        STACK_COMPOSE_PATH : (
+        STACK_COMPOSE_PATH: (
             get_config('stack', STACK_COMPOSE_FILENAME, substitute=True), compose_header
         ),
-        GRAFANA_DATASOURCE_PATH : get_config('stack', 'grafana', 'datasource', substitute=True),
-        GRAFANA_DASHBOARD_PATH : get_config('stack', 'grafana', 'dashboard', substitute=True),
+        GRAFANA_DATASOURCE_PATH: get_config('stack', 'grafana', 'datasource', substitute=True),
+        GRAFANA_DASHBOARD_PATH: get_config('stack', 'grafana', 'dashboard', substitute=True),
     }
 
 
 def write_stack(
         debug: bool = False 
     ):
     """Write Docker Compose configuration files."""
     from meerschaum.config._edit import general_write_yaml_config
     from meerschaum.config._sync import sync_files
     general_write_yaml_config(get_necessary_files(), debug=debug)
     return sync_files(['stack'])
    
 def edit_stack(
-        action : Optional[List[str]] = None,
-        debug : bool = False,
+        action: Optional[List[str]] = None,
+        debug: bool = False,
         **kw
     ):
     """Open docker-compose.yaml or .env for editing."""
     from meerschaum.config._edit import general_edit_config
     if action is None:
         action = []
     files = {
```

### Comparing `meerschaum-2.2.0rc1/meerschaum/config/stack/grafana/__init__.py` & `meerschaum-2.2.0rc2/meerschaum/config/stack/grafana/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     'apiVersion': 1,
     'datasources': [
         {
             'name': 'Meerschaum Main',
             'type': 'postgres',
             'jsonData': {
                 'sslmode': 'disable',
-                'postgresVersion': 1400,
+                'postgresVersion': 1500,
                 'timescaledb': True,
             },
             'user': db_user,
             'secureJsonData': {
                 'password': db_pass,
             },
             'database': db_base,
```

### Comparing `meerschaum-2.2.0rc1/meerschaum/config/static/__init__.py` & `meerschaum-2.2.0rc2/meerschaum/config/static/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,19 +99,21 @@
         'default_label': 'main',
     },
     'stack': {
         'dollar_standin': '<DOLLAR>', ### Temporary replacement for docker-compose.yaml.
     },
     'users': {
         'password_hash': {
+            'algorithm_name': 'sha256',
+            'salt_bytes': 16,
             'schemes': [
                 'pbkdf2_sha256',
             ],
             'default': 'pbkdf2_sha256',
-            'pbkdf2_sha256__default_rounds': 30000,
+            'pbkdf2_sha256__default_rounds': 3_000_000,
         },
         'min_username_length': 1,
         'max_username_length': 26,
         'min_password_length': 5,
     },
     'plugins': {
         'repo_separator': '@',
```

### Comparing `meerschaum-2.2.0rc1/meerschaum/connectors/Connector.py` & `meerschaum-2.2.0rc2/meerschaum/connectors/Connector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/connectors/__init__.py` & `meerschaum-2.2.0rc2/meerschaum/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/connectors/api/APIConnector.py` & `meerschaum-2.2.0rc2/meerschaum/connectors/api/APIConnector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/connectors/api/_actions.py` & `meerschaum-2.2.0rc2/meerschaum/connectors/api/_actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/connectors/api/_fetch.py` & `meerschaum-2.2.0rc2/meerschaum/connectors/api/_fetch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/connectors/api/_login.py` & `meerschaum-2.2.0rc2/meerschaum/connectors/api/_login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/connectors/api/_misc.py` & `meerschaum-2.2.0rc2/meerschaum/connectors/api/_misc.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/connectors/api/_pipes.py` & `meerschaum-2.2.0rc2/meerschaum/connectors/api/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/connectors/api/_plugins.py` & `meerschaum-2.2.0rc2/meerschaum/connectors/api/_plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/connectors/api/_request.py` & `meerschaum-2.2.0rc2/meerschaum/connectors/api/_request.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/connectors/api/_uri.py` & `meerschaum-2.2.0rc2/meerschaum/connectors/api/_uri.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/connectors/api/_users.py` & `meerschaum-2.2.0rc2/meerschaum/connectors/api/_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/connectors/parse.py` & `meerschaum-2.2.0rc2/meerschaum/connectors/parse.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/connectors/plugin/PluginConnector.py` & `meerschaum-2.2.0rc2/meerschaum/connectors/plugin/PluginConnector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/connectors/poll.py` & `meerschaum-2.2.0rc2/meerschaum/connectors/poll.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/connectors/sql/SQLConnector.py` & `meerschaum-2.2.0rc2/meerschaum/connectors/sql/SQLConnector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/connectors/sql/_cli.py` & `meerschaum-2.2.0rc2/meerschaum/connectors/sql/_cli.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/connectors/sql/_create_engine.py` & `meerschaum-2.2.0rc2/meerschaum/connectors/sql/_create_engine.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/connectors/sql/_fetch.py` & `meerschaum-2.2.0rc2/meerschaum/connectors/sql/_fetch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/connectors/sql/_instance.py` & `meerschaum-2.2.0rc2/meerschaum/connectors/sql/_instance.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/connectors/sql/_pipes.py` & `meerschaum-2.2.0rc2/meerschaum/connectors/sql/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/connectors/sql/_plugins.py` & `meerschaum-2.2.0rc2/meerschaum/connectors/sql/_plugins.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,17 +104,15 @@
     Return a plugin's version.
     """
     ### ensure plugins table exists
     from meerschaum.connectors.sql.tables import get_tables
     plugins_tbl = get_tables(mrsm_instance=self, debug=debug)['plugins']
     from meerschaum.utils.packages import attempt_import
     sqlalchemy = attempt_import('sqlalchemy')
-
     query = sqlalchemy.select(plugins_tbl.c.version).where(plugins_tbl.c.plugin_name == plugin.name)
-
     return self.value(query, debug=debug)
 
 def get_plugin_user_id(
         self,
         plugin: 'meerschaum.core.Plugin',
         debug: bool = False
     ) -> Optional[int]:
```

### Comparing `meerschaum-2.2.0rc1/meerschaum/connectors/sql/_sql.py` & `meerschaum-2.2.0rc2/meerschaum/connectors/sql/_sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/connectors/sql/_uri.py` & `meerschaum-2.2.0rc2/meerschaum/connectors/sql/_uri.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/connectors/sql/_users.py` & `meerschaum-2.2.0rc2/meerschaum/connectors/sql/_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/connectors/sql/tables/__init__.py` & `meerschaum-2.2.0rc2/meerschaum/connectors/sql/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/connectors/sql/tables/types.py` & `meerschaum-2.2.0rc2/meerschaum/connectors/sql/tables/types.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/core/Pipe/__init__.py` & `meerschaum-2.2.0rc2/meerschaum/core/Pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/core/Pipe/_attributes.py` & `meerschaum-2.2.0rc2/meerschaum/core/Pipe/_attributes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/core/Pipe/_bootstrap.py` & `meerschaum-2.2.0rc2/meerschaum/core/Pipe/_bootstrap.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/core/Pipe/_clear.py` & `meerschaum-2.2.0rc2/meerschaum/core/Pipe/_clear.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/core/Pipe/_data.py` & `meerschaum-2.2.0rc2/meerschaum/core/Pipe/_data.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/core/Pipe/_deduplicate.py` & `meerschaum-2.2.0rc2/meerschaum/core/Pipe/_deduplicate.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/core/Pipe/_delete.py` & `meerschaum-2.2.0rc2/meerschaum/core/Pipe/_delete.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/core/Pipe/_drop.py` & `meerschaum-2.2.0rc2/meerschaum/core/Pipe/_drop.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/core/Pipe/_dtypes.py` & `meerschaum-2.2.0rc2/meerschaum/core/Pipe/_dtypes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/core/Pipe/_edit.py` & `meerschaum-2.2.0rc2/meerschaum/core/Pipe/_edit.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/core/Pipe/_fetch.py` & `meerschaum-2.2.0rc2/meerschaum/core/Pipe/_fetch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/core/Pipe/_register.py` & `meerschaum-2.2.0rc2/meerschaum/core/Pipe/_register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/core/Pipe/_show.py` & `meerschaum-2.2.0rc2/meerschaum/core/Pipe/_show.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/core/Pipe/_sync.py` & `meerschaum-2.2.0rc2/meerschaum/core/Pipe/_sync.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/core/Pipe/_verify.py` & `meerschaum-2.2.0rc2/meerschaum/core/Pipe/_verify.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/plugins/_Plugin.py` & `meerschaum-2.2.0rc2/meerschaum/plugins/_Plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,15 @@
             '__pypackages__/',
             '.git',
         ]
 
         def parse_gitignore() -> 'Set[str]':
             gitignore_path = pathlib.Path(path) / '.gitignore'
             if not gitignore_path.exists():
-                return set()
+                return set(default_patterns_to_ignore)
             with open(gitignore_path, 'r', encoding='utf-8') as f:
                 gitignore_text = f.read()
             return set(pathspec.PathSpec.from_lines(
                 pathspec.patterns.GitWildMatchPattern,
                 default_patterns_to_ignore + gitignore_text.splitlines()
             ).match_tree(path))
```

### Comparing `meerschaum-2.2.0rc1/meerschaum/plugins/__init__.py` & `meerschaum-2.2.0rc2/meerschaum/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/utils/__init__.py` & `meerschaum-2.2.0rc2/meerschaum/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/utils/_get_pipes.py` & `meerschaum-2.2.0rc2/meerschaum/utils/_get_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/utils/daemon/Daemon.py` & `meerschaum-2.2.0rc2/meerschaum/utils/daemon/Daemon.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import pathlib
 import json
 import shutil
 import signal
 import sys
 import time
 import traceback
+from functools import partial
 from datetime import datetime, timezone
 from meerschaum.utils.typing import Optional, Dict, Any, SuccessTuple, Callable, List, Union
 from meerschaum.config import get_config
 from meerschaum.config._paths import DAEMON_RESOURCES_PATH, LOGS_RESOURCES_PATH
 from meerschaum.config._patch import apply_patch_to_config
 from meerschaum.utils.warnings import warn, error
 from meerschaum.utils.packages import attempt_import
@@ -135,19 +136,20 @@
             the last to finish will overwrite the output of the first.
 
         Returns
         -------
         Nothing — this will exit the parent process.
         """
         import platform, sys, os, traceback
-        from meerschaum.config._paths import LOGS_RESOURCES_PATH
+        from meerschaum.config._paths import DAEMON_ERROR_LOG_PATH
         from meerschaum.utils.warnings import warn
-        daemons_error_log_path = LOGS_RESOURCES_PATH / 'daemons_error.log'
-
+        from meerschaum.config import get_config
         daemon = attempt_import('daemon')
+        lines = get_config('jobs', 'terminal', 'lines')
+        columns = get_config('jobs','terminal', 'columns')
 
         if platform.system() == 'Windows':
             return False, "Windows is no longer supported."
 
         self._setup(allow_dirty_run)
 
         self._daemon_context = daemon.DaemonContext(
@@ -160,18 +162,22 @@
             signal_map = {
                 signal.SIGINT: self._handle_interrupt,
                 signal.SIGTERM: self._handle_sigterm,
             },
         )
 
         log_refresh_seconds = get_config('jobs', 'logs', 'refresh_files_seconds')
-        self._log_refresh_timer = RepeatTimer(log_refresh_seconds, self.rotating_log.refresh_files)
-
+        self._log_refresh_timer = RepeatTimer(
+            log_refresh_seconds,
+            partial(self.rotating_log.refresh_files, start_interception=True),
+        )
         try:
+            os.environ['LINES'], os.environ['COLUMNS'] = str(int(lines)), str(int(columns))
             with self._daemon_context:
+                self.rotating_log.refresh_files(start_interception=True)
                 try:
                     with open(self.pid_path, 'w+', encoding='utf-8') as f:
                         f.write(str(os.getpid()))
 
                     self._log_refresh_timer.start()
                     result = self.target(*self.target_args, **self.target_kw)
                     self.properties['result'] = result
@@ -188,19 +194,19 @@
                     self._capture_process_timestamp('ended')
                 else:
                     self.cleanup()
 
                 return result
         except Exception as e:
             daemon_error = traceback.format_exc()
-            with open(LOGS_RESOURCES_PATH, 'a+', encoding='utf-8') as f:
+            with open(DAEMON_ERROR_LOG_PATH, 'a+', encoding='utf-8') as f:
                 f.write(daemon_error)
 
         if daemon_error:
-            warn("Encountered an error while starting the daemon '{self}':\n{daemon_error}")
+            warn(f"Encountered an error while starting the daemon '{self}':\n{daemon_error}")
 
 
     def _capture_process_timestamp(
             self,
             process_key: str,
             write_properties: bool = True,
         ) -> None:
@@ -460,18 +466,17 @@
         if timer is not None:
             timer.cancel()
 
         daemon_context = self.__dict__.get('_daemon_context', None)
         if daemon_context is not None:
             daemon_context.close()
 
-        self.rotating_log.stop_log_fd_interception()
-
         _close_pools()
-        raise SystemExit(0)
+        self.rotating_log.stop_log_fd_interception()
+        raise KeyboardInterrupt()
 
 
     def _handle_sigterm(self, signal_number: int, stack_frame: 'frame') -> None:
         """
         Handle `SIGTERM` within the `Daemon` context.
         This method is injected into the `DaemonContext`.
         """
@@ -479,16 +484,14 @@
         if timer is not None:
             timer.cancel()
 
         daemon_context = self.__dict__.get('_daemon_context', None)
         if daemon_context is not None:
             daemon_context.close()
 
-        self.rotating_log.stop_log_fd_interception()
-
         _close_pools()
         raise SystemExit(1)
 
  
     def _send_signal(
             self,
             signal_to_send,
@@ -663,14 +666,15 @@
         if '_rotating_log' in self.__dict__:
             return self._rotating_log
 
         self._rotating_log = RotatingFile(
             self.log_path,
             redirect_streams = True,
             write_timestamps = True,
+            timestamp_format = get_config('jobs', 'logs', 'timestamp_format'),
         )
         return self._rotating_log
 
 
     @property
     def log_text(self) -> Optional[str]:
         """Read the log files and return their contents.
@@ -901,14 +905,21 @@
                 shutil.rmtree(self.path)
             except Exception as e:
                 msg = f"Failed to clean up '{self.daemon_id}':\n{e}"
                 warn(msg)
                 return False, msg
         if not keep_logs:
             self.rotating_log.delete()
+            try:
+                if self.log_offset_path.exists():
+                    self.log_offset_path.unlink()
+            except Exception as e:
+                msg = f"Failed to remove offset file for '{self.daemon_id}':\n{e}"
+                warn(msg)
+                return False, msg
         return True, "Success"
 
 
     def get_timeout_seconds(self, timeout: Union[int, float, None] = None) -> Union[int, float]:
         """
         Return the timeout value to use. Use `--timeout-seconds` if provided,
         else the configured default (8).
```

### Comparing `meerschaum-2.2.0rc1/meerschaum/utils/daemon/RotatingFile.py` & `meerschaum-2.2.0rc2/meerschaum/utils/daemon/RotatingFile.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     def __init__(
             self,
             file_path: pathlib.Path,
             num_files_to_keep: Optional[int] = None,
             max_file_size: Optional[int] = None,
             redirect_streams: bool = False,
             write_timestamps: bool = False,
-            timestamps_format: str = '%Y-%m-%d %H:%M | ',
+            timestamp_format: str = '%Y-%m-%d %H:%M',
         ):
         """
         Create a file-like object which manages other files.
 
         Parameters
         ----------
         num_files_to_keep: int, default None
@@ -74,15 +74,15 @@
         if max_file_size < 1:
             raise ValueError("Subfiles must contain at least one byte.")
 
         self.num_files_to_keep = num_files_to_keep
         self.max_file_size = max_file_size
         self.redirect_streams = redirect_streams
         self.write_timestamps = write_timestamps
-        self.timestamps_format = timestamps_format
+        self.timestamp_format = timestamp_format
         self.subfile_regex_pattern = re.compile(
             r'^'
             + self.file_path.name
             + r'(?:\.\d+)?$'
         )
 
         ### When subfiles are opened, map from their index to the file objects.
@@ -94,42 +94,22 @@
         ### When reading, keep track of the file index and position.
         self._cursor: Tuple[int, int] = (0, 0)
 
         ### Don't forget to close any stray files.
         atexit.register(self.close)
 
 
-
     def fileno(self):
         """
         Return the file descriptor for the latest subfile.
         """
-        import inspect
-        stack = inspect.stack()
-        parent_level = stack[1]
-        parent_module = parent_level[0].f_globals.get('__file__')
-        #  if parent_module.endswith('daemon.py'):
-            #  self._monkey_patch_os_write()
-        self.refresh_files()
+        self.refresh_files(start_interception=False)
         return self._current_file_obj.fileno()
 
 
-    def _monkey_patch_os_write(self):
-        import os
-        import sys
-        import pathlib
-        path = pathlib.Path('/home/bmeares/test1.log')
-        original_write = os.write
-        def intercept(*args, **kwargs):
-            with open(path, 'w', encoding='utf-8') as f:
-                f.write(str(args))
-            original_write(*args, **kwargs)
-        os.write = intercept
-
-
     def get_latest_subfile_path(self) -> pathlib.Path:
         """
         Return the path for the latest subfile to which to write into.
         """
         return self.get_subfile_path_from_index(
             self.get_latest_subfile_index()
         )
@@ -248,22 +228,29 @@
         )
         return [
             (self.file_path.parent / file_name)
             for file_name, _ in subfile_names_indices
         ]
 
 
-    def refresh_files(self, potential_new_len: int = 0) -> '_io.TextUIWrapper':
+    def refresh_files(
+            self,
+            potential_new_len: int = 0,
+            start_interception: bool = False,
+        ) -> '_io.TextUIWrapper':
         """
         Check the state of the subfiles.
         If the latest subfile is too large, create a new file and delete old ones.
 
         Parameters
         ----------
         potential_new_len: int, default 0
+
+        start_interception: bool, default False
+            If `True`, kick off the file interception threads.
         """
         self.flush()
 
         latest_subfile_index = self.get_latest_subfile_index()
         latest_subfile_path = self.get_subfile_path_from_index(latest_subfile_index)
 
         ### First run with existing log files: open the most recent log file.
@@ -274,18 +261,23 @@
             self._current_file_obj is not None
             and
             self.get_index_from_subfile_name(self._current_file_obj.name) == -1
         )
         if is_first_run_with_logs or lost_latest_handle:
             self._current_file_obj = open(latest_subfile_path, 'a+', encoding='utf-8')
             if self.redirect_streams:
-                self.stop_log_fd_interception()
-                daemon.daemon.redirect_stream(sys.stdout, self._current_file_obj)
-                daemon.daemon.redirect_stream(sys.stderr, self._current_file_obj)
-                self.start_log_fd_interception()
+                try:
+                    daemon.daemon.redirect_stream(sys.stdout, self._current_file_obj)
+                    daemon.daemon.redirect_stream(sys.stderr, self._current_file_obj)
+                except OSError as e:
+                    warn(
+                        f"Encountered an issue when redirecting streams:\n{traceback.format_exc()}"
+                    )
+                if start_interception:
+                    self.start_log_fd_interception()
 
         create_new_file = (
             (latest_subfile_index == -1)
             or
             self._current_file_obj is None
             or
             self.is_subfile_too_large(latest_subfile_index, potential_new_len)
@@ -298,65 +290,63 @@
             self._current_file_obj = open(new_file_path, 'a+', encoding='utf-8')
             self.subfile_objects[new_subfile_index] = self._current_file_obj
             self.flush()
 
             if self._previous_file_obj is not None:
                 if self.redirect_streams:
                     self._redirected_subfile_objects[old_subfile_index] = self._previous_file_obj
-                    self.stop_log_fd_interception()
                     daemon.daemon.redirect_stream(self._previous_file_obj, self._current_file_obj)
                     daemon.daemon.redirect_stream(sys.stdout, self._current_file_obj)
                     daemon.daemon.redirect_stream(sys.stderr, self._current_file_obj)
-                    self.start_log_fd_interception()
                 self.close(unused_only=True)
 
             ### Sanity check in case writing somehow fails.
             if self._previous_file_obj is self._current_file_obj:
-                self._previous_file_obj is None
+                self._previous_file_obj = None
 
             self.delete(unused_only=True)
 
-
         return self._current_file_obj
 
 
     def close(self, unused_only: bool = False) -> None:
         """
         Close any open file descriptors.
 
         Parameters
         ----------
         unused_only: bool, default False
             If `True`, only close file descriptors not currently in use.
         """
+        self.stop_log_fd_interception(unused_only=unused_only)
         subfile_indices = sorted(self.subfile_objects.keys())
         for subfile_index in subfile_indices:
             subfile_object = self.subfile_objects[subfile_index]
             if unused_only and subfile_object in (self._previous_file_obj, self._current_file_obj):
                 continue
             try:
                 if not subfile_object.closed:
-                    #  subfile_object.flush()
                     subfile_object.close()
-                _ = self.subfile_objects.pop(subfile_index, None)
-                if self.redirect_streams:
-                    _ = self._redirected_subfile_objects.pop(subfile_index, None)
             except Exception as e:
                 warn(f"Failed to close an open subfile:\n{traceback.format_exc()}")
 
+            _ = self.subfile_objects.pop(subfile_index, None)
+            if self.redirect_streams:
+                _ = self._redirected_subfile_objects.pop(subfile_index, None)
+
         if not unused_only:
             self._previous_file_obj = None
             self._current_file_obj = None
 
 
     def get_timestamp_prefix_str(self) -> str:
         """
         Return the current minute prefixm string.
         """
-        return datetime.now(timezone.utc).strftime(self.timestamps_format)
+        return datetime.now(timezone.utc).strftime(self.timestamp_format) + ' | '
 
 
     def write(self, data: str) -> None:
         """
         Write the given text into the latest subfile.
         If the subfile will be too large, create a new subfile.
         If too many subfiles exist at once, the oldest one will be deleted.
@@ -367,15 +357,18 @@
         """
         self.file_path.parent.mkdir(exist_ok=True, parents=True)
         if isinstance(data, bytes):
             data = data.decode('utf-8')
 
         prefix_str = self.get_timestamp_prefix_str() if self.write_timestamps else ""
         suffix_str = "\n" if self.write_timestamps else ""
-        self.refresh_files(potential_new_len=len(prefix_str + data + suffix_str))
+        self.refresh_files(
+            potential_new_len = len(prefix_str + data + suffix_str),
+            start_interception = True,
+        )
         try:
             if prefix_str:
                 self._current_file_obj.write(prefix_str)
             self._current_file_obj.write(data)
             if suffix_str:
                 self._current_file_obj.write(suffix_str)
         except Exception as e:
@@ -578,55 +571,81 @@
         Flush any open subfiles.
         """
         for subfile_index, subfile_object in self.subfile_objects.items():
             if not subfile_object.closed:
                 try:
                     subfile_object.flush()
                 except Exception as e:
-                    warn(f"Failed to flush subfile:\n{traceback.format_exc()}")
+                    warn(f"Failed to flush subfile {subfile_index}:\n{traceback.format_exc()}")
         if self.redirect_streams:
-            sys.stdout.flush()
-            sys.stderr.flush()
+            try:
+                sys.stdout.flush()
+            except Exception as e:
+                warn(f"Failed to flush STDOUT:\n{traceback.format_exc()}")
+            try:
+                sys.stderr.flush()
+            except Exception as e:
+                warn(f"Failed to flush STDERR:\n{traceback.format_exc()}")
 
 
     def start_log_fd_interception(self):
         """
         Start the file descriptor monitoring threads.
         """
+        threads = self.__dict__.get('_interceptor_threads', [])
         self._stdout_interceptor = FileDescriptorInterceptor(
             sys.stdout.fileno(),
             self.get_timestamp_prefix_str,
         )
         self._stderr_interceptor = FileDescriptorInterceptor(
             sys.stderr.fileno(),
             self.get_timestamp_prefix_str,
         )
-        self._stdout_interceptor_thread = Thread(target=self._stdout_interceptor.start_interception)
-        self._stderr_interceptor_thread = Thread(target=self._stderr_interceptor.start_interception)
+
+        self._stdout_interceptor_thread = Thread(
+            target = self._stdout_interceptor.start_interception,
+            daemon = True,
+        )
+        self._stderr_interceptor_thread = Thread(
+            target = self._stderr_interceptor.start_interception,
+            daemon = True,
+        )
         self._stdout_interceptor_thread.start()
         self._stderr_interceptor_thread.start()
+        self._intercepting = True
 
+        if '_interceptor_threads' not in self.__dict__:
+            self._interceptor_threads = []
+        if '_interceptors' not in self.__dict__:
+            self._interceptors = []
+        self._interceptor_threads.extend([
+            self._stdout_interceptor_thread,
+            self._stderr_interceptor_thread,
+        ])
+        self.stop_log_fd_interception(unused_only=True)
 
-    def stop_log_fd_interception(self):
+    def stop_log_fd_interception(self, unused_only: bool = False):
         """
         Stop the file descriptor monitoring threads.
         """
-        stdout_interceptor = self.__dict__.get('_stdout_interceptor', None)
-        stderr_interceptor = self.__dict__.get('_stderr_interceptor', None)
-        stdout_interceptor_thread = self.__dict__.get('_stdout_interceptor_thread', None)
-        stderr_interceptor_thread = self.__dict__.get('_stderr_interceptor_thread', None)
-        if stdout_interceptor is None:
-            return
-        stdout_interceptor.stop_interception()
-        stderr_interceptor.stop_interception()
-        try:
-            stdout_interceptor_thread.join()
-            stderr_interceptor_thread.join()
-        except Exception:
-            pass
+        interceptors = self.__dict__.get('_interceptors', [])
+        interceptor_threads = self.__dict__.get('_interceptor_threads', [])
+
+        end_ix = len(interceptors) if not unused_only else -2
+
+        for interceptor in interceptors[:end_ix]:
+            interceptor.stop_interception()
+        del interceptors[:end_ix]
+
+        for thread in interceptor_threads[:end_ix]:
+            try:
+                thread.join()
+            except Exception as e:
+                warn(f"Failed to join interceptor threads:\n{traceback.format_exc()}")
+        del interceptor_threads[:end_ix]
 
 
     def __repr__(self) -> str:
         """
         Return basic info for this `RotatingFile`.
         """
         return (
```

### Comparing `meerschaum-2.2.0rc1/meerschaum/utils/daemon/__init__.py` & `meerschaum-2.2.0rc2/meerschaum/utils/daemon/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from __future__ import annotations
 import os, pathlib, shutil, json, datetime, threading, shlex
 from meerschaum.utils.typing import SuccessTuple, List, Optional, Callable, Any, Dict
 from meerschaum.config._paths import DAEMON_RESOURCES_PATH
 from meerschaum.utils.daemon.Daemon import Daemon
 from meerschaum.utils.daemon.RotatingFile import RotatingFile
+from meerschaum.utils.daemon.FileDescriptorInterceptor import FileDescriptorInterceptor
 
 
 def daemon_entry(sysargs: Optional[List[str]] = None) -> SuccessTuple:
     """Parse sysargs and execute a Meerschaum action as a daemon.
 
     Parameters
     ----------
```

### Comparing `meerschaum-2.2.0rc1/meerschaum/utils/daemon/_names.py` & `meerschaum-2.2.0rc2/meerschaum/utils/daemon/_names.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/utils/dataframe.py` & `meerschaum-2.2.0rc2/meerschaum/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/utils/debug.py` & `meerschaum-2.2.0rc2/meerschaum/utils/debug.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/utils/dtypes/__init__.py` & `meerschaum-2.2.0rc2/meerschaum/utils/dtypes/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/utils/dtypes/sql.py` & `meerschaum-2.2.0rc2/meerschaum/utils/dtypes/sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/utils/formatting/__init__.py` & `meerschaum-2.2.0rc2/meerschaum/utils/formatting/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/utils/formatting/_jobs.py` & `meerschaum-2.2.0rc2/meerschaum/utils/formatting/_jobs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/utils/formatting/_pipes.py` & `meerschaum-2.2.0rc2/meerschaum/utils/formatting/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/utils/formatting/_pprint.py` & `meerschaum-2.2.0rc2/meerschaum/utils/formatting/_pprint.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/utils/formatting/_shell.py` & `meerschaum-2.2.0rc2/meerschaum/utils/formatting/_shell.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/utils/interactive.py` & `meerschaum-2.2.0rc2/meerschaum/utils/interactive.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/utils/misc.py` & `meerschaum-2.2.0rc2/meerschaum/utils/misc.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/utils/networking.py` & `meerschaum-2.2.0rc2/meerschaum/utils/networking.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/utils/packages/__init__.py` & `meerschaum-2.2.0rc2/meerschaum/utils/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/utils/packages/_packages.py` & `meerschaum-2.2.0rc2/meerschaum/utils/packages/_packages.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/utils/packages/lazy_loader.py` & `meerschaum-2.2.0rc2/meerschaum/utils/packages/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/utils/pool.py` & `meerschaum-2.2.0rc2/meerschaum/utils/pool.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/utils/process.py` & `meerschaum-2.2.0rc2/meerschaum/utils/process.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/utils/prompt.py` & `meerschaum-2.2.0rc2/meerschaum/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/utils/schedule.py` & `meerschaum-2.2.0rc2/meerschaum/utils/schedule.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/utils/sql.py` & `meerschaum-2.2.0rc2/meerschaum/utils/sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/utils/threading.py` & `meerschaum-2.2.0rc2/meerschaum/utils/threading.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 Define a custom Thread class with a callback method.
 """
 
 from __future__ import annotations
 from meerschaum.utils.typing import Optional
 
 import threading
+import traceback
 Lock = threading.Lock
 RLock = threading.RLock
 Event = threading.Event
 Timer = threading.Timer
 get_ident = threading.get_ident
 
 class Thread(threading.Thread):
```

### Comparing `meerschaum-2.2.0rc1/meerschaum/utils/typing.py` & `meerschaum-2.2.0rc2/meerschaum/utils/typing.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/utils/venv/_Venv.py` & `meerschaum-2.2.0rc2/meerschaum/utils/venv/_Venv.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/utils/venv/__init__.py` & `meerschaum-2.2.0rc2/meerschaum/utils/venv/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/utils/warnings.py` & `meerschaum-2.2.0rc2/meerschaum/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum/utils/yaml.py` & `meerschaum-2.2.0rc2/meerschaum/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/meerschaum.egg-info/PKG-INFO` & `meerschaum-2.2.0rc2/meerschaum.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meerschaum
-Version: 2.2.0rc1
+Version: 2.2.0rc2
 Summary: Sync Time-Series Pipes with Meerschaum
 Home-page: https://meerschaum.io
 Author: Bennett Meares
 Author-email: bennett.meares@gmail.com
 Maintainer-email: bennett.meares@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://docs.meerschaum.io
```

### Comparing `meerschaum-2.2.0rc1/meerschaum.egg-info/SOURCES.txt` & `meerschaum-2.2.0rc2/meerschaum.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -130,14 +130,15 @@
 meerschaum/api/routes/_pipes.py
 meerschaum/api/routes/_plugins.py
 meerschaum/api/routes/_users.py
 meerschaum/api/routes/_version.py
 meerschaum/api/routes/_webterm.py
 meerschaum/api/tables/__init__.py
 meerschaum/config/__init__.py
+meerschaum/config/_dash.py
 meerschaum/config/_default.py
 meerschaum/config/_edit.py
 meerschaum/config/_environment.py
 meerschaum/config/_formatting.py
 meerschaum/config/_jobs.py
 meerschaum/config/_patch.py
 meerschaum/config/_paths.py
```

### Comparing `meerschaum-2.2.0rc1/meerschaum.egg-info/requires.txt` & `meerschaum-2.2.0rc2/meerschaum.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/setup.py` & `meerschaum-2.2.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/tests/test_deduplicate.py` & `meerschaum-2.2.0rc2/tests/test_deduplicate.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/tests/test_pipes_dtypes.py` & `meerschaum-2.2.0rc2/tests/test_pipes_dtypes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/tests/test_sql.py` & `meerschaum-2.2.0rc2/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/tests/test_sync.py` & `meerschaum-2.2.0rc2/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/tests/test_users.py` & `meerschaum-2.2.0rc2/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-2.2.0rc1/tests/test_verify.py` & `meerschaum-2.2.0rc2/tests/test_verify.py`

 * *Files identical despite different names*

